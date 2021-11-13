<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:1.7`](#traefik17)
-	[`traefik:1.7-alpine`](#traefik17-alpine)
-	[`traefik:1.7-windowsservercore-1809`](#traefik17-windowsservercore-1809)
-	[`traefik:1.7.33`](#traefik1733)
-	[`traefik:1.7.33-alpine`](#traefik1733-alpine)
-	[`traefik:1.7.33-windowsservercore-1809`](#traefik1733-windowsservercore-1809)
-	[`traefik:2.5`](#traefik25)
-	[`traefik:2.5-windowsservercore-1809`](#traefik25-windowsservercore-1809)
-	[`traefik:2.5.4`](#traefik254)
-	[`traefik:2.5.4-windowsservercore-1809`](#traefik254-windowsservercore-1809)
-	[`traefik:brie`](#traefikbrie)
-	[`traefik:brie-windowsservercore-1809`](#traefikbrie-windowsservercore-1809)
-	[`traefik:latest`](#traefiklatest)
-	[`traefik:maroilles`](#traefikmaroilles)
-	[`traefik:maroilles-alpine`](#traefikmaroilles-alpine)
-	[`traefik:maroilles-windowsservercore-1809`](#traefikmaroilles-windowsservercore-1809)
-	[`traefik:v1.7`](#traefikv17)
-	[`traefik:v1.7-alpine`](#traefikv17-alpine)
-	[`traefik:v1.7-windowsservercore-1809`](#traefikv17-windowsservercore-1809)
-	[`traefik:v1.7.33`](#traefikv1733)
-	[`traefik:v1.7.33-alpine`](#traefikv1733-alpine)
-	[`traefik:v1.7.33-windowsservercore-1809`](#traefikv1733-windowsservercore-1809)
-	[`traefik:v2.5`](#traefikv25)
-	[`traefik:v2.5-windowsservercore-1809`](#traefikv25-windowsservercore-1809)
-	[`traefik:v2.5.4`](#traefikv254)
-	[`traefik:v2.5.4-windowsservercore-1809`](#traefikv254-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:1.7`

```console
$ docker pull traefik@sha256:c28f00fc0070755b8e3fa3befd800dcf4505e631e7627a41c96a0b1de5b7c8c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7` - linux; amd64

```console
$ docker pull traefik@sha256:fd8690c11f1375f07ae9841582868f64628eb7b1e7081e71730c7a992fc8f235
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22591637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85d1b251ae417bc825b2b8d1473d5f4e6451f6cfbadf53fb892e65975a6de1aa`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 05 Oct 2021 17:58:25 GMT
COPY file:c8f727cb8b17c5a8735e609a9b9f333f20765e36c457d0557ed48693a6694880 in /etc/ssl/certs/ 
# Tue, 05 Oct 2021 17:58:26 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 07 Oct 2021 20:04:59 GMT
COPY file:e409355a2ff570f276c91d9f7a80f98e14727655971d95deeb1f7e641b865101 in / 
# Thu, 07 Oct 2021 20:04:59 GMT
EXPOSE 80
# Thu, 07 Oct 2021 20:04:59 GMT
VOLUME [/tmp]
# Thu, 07 Oct 2021 20:04:59 GMT
ENTRYPOINT ["/traefik"]
# Thu, 07 Oct 2021 20:05:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:13e52be55f8d958b3ebb4e73685de5dd10ff4b4af613c4d23424519693aa01e0`  
		Last Modified: Tue, 05 Oct 2021 17:59:12 GMT  
		Size: 122.4 KB (122407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f116118f8a36a09eba9c55ae29c9925e0ae854aa36d9dc1fc271a7be43b820c`  
		Last Modified: Tue, 05 Oct 2021 17:59:11 GMT  
		Size: 308.8 KB (308839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0968db303bdc7c1cd8bedcde2a1d2efaadf77eacdac7f4ad24ff18e990f384b`  
		Last Modified: Thu, 07 Oct 2021 20:06:25 GMT  
		Size: 22.2 MB (22160391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:d1bf188870da15d1c22f8da3ae6bc614e3581477d3feb4eada90186003f43f3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21069245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a07e35b9622e89560baf105486fce1e43a9e3fef0261c41227dc7e966df4fe7f`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 05 Oct 2021 00:02:38 GMT
COPY file:c8f727cb8b17c5a8735e609a9b9f333f20765e36c457d0557ed48693a6694880 in /etc/ssl/certs/ 
# Sat, 13 Nov 2021 06:52:39 GMT
COPY dir:c22cc1c2c366de443c999e78a53f0bde0b523a72b38a70fa92f5c6322439c95e in /usr/share/ 
# Sat, 13 Nov 2021 06:52:44 GMT
COPY file:37d0f8b70c5da3bdf158098e422d0bfc00d82405c51ca41ee81a5e564433a943 in / 
# Sat, 13 Nov 2021 06:52:45 GMT
EXPOSE 80
# Sat, 13 Nov 2021 06:52:45 GMT
VOLUME [/tmp]
# Sat, 13 Nov 2021 06:52:46 GMT
ENTRYPOINT ["/traefik"]
# Sat, 13 Nov 2021 06:52:46 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:611185932e68f8b41b94235c966a6c2d26bb4a0f053993c6e49edc01123213f9`  
		Last Modified: Tue, 05 Oct 2021 00:04:56 GMT  
		Size: 122.4 KB (122407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81282f8b9fcf1f821d7dab2ed1f6addbda565118cc5ee95d9de4ae8ff91333f`  
		Last Modified: Sat, 13 Nov 2021 06:55:43 GMT  
		Size: 328.6 KB (328578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec6501fe03be7dfb2746de58fa6f69cd43c44f59e5743b529fe980f6f9855c9`  
		Last Modified: Sat, 13 Nov 2021 06:55:52 GMT  
		Size: 20.6 MB (20618260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:731733ac032dea4cea1b9ab054908f17b63ef884e861bd58b5b3d9d3c56257a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20575143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48fc834a31f8efc387885a01430806a70be2becd45240dd06c0441dc6c703e66`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Mon, 08 Nov 2021 20:23:04 GMT
COPY file:c8f727cb8b17c5a8735e609a9b9f333f20765e36c457d0557ed48693a6694880 in /etc/ssl/certs/ 
# Mon, 08 Nov 2021 20:23:05 GMT
COPY dir:c22cc1c2c366de443c999e78a53f0bde0b523a72b38a70fa92f5c6322439c95e in /usr/share/ 
# Mon, 08 Nov 2021 20:23:06 GMT
COPY file:cd6a95e409278a374fb6ef69098a37f7bc0c8d4eddd3ac751de25d783adf1227 in / 
# Mon, 08 Nov 2021 20:23:06 GMT
EXPOSE 80
# Mon, 08 Nov 2021 20:23:07 GMT
VOLUME [/tmp]
# Mon, 08 Nov 2021 20:23:08 GMT
ENTRYPOINT ["/traefik"]
# Mon, 08 Nov 2021 20:23:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:078e101c84a7a75069b9c18efdfc2b24c9840aa136b34eb6e3a0ebe1b74d0a94`  
		Last Modified: Mon, 08 Nov 2021 20:24:37 GMT  
		Size: 122.4 KB (122399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7a624fda7cabc945cc9d9f610f256d933b121fdafa2052d617cf3144bbe2aa`  
		Last Modified: Mon, 08 Nov 2021 20:24:37 GMT  
		Size: 328.5 KB (328545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615fe0c03a3e5c4c76f7ef9722b5a160e05898d03f2ecf3aa00c6f93b560b654`  
		Last Modified: Mon, 08 Nov 2021 20:24:42 GMT  
		Size: 20.1 MB (20124199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-alpine`

```console
$ docker pull traefik@sha256:4c066039f31aee5ffe6f8d810d86a85aa37816caf3767e4880df1207eb48b774
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:a7216aa72c026d4ca0b5fb9cedb5c9e8bf21ba5e3352d4e14ae2ccb0c2ca50f6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25631512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2edc46527be5da9cc20fe71d011f044ef2809203c192636ac1f2457fc11d292`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:28:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 07 Oct 2021 20:04:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 07 Oct 2021 20:04:36 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 07 Oct 2021 20:04:36 GMT
EXPOSE 80
# Thu, 07 Oct 2021 20:04:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Oct 2021 20:04:37 GMT
CMD ["traefik"]
# Thu, 07 Oct 2021 20:04:37 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5295d3cd66d0f8651338b81063a408fcc2c70d810c92e5cb435c467a1939d60`  
		Last Modified: Thu, 02 Sep 2021 17:29:12 GMT  
		Size: 656.4 KB (656356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97ae40f614f61bae620d88f81210f6f68badbd591793811c9d070e8407abfc6`  
		Last Modified: Thu, 07 Oct 2021 20:05:28 GMT  
		Size: 22.2 MB (22160342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a1066c5e04bc425dd4ec2bedad7fee468ce0ef54cc9010d8f5fd1f125bac99`  
		Last Modified: Thu, 07 Oct 2021 20:05:24 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:a52a7bc8595611ebd4be28a1c1ff5f344ae146cff12024496244981d276fcc43
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23937163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10f4734a371bdc50ecea01f7067b4b7b51f929375935f24db4066e86e10b0d9a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:51:34 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 13 Nov 2021 06:52:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Sat, 13 Nov 2021 06:52:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 13 Nov 2021 06:52:17 GMT
EXPOSE 80
# Sat, 13 Nov 2021 06:52:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:52:18 GMT
CMD ["traefik"]
# Sat, 13 Nov 2021 06:52:19 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b00cdbc51db9651a9c09390b641face7e18e642e3ff49397c6d477c89c3d7e`  
		Last Modified: Sat, 13 Nov 2021 06:54:26 GMT  
		Size: 683.0 KB (682972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7034046f5f5ec87c3e6f3f0ec53c2f503aacf02a2b838f771054bc9f0f341a7a`  
		Last Modified: Sat, 13 Nov 2021 06:55:17 GMT  
		Size: 20.6 MB (20618431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bc931b12c3ec19e39c375974b827278a96a38896854112c3dee959f13f709e`  
		Last Modified: Sat, 13 Nov 2021 06:55:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:bf623d4dceb05f5385fdc9b50686849c58ed1bec7b8740daf447cced2c011656
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23522334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8d2cd70545692a5348584b716f1a72a121098a1e94264c03c991e5e462d84e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:16:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 12 Nov 2021 18:16:50 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 12 Nov 2021 18:16:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 12 Nov 2021 18:16:52 GMT
EXPOSE 80
# Fri, 12 Nov 2021 18:16:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 18:16:54 GMT
CMD ["traefik"]
# Fri, 12 Nov 2021 18:16:55 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cc5a4b7f102f236064e4712164f29c52d256612820409cc28c41a7f5def4a5`  
		Last Modified: Fri, 12 Nov 2021 18:17:40 GMT  
		Size: 680.0 KB (680008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3283e6a7888f1f1ba0cfe0b0532a69f6c3036443be824e2bc89580587e0247f`  
		Last Modified: Fri, 12 Nov 2021 18:18:09 GMT  
		Size: 20.1 MB (20124258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9515da1d1aa1c2b9d89c2e66d9b46452fcf8c436e6e86b341cca564107abc3d9`  
		Last Modified: Fri, 12 Nov 2021 18:18:05 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:8947c337b29375e8b8c7e327209b3ee4ebf835f2f3319131494ee875f43b66b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `traefik:1.7-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull traefik@sha256:b6a7d8bd77893cc59a7ed693bcf1d8c8cc97246c872fad9a07a88dad727142f9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728969379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afb6fcd7cb1a41e077e776cecc4b37b62bcdca91a77e351f5baaf9a6e10d6b62`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 19:04:20 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 10 Nov 2021 19:04:22 GMT
EXPOSE 80
# Wed, 10 Nov 2021 19:04:23 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Nov 2021 19:04:24 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbe7df586a8125285cae7dac6ad774b05129e99156a632ea1d20f883029d03c`  
		Last Modified: Wed, 10 Nov 2021 19:05:48 GMT  
		Size: 22.8 MB (22842554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52b885ca238073b5f9093f48de5c52b015ffa93ef1dff1744d9dba6be4d64dc`  
		Last Modified: Wed, 10 Nov 2021 19:05:42 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852f60a1a31dbed66a29d09964528f56907495e407d124284d744ead5697a9bc`  
		Last Modified: Wed, 10 Nov 2021 19:05:42 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa570cc10582d59ee894f65e0e6a6384ab191442f61c45fc2b8a8e9df933576`  
		Last Modified: Wed, 10 Nov 2021 19:05:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.33`

```console
$ docker pull traefik@sha256:c28f00fc0070755b8e3fa3befd800dcf4505e631e7627a41c96a0b1de5b7c8c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.33` - linux; amd64

```console
$ docker pull traefik@sha256:fd8690c11f1375f07ae9841582868f64628eb7b1e7081e71730c7a992fc8f235
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22591637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85d1b251ae417bc825b2b8d1473d5f4e6451f6cfbadf53fb892e65975a6de1aa`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 05 Oct 2021 17:58:25 GMT
COPY file:c8f727cb8b17c5a8735e609a9b9f333f20765e36c457d0557ed48693a6694880 in /etc/ssl/certs/ 
# Tue, 05 Oct 2021 17:58:26 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 07 Oct 2021 20:04:59 GMT
COPY file:e409355a2ff570f276c91d9f7a80f98e14727655971d95deeb1f7e641b865101 in / 
# Thu, 07 Oct 2021 20:04:59 GMT
EXPOSE 80
# Thu, 07 Oct 2021 20:04:59 GMT
VOLUME [/tmp]
# Thu, 07 Oct 2021 20:04:59 GMT
ENTRYPOINT ["/traefik"]
# Thu, 07 Oct 2021 20:05:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:13e52be55f8d958b3ebb4e73685de5dd10ff4b4af613c4d23424519693aa01e0`  
		Last Modified: Tue, 05 Oct 2021 17:59:12 GMT  
		Size: 122.4 KB (122407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f116118f8a36a09eba9c55ae29c9925e0ae854aa36d9dc1fc271a7be43b820c`  
		Last Modified: Tue, 05 Oct 2021 17:59:11 GMT  
		Size: 308.8 KB (308839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0968db303bdc7c1cd8bedcde2a1d2efaadf77eacdac7f4ad24ff18e990f384b`  
		Last Modified: Thu, 07 Oct 2021 20:06:25 GMT  
		Size: 22.2 MB (22160391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.33` - linux; arm variant v6

```console
$ docker pull traefik@sha256:d1bf188870da15d1c22f8da3ae6bc614e3581477d3feb4eada90186003f43f3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21069245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a07e35b9622e89560baf105486fce1e43a9e3fef0261c41227dc7e966df4fe7f`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 05 Oct 2021 00:02:38 GMT
COPY file:c8f727cb8b17c5a8735e609a9b9f333f20765e36c457d0557ed48693a6694880 in /etc/ssl/certs/ 
# Sat, 13 Nov 2021 06:52:39 GMT
COPY dir:c22cc1c2c366de443c999e78a53f0bde0b523a72b38a70fa92f5c6322439c95e in /usr/share/ 
# Sat, 13 Nov 2021 06:52:44 GMT
COPY file:37d0f8b70c5da3bdf158098e422d0bfc00d82405c51ca41ee81a5e564433a943 in / 
# Sat, 13 Nov 2021 06:52:45 GMT
EXPOSE 80
# Sat, 13 Nov 2021 06:52:45 GMT
VOLUME [/tmp]
# Sat, 13 Nov 2021 06:52:46 GMT
ENTRYPOINT ["/traefik"]
# Sat, 13 Nov 2021 06:52:46 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:611185932e68f8b41b94235c966a6c2d26bb4a0f053993c6e49edc01123213f9`  
		Last Modified: Tue, 05 Oct 2021 00:04:56 GMT  
		Size: 122.4 KB (122407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81282f8b9fcf1f821d7dab2ed1f6addbda565118cc5ee95d9de4ae8ff91333f`  
		Last Modified: Sat, 13 Nov 2021 06:55:43 GMT  
		Size: 328.6 KB (328578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec6501fe03be7dfb2746de58fa6f69cd43c44f59e5743b529fe980f6f9855c9`  
		Last Modified: Sat, 13 Nov 2021 06:55:52 GMT  
		Size: 20.6 MB (20618260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.33` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:731733ac032dea4cea1b9ab054908f17b63ef884e861bd58b5b3d9d3c56257a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20575143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48fc834a31f8efc387885a01430806a70be2becd45240dd06c0441dc6c703e66`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Mon, 08 Nov 2021 20:23:04 GMT
COPY file:c8f727cb8b17c5a8735e609a9b9f333f20765e36c457d0557ed48693a6694880 in /etc/ssl/certs/ 
# Mon, 08 Nov 2021 20:23:05 GMT
COPY dir:c22cc1c2c366de443c999e78a53f0bde0b523a72b38a70fa92f5c6322439c95e in /usr/share/ 
# Mon, 08 Nov 2021 20:23:06 GMT
COPY file:cd6a95e409278a374fb6ef69098a37f7bc0c8d4eddd3ac751de25d783adf1227 in / 
# Mon, 08 Nov 2021 20:23:06 GMT
EXPOSE 80
# Mon, 08 Nov 2021 20:23:07 GMT
VOLUME [/tmp]
# Mon, 08 Nov 2021 20:23:08 GMT
ENTRYPOINT ["/traefik"]
# Mon, 08 Nov 2021 20:23:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:078e101c84a7a75069b9c18efdfc2b24c9840aa136b34eb6e3a0ebe1b74d0a94`  
		Last Modified: Mon, 08 Nov 2021 20:24:37 GMT  
		Size: 122.4 KB (122399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7a624fda7cabc945cc9d9f610f256d933b121fdafa2052d617cf3144bbe2aa`  
		Last Modified: Mon, 08 Nov 2021 20:24:37 GMT  
		Size: 328.5 KB (328545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615fe0c03a3e5c4c76f7ef9722b5a160e05898d03f2ecf3aa00c6f93b560b654`  
		Last Modified: Mon, 08 Nov 2021 20:24:42 GMT  
		Size: 20.1 MB (20124199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.33-alpine`

```console
$ docker pull traefik@sha256:4c066039f31aee5ffe6f8d810d86a85aa37816caf3767e4880df1207eb48b774
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.33-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:a7216aa72c026d4ca0b5fb9cedb5c9e8bf21ba5e3352d4e14ae2ccb0c2ca50f6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25631512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2edc46527be5da9cc20fe71d011f044ef2809203c192636ac1f2457fc11d292`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:28:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 07 Oct 2021 20:04:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 07 Oct 2021 20:04:36 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 07 Oct 2021 20:04:36 GMT
EXPOSE 80
# Thu, 07 Oct 2021 20:04:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Oct 2021 20:04:37 GMT
CMD ["traefik"]
# Thu, 07 Oct 2021 20:04:37 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5295d3cd66d0f8651338b81063a408fcc2c70d810c92e5cb435c467a1939d60`  
		Last Modified: Thu, 02 Sep 2021 17:29:12 GMT  
		Size: 656.4 KB (656356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97ae40f614f61bae620d88f81210f6f68badbd591793811c9d070e8407abfc6`  
		Last Modified: Thu, 07 Oct 2021 20:05:28 GMT  
		Size: 22.2 MB (22160342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a1066c5e04bc425dd4ec2bedad7fee468ce0ef54cc9010d8f5fd1f125bac99`  
		Last Modified: Thu, 07 Oct 2021 20:05:24 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.33-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:a52a7bc8595611ebd4be28a1c1ff5f344ae146cff12024496244981d276fcc43
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23937163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10f4734a371bdc50ecea01f7067b4b7b51f929375935f24db4066e86e10b0d9a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:51:34 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 13 Nov 2021 06:52:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Sat, 13 Nov 2021 06:52:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 13 Nov 2021 06:52:17 GMT
EXPOSE 80
# Sat, 13 Nov 2021 06:52:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:52:18 GMT
CMD ["traefik"]
# Sat, 13 Nov 2021 06:52:19 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b00cdbc51db9651a9c09390b641face7e18e642e3ff49397c6d477c89c3d7e`  
		Last Modified: Sat, 13 Nov 2021 06:54:26 GMT  
		Size: 683.0 KB (682972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7034046f5f5ec87c3e6f3f0ec53c2f503aacf02a2b838f771054bc9f0f341a7a`  
		Last Modified: Sat, 13 Nov 2021 06:55:17 GMT  
		Size: 20.6 MB (20618431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bc931b12c3ec19e39c375974b827278a96a38896854112c3dee959f13f709e`  
		Last Modified: Sat, 13 Nov 2021 06:55:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.33-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:bf623d4dceb05f5385fdc9b50686849c58ed1bec7b8740daf447cced2c011656
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23522334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8d2cd70545692a5348584b716f1a72a121098a1e94264c03c991e5e462d84e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:16:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 12 Nov 2021 18:16:50 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 12 Nov 2021 18:16:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 12 Nov 2021 18:16:52 GMT
EXPOSE 80
# Fri, 12 Nov 2021 18:16:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 18:16:54 GMT
CMD ["traefik"]
# Fri, 12 Nov 2021 18:16:55 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cc5a4b7f102f236064e4712164f29c52d256612820409cc28c41a7f5def4a5`  
		Last Modified: Fri, 12 Nov 2021 18:17:40 GMT  
		Size: 680.0 KB (680008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3283e6a7888f1f1ba0cfe0b0532a69f6c3036443be824e2bc89580587e0247f`  
		Last Modified: Fri, 12 Nov 2021 18:18:09 GMT  
		Size: 20.1 MB (20124258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9515da1d1aa1c2b9d89c2e66d9b46452fcf8c436e6e86b341cca564107abc3d9`  
		Last Modified: Fri, 12 Nov 2021 18:18:05 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.33-windowsservercore-1809`

```console
$ docker pull traefik@sha256:8947c337b29375e8b8c7e327209b3ee4ebf835f2f3319131494ee875f43b66b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `traefik:1.7.33-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull traefik@sha256:b6a7d8bd77893cc59a7ed693bcf1d8c8cc97246c872fad9a07a88dad727142f9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728969379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afb6fcd7cb1a41e077e776cecc4b37b62bcdca91a77e351f5baaf9a6e10d6b62`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 19:04:20 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 10 Nov 2021 19:04:22 GMT
EXPOSE 80
# Wed, 10 Nov 2021 19:04:23 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Nov 2021 19:04:24 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbe7df586a8125285cae7dac6ad774b05129e99156a632ea1d20f883029d03c`  
		Last Modified: Wed, 10 Nov 2021 19:05:48 GMT  
		Size: 22.8 MB (22842554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52b885ca238073b5f9093f48de5c52b015ffa93ef1dff1744d9dba6be4d64dc`  
		Last Modified: Wed, 10 Nov 2021 19:05:42 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852f60a1a31dbed66a29d09964528f56907495e407d124284d744ead5697a9bc`  
		Last Modified: Wed, 10 Nov 2021 19:05:42 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa570cc10582d59ee894f65e0e6a6384ab191442f61c45fc2b8a8e9df933576`  
		Last Modified: Wed, 10 Nov 2021 19:05:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.5`

```console
$ docker pull traefik@sha256:b120cca907a99c63ff32e71c25a571c0563a7f905aa63407cb6b27f2b426346e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.5` - linux; amd64

```console
$ docker pull traefik@sha256:212aee66cc6eecbd6a04ef0af0b8616fbc4f716d4c9a52dfa9808b4a8dea5d8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29845535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3bb9550d562ded287f2fc5f71056c652d49cd1ae0ddde3a39acefb3b10dc1ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:28:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 08 Nov 2021 20:51:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 08 Nov 2021 20:51:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 08 Nov 2021 20:51:20 GMT
EXPOSE 80
# Mon, 08 Nov 2021 20:51:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 08 Nov 2021 20:51:21 GMT
CMD ["traefik"]
# Mon, 08 Nov 2021 20:51:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5295d3cd66d0f8651338b81063a408fcc2c70d810c92e5cb435c467a1939d60`  
		Last Modified: Thu, 02 Sep 2021 17:29:12 GMT  
		Size: 656.4 KB (656356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c117e813430bc0788d2b53069f51b9f1387ffaf32a071b5b966237a4e8be398c`  
		Last Modified: Mon, 08 Nov 2021 20:51:51 GMT  
		Size: 26.4 MB (26374365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aedf838ed1f44594dd320fce1909f9563036b91ae4efdbc35f75a5a73473b2d`  
		Last Modified: Mon, 08 Nov 2021 20:51:46 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.5` - linux; arm variant v6

```console
$ docker pull traefik@sha256:c489cc16b0d37e7c0dd106ee095d0481f3ccba3e81f6192affa6bfa07edc85ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28082693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76490c753f69e74602fb79cf36a7893247758dd8d7f4b159c12a83ec4922de99`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:51:34 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 13 Nov 2021 06:51:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Sat, 13 Nov 2021 06:51:45 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 13 Nov 2021 06:51:46 GMT
EXPOSE 80
# Sat, 13 Nov 2021 06:51:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:51:48 GMT
CMD ["traefik"]
# Sat, 13 Nov 2021 06:51:48 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b00cdbc51db9651a9c09390b641face7e18e642e3ff49397c6d477c89c3d7e`  
		Last Modified: Sat, 13 Nov 2021 06:54:26 GMT  
		Size: 683.0 KB (682972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c6a0aef2ab8157f246bbc4e0a2171e4d18ab19258dc3bd97ab2dea6f096f44`  
		Last Modified: Sat, 13 Nov 2021 06:54:36 GMT  
		Size: 24.8 MB (24763961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3910da118b09f25ef883d4a46e512db99a6a9f12a1031790d8b8ffd4c9d606fa`  
		Last Modified: Sat, 13 Nov 2021 06:54:25 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.5` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:317dbd98705ff9a2719bb8357e83c496ea70f7caff8aca06b123e1d0862dbee0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27461064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bd5494cab630ed31508338889d5d02c98d6113f9d818584913b8ddd68dd1121`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:16:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 12 Nov 2021 18:16:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 12 Nov 2021 18:16:37 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 12 Nov 2021 18:16:37 GMT
EXPOSE 80
# Fri, 12 Nov 2021 18:16:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 18:16:39 GMT
CMD ["traefik"]
# Fri, 12 Nov 2021 18:16:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cc5a4b7f102f236064e4712164f29c52d256612820409cc28c41a7f5def4a5`  
		Last Modified: Fri, 12 Nov 2021 18:17:40 GMT  
		Size: 680.0 KB (680008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd938bc8aa751ad66221cfd63d8acc173d3ceed14728f87fdac32ed0598cd3af`  
		Last Modified: Fri, 12 Nov 2021 18:17:44 GMT  
		Size: 24.1 MB (24062987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ef3656e6ddb41988a45143ead13d5199714713ea7eee816d82ed9d85f35b5c`  
		Last Modified: Fri, 12 Nov 2021 18:17:40 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.5-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b1a9946eaeebb1c00c1400c54ce78bef39faf169fca9f6a595a893c843b72ead
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `traefik:2.5-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull traefik@sha256:42357fbc16fa6562f694dbd067f5b3bed471dc95add1250f2ac093c6f0073e91
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2733082630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0e334d0f14b68204e26ab00c216d99705a81caf654aece76109da97517a227c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 19:03:10 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 10 Nov 2021 19:03:12 GMT
EXPOSE 80
# Wed, 10 Nov 2021 19:03:13 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Nov 2021 19:03:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908fd75d4d7401dab2f0ff42955f8f0d742329f415770c4cd0f106b36386e8ca`  
		Last Modified: Wed, 10 Nov 2021 19:05:24 GMT  
		Size: 27.0 MB (26955862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c368cdf7d267763d786cd3906111dc6e50bda11d0503b8abe85752bb7ebad413`  
		Last Modified: Wed, 10 Nov 2021 19:04:54 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f47c40e5c1ec2e7fb9152f280ad6b183350baba9dcf50eaf9f48945b0f00ef`  
		Last Modified: Wed, 10 Nov 2021 19:04:54 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f66e9bd16b34b84de1acbb8aae706a113f9a876d34f5e41fbc6d0411bab824`  
		Last Modified: Wed, 10 Nov 2021 19:04:54 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.5.4`

```console
$ docker pull traefik@sha256:b120cca907a99c63ff32e71c25a571c0563a7f905aa63407cb6b27f2b426346e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.5.4` - linux; amd64

```console
$ docker pull traefik@sha256:212aee66cc6eecbd6a04ef0af0b8616fbc4f716d4c9a52dfa9808b4a8dea5d8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29845535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3bb9550d562ded287f2fc5f71056c652d49cd1ae0ddde3a39acefb3b10dc1ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:28:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 08 Nov 2021 20:51:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 08 Nov 2021 20:51:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 08 Nov 2021 20:51:20 GMT
EXPOSE 80
# Mon, 08 Nov 2021 20:51:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 08 Nov 2021 20:51:21 GMT
CMD ["traefik"]
# Mon, 08 Nov 2021 20:51:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5295d3cd66d0f8651338b81063a408fcc2c70d810c92e5cb435c467a1939d60`  
		Last Modified: Thu, 02 Sep 2021 17:29:12 GMT  
		Size: 656.4 KB (656356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c117e813430bc0788d2b53069f51b9f1387ffaf32a071b5b966237a4e8be398c`  
		Last Modified: Mon, 08 Nov 2021 20:51:51 GMT  
		Size: 26.4 MB (26374365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aedf838ed1f44594dd320fce1909f9563036b91ae4efdbc35f75a5a73473b2d`  
		Last Modified: Mon, 08 Nov 2021 20:51:46 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.5.4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:c489cc16b0d37e7c0dd106ee095d0481f3ccba3e81f6192affa6bfa07edc85ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28082693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76490c753f69e74602fb79cf36a7893247758dd8d7f4b159c12a83ec4922de99`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:51:34 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 13 Nov 2021 06:51:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Sat, 13 Nov 2021 06:51:45 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 13 Nov 2021 06:51:46 GMT
EXPOSE 80
# Sat, 13 Nov 2021 06:51:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:51:48 GMT
CMD ["traefik"]
# Sat, 13 Nov 2021 06:51:48 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b00cdbc51db9651a9c09390b641face7e18e642e3ff49397c6d477c89c3d7e`  
		Last Modified: Sat, 13 Nov 2021 06:54:26 GMT  
		Size: 683.0 KB (682972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c6a0aef2ab8157f246bbc4e0a2171e4d18ab19258dc3bd97ab2dea6f096f44`  
		Last Modified: Sat, 13 Nov 2021 06:54:36 GMT  
		Size: 24.8 MB (24763961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3910da118b09f25ef883d4a46e512db99a6a9f12a1031790d8b8ffd4c9d606fa`  
		Last Modified: Sat, 13 Nov 2021 06:54:25 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.5.4` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:317dbd98705ff9a2719bb8357e83c496ea70f7caff8aca06b123e1d0862dbee0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27461064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bd5494cab630ed31508338889d5d02c98d6113f9d818584913b8ddd68dd1121`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:16:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 12 Nov 2021 18:16:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 12 Nov 2021 18:16:37 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 12 Nov 2021 18:16:37 GMT
EXPOSE 80
# Fri, 12 Nov 2021 18:16:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 18:16:39 GMT
CMD ["traefik"]
# Fri, 12 Nov 2021 18:16:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cc5a4b7f102f236064e4712164f29c52d256612820409cc28c41a7f5def4a5`  
		Last Modified: Fri, 12 Nov 2021 18:17:40 GMT  
		Size: 680.0 KB (680008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd938bc8aa751ad66221cfd63d8acc173d3ceed14728f87fdac32ed0598cd3af`  
		Last Modified: Fri, 12 Nov 2021 18:17:44 GMT  
		Size: 24.1 MB (24062987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ef3656e6ddb41988a45143ead13d5199714713ea7eee816d82ed9d85f35b5c`  
		Last Modified: Fri, 12 Nov 2021 18:17:40 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.5.4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b1a9946eaeebb1c00c1400c54ce78bef39faf169fca9f6a595a893c843b72ead
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `traefik:2.5.4-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull traefik@sha256:42357fbc16fa6562f694dbd067f5b3bed471dc95add1250f2ac093c6f0073e91
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2733082630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0e334d0f14b68204e26ab00c216d99705a81caf654aece76109da97517a227c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 19:03:10 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 10 Nov 2021 19:03:12 GMT
EXPOSE 80
# Wed, 10 Nov 2021 19:03:13 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Nov 2021 19:03:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908fd75d4d7401dab2f0ff42955f8f0d742329f415770c4cd0f106b36386e8ca`  
		Last Modified: Wed, 10 Nov 2021 19:05:24 GMT  
		Size: 27.0 MB (26955862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c368cdf7d267763d786cd3906111dc6e50bda11d0503b8abe85752bb7ebad413`  
		Last Modified: Wed, 10 Nov 2021 19:04:54 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f47c40e5c1ec2e7fb9152f280ad6b183350baba9dcf50eaf9f48945b0f00ef`  
		Last Modified: Wed, 10 Nov 2021 19:04:54 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f66e9bd16b34b84de1acbb8aae706a113f9a876d34f5e41fbc6d0411bab824`  
		Last Modified: Wed, 10 Nov 2021 19:04:54 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:brie`

```console
$ docker pull traefik@sha256:b120cca907a99c63ff32e71c25a571c0563a7f905aa63407cb6b27f2b426346e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:brie` - linux; amd64

```console
$ docker pull traefik@sha256:212aee66cc6eecbd6a04ef0af0b8616fbc4f716d4c9a52dfa9808b4a8dea5d8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29845535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3bb9550d562ded287f2fc5f71056c652d49cd1ae0ddde3a39acefb3b10dc1ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:28:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 08 Nov 2021 20:51:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 08 Nov 2021 20:51:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 08 Nov 2021 20:51:20 GMT
EXPOSE 80
# Mon, 08 Nov 2021 20:51:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 08 Nov 2021 20:51:21 GMT
CMD ["traefik"]
# Mon, 08 Nov 2021 20:51:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5295d3cd66d0f8651338b81063a408fcc2c70d810c92e5cb435c467a1939d60`  
		Last Modified: Thu, 02 Sep 2021 17:29:12 GMT  
		Size: 656.4 KB (656356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c117e813430bc0788d2b53069f51b9f1387ffaf32a071b5b966237a4e8be398c`  
		Last Modified: Mon, 08 Nov 2021 20:51:51 GMT  
		Size: 26.4 MB (26374365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aedf838ed1f44594dd320fce1909f9563036b91ae4efdbc35f75a5a73473b2d`  
		Last Modified: Mon, 08 Nov 2021 20:51:46 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:brie` - linux; arm variant v6

```console
$ docker pull traefik@sha256:c489cc16b0d37e7c0dd106ee095d0481f3ccba3e81f6192affa6bfa07edc85ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28082693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76490c753f69e74602fb79cf36a7893247758dd8d7f4b159c12a83ec4922de99`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:51:34 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 13 Nov 2021 06:51:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Sat, 13 Nov 2021 06:51:45 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 13 Nov 2021 06:51:46 GMT
EXPOSE 80
# Sat, 13 Nov 2021 06:51:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:51:48 GMT
CMD ["traefik"]
# Sat, 13 Nov 2021 06:51:48 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b00cdbc51db9651a9c09390b641face7e18e642e3ff49397c6d477c89c3d7e`  
		Last Modified: Sat, 13 Nov 2021 06:54:26 GMT  
		Size: 683.0 KB (682972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c6a0aef2ab8157f246bbc4e0a2171e4d18ab19258dc3bd97ab2dea6f096f44`  
		Last Modified: Sat, 13 Nov 2021 06:54:36 GMT  
		Size: 24.8 MB (24763961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3910da118b09f25ef883d4a46e512db99a6a9f12a1031790d8b8ffd4c9d606fa`  
		Last Modified: Sat, 13 Nov 2021 06:54:25 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:brie` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:317dbd98705ff9a2719bb8357e83c496ea70f7caff8aca06b123e1d0862dbee0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27461064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bd5494cab630ed31508338889d5d02c98d6113f9d818584913b8ddd68dd1121`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:16:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 12 Nov 2021 18:16:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 12 Nov 2021 18:16:37 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 12 Nov 2021 18:16:37 GMT
EXPOSE 80
# Fri, 12 Nov 2021 18:16:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 18:16:39 GMT
CMD ["traefik"]
# Fri, 12 Nov 2021 18:16:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cc5a4b7f102f236064e4712164f29c52d256612820409cc28c41a7f5def4a5`  
		Last Modified: Fri, 12 Nov 2021 18:17:40 GMT  
		Size: 680.0 KB (680008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd938bc8aa751ad66221cfd63d8acc173d3ceed14728f87fdac32ed0598cd3af`  
		Last Modified: Fri, 12 Nov 2021 18:17:44 GMT  
		Size: 24.1 MB (24062987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ef3656e6ddb41988a45143ead13d5199714713ea7eee816d82ed9d85f35b5c`  
		Last Modified: Fri, 12 Nov 2021 18:17:40 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:brie-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b1a9946eaeebb1c00c1400c54ce78bef39faf169fca9f6a595a893c843b72ead
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `traefik:brie-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull traefik@sha256:42357fbc16fa6562f694dbd067f5b3bed471dc95add1250f2ac093c6f0073e91
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2733082630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0e334d0f14b68204e26ab00c216d99705a81caf654aece76109da97517a227c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 19:03:10 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 10 Nov 2021 19:03:12 GMT
EXPOSE 80
# Wed, 10 Nov 2021 19:03:13 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Nov 2021 19:03:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908fd75d4d7401dab2f0ff42955f8f0d742329f415770c4cd0f106b36386e8ca`  
		Last Modified: Wed, 10 Nov 2021 19:05:24 GMT  
		Size: 27.0 MB (26955862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c368cdf7d267763d786cd3906111dc6e50bda11d0503b8abe85752bb7ebad413`  
		Last Modified: Wed, 10 Nov 2021 19:04:54 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f47c40e5c1ec2e7fb9152f280ad6b183350baba9dcf50eaf9f48945b0f00ef`  
		Last Modified: Wed, 10 Nov 2021 19:04:54 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f66e9bd16b34b84de1acbb8aae706a113f9a876d34f5e41fbc6d0411bab824`  
		Last Modified: Wed, 10 Nov 2021 19:04:54 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:b120cca907a99c63ff32e71c25a571c0563a7f905aa63407cb6b27f2b426346e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:212aee66cc6eecbd6a04ef0af0b8616fbc4f716d4c9a52dfa9808b4a8dea5d8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29845535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3bb9550d562ded287f2fc5f71056c652d49cd1ae0ddde3a39acefb3b10dc1ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:28:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 08 Nov 2021 20:51:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 08 Nov 2021 20:51:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 08 Nov 2021 20:51:20 GMT
EXPOSE 80
# Mon, 08 Nov 2021 20:51:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 08 Nov 2021 20:51:21 GMT
CMD ["traefik"]
# Mon, 08 Nov 2021 20:51:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5295d3cd66d0f8651338b81063a408fcc2c70d810c92e5cb435c467a1939d60`  
		Last Modified: Thu, 02 Sep 2021 17:29:12 GMT  
		Size: 656.4 KB (656356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c117e813430bc0788d2b53069f51b9f1387ffaf32a071b5b966237a4e8be398c`  
		Last Modified: Mon, 08 Nov 2021 20:51:51 GMT  
		Size: 26.4 MB (26374365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aedf838ed1f44594dd320fce1909f9563036b91ae4efdbc35f75a5a73473b2d`  
		Last Modified: Mon, 08 Nov 2021 20:51:46 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:c489cc16b0d37e7c0dd106ee095d0481f3ccba3e81f6192affa6bfa07edc85ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28082693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76490c753f69e74602fb79cf36a7893247758dd8d7f4b159c12a83ec4922de99`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:51:34 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 13 Nov 2021 06:51:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Sat, 13 Nov 2021 06:51:45 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 13 Nov 2021 06:51:46 GMT
EXPOSE 80
# Sat, 13 Nov 2021 06:51:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:51:48 GMT
CMD ["traefik"]
# Sat, 13 Nov 2021 06:51:48 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b00cdbc51db9651a9c09390b641face7e18e642e3ff49397c6d477c89c3d7e`  
		Last Modified: Sat, 13 Nov 2021 06:54:26 GMT  
		Size: 683.0 KB (682972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c6a0aef2ab8157f246bbc4e0a2171e4d18ab19258dc3bd97ab2dea6f096f44`  
		Last Modified: Sat, 13 Nov 2021 06:54:36 GMT  
		Size: 24.8 MB (24763961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3910da118b09f25ef883d4a46e512db99a6a9f12a1031790d8b8ffd4c9d606fa`  
		Last Modified: Sat, 13 Nov 2021 06:54:25 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:317dbd98705ff9a2719bb8357e83c496ea70f7caff8aca06b123e1d0862dbee0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27461064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bd5494cab630ed31508338889d5d02c98d6113f9d818584913b8ddd68dd1121`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:16:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 12 Nov 2021 18:16:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 12 Nov 2021 18:16:37 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 12 Nov 2021 18:16:37 GMT
EXPOSE 80
# Fri, 12 Nov 2021 18:16:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 18:16:39 GMT
CMD ["traefik"]
# Fri, 12 Nov 2021 18:16:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cc5a4b7f102f236064e4712164f29c52d256612820409cc28c41a7f5def4a5`  
		Last Modified: Fri, 12 Nov 2021 18:17:40 GMT  
		Size: 680.0 KB (680008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd938bc8aa751ad66221cfd63d8acc173d3ceed14728f87fdac32ed0598cd3af`  
		Last Modified: Fri, 12 Nov 2021 18:17:44 GMT  
		Size: 24.1 MB (24062987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ef3656e6ddb41988a45143ead13d5199714713ea7eee816d82ed9d85f35b5c`  
		Last Modified: Fri, 12 Nov 2021 18:17:40 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles`

```console
$ docker pull traefik@sha256:c28f00fc0070755b8e3fa3befd800dcf4505e631e7627a41c96a0b1de5b7c8c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles` - linux; amd64

```console
$ docker pull traefik@sha256:fd8690c11f1375f07ae9841582868f64628eb7b1e7081e71730c7a992fc8f235
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22591637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85d1b251ae417bc825b2b8d1473d5f4e6451f6cfbadf53fb892e65975a6de1aa`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 05 Oct 2021 17:58:25 GMT
COPY file:c8f727cb8b17c5a8735e609a9b9f333f20765e36c457d0557ed48693a6694880 in /etc/ssl/certs/ 
# Tue, 05 Oct 2021 17:58:26 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 07 Oct 2021 20:04:59 GMT
COPY file:e409355a2ff570f276c91d9f7a80f98e14727655971d95deeb1f7e641b865101 in / 
# Thu, 07 Oct 2021 20:04:59 GMT
EXPOSE 80
# Thu, 07 Oct 2021 20:04:59 GMT
VOLUME [/tmp]
# Thu, 07 Oct 2021 20:04:59 GMT
ENTRYPOINT ["/traefik"]
# Thu, 07 Oct 2021 20:05:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:13e52be55f8d958b3ebb4e73685de5dd10ff4b4af613c4d23424519693aa01e0`  
		Last Modified: Tue, 05 Oct 2021 17:59:12 GMT  
		Size: 122.4 KB (122407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f116118f8a36a09eba9c55ae29c9925e0ae854aa36d9dc1fc271a7be43b820c`  
		Last Modified: Tue, 05 Oct 2021 17:59:11 GMT  
		Size: 308.8 KB (308839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0968db303bdc7c1cd8bedcde2a1d2efaadf77eacdac7f4ad24ff18e990f384b`  
		Last Modified: Thu, 07 Oct 2021 20:06:25 GMT  
		Size: 22.2 MB (22160391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm variant v6

```console
$ docker pull traefik@sha256:d1bf188870da15d1c22f8da3ae6bc614e3581477d3feb4eada90186003f43f3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21069245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a07e35b9622e89560baf105486fce1e43a9e3fef0261c41227dc7e966df4fe7f`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 05 Oct 2021 00:02:38 GMT
COPY file:c8f727cb8b17c5a8735e609a9b9f333f20765e36c457d0557ed48693a6694880 in /etc/ssl/certs/ 
# Sat, 13 Nov 2021 06:52:39 GMT
COPY dir:c22cc1c2c366de443c999e78a53f0bde0b523a72b38a70fa92f5c6322439c95e in /usr/share/ 
# Sat, 13 Nov 2021 06:52:44 GMT
COPY file:37d0f8b70c5da3bdf158098e422d0bfc00d82405c51ca41ee81a5e564433a943 in / 
# Sat, 13 Nov 2021 06:52:45 GMT
EXPOSE 80
# Sat, 13 Nov 2021 06:52:45 GMT
VOLUME [/tmp]
# Sat, 13 Nov 2021 06:52:46 GMT
ENTRYPOINT ["/traefik"]
# Sat, 13 Nov 2021 06:52:46 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:611185932e68f8b41b94235c966a6c2d26bb4a0f053993c6e49edc01123213f9`  
		Last Modified: Tue, 05 Oct 2021 00:04:56 GMT  
		Size: 122.4 KB (122407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81282f8b9fcf1f821d7dab2ed1f6addbda565118cc5ee95d9de4ae8ff91333f`  
		Last Modified: Sat, 13 Nov 2021 06:55:43 GMT  
		Size: 328.6 KB (328578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec6501fe03be7dfb2746de58fa6f69cd43c44f59e5743b529fe980f6f9855c9`  
		Last Modified: Sat, 13 Nov 2021 06:55:52 GMT  
		Size: 20.6 MB (20618260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:731733ac032dea4cea1b9ab054908f17b63ef884e861bd58b5b3d9d3c56257a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20575143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48fc834a31f8efc387885a01430806a70be2becd45240dd06c0441dc6c703e66`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Mon, 08 Nov 2021 20:23:04 GMT
COPY file:c8f727cb8b17c5a8735e609a9b9f333f20765e36c457d0557ed48693a6694880 in /etc/ssl/certs/ 
# Mon, 08 Nov 2021 20:23:05 GMT
COPY dir:c22cc1c2c366de443c999e78a53f0bde0b523a72b38a70fa92f5c6322439c95e in /usr/share/ 
# Mon, 08 Nov 2021 20:23:06 GMT
COPY file:cd6a95e409278a374fb6ef69098a37f7bc0c8d4eddd3ac751de25d783adf1227 in / 
# Mon, 08 Nov 2021 20:23:06 GMT
EXPOSE 80
# Mon, 08 Nov 2021 20:23:07 GMT
VOLUME [/tmp]
# Mon, 08 Nov 2021 20:23:08 GMT
ENTRYPOINT ["/traefik"]
# Mon, 08 Nov 2021 20:23:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:078e101c84a7a75069b9c18efdfc2b24c9840aa136b34eb6e3a0ebe1b74d0a94`  
		Last Modified: Mon, 08 Nov 2021 20:24:37 GMT  
		Size: 122.4 KB (122399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7a624fda7cabc945cc9d9f610f256d933b121fdafa2052d617cf3144bbe2aa`  
		Last Modified: Mon, 08 Nov 2021 20:24:37 GMT  
		Size: 328.5 KB (328545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615fe0c03a3e5c4c76f7ef9722b5a160e05898d03f2ecf3aa00c6f93b560b654`  
		Last Modified: Mon, 08 Nov 2021 20:24:42 GMT  
		Size: 20.1 MB (20124199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-alpine`

```console
$ docker pull traefik@sha256:4c066039f31aee5ffe6f8d810d86a85aa37816caf3767e4880df1207eb48b774
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:a7216aa72c026d4ca0b5fb9cedb5c9e8bf21ba5e3352d4e14ae2ccb0c2ca50f6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25631512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2edc46527be5da9cc20fe71d011f044ef2809203c192636ac1f2457fc11d292`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:28:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 07 Oct 2021 20:04:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 07 Oct 2021 20:04:36 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 07 Oct 2021 20:04:36 GMT
EXPOSE 80
# Thu, 07 Oct 2021 20:04:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Oct 2021 20:04:37 GMT
CMD ["traefik"]
# Thu, 07 Oct 2021 20:04:37 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5295d3cd66d0f8651338b81063a408fcc2c70d810c92e5cb435c467a1939d60`  
		Last Modified: Thu, 02 Sep 2021 17:29:12 GMT  
		Size: 656.4 KB (656356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97ae40f614f61bae620d88f81210f6f68badbd591793811c9d070e8407abfc6`  
		Last Modified: Thu, 07 Oct 2021 20:05:28 GMT  
		Size: 22.2 MB (22160342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a1066c5e04bc425dd4ec2bedad7fee468ce0ef54cc9010d8f5fd1f125bac99`  
		Last Modified: Thu, 07 Oct 2021 20:05:24 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:a52a7bc8595611ebd4be28a1c1ff5f344ae146cff12024496244981d276fcc43
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23937163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10f4734a371bdc50ecea01f7067b4b7b51f929375935f24db4066e86e10b0d9a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:51:34 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 13 Nov 2021 06:52:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Sat, 13 Nov 2021 06:52:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 13 Nov 2021 06:52:17 GMT
EXPOSE 80
# Sat, 13 Nov 2021 06:52:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:52:18 GMT
CMD ["traefik"]
# Sat, 13 Nov 2021 06:52:19 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b00cdbc51db9651a9c09390b641face7e18e642e3ff49397c6d477c89c3d7e`  
		Last Modified: Sat, 13 Nov 2021 06:54:26 GMT  
		Size: 683.0 KB (682972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7034046f5f5ec87c3e6f3f0ec53c2f503aacf02a2b838f771054bc9f0f341a7a`  
		Last Modified: Sat, 13 Nov 2021 06:55:17 GMT  
		Size: 20.6 MB (20618431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bc931b12c3ec19e39c375974b827278a96a38896854112c3dee959f13f709e`  
		Last Modified: Sat, 13 Nov 2021 06:55:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:bf623d4dceb05f5385fdc9b50686849c58ed1bec7b8740daf447cced2c011656
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23522334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8d2cd70545692a5348584b716f1a72a121098a1e94264c03c991e5e462d84e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:16:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 12 Nov 2021 18:16:50 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 12 Nov 2021 18:16:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 12 Nov 2021 18:16:52 GMT
EXPOSE 80
# Fri, 12 Nov 2021 18:16:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 18:16:54 GMT
CMD ["traefik"]
# Fri, 12 Nov 2021 18:16:55 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cc5a4b7f102f236064e4712164f29c52d256612820409cc28c41a7f5def4a5`  
		Last Modified: Fri, 12 Nov 2021 18:17:40 GMT  
		Size: 680.0 KB (680008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3283e6a7888f1f1ba0cfe0b0532a69f6c3036443be824e2bc89580587e0247f`  
		Last Modified: Fri, 12 Nov 2021 18:18:09 GMT  
		Size: 20.1 MB (20124258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9515da1d1aa1c2b9d89c2e66d9b46452fcf8c436e6e86b341cca564107abc3d9`  
		Last Modified: Fri, 12 Nov 2021 18:18:05 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-windowsservercore-1809`

```console
$ docker pull traefik@sha256:8947c337b29375e8b8c7e327209b3ee4ebf835f2f3319131494ee875f43b66b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull traefik@sha256:b6a7d8bd77893cc59a7ed693bcf1d8c8cc97246c872fad9a07a88dad727142f9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728969379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afb6fcd7cb1a41e077e776cecc4b37b62bcdca91a77e351f5baaf9a6e10d6b62`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 19:04:20 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 10 Nov 2021 19:04:22 GMT
EXPOSE 80
# Wed, 10 Nov 2021 19:04:23 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Nov 2021 19:04:24 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbe7df586a8125285cae7dac6ad774b05129e99156a632ea1d20f883029d03c`  
		Last Modified: Wed, 10 Nov 2021 19:05:48 GMT  
		Size: 22.8 MB (22842554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52b885ca238073b5f9093f48de5c52b015ffa93ef1dff1744d9dba6be4d64dc`  
		Last Modified: Wed, 10 Nov 2021 19:05:42 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852f60a1a31dbed66a29d09964528f56907495e407d124284d744ead5697a9bc`  
		Last Modified: Wed, 10 Nov 2021 19:05:42 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa570cc10582d59ee894f65e0e6a6384ab191442f61c45fc2b8a8e9df933576`  
		Last Modified: Wed, 10 Nov 2021 19:05:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7`

```console
$ docker pull traefik@sha256:c28f00fc0070755b8e3fa3befd800dcf4505e631e7627a41c96a0b1de5b7c8c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7` - linux; amd64

```console
$ docker pull traefik@sha256:fd8690c11f1375f07ae9841582868f64628eb7b1e7081e71730c7a992fc8f235
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22591637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85d1b251ae417bc825b2b8d1473d5f4e6451f6cfbadf53fb892e65975a6de1aa`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 05 Oct 2021 17:58:25 GMT
COPY file:c8f727cb8b17c5a8735e609a9b9f333f20765e36c457d0557ed48693a6694880 in /etc/ssl/certs/ 
# Tue, 05 Oct 2021 17:58:26 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 07 Oct 2021 20:04:59 GMT
COPY file:e409355a2ff570f276c91d9f7a80f98e14727655971d95deeb1f7e641b865101 in / 
# Thu, 07 Oct 2021 20:04:59 GMT
EXPOSE 80
# Thu, 07 Oct 2021 20:04:59 GMT
VOLUME [/tmp]
# Thu, 07 Oct 2021 20:04:59 GMT
ENTRYPOINT ["/traefik"]
# Thu, 07 Oct 2021 20:05:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:13e52be55f8d958b3ebb4e73685de5dd10ff4b4af613c4d23424519693aa01e0`  
		Last Modified: Tue, 05 Oct 2021 17:59:12 GMT  
		Size: 122.4 KB (122407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f116118f8a36a09eba9c55ae29c9925e0ae854aa36d9dc1fc271a7be43b820c`  
		Last Modified: Tue, 05 Oct 2021 17:59:11 GMT  
		Size: 308.8 KB (308839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0968db303bdc7c1cd8bedcde2a1d2efaadf77eacdac7f4ad24ff18e990f384b`  
		Last Modified: Thu, 07 Oct 2021 20:06:25 GMT  
		Size: 22.2 MB (22160391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:d1bf188870da15d1c22f8da3ae6bc614e3581477d3feb4eada90186003f43f3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21069245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a07e35b9622e89560baf105486fce1e43a9e3fef0261c41227dc7e966df4fe7f`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 05 Oct 2021 00:02:38 GMT
COPY file:c8f727cb8b17c5a8735e609a9b9f333f20765e36c457d0557ed48693a6694880 in /etc/ssl/certs/ 
# Sat, 13 Nov 2021 06:52:39 GMT
COPY dir:c22cc1c2c366de443c999e78a53f0bde0b523a72b38a70fa92f5c6322439c95e in /usr/share/ 
# Sat, 13 Nov 2021 06:52:44 GMT
COPY file:37d0f8b70c5da3bdf158098e422d0bfc00d82405c51ca41ee81a5e564433a943 in / 
# Sat, 13 Nov 2021 06:52:45 GMT
EXPOSE 80
# Sat, 13 Nov 2021 06:52:45 GMT
VOLUME [/tmp]
# Sat, 13 Nov 2021 06:52:46 GMT
ENTRYPOINT ["/traefik"]
# Sat, 13 Nov 2021 06:52:46 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:611185932e68f8b41b94235c966a6c2d26bb4a0f053993c6e49edc01123213f9`  
		Last Modified: Tue, 05 Oct 2021 00:04:56 GMT  
		Size: 122.4 KB (122407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81282f8b9fcf1f821d7dab2ed1f6addbda565118cc5ee95d9de4ae8ff91333f`  
		Last Modified: Sat, 13 Nov 2021 06:55:43 GMT  
		Size: 328.6 KB (328578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec6501fe03be7dfb2746de58fa6f69cd43c44f59e5743b529fe980f6f9855c9`  
		Last Modified: Sat, 13 Nov 2021 06:55:52 GMT  
		Size: 20.6 MB (20618260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:731733ac032dea4cea1b9ab054908f17b63ef884e861bd58b5b3d9d3c56257a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20575143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48fc834a31f8efc387885a01430806a70be2becd45240dd06c0441dc6c703e66`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Mon, 08 Nov 2021 20:23:04 GMT
COPY file:c8f727cb8b17c5a8735e609a9b9f333f20765e36c457d0557ed48693a6694880 in /etc/ssl/certs/ 
# Mon, 08 Nov 2021 20:23:05 GMT
COPY dir:c22cc1c2c366de443c999e78a53f0bde0b523a72b38a70fa92f5c6322439c95e in /usr/share/ 
# Mon, 08 Nov 2021 20:23:06 GMT
COPY file:cd6a95e409278a374fb6ef69098a37f7bc0c8d4eddd3ac751de25d783adf1227 in / 
# Mon, 08 Nov 2021 20:23:06 GMT
EXPOSE 80
# Mon, 08 Nov 2021 20:23:07 GMT
VOLUME [/tmp]
# Mon, 08 Nov 2021 20:23:08 GMT
ENTRYPOINT ["/traefik"]
# Mon, 08 Nov 2021 20:23:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:078e101c84a7a75069b9c18efdfc2b24c9840aa136b34eb6e3a0ebe1b74d0a94`  
		Last Modified: Mon, 08 Nov 2021 20:24:37 GMT  
		Size: 122.4 KB (122399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7a624fda7cabc945cc9d9f610f256d933b121fdafa2052d617cf3144bbe2aa`  
		Last Modified: Mon, 08 Nov 2021 20:24:37 GMT  
		Size: 328.5 KB (328545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615fe0c03a3e5c4c76f7ef9722b5a160e05898d03f2ecf3aa00c6f93b560b654`  
		Last Modified: Mon, 08 Nov 2021 20:24:42 GMT  
		Size: 20.1 MB (20124199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-alpine`

```console
$ docker pull traefik@sha256:4c066039f31aee5ffe6f8d810d86a85aa37816caf3767e4880df1207eb48b774
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:a7216aa72c026d4ca0b5fb9cedb5c9e8bf21ba5e3352d4e14ae2ccb0c2ca50f6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25631512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2edc46527be5da9cc20fe71d011f044ef2809203c192636ac1f2457fc11d292`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:28:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 07 Oct 2021 20:04:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 07 Oct 2021 20:04:36 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 07 Oct 2021 20:04:36 GMT
EXPOSE 80
# Thu, 07 Oct 2021 20:04:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Oct 2021 20:04:37 GMT
CMD ["traefik"]
# Thu, 07 Oct 2021 20:04:37 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5295d3cd66d0f8651338b81063a408fcc2c70d810c92e5cb435c467a1939d60`  
		Last Modified: Thu, 02 Sep 2021 17:29:12 GMT  
		Size: 656.4 KB (656356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97ae40f614f61bae620d88f81210f6f68badbd591793811c9d070e8407abfc6`  
		Last Modified: Thu, 07 Oct 2021 20:05:28 GMT  
		Size: 22.2 MB (22160342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a1066c5e04bc425dd4ec2bedad7fee468ce0ef54cc9010d8f5fd1f125bac99`  
		Last Modified: Thu, 07 Oct 2021 20:05:24 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:a52a7bc8595611ebd4be28a1c1ff5f344ae146cff12024496244981d276fcc43
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23937163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10f4734a371bdc50ecea01f7067b4b7b51f929375935f24db4066e86e10b0d9a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:51:34 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 13 Nov 2021 06:52:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Sat, 13 Nov 2021 06:52:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 13 Nov 2021 06:52:17 GMT
EXPOSE 80
# Sat, 13 Nov 2021 06:52:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:52:18 GMT
CMD ["traefik"]
# Sat, 13 Nov 2021 06:52:19 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b00cdbc51db9651a9c09390b641face7e18e642e3ff49397c6d477c89c3d7e`  
		Last Modified: Sat, 13 Nov 2021 06:54:26 GMT  
		Size: 683.0 KB (682972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7034046f5f5ec87c3e6f3f0ec53c2f503aacf02a2b838f771054bc9f0f341a7a`  
		Last Modified: Sat, 13 Nov 2021 06:55:17 GMT  
		Size: 20.6 MB (20618431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bc931b12c3ec19e39c375974b827278a96a38896854112c3dee959f13f709e`  
		Last Modified: Sat, 13 Nov 2021 06:55:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:bf623d4dceb05f5385fdc9b50686849c58ed1bec7b8740daf447cced2c011656
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23522334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8d2cd70545692a5348584b716f1a72a121098a1e94264c03c991e5e462d84e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:16:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 12 Nov 2021 18:16:50 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 12 Nov 2021 18:16:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 12 Nov 2021 18:16:52 GMT
EXPOSE 80
# Fri, 12 Nov 2021 18:16:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 18:16:54 GMT
CMD ["traefik"]
# Fri, 12 Nov 2021 18:16:55 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cc5a4b7f102f236064e4712164f29c52d256612820409cc28c41a7f5def4a5`  
		Last Modified: Fri, 12 Nov 2021 18:17:40 GMT  
		Size: 680.0 KB (680008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3283e6a7888f1f1ba0cfe0b0532a69f6c3036443be824e2bc89580587e0247f`  
		Last Modified: Fri, 12 Nov 2021 18:18:09 GMT  
		Size: 20.1 MB (20124258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9515da1d1aa1c2b9d89c2e66d9b46452fcf8c436e6e86b341cca564107abc3d9`  
		Last Modified: Fri, 12 Nov 2021 18:18:05 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:8947c337b29375e8b8c7e327209b3ee4ebf835f2f3319131494ee875f43b66b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `traefik:v1.7-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull traefik@sha256:b6a7d8bd77893cc59a7ed693bcf1d8c8cc97246c872fad9a07a88dad727142f9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728969379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afb6fcd7cb1a41e077e776cecc4b37b62bcdca91a77e351f5baaf9a6e10d6b62`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 19:04:20 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 10 Nov 2021 19:04:22 GMT
EXPOSE 80
# Wed, 10 Nov 2021 19:04:23 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Nov 2021 19:04:24 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbe7df586a8125285cae7dac6ad774b05129e99156a632ea1d20f883029d03c`  
		Last Modified: Wed, 10 Nov 2021 19:05:48 GMT  
		Size: 22.8 MB (22842554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52b885ca238073b5f9093f48de5c52b015ffa93ef1dff1744d9dba6be4d64dc`  
		Last Modified: Wed, 10 Nov 2021 19:05:42 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852f60a1a31dbed66a29d09964528f56907495e407d124284d744ead5697a9bc`  
		Last Modified: Wed, 10 Nov 2021 19:05:42 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa570cc10582d59ee894f65e0e6a6384ab191442f61c45fc2b8a8e9df933576`  
		Last Modified: Wed, 10 Nov 2021 19:05:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.33`

```console
$ docker pull traefik@sha256:c28f00fc0070755b8e3fa3befd800dcf4505e631e7627a41c96a0b1de5b7c8c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.33` - linux; amd64

```console
$ docker pull traefik@sha256:fd8690c11f1375f07ae9841582868f64628eb7b1e7081e71730c7a992fc8f235
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22591637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85d1b251ae417bc825b2b8d1473d5f4e6451f6cfbadf53fb892e65975a6de1aa`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 05 Oct 2021 17:58:25 GMT
COPY file:c8f727cb8b17c5a8735e609a9b9f333f20765e36c457d0557ed48693a6694880 in /etc/ssl/certs/ 
# Tue, 05 Oct 2021 17:58:26 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 07 Oct 2021 20:04:59 GMT
COPY file:e409355a2ff570f276c91d9f7a80f98e14727655971d95deeb1f7e641b865101 in / 
# Thu, 07 Oct 2021 20:04:59 GMT
EXPOSE 80
# Thu, 07 Oct 2021 20:04:59 GMT
VOLUME [/tmp]
# Thu, 07 Oct 2021 20:04:59 GMT
ENTRYPOINT ["/traefik"]
# Thu, 07 Oct 2021 20:05:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:13e52be55f8d958b3ebb4e73685de5dd10ff4b4af613c4d23424519693aa01e0`  
		Last Modified: Tue, 05 Oct 2021 17:59:12 GMT  
		Size: 122.4 KB (122407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f116118f8a36a09eba9c55ae29c9925e0ae854aa36d9dc1fc271a7be43b820c`  
		Last Modified: Tue, 05 Oct 2021 17:59:11 GMT  
		Size: 308.8 KB (308839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0968db303bdc7c1cd8bedcde2a1d2efaadf77eacdac7f4ad24ff18e990f384b`  
		Last Modified: Thu, 07 Oct 2021 20:06:25 GMT  
		Size: 22.2 MB (22160391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.33` - linux; arm variant v6

```console
$ docker pull traefik@sha256:d1bf188870da15d1c22f8da3ae6bc614e3581477d3feb4eada90186003f43f3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21069245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a07e35b9622e89560baf105486fce1e43a9e3fef0261c41227dc7e966df4fe7f`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 05 Oct 2021 00:02:38 GMT
COPY file:c8f727cb8b17c5a8735e609a9b9f333f20765e36c457d0557ed48693a6694880 in /etc/ssl/certs/ 
# Sat, 13 Nov 2021 06:52:39 GMT
COPY dir:c22cc1c2c366de443c999e78a53f0bde0b523a72b38a70fa92f5c6322439c95e in /usr/share/ 
# Sat, 13 Nov 2021 06:52:44 GMT
COPY file:37d0f8b70c5da3bdf158098e422d0bfc00d82405c51ca41ee81a5e564433a943 in / 
# Sat, 13 Nov 2021 06:52:45 GMT
EXPOSE 80
# Sat, 13 Nov 2021 06:52:45 GMT
VOLUME [/tmp]
# Sat, 13 Nov 2021 06:52:46 GMT
ENTRYPOINT ["/traefik"]
# Sat, 13 Nov 2021 06:52:46 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:611185932e68f8b41b94235c966a6c2d26bb4a0f053993c6e49edc01123213f9`  
		Last Modified: Tue, 05 Oct 2021 00:04:56 GMT  
		Size: 122.4 KB (122407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81282f8b9fcf1f821d7dab2ed1f6addbda565118cc5ee95d9de4ae8ff91333f`  
		Last Modified: Sat, 13 Nov 2021 06:55:43 GMT  
		Size: 328.6 KB (328578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec6501fe03be7dfb2746de58fa6f69cd43c44f59e5743b529fe980f6f9855c9`  
		Last Modified: Sat, 13 Nov 2021 06:55:52 GMT  
		Size: 20.6 MB (20618260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.33` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:731733ac032dea4cea1b9ab054908f17b63ef884e861bd58b5b3d9d3c56257a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20575143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48fc834a31f8efc387885a01430806a70be2becd45240dd06c0441dc6c703e66`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Mon, 08 Nov 2021 20:23:04 GMT
COPY file:c8f727cb8b17c5a8735e609a9b9f333f20765e36c457d0557ed48693a6694880 in /etc/ssl/certs/ 
# Mon, 08 Nov 2021 20:23:05 GMT
COPY dir:c22cc1c2c366de443c999e78a53f0bde0b523a72b38a70fa92f5c6322439c95e in /usr/share/ 
# Mon, 08 Nov 2021 20:23:06 GMT
COPY file:cd6a95e409278a374fb6ef69098a37f7bc0c8d4eddd3ac751de25d783adf1227 in / 
# Mon, 08 Nov 2021 20:23:06 GMT
EXPOSE 80
# Mon, 08 Nov 2021 20:23:07 GMT
VOLUME [/tmp]
# Mon, 08 Nov 2021 20:23:08 GMT
ENTRYPOINT ["/traefik"]
# Mon, 08 Nov 2021 20:23:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:078e101c84a7a75069b9c18efdfc2b24c9840aa136b34eb6e3a0ebe1b74d0a94`  
		Last Modified: Mon, 08 Nov 2021 20:24:37 GMT  
		Size: 122.4 KB (122399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7a624fda7cabc945cc9d9f610f256d933b121fdafa2052d617cf3144bbe2aa`  
		Last Modified: Mon, 08 Nov 2021 20:24:37 GMT  
		Size: 328.5 KB (328545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615fe0c03a3e5c4c76f7ef9722b5a160e05898d03f2ecf3aa00c6f93b560b654`  
		Last Modified: Mon, 08 Nov 2021 20:24:42 GMT  
		Size: 20.1 MB (20124199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.33-alpine`

```console
$ docker pull traefik@sha256:4c066039f31aee5ffe6f8d810d86a85aa37816caf3767e4880df1207eb48b774
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.33-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:a7216aa72c026d4ca0b5fb9cedb5c9e8bf21ba5e3352d4e14ae2ccb0c2ca50f6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25631512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2edc46527be5da9cc20fe71d011f044ef2809203c192636ac1f2457fc11d292`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:28:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 07 Oct 2021 20:04:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 07 Oct 2021 20:04:36 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 07 Oct 2021 20:04:36 GMT
EXPOSE 80
# Thu, 07 Oct 2021 20:04:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Oct 2021 20:04:37 GMT
CMD ["traefik"]
# Thu, 07 Oct 2021 20:04:37 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5295d3cd66d0f8651338b81063a408fcc2c70d810c92e5cb435c467a1939d60`  
		Last Modified: Thu, 02 Sep 2021 17:29:12 GMT  
		Size: 656.4 KB (656356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97ae40f614f61bae620d88f81210f6f68badbd591793811c9d070e8407abfc6`  
		Last Modified: Thu, 07 Oct 2021 20:05:28 GMT  
		Size: 22.2 MB (22160342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a1066c5e04bc425dd4ec2bedad7fee468ce0ef54cc9010d8f5fd1f125bac99`  
		Last Modified: Thu, 07 Oct 2021 20:05:24 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.33-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:a52a7bc8595611ebd4be28a1c1ff5f344ae146cff12024496244981d276fcc43
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23937163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10f4734a371bdc50ecea01f7067b4b7b51f929375935f24db4066e86e10b0d9a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:51:34 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 13 Nov 2021 06:52:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Sat, 13 Nov 2021 06:52:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 13 Nov 2021 06:52:17 GMT
EXPOSE 80
# Sat, 13 Nov 2021 06:52:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:52:18 GMT
CMD ["traefik"]
# Sat, 13 Nov 2021 06:52:19 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b00cdbc51db9651a9c09390b641face7e18e642e3ff49397c6d477c89c3d7e`  
		Last Modified: Sat, 13 Nov 2021 06:54:26 GMT  
		Size: 683.0 KB (682972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7034046f5f5ec87c3e6f3f0ec53c2f503aacf02a2b838f771054bc9f0f341a7a`  
		Last Modified: Sat, 13 Nov 2021 06:55:17 GMT  
		Size: 20.6 MB (20618431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bc931b12c3ec19e39c375974b827278a96a38896854112c3dee959f13f709e`  
		Last Modified: Sat, 13 Nov 2021 06:55:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.33-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:bf623d4dceb05f5385fdc9b50686849c58ed1bec7b8740daf447cced2c011656
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23522334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8d2cd70545692a5348584b716f1a72a121098a1e94264c03c991e5e462d84e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:16:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 12 Nov 2021 18:16:50 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 12 Nov 2021 18:16:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 12 Nov 2021 18:16:52 GMT
EXPOSE 80
# Fri, 12 Nov 2021 18:16:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 18:16:54 GMT
CMD ["traefik"]
# Fri, 12 Nov 2021 18:16:55 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cc5a4b7f102f236064e4712164f29c52d256612820409cc28c41a7f5def4a5`  
		Last Modified: Fri, 12 Nov 2021 18:17:40 GMT  
		Size: 680.0 KB (680008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3283e6a7888f1f1ba0cfe0b0532a69f6c3036443be824e2bc89580587e0247f`  
		Last Modified: Fri, 12 Nov 2021 18:18:09 GMT  
		Size: 20.1 MB (20124258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9515da1d1aa1c2b9d89c2e66d9b46452fcf8c436e6e86b341cca564107abc3d9`  
		Last Modified: Fri, 12 Nov 2021 18:18:05 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.33-windowsservercore-1809`

```console
$ docker pull traefik@sha256:8947c337b29375e8b8c7e327209b3ee4ebf835f2f3319131494ee875f43b66b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `traefik:v1.7.33-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull traefik@sha256:b6a7d8bd77893cc59a7ed693bcf1d8c8cc97246c872fad9a07a88dad727142f9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728969379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afb6fcd7cb1a41e077e776cecc4b37b62bcdca91a77e351f5baaf9a6e10d6b62`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 19:04:20 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 10 Nov 2021 19:04:22 GMT
EXPOSE 80
# Wed, 10 Nov 2021 19:04:23 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Nov 2021 19:04:24 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbe7df586a8125285cae7dac6ad774b05129e99156a632ea1d20f883029d03c`  
		Last Modified: Wed, 10 Nov 2021 19:05:48 GMT  
		Size: 22.8 MB (22842554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52b885ca238073b5f9093f48de5c52b015ffa93ef1dff1744d9dba6be4d64dc`  
		Last Modified: Wed, 10 Nov 2021 19:05:42 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852f60a1a31dbed66a29d09964528f56907495e407d124284d744ead5697a9bc`  
		Last Modified: Wed, 10 Nov 2021 19:05:42 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa570cc10582d59ee894f65e0e6a6384ab191442f61c45fc2b8a8e9df933576`  
		Last Modified: Wed, 10 Nov 2021 19:05:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.5`

```console
$ docker pull traefik@sha256:b120cca907a99c63ff32e71c25a571c0563a7f905aa63407cb6b27f2b426346e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.5` - linux; amd64

```console
$ docker pull traefik@sha256:212aee66cc6eecbd6a04ef0af0b8616fbc4f716d4c9a52dfa9808b4a8dea5d8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29845535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3bb9550d562ded287f2fc5f71056c652d49cd1ae0ddde3a39acefb3b10dc1ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:28:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 08 Nov 2021 20:51:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 08 Nov 2021 20:51:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 08 Nov 2021 20:51:20 GMT
EXPOSE 80
# Mon, 08 Nov 2021 20:51:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 08 Nov 2021 20:51:21 GMT
CMD ["traefik"]
# Mon, 08 Nov 2021 20:51:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5295d3cd66d0f8651338b81063a408fcc2c70d810c92e5cb435c467a1939d60`  
		Last Modified: Thu, 02 Sep 2021 17:29:12 GMT  
		Size: 656.4 KB (656356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c117e813430bc0788d2b53069f51b9f1387ffaf32a071b5b966237a4e8be398c`  
		Last Modified: Mon, 08 Nov 2021 20:51:51 GMT  
		Size: 26.4 MB (26374365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aedf838ed1f44594dd320fce1909f9563036b91ae4efdbc35f75a5a73473b2d`  
		Last Modified: Mon, 08 Nov 2021 20:51:46 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.5` - linux; arm variant v6

```console
$ docker pull traefik@sha256:c489cc16b0d37e7c0dd106ee095d0481f3ccba3e81f6192affa6bfa07edc85ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28082693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76490c753f69e74602fb79cf36a7893247758dd8d7f4b159c12a83ec4922de99`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:51:34 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 13 Nov 2021 06:51:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Sat, 13 Nov 2021 06:51:45 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 13 Nov 2021 06:51:46 GMT
EXPOSE 80
# Sat, 13 Nov 2021 06:51:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:51:48 GMT
CMD ["traefik"]
# Sat, 13 Nov 2021 06:51:48 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b00cdbc51db9651a9c09390b641face7e18e642e3ff49397c6d477c89c3d7e`  
		Last Modified: Sat, 13 Nov 2021 06:54:26 GMT  
		Size: 683.0 KB (682972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c6a0aef2ab8157f246bbc4e0a2171e4d18ab19258dc3bd97ab2dea6f096f44`  
		Last Modified: Sat, 13 Nov 2021 06:54:36 GMT  
		Size: 24.8 MB (24763961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3910da118b09f25ef883d4a46e512db99a6a9f12a1031790d8b8ffd4c9d606fa`  
		Last Modified: Sat, 13 Nov 2021 06:54:25 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.5` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:317dbd98705ff9a2719bb8357e83c496ea70f7caff8aca06b123e1d0862dbee0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27461064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bd5494cab630ed31508338889d5d02c98d6113f9d818584913b8ddd68dd1121`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:16:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 12 Nov 2021 18:16:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 12 Nov 2021 18:16:37 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 12 Nov 2021 18:16:37 GMT
EXPOSE 80
# Fri, 12 Nov 2021 18:16:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 18:16:39 GMT
CMD ["traefik"]
# Fri, 12 Nov 2021 18:16:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cc5a4b7f102f236064e4712164f29c52d256612820409cc28c41a7f5def4a5`  
		Last Modified: Fri, 12 Nov 2021 18:17:40 GMT  
		Size: 680.0 KB (680008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd938bc8aa751ad66221cfd63d8acc173d3ceed14728f87fdac32ed0598cd3af`  
		Last Modified: Fri, 12 Nov 2021 18:17:44 GMT  
		Size: 24.1 MB (24062987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ef3656e6ddb41988a45143ead13d5199714713ea7eee816d82ed9d85f35b5c`  
		Last Modified: Fri, 12 Nov 2021 18:17:40 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.5-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b1a9946eaeebb1c00c1400c54ce78bef39faf169fca9f6a595a893c843b72ead
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `traefik:v2.5-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull traefik@sha256:42357fbc16fa6562f694dbd067f5b3bed471dc95add1250f2ac093c6f0073e91
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2733082630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0e334d0f14b68204e26ab00c216d99705a81caf654aece76109da97517a227c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 19:03:10 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 10 Nov 2021 19:03:12 GMT
EXPOSE 80
# Wed, 10 Nov 2021 19:03:13 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Nov 2021 19:03:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908fd75d4d7401dab2f0ff42955f8f0d742329f415770c4cd0f106b36386e8ca`  
		Last Modified: Wed, 10 Nov 2021 19:05:24 GMT  
		Size: 27.0 MB (26955862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c368cdf7d267763d786cd3906111dc6e50bda11d0503b8abe85752bb7ebad413`  
		Last Modified: Wed, 10 Nov 2021 19:04:54 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f47c40e5c1ec2e7fb9152f280ad6b183350baba9dcf50eaf9f48945b0f00ef`  
		Last Modified: Wed, 10 Nov 2021 19:04:54 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f66e9bd16b34b84de1acbb8aae706a113f9a876d34f5e41fbc6d0411bab824`  
		Last Modified: Wed, 10 Nov 2021 19:04:54 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.5.4`

```console
$ docker pull traefik@sha256:b120cca907a99c63ff32e71c25a571c0563a7f905aa63407cb6b27f2b426346e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.5.4` - linux; amd64

```console
$ docker pull traefik@sha256:212aee66cc6eecbd6a04ef0af0b8616fbc4f716d4c9a52dfa9808b4a8dea5d8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29845535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3bb9550d562ded287f2fc5f71056c652d49cd1ae0ddde3a39acefb3b10dc1ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:28:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 08 Nov 2021 20:51:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 08 Nov 2021 20:51:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 08 Nov 2021 20:51:20 GMT
EXPOSE 80
# Mon, 08 Nov 2021 20:51:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 08 Nov 2021 20:51:21 GMT
CMD ["traefik"]
# Mon, 08 Nov 2021 20:51:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5295d3cd66d0f8651338b81063a408fcc2c70d810c92e5cb435c467a1939d60`  
		Last Modified: Thu, 02 Sep 2021 17:29:12 GMT  
		Size: 656.4 KB (656356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c117e813430bc0788d2b53069f51b9f1387ffaf32a071b5b966237a4e8be398c`  
		Last Modified: Mon, 08 Nov 2021 20:51:51 GMT  
		Size: 26.4 MB (26374365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aedf838ed1f44594dd320fce1909f9563036b91ae4efdbc35f75a5a73473b2d`  
		Last Modified: Mon, 08 Nov 2021 20:51:46 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.5.4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:c489cc16b0d37e7c0dd106ee095d0481f3ccba3e81f6192affa6bfa07edc85ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28082693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76490c753f69e74602fb79cf36a7893247758dd8d7f4b159c12a83ec4922de99`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:51:34 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 13 Nov 2021 06:51:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Sat, 13 Nov 2021 06:51:45 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 13 Nov 2021 06:51:46 GMT
EXPOSE 80
# Sat, 13 Nov 2021 06:51:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:51:48 GMT
CMD ["traefik"]
# Sat, 13 Nov 2021 06:51:48 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b00cdbc51db9651a9c09390b641face7e18e642e3ff49397c6d477c89c3d7e`  
		Last Modified: Sat, 13 Nov 2021 06:54:26 GMT  
		Size: 683.0 KB (682972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c6a0aef2ab8157f246bbc4e0a2171e4d18ab19258dc3bd97ab2dea6f096f44`  
		Last Modified: Sat, 13 Nov 2021 06:54:36 GMT  
		Size: 24.8 MB (24763961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3910da118b09f25ef883d4a46e512db99a6a9f12a1031790d8b8ffd4c9d606fa`  
		Last Modified: Sat, 13 Nov 2021 06:54:25 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.5.4` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:317dbd98705ff9a2719bb8357e83c496ea70f7caff8aca06b123e1d0862dbee0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27461064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bd5494cab630ed31508338889d5d02c98d6113f9d818584913b8ddd68dd1121`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:16:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 12 Nov 2021 18:16:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 12 Nov 2021 18:16:37 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 12 Nov 2021 18:16:37 GMT
EXPOSE 80
# Fri, 12 Nov 2021 18:16:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 18:16:39 GMT
CMD ["traefik"]
# Fri, 12 Nov 2021 18:16:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cc5a4b7f102f236064e4712164f29c52d256612820409cc28c41a7f5def4a5`  
		Last Modified: Fri, 12 Nov 2021 18:17:40 GMT  
		Size: 680.0 KB (680008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd938bc8aa751ad66221cfd63d8acc173d3ceed14728f87fdac32ed0598cd3af`  
		Last Modified: Fri, 12 Nov 2021 18:17:44 GMT  
		Size: 24.1 MB (24062987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ef3656e6ddb41988a45143ead13d5199714713ea7eee816d82ed9d85f35b5c`  
		Last Modified: Fri, 12 Nov 2021 18:17:40 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.5.4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b1a9946eaeebb1c00c1400c54ce78bef39faf169fca9f6a595a893c843b72ead
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `traefik:v2.5.4-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull traefik@sha256:42357fbc16fa6562f694dbd067f5b3bed471dc95add1250f2ac093c6f0073e91
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2733082630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0e334d0f14b68204e26ab00c216d99705a81caf654aece76109da97517a227c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 19:03:10 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 10 Nov 2021 19:03:12 GMT
EXPOSE 80
# Wed, 10 Nov 2021 19:03:13 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Nov 2021 19:03:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908fd75d4d7401dab2f0ff42955f8f0d742329f415770c4cd0f106b36386e8ca`  
		Last Modified: Wed, 10 Nov 2021 19:05:24 GMT  
		Size: 27.0 MB (26955862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c368cdf7d267763d786cd3906111dc6e50bda11d0503b8abe85752bb7ebad413`  
		Last Modified: Wed, 10 Nov 2021 19:04:54 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f47c40e5c1ec2e7fb9152f280ad6b183350baba9dcf50eaf9f48945b0f00ef`  
		Last Modified: Wed, 10 Nov 2021 19:04:54 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f66e9bd16b34b84de1acbb8aae706a113f9a876d34f5e41fbc6d0411bab824`  
		Last Modified: Wed, 10 Nov 2021 19:04:54 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:b1a9946eaeebb1c00c1400c54ce78bef39faf169fca9f6a595a893c843b72ead
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull traefik@sha256:42357fbc16fa6562f694dbd067f5b3bed471dc95add1250f2ac093c6f0073e91
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2733082630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0e334d0f14b68204e26ab00c216d99705a81caf654aece76109da97517a227c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 19:03:10 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 10 Nov 2021 19:03:12 GMT
EXPOSE 80
# Wed, 10 Nov 2021 19:03:13 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Nov 2021 19:03:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908fd75d4d7401dab2f0ff42955f8f0d742329f415770c4cd0f106b36386e8ca`  
		Last Modified: Wed, 10 Nov 2021 19:05:24 GMT  
		Size: 27.0 MB (26955862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c368cdf7d267763d786cd3906111dc6e50bda11d0503b8abe85752bb7ebad413`  
		Last Modified: Wed, 10 Nov 2021 19:04:54 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f47c40e5c1ec2e7fb9152f280ad6b183350baba9dcf50eaf9f48945b0f00ef`  
		Last Modified: Wed, 10 Nov 2021 19:04:54 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f66e9bd16b34b84de1acbb8aae706a113f9a876d34f5e41fbc6d0411bab824`  
		Last Modified: Wed, 10 Nov 2021 19:04:54 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
