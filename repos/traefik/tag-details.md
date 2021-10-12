<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:1.7`](#traefik17)
-	[`traefik:1.7.33`](#traefik1733)
-	[`traefik:1.7.33-alpine`](#traefik1733-alpine)
-	[`traefik:1.7.33-windowsservercore-1809`](#traefik1733-windowsservercore-1809)
-	[`traefik:1.7-alpine`](#traefik17-alpine)
-	[`traefik:1.7-windowsservercore-1809`](#traefik17-windowsservercore-1809)
-	[`traefik:2.5`](#traefik25)
-	[`traefik:2.5.3`](#traefik253)
-	[`traefik:2.5.3-windowsservercore-1809`](#traefik253-windowsservercore-1809)
-	[`traefik:2.5-windowsservercore-1809`](#traefik25-windowsservercore-1809)
-	[`traefik:brie`](#traefikbrie)
-	[`traefik:brie-windowsservercore-1809`](#traefikbrie-windowsservercore-1809)
-	[`traefik:latest`](#traefiklatest)
-	[`traefik:maroilles`](#traefikmaroilles)
-	[`traefik:maroilles-alpine`](#traefikmaroilles-alpine)
-	[`traefik:maroilles-windowsservercore-1809`](#traefikmaroilles-windowsservercore-1809)
-	[`traefik:v1.7`](#traefikv17)
-	[`traefik:v1.7.33`](#traefikv1733)
-	[`traefik:v1.7.33-alpine`](#traefikv1733-alpine)
-	[`traefik:v1.7.33-windowsservercore-1809`](#traefikv1733-windowsservercore-1809)
-	[`traefik:v1.7-alpine`](#traefikv17-alpine)
-	[`traefik:v1.7-windowsservercore-1809`](#traefikv17-windowsservercore-1809)
-	[`traefik:v2.5`](#traefikv25)
-	[`traefik:v2.5.3`](#traefikv253)
-	[`traefik:v2.5.3-windowsservercore-1809`](#traefikv253-windowsservercore-1809)
-	[`traefik:v2.5-windowsservercore-1809`](#traefikv25-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:1.7`

```console
$ docker pull traefik@sha256:480a9b5c640886b8171757f3ca3dee3df74e25469df8ffbf8cc23a780ae17f0e
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
$ docker pull traefik@sha256:a9115bd64291c28569b4da6603043fe5c5f77b67ac16c9573a639842d19f55f6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.0 MB (21049536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa32dfeccdefca2de2d0b79a80eed77609a1a3e53683324ce24ccb1eec093cb0`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 05 Oct 2021 00:02:38 GMT
COPY file:c8f727cb8b17c5a8735e609a9b9f333f20765e36c457d0557ed48693a6694880 in /etc/ssl/certs/ 
# Tue, 05 Oct 2021 00:02:40 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 07 Oct 2021 19:31:28 GMT
COPY file:37d0f8b70c5da3bdf158098e422d0bfc00d82405c51ca41ee81a5e564433a943 in / 
# Thu, 07 Oct 2021 19:31:29 GMT
EXPOSE 80
# Thu, 07 Oct 2021 19:31:29 GMT
VOLUME [/tmp]
# Thu, 07 Oct 2021 19:31:30 GMT
ENTRYPOINT ["/traefik"]
# Thu, 07 Oct 2021 19:31:30 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:611185932e68f8b41b94235c966a6c2d26bb4a0f053993c6e49edc01123213f9`  
		Last Modified: Tue, 05 Oct 2021 00:04:56 GMT  
		Size: 122.4 KB (122407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07230710ce3c527700e0de335b44592e9a29b741a0fd3b5c78768beb4d5378e`  
		Last Modified: Tue, 05 Oct 2021 00:04:56 GMT  
		Size: 308.9 KB (308869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58879bf3ff90c00bf7b32d71c06d81a17679e973ce7bf8c2e6cdaac88ab37518`  
		Last Modified: Thu, 07 Oct 2021 19:33:51 GMT  
		Size: 20.6 MB (20618260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9d7e644bda91d73cdc6d25422b9b1fa9bc078f7af84afda4950854bb14e9dc8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20555472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c43fb1698cff19b134d727d7575eb7850b10576ee52b6c8987baa9af24ae2b2`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Mon, 04 Oct 2021 23:44:22 GMT
COPY file:c8f727cb8b17c5a8735e609a9b9f333f20765e36c457d0557ed48693a6694880 in /etc/ssl/certs/ 
# Mon, 04 Oct 2021 23:44:23 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 07 Oct 2021 19:39:58 GMT
COPY file:cd6a95e409278a374fb6ef69098a37f7bc0c8d4eddd3ac751de25d783adf1227 in / 
# Thu, 07 Oct 2021 19:39:58 GMT
EXPOSE 80
# Thu, 07 Oct 2021 19:39:58 GMT
VOLUME [/tmp]
# Thu, 07 Oct 2021 19:39:58 GMT
ENTRYPOINT ["/traefik"]
# Thu, 07 Oct 2021 19:39:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:3c562953a5524a25157fc08c1e7009693f341518b2dcfdcab8ae04d990438254`  
		Last Modified: Mon, 04 Oct 2021 23:45:36 GMT  
		Size: 122.4 KB (122408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086b385acba426fecb8a1f24e7e5b29c5b3dfdf54524653104e29d181dcbcd5b`  
		Last Modified: Mon, 04 Oct 2021 23:45:36 GMT  
		Size: 308.9 KB (308866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baba49691f4c4477b848e632ac02b60345178820d53252af24c6e0100ae6f1ee`  
		Last Modified: Thu, 07 Oct 2021 19:41:12 GMT  
		Size: 20.1 MB (20124198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.33`

```console
$ docker pull traefik@sha256:480a9b5c640886b8171757f3ca3dee3df74e25469df8ffbf8cc23a780ae17f0e
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
$ docker pull traefik@sha256:a9115bd64291c28569b4da6603043fe5c5f77b67ac16c9573a639842d19f55f6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.0 MB (21049536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa32dfeccdefca2de2d0b79a80eed77609a1a3e53683324ce24ccb1eec093cb0`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 05 Oct 2021 00:02:38 GMT
COPY file:c8f727cb8b17c5a8735e609a9b9f333f20765e36c457d0557ed48693a6694880 in /etc/ssl/certs/ 
# Tue, 05 Oct 2021 00:02:40 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 07 Oct 2021 19:31:28 GMT
COPY file:37d0f8b70c5da3bdf158098e422d0bfc00d82405c51ca41ee81a5e564433a943 in / 
# Thu, 07 Oct 2021 19:31:29 GMT
EXPOSE 80
# Thu, 07 Oct 2021 19:31:29 GMT
VOLUME [/tmp]
# Thu, 07 Oct 2021 19:31:30 GMT
ENTRYPOINT ["/traefik"]
# Thu, 07 Oct 2021 19:31:30 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:611185932e68f8b41b94235c966a6c2d26bb4a0f053993c6e49edc01123213f9`  
		Last Modified: Tue, 05 Oct 2021 00:04:56 GMT  
		Size: 122.4 KB (122407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07230710ce3c527700e0de335b44592e9a29b741a0fd3b5c78768beb4d5378e`  
		Last Modified: Tue, 05 Oct 2021 00:04:56 GMT  
		Size: 308.9 KB (308869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58879bf3ff90c00bf7b32d71c06d81a17679e973ce7bf8c2e6cdaac88ab37518`  
		Last Modified: Thu, 07 Oct 2021 19:33:51 GMT  
		Size: 20.6 MB (20618260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.33` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9d7e644bda91d73cdc6d25422b9b1fa9bc078f7af84afda4950854bb14e9dc8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20555472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c43fb1698cff19b134d727d7575eb7850b10576ee52b6c8987baa9af24ae2b2`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Mon, 04 Oct 2021 23:44:22 GMT
COPY file:c8f727cb8b17c5a8735e609a9b9f333f20765e36c457d0557ed48693a6694880 in /etc/ssl/certs/ 
# Mon, 04 Oct 2021 23:44:23 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 07 Oct 2021 19:39:58 GMT
COPY file:cd6a95e409278a374fb6ef69098a37f7bc0c8d4eddd3ac751de25d783adf1227 in / 
# Thu, 07 Oct 2021 19:39:58 GMT
EXPOSE 80
# Thu, 07 Oct 2021 19:39:58 GMT
VOLUME [/tmp]
# Thu, 07 Oct 2021 19:39:58 GMT
ENTRYPOINT ["/traefik"]
# Thu, 07 Oct 2021 19:39:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:3c562953a5524a25157fc08c1e7009693f341518b2dcfdcab8ae04d990438254`  
		Last Modified: Mon, 04 Oct 2021 23:45:36 GMT  
		Size: 122.4 KB (122408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086b385acba426fecb8a1f24e7e5b29c5b3dfdf54524653104e29d181dcbcd5b`  
		Last Modified: Mon, 04 Oct 2021 23:45:36 GMT  
		Size: 308.9 KB (308866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baba49691f4c4477b848e632ac02b60345178820d53252af24c6e0100ae6f1ee`  
		Last Modified: Thu, 07 Oct 2021 19:41:12 GMT  
		Size: 20.1 MB (20124198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.33-alpine`

```console
$ docker pull traefik@sha256:fb358034c340794bd43c591002c926382820df7205e65c0879f3e70385e51322
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
$ docker pull traefik@sha256:14c6316a9d20558e4d28e13d6a6eb4e6f3199cc47e1d5287ef8d482849b4ec52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23908243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:629912e245f4d430278f3e14ef32be01ea70c04ae40e131d7d39bf0042d00c63`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 18:16:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 07 Oct 2021 19:31:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 07 Oct 2021 19:31:06 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 07 Oct 2021 19:31:06 GMT
EXPOSE 80
# Thu, 07 Oct 2021 19:31:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Oct 2021 19:31:07 GMT
CMD ["traefik"]
# Thu, 07 Oct 2021 19:31:08 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac532a93bbc80e8fcf54dcb6ef0229a94aa4f2c94f0e9afec75226cfd91451c`  
		Last Modified: Thu, 02 Sep 2021 18:17:59 GMT  
		Size: 662.0 KB (661991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62b9cbace357f1af4892553b0e7d5985c60f32d1401fe4991432ec1028bd2ae`  
		Last Modified: Thu, 07 Oct 2021 19:33:14 GMT  
		Size: 20.6 MB (20618436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a3411058b7ed63da77792b8c2e2ccf0bc0ff03528e597a3c75e6ee529ff4b9`  
		Last Modified: Thu, 07 Oct 2021 19:33:00 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.33-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:4d46f44cb8f6e923a789bce72bb21ac3e3f17b1bb1c0afeae696d111b68ae0a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23495299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a99fbda519f3c0712c4582233fe0106e3cf17204799fdda7b18ec7b7be27f9b9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:46:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 07 Oct 2021 19:39:44 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 07 Oct 2021 19:39:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 07 Oct 2021 19:39:44 GMT
EXPOSE 80
# Thu, 07 Oct 2021 19:39:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Oct 2021 19:39:44 GMT
CMD ["traefik"]
# Thu, 07 Oct 2021 19:39:45 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55b5f395e28da206554aa30d5732a9b9a134cb909215e47a12301afbb1dba15`  
		Last Modified: Thu, 02 Sep 2021 17:47:55 GMT  
		Size: 658.9 KB (658858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814fda492f8bb5f7a9175b058062dc3347924a09e9d05326d780c86ff219ddf1`  
		Last Modified: Thu, 07 Oct 2021 19:40:47 GMT  
		Size: 20.1 MB (20124247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf21937c0359e10bf99379e506ad7dfe0e56dc2fd8911234b935558480ff38e0`  
		Last Modified: Thu, 07 Oct 2021 19:40:44 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.33-windowsservercore-1809`

```console
$ docker pull traefik@sha256:1b2705448077d8cc37f49f9185485d7d77f7872a8ca1bd5569c6e447d1ccd83f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `traefik:1.7.33-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull traefik@sha256:437bb3298f50ba92370d44507a0810b57791e10056e7968d99287bc9957bb366
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2709549668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12bf5af8e35c139620f26df2edcc883c7c6add7c30d9601fac329bc574e62a92`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 07 Oct 2021 19:18:36 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 07 Oct 2021 19:18:37 GMT
EXPOSE 80
# Thu, 07 Oct 2021 19:18:38 GMT
ENTRYPOINT ["/traefik"]
# Thu, 07 Oct 2021 19:18:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e6a78c2cc1b3b87f01fe5643ca6635c8d84211449dcdbca2f40485cc4d0732`  
		Last Modified: Thu, 07 Oct 2021 19:19:14 GMT  
		Size: 22.8 MB (22846068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c1b67f1976804b7e4436fca932b868aefafab88a428c407fedd2a158ee7fc1`  
		Last Modified: Thu, 07 Oct 2021 19:19:08 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f02d143ace29a045b87e7c7d8166bfce2e26c53563e6267847323f67779d86`  
		Last Modified: Thu, 07 Oct 2021 19:19:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364f6175eb5c6e45ec71345b85c48e45bc32fd0d18dab39a71d8eb5bc8df1161`  
		Last Modified: Thu, 07 Oct 2021 19:19:08 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-alpine`

```console
$ docker pull traefik@sha256:fb358034c340794bd43c591002c926382820df7205e65c0879f3e70385e51322
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
$ docker pull traefik@sha256:14c6316a9d20558e4d28e13d6a6eb4e6f3199cc47e1d5287ef8d482849b4ec52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23908243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:629912e245f4d430278f3e14ef32be01ea70c04ae40e131d7d39bf0042d00c63`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 18:16:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 07 Oct 2021 19:31:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 07 Oct 2021 19:31:06 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 07 Oct 2021 19:31:06 GMT
EXPOSE 80
# Thu, 07 Oct 2021 19:31:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Oct 2021 19:31:07 GMT
CMD ["traefik"]
# Thu, 07 Oct 2021 19:31:08 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac532a93bbc80e8fcf54dcb6ef0229a94aa4f2c94f0e9afec75226cfd91451c`  
		Last Modified: Thu, 02 Sep 2021 18:17:59 GMT  
		Size: 662.0 KB (661991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62b9cbace357f1af4892553b0e7d5985c60f32d1401fe4991432ec1028bd2ae`  
		Last Modified: Thu, 07 Oct 2021 19:33:14 GMT  
		Size: 20.6 MB (20618436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a3411058b7ed63da77792b8c2e2ccf0bc0ff03528e597a3c75e6ee529ff4b9`  
		Last Modified: Thu, 07 Oct 2021 19:33:00 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:4d46f44cb8f6e923a789bce72bb21ac3e3f17b1bb1c0afeae696d111b68ae0a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23495299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a99fbda519f3c0712c4582233fe0106e3cf17204799fdda7b18ec7b7be27f9b9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:46:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 07 Oct 2021 19:39:44 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 07 Oct 2021 19:39:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 07 Oct 2021 19:39:44 GMT
EXPOSE 80
# Thu, 07 Oct 2021 19:39:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Oct 2021 19:39:44 GMT
CMD ["traefik"]
# Thu, 07 Oct 2021 19:39:45 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55b5f395e28da206554aa30d5732a9b9a134cb909215e47a12301afbb1dba15`  
		Last Modified: Thu, 02 Sep 2021 17:47:55 GMT  
		Size: 658.9 KB (658858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814fda492f8bb5f7a9175b058062dc3347924a09e9d05326d780c86ff219ddf1`  
		Last Modified: Thu, 07 Oct 2021 19:40:47 GMT  
		Size: 20.1 MB (20124247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf21937c0359e10bf99379e506ad7dfe0e56dc2fd8911234b935558480ff38e0`  
		Last Modified: Thu, 07 Oct 2021 19:40:44 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:1b2705448077d8cc37f49f9185485d7d77f7872a8ca1bd5569c6e447d1ccd83f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `traefik:1.7-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull traefik@sha256:437bb3298f50ba92370d44507a0810b57791e10056e7968d99287bc9957bb366
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2709549668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12bf5af8e35c139620f26df2edcc883c7c6add7c30d9601fac329bc574e62a92`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 07 Oct 2021 19:18:36 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 07 Oct 2021 19:18:37 GMT
EXPOSE 80
# Thu, 07 Oct 2021 19:18:38 GMT
ENTRYPOINT ["/traefik"]
# Thu, 07 Oct 2021 19:18:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e6a78c2cc1b3b87f01fe5643ca6635c8d84211449dcdbca2f40485cc4d0732`  
		Last Modified: Thu, 07 Oct 2021 19:19:14 GMT  
		Size: 22.8 MB (22846068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c1b67f1976804b7e4436fca932b868aefafab88a428c407fedd2a158ee7fc1`  
		Last Modified: Thu, 07 Oct 2021 19:19:08 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f02d143ace29a045b87e7c7d8166bfce2e26c53563e6267847323f67779d86`  
		Last Modified: Thu, 07 Oct 2021 19:19:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364f6175eb5c6e45ec71345b85c48e45bc32fd0d18dab39a71d8eb5bc8df1161`  
		Last Modified: Thu, 07 Oct 2021 19:19:08 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.5`

```console
$ docker pull traefik@sha256:f40028d9771cb29a35392b4cbdd655625596a319b915061e306c503059d0b6f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.5` - linux; amd64

```console
$ docker pull traefik@sha256:b3f4abc5706a00dc886b8b8483dbadf691314d6000f7f2f8736bfe9158cfddbf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29057668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d933d21fd8a09022ca5cf067fb195fbfccf0f5c2b5d750d2d1d6eb562b6a8b23`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:28:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Sep 2021 22:33:57 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.3/traefik_v2.5.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Sep 2021 22:33:57 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Sep 2021 22:33:57 GMT
EXPOSE 80
# Mon, 20 Sep 2021 22:33:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Sep 2021 22:33:58 GMT
CMD ["traefik"]
# Mon, 20 Sep 2021 22:33:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:709a291a928e2c186dfda0482997e46082d5f3f59ece15af68d716daaece906a`  
		Last Modified: Mon, 20 Sep 2021 22:34:29 GMT  
		Size: 25.6 MB (25586499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2367d83d5091433850e079372929625c34f7297930b7c5853c4af8740df8c470`  
		Last Modified: Mon, 20 Sep 2021 22:34:24 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.5` - linux; arm variant v6

```console
$ docker pull traefik@sha256:e12c0a18cae5675bbc0c133f445b96489fbf6617c66ebf254aa4499b5e4bce04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27303193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:439f235df3e981ae502eea1719af18b8fdf666ff7adf6602fd7522a02428fe2d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 18:16:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Sep 2021 23:02:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.3/traefik_v2.5.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Sep 2021 23:02:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Sep 2021 23:02:06 GMT
EXPOSE 80
# Mon, 20 Sep 2021 23:02:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Sep 2021 23:02:06 GMT
CMD ["traefik"]
# Mon, 20 Sep 2021 23:02:07 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac532a93bbc80e8fcf54dcb6ef0229a94aa4f2c94f0e9afec75226cfd91451c`  
		Last Modified: Thu, 02 Sep 2021 18:17:59 GMT  
		Size: 662.0 KB (661991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06452c3a5e8e127597025204daab5d7e08fd26a9604e469bffead7c88192f263`  
		Last Modified: Mon, 20 Sep 2021 23:04:10 GMT  
		Size: 24.0 MB (24013387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c9059e1c58be06e68f3ff3d92f20dc6295e8bbd7a588693346718bf872ee57`  
		Last Modified: Mon, 20 Sep 2021 23:03:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.5` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:642ea446082cd3cd29a00d89447be819f0e1226e0c2643cb5ecfc9259c2d85e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26720590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:026ae4c43ba7bf101b11c8a12d09e3a0bc6858ac98433c5b9c0133b379b6c36b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:46:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Sep 2021 22:44:57 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.3/traefik_v2.5.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Sep 2021 22:44:58 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Sep 2021 22:44:58 GMT
EXPOSE 80
# Mon, 20 Sep 2021 22:44:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Sep 2021 22:44:58 GMT
CMD ["traefik"]
# Mon, 20 Sep 2021 22:44:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55b5f395e28da206554aa30d5732a9b9a134cb909215e47a12301afbb1dba15`  
		Last Modified: Thu, 02 Sep 2021 17:47:55 GMT  
		Size: 658.9 KB (658858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef03ca17e72ecae6b44198d22bbcbf2a29c03bfdc2e63a0083dc77967bbd8b9`  
		Last Modified: Mon, 20 Sep 2021 22:45:57 GMT  
		Size: 23.3 MB (23349537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267983b7cc1765fa911ad76ce5d7d6c3ff57cf87ae52ff4a8cf79bd810aa8ce3`  
		Last Modified: Mon, 20 Sep 2021 22:45:53 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.5.3`

```console
$ docker pull traefik@sha256:f40028d9771cb29a35392b4cbdd655625596a319b915061e306c503059d0b6f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.5.3` - linux; amd64

```console
$ docker pull traefik@sha256:b3f4abc5706a00dc886b8b8483dbadf691314d6000f7f2f8736bfe9158cfddbf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29057668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d933d21fd8a09022ca5cf067fb195fbfccf0f5c2b5d750d2d1d6eb562b6a8b23`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:28:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Sep 2021 22:33:57 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.3/traefik_v2.5.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Sep 2021 22:33:57 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Sep 2021 22:33:57 GMT
EXPOSE 80
# Mon, 20 Sep 2021 22:33:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Sep 2021 22:33:58 GMT
CMD ["traefik"]
# Mon, 20 Sep 2021 22:33:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:709a291a928e2c186dfda0482997e46082d5f3f59ece15af68d716daaece906a`  
		Last Modified: Mon, 20 Sep 2021 22:34:29 GMT  
		Size: 25.6 MB (25586499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2367d83d5091433850e079372929625c34f7297930b7c5853c4af8740df8c470`  
		Last Modified: Mon, 20 Sep 2021 22:34:24 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.5.3` - linux; arm variant v6

```console
$ docker pull traefik@sha256:e12c0a18cae5675bbc0c133f445b96489fbf6617c66ebf254aa4499b5e4bce04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27303193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:439f235df3e981ae502eea1719af18b8fdf666ff7adf6602fd7522a02428fe2d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 18:16:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Sep 2021 23:02:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.3/traefik_v2.5.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Sep 2021 23:02:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Sep 2021 23:02:06 GMT
EXPOSE 80
# Mon, 20 Sep 2021 23:02:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Sep 2021 23:02:06 GMT
CMD ["traefik"]
# Mon, 20 Sep 2021 23:02:07 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac532a93bbc80e8fcf54dcb6ef0229a94aa4f2c94f0e9afec75226cfd91451c`  
		Last Modified: Thu, 02 Sep 2021 18:17:59 GMT  
		Size: 662.0 KB (661991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06452c3a5e8e127597025204daab5d7e08fd26a9604e469bffead7c88192f263`  
		Last Modified: Mon, 20 Sep 2021 23:04:10 GMT  
		Size: 24.0 MB (24013387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c9059e1c58be06e68f3ff3d92f20dc6295e8bbd7a588693346718bf872ee57`  
		Last Modified: Mon, 20 Sep 2021 23:03:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.5.3` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:642ea446082cd3cd29a00d89447be819f0e1226e0c2643cb5ecfc9259c2d85e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26720590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:026ae4c43ba7bf101b11c8a12d09e3a0bc6858ac98433c5b9c0133b379b6c36b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:46:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Sep 2021 22:44:57 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.3/traefik_v2.5.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Sep 2021 22:44:58 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Sep 2021 22:44:58 GMT
EXPOSE 80
# Mon, 20 Sep 2021 22:44:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Sep 2021 22:44:58 GMT
CMD ["traefik"]
# Mon, 20 Sep 2021 22:44:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55b5f395e28da206554aa30d5732a9b9a134cb909215e47a12301afbb1dba15`  
		Last Modified: Thu, 02 Sep 2021 17:47:55 GMT  
		Size: 658.9 KB (658858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef03ca17e72ecae6b44198d22bbcbf2a29c03bfdc2e63a0083dc77967bbd8b9`  
		Last Modified: Mon, 20 Sep 2021 22:45:57 GMT  
		Size: 23.3 MB (23349537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267983b7cc1765fa911ad76ce5d7d6c3ff57cf87ae52ff4a8cf79bd810aa8ce3`  
		Last Modified: Mon, 20 Sep 2021 22:45:53 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.5.3-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f477c676d05e5445ca0a7dfd08f2b46de13a95d760f27704cc2352970b7c1e36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `traefik:2.5.3-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull traefik@sha256:83ba3ec6a46a9674e26043fe76cad156bf41d997f816b29a2744dbee81f998c2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2712907530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4ed3ac6db10312765b3172f418f0b2e08d33e8a0427fd1521e61911c3353dbf`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 20 Sep 2021 23:09:34 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.5.3/traefik_v2.5.3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 20 Sep 2021 23:09:35 GMT
EXPOSE 80
# Mon, 20 Sep 2021 23:09:36 GMT
ENTRYPOINT ["/traefik"]
# Mon, 20 Sep 2021 23:09:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ade23375ad0841426448992a4f25970f6534b0cb39834cecbdab93bed1ef17`  
		Last Modified: Mon, 20 Sep 2021 23:10:38 GMT  
		Size: 26.2 MB (26204294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbf980003c9648a4ed498899b26dd4fcd5fd3ec2e195a6c9c977a5c8696c4f8`  
		Last Modified: Mon, 20 Sep 2021 23:10:11 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28328bfa6a8a6ec8758c589337295e05e5b6ed23e701cc6c77d3132e962505e7`  
		Last Modified: Mon, 20 Sep 2021 23:10:11 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9408aeb13ffb205eebfce6da260fffa9bc5949eee4ca3e5d208a2e097d290933`  
		Last Modified: Mon, 20 Sep 2021 23:10:11 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.5-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f477c676d05e5445ca0a7dfd08f2b46de13a95d760f27704cc2352970b7c1e36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `traefik:2.5-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull traefik@sha256:83ba3ec6a46a9674e26043fe76cad156bf41d997f816b29a2744dbee81f998c2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2712907530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4ed3ac6db10312765b3172f418f0b2e08d33e8a0427fd1521e61911c3353dbf`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 20 Sep 2021 23:09:34 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.5.3/traefik_v2.5.3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 20 Sep 2021 23:09:35 GMT
EXPOSE 80
# Mon, 20 Sep 2021 23:09:36 GMT
ENTRYPOINT ["/traefik"]
# Mon, 20 Sep 2021 23:09:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ade23375ad0841426448992a4f25970f6534b0cb39834cecbdab93bed1ef17`  
		Last Modified: Mon, 20 Sep 2021 23:10:38 GMT  
		Size: 26.2 MB (26204294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbf980003c9648a4ed498899b26dd4fcd5fd3ec2e195a6c9c977a5c8696c4f8`  
		Last Modified: Mon, 20 Sep 2021 23:10:11 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28328bfa6a8a6ec8758c589337295e05e5b6ed23e701cc6c77d3132e962505e7`  
		Last Modified: Mon, 20 Sep 2021 23:10:11 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9408aeb13ffb205eebfce6da260fffa9bc5949eee4ca3e5d208a2e097d290933`  
		Last Modified: Mon, 20 Sep 2021 23:10:11 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:brie`

```console
$ docker pull traefik@sha256:f40028d9771cb29a35392b4cbdd655625596a319b915061e306c503059d0b6f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:brie` - linux; amd64

```console
$ docker pull traefik@sha256:b3f4abc5706a00dc886b8b8483dbadf691314d6000f7f2f8736bfe9158cfddbf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29057668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d933d21fd8a09022ca5cf067fb195fbfccf0f5c2b5d750d2d1d6eb562b6a8b23`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:28:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Sep 2021 22:33:57 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.3/traefik_v2.5.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Sep 2021 22:33:57 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Sep 2021 22:33:57 GMT
EXPOSE 80
# Mon, 20 Sep 2021 22:33:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Sep 2021 22:33:58 GMT
CMD ["traefik"]
# Mon, 20 Sep 2021 22:33:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:709a291a928e2c186dfda0482997e46082d5f3f59ece15af68d716daaece906a`  
		Last Modified: Mon, 20 Sep 2021 22:34:29 GMT  
		Size: 25.6 MB (25586499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2367d83d5091433850e079372929625c34f7297930b7c5853c4af8740df8c470`  
		Last Modified: Mon, 20 Sep 2021 22:34:24 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:brie` - linux; arm variant v6

```console
$ docker pull traefik@sha256:e12c0a18cae5675bbc0c133f445b96489fbf6617c66ebf254aa4499b5e4bce04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27303193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:439f235df3e981ae502eea1719af18b8fdf666ff7adf6602fd7522a02428fe2d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 18:16:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Sep 2021 23:02:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.3/traefik_v2.5.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Sep 2021 23:02:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Sep 2021 23:02:06 GMT
EXPOSE 80
# Mon, 20 Sep 2021 23:02:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Sep 2021 23:02:06 GMT
CMD ["traefik"]
# Mon, 20 Sep 2021 23:02:07 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac532a93bbc80e8fcf54dcb6ef0229a94aa4f2c94f0e9afec75226cfd91451c`  
		Last Modified: Thu, 02 Sep 2021 18:17:59 GMT  
		Size: 662.0 KB (661991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06452c3a5e8e127597025204daab5d7e08fd26a9604e469bffead7c88192f263`  
		Last Modified: Mon, 20 Sep 2021 23:04:10 GMT  
		Size: 24.0 MB (24013387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c9059e1c58be06e68f3ff3d92f20dc6295e8bbd7a588693346718bf872ee57`  
		Last Modified: Mon, 20 Sep 2021 23:03:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:brie` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:642ea446082cd3cd29a00d89447be819f0e1226e0c2643cb5ecfc9259c2d85e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26720590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:026ae4c43ba7bf101b11c8a12d09e3a0bc6858ac98433c5b9c0133b379b6c36b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:46:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Sep 2021 22:44:57 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.3/traefik_v2.5.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Sep 2021 22:44:58 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Sep 2021 22:44:58 GMT
EXPOSE 80
# Mon, 20 Sep 2021 22:44:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Sep 2021 22:44:58 GMT
CMD ["traefik"]
# Mon, 20 Sep 2021 22:44:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55b5f395e28da206554aa30d5732a9b9a134cb909215e47a12301afbb1dba15`  
		Last Modified: Thu, 02 Sep 2021 17:47:55 GMT  
		Size: 658.9 KB (658858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef03ca17e72ecae6b44198d22bbcbf2a29c03bfdc2e63a0083dc77967bbd8b9`  
		Last Modified: Mon, 20 Sep 2021 22:45:57 GMT  
		Size: 23.3 MB (23349537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267983b7cc1765fa911ad76ce5d7d6c3ff57cf87ae52ff4a8cf79bd810aa8ce3`  
		Last Modified: Mon, 20 Sep 2021 22:45:53 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:brie-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f477c676d05e5445ca0a7dfd08f2b46de13a95d760f27704cc2352970b7c1e36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `traefik:brie-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull traefik@sha256:83ba3ec6a46a9674e26043fe76cad156bf41d997f816b29a2744dbee81f998c2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2712907530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4ed3ac6db10312765b3172f418f0b2e08d33e8a0427fd1521e61911c3353dbf`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 20 Sep 2021 23:09:34 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.5.3/traefik_v2.5.3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 20 Sep 2021 23:09:35 GMT
EXPOSE 80
# Mon, 20 Sep 2021 23:09:36 GMT
ENTRYPOINT ["/traefik"]
# Mon, 20 Sep 2021 23:09:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ade23375ad0841426448992a4f25970f6534b0cb39834cecbdab93bed1ef17`  
		Last Modified: Mon, 20 Sep 2021 23:10:38 GMT  
		Size: 26.2 MB (26204294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbf980003c9648a4ed498899b26dd4fcd5fd3ec2e195a6c9c977a5c8696c4f8`  
		Last Modified: Mon, 20 Sep 2021 23:10:11 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28328bfa6a8a6ec8758c589337295e05e5b6ed23e701cc6c77d3132e962505e7`  
		Last Modified: Mon, 20 Sep 2021 23:10:11 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9408aeb13ffb205eebfce6da260fffa9bc5949eee4ca3e5d208a2e097d290933`  
		Last Modified: Mon, 20 Sep 2021 23:10:11 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:f40028d9771cb29a35392b4cbdd655625596a319b915061e306c503059d0b6f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:b3f4abc5706a00dc886b8b8483dbadf691314d6000f7f2f8736bfe9158cfddbf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29057668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d933d21fd8a09022ca5cf067fb195fbfccf0f5c2b5d750d2d1d6eb562b6a8b23`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:28:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Sep 2021 22:33:57 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.3/traefik_v2.5.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Sep 2021 22:33:57 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Sep 2021 22:33:57 GMT
EXPOSE 80
# Mon, 20 Sep 2021 22:33:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Sep 2021 22:33:58 GMT
CMD ["traefik"]
# Mon, 20 Sep 2021 22:33:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:709a291a928e2c186dfda0482997e46082d5f3f59ece15af68d716daaece906a`  
		Last Modified: Mon, 20 Sep 2021 22:34:29 GMT  
		Size: 25.6 MB (25586499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2367d83d5091433850e079372929625c34f7297930b7c5853c4af8740df8c470`  
		Last Modified: Mon, 20 Sep 2021 22:34:24 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:e12c0a18cae5675bbc0c133f445b96489fbf6617c66ebf254aa4499b5e4bce04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27303193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:439f235df3e981ae502eea1719af18b8fdf666ff7adf6602fd7522a02428fe2d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 18:16:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Sep 2021 23:02:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.3/traefik_v2.5.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Sep 2021 23:02:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Sep 2021 23:02:06 GMT
EXPOSE 80
# Mon, 20 Sep 2021 23:02:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Sep 2021 23:02:06 GMT
CMD ["traefik"]
# Mon, 20 Sep 2021 23:02:07 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac532a93bbc80e8fcf54dcb6ef0229a94aa4f2c94f0e9afec75226cfd91451c`  
		Last Modified: Thu, 02 Sep 2021 18:17:59 GMT  
		Size: 662.0 KB (661991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06452c3a5e8e127597025204daab5d7e08fd26a9604e469bffead7c88192f263`  
		Last Modified: Mon, 20 Sep 2021 23:04:10 GMT  
		Size: 24.0 MB (24013387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c9059e1c58be06e68f3ff3d92f20dc6295e8bbd7a588693346718bf872ee57`  
		Last Modified: Mon, 20 Sep 2021 23:03:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:642ea446082cd3cd29a00d89447be819f0e1226e0c2643cb5ecfc9259c2d85e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26720590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:026ae4c43ba7bf101b11c8a12d09e3a0bc6858ac98433c5b9c0133b379b6c36b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:46:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Sep 2021 22:44:57 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.3/traefik_v2.5.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Sep 2021 22:44:58 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Sep 2021 22:44:58 GMT
EXPOSE 80
# Mon, 20 Sep 2021 22:44:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Sep 2021 22:44:58 GMT
CMD ["traefik"]
# Mon, 20 Sep 2021 22:44:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55b5f395e28da206554aa30d5732a9b9a134cb909215e47a12301afbb1dba15`  
		Last Modified: Thu, 02 Sep 2021 17:47:55 GMT  
		Size: 658.9 KB (658858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef03ca17e72ecae6b44198d22bbcbf2a29c03bfdc2e63a0083dc77967bbd8b9`  
		Last Modified: Mon, 20 Sep 2021 22:45:57 GMT  
		Size: 23.3 MB (23349537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267983b7cc1765fa911ad76ce5d7d6c3ff57cf87ae52ff4a8cf79bd810aa8ce3`  
		Last Modified: Mon, 20 Sep 2021 22:45:53 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles`

```console
$ docker pull traefik@sha256:480a9b5c640886b8171757f3ca3dee3df74e25469df8ffbf8cc23a780ae17f0e
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
$ docker pull traefik@sha256:a9115bd64291c28569b4da6603043fe5c5f77b67ac16c9573a639842d19f55f6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.0 MB (21049536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa32dfeccdefca2de2d0b79a80eed77609a1a3e53683324ce24ccb1eec093cb0`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 05 Oct 2021 00:02:38 GMT
COPY file:c8f727cb8b17c5a8735e609a9b9f333f20765e36c457d0557ed48693a6694880 in /etc/ssl/certs/ 
# Tue, 05 Oct 2021 00:02:40 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 07 Oct 2021 19:31:28 GMT
COPY file:37d0f8b70c5da3bdf158098e422d0bfc00d82405c51ca41ee81a5e564433a943 in / 
# Thu, 07 Oct 2021 19:31:29 GMT
EXPOSE 80
# Thu, 07 Oct 2021 19:31:29 GMT
VOLUME [/tmp]
# Thu, 07 Oct 2021 19:31:30 GMT
ENTRYPOINT ["/traefik"]
# Thu, 07 Oct 2021 19:31:30 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:611185932e68f8b41b94235c966a6c2d26bb4a0f053993c6e49edc01123213f9`  
		Last Modified: Tue, 05 Oct 2021 00:04:56 GMT  
		Size: 122.4 KB (122407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07230710ce3c527700e0de335b44592e9a29b741a0fd3b5c78768beb4d5378e`  
		Last Modified: Tue, 05 Oct 2021 00:04:56 GMT  
		Size: 308.9 KB (308869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58879bf3ff90c00bf7b32d71c06d81a17679e973ce7bf8c2e6cdaac88ab37518`  
		Last Modified: Thu, 07 Oct 2021 19:33:51 GMT  
		Size: 20.6 MB (20618260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9d7e644bda91d73cdc6d25422b9b1fa9bc078f7af84afda4950854bb14e9dc8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20555472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c43fb1698cff19b134d727d7575eb7850b10576ee52b6c8987baa9af24ae2b2`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Mon, 04 Oct 2021 23:44:22 GMT
COPY file:c8f727cb8b17c5a8735e609a9b9f333f20765e36c457d0557ed48693a6694880 in /etc/ssl/certs/ 
# Mon, 04 Oct 2021 23:44:23 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 07 Oct 2021 19:39:58 GMT
COPY file:cd6a95e409278a374fb6ef69098a37f7bc0c8d4eddd3ac751de25d783adf1227 in / 
# Thu, 07 Oct 2021 19:39:58 GMT
EXPOSE 80
# Thu, 07 Oct 2021 19:39:58 GMT
VOLUME [/tmp]
# Thu, 07 Oct 2021 19:39:58 GMT
ENTRYPOINT ["/traefik"]
# Thu, 07 Oct 2021 19:39:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:3c562953a5524a25157fc08c1e7009693f341518b2dcfdcab8ae04d990438254`  
		Last Modified: Mon, 04 Oct 2021 23:45:36 GMT  
		Size: 122.4 KB (122408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086b385acba426fecb8a1f24e7e5b29c5b3dfdf54524653104e29d181dcbcd5b`  
		Last Modified: Mon, 04 Oct 2021 23:45:36 GMT  
		Size: 308.9 KB (308866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baba49691f4c4477b848e632ac02b60345178820d53252af24c6e0100ae6f1ee`  
		Last Modified: Thu, 07 Oct 2021 19:41:12 GMT  
		Size: 20.1 MB (20124198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-alpine`

```console
$ docker pull traefik@sha256:fb358034c340794bd43c591002c926382820df7205e65c0879f3e70385e51322
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
$ docker pull traefik@sha256:14c6316a9d20558e4d28e13d6a6eb4e6f3199cc47e1d5287ef8d482849b4ec52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23908243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:629912e245f4d430278f3e14ef32be01ea70c04ae40e131d7d39bf0042d00c63`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 18:16:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 07 Oct 2021 19:31:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 07 Oct 2021 19:31:06 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 07 Oct 2021 19:31:06 GMT
EXPOSE 80
# Thu, 07 Oct 2021 19:31:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Oct 2021 19:31:07 GMT
CMD ["traefik"]
# Thu, 07 Oct 2021 19:31:08 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac532a93bbc80e8fcf54dcb6ef0229a94aa4f2c94f0e9afec75226cfd91451c`  
		Last Modified: Thu, 02 Sep 2021 18:17:59 GMT  
		Size: 662.0 KB (661991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62b9cbace357f1af4892553b0e7d5985c60f32d1401fe4991432ec1028bd2ae`  
		Last Modified: Thu, 07 Oct 2021 19:33:14 GMT  
		Size: 20.6 MB (20618436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a3411058b7ed63da77792b8c2e2ccf0bc0ff03528e597a3c75e6ee529ff4b9`  
		Last Modified: Thu, 07 Oct 2021 19:33:00 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:4d46f44cb8f6e923a789bce72bb21ac3e3f17b1bb1c0afeae696d111b68ae0a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23495299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a99fbda519f3c0712c4582233fe0106e3cf17204799fdda7b18ec7b7be27f9b9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:46:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 07 Oct 2021 19:39:44 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 07 Oct 2021 19:39:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 07 Oct 2021 19:39:44 GMT
EXPOSE 80
# Thu, 07 Oct 2021 19:39:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Oct 2021 19:39:44 GMT
CMD ["traefik"]
# Thu, 07 Oct 2021 19:39:45 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55b5f395e28da206554aa30d5732a9b9a134cb909215e47a12301afbb1dba15`  
		Last Modified: Thu, 02 Sep 2021 17:47:55 GMT  
		Size: 658.9 KB (658858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814fda492f8bb5f7a9175b058062dc3347924a09e9d05326d780c86ff219ddf1`  
		Last Modified: Thu, 07 Oct 2021 19:40:47 GMT  
		Size: 20.1 MB (20124247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf21937c0359e10bf99379e506ad7dfe0e56dc2fd8911234b935558480ff38e0`  
		Last Modified: Thu, 07 Oct 2021 19:40:44 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-windowsservercore-1809`

```console
$ docker pull traefik@sha256:1b2705448077d8cc37f49f9185485d7d77f7872a8ca1bd5569c6e447d1ccd83f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull traefik@sha256:437bb3298f50ba92370d44507a0810b57791e10056e7968d99287bc9957bb366
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2709549668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12bf5af8e35c139620f26df2edcc883c7c6add7c30d9601fac329bc574e62a92`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 07 Oct 2021 19:18:36 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 07 Oct 2021 19:18:37 GMT
EXPOSE 80
# Thu, 07 Oct 2021 19:18:38 GMT
ENTRYPOINT ["/traefik"]
# Thu, 07 Oct 2021 19:18:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e6a78c2cc1b3b87f01fe5643ca6635c8d84211449dcdbca2f40485cc4d0732`  
		Last Modified: Thu, 07 Oct 2021 19:19:14 GMT  
		Size: 22.8 MB (22846068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c1b67f1976804b7e4436fca932b868aefafab88a428c407fedd2a158ee7fc1`  
		Last Modified: Thu, 07 Oct 2021 19:19:08 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f02d143ace29a045b87e7c7d8166bfce2e26c53563e6267847323f67779d86`  
		Last Modified: Thu, 07 Oct 2021 19:19:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364f6175eb5c6e45ec71345b85c48e45bc32fd0d18dab39a71d8eb5bc8df1161`  
		Last Modified: Thu, 07 Oct 2021 19:19:08 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7`

```console
$ docker pull traefik@sha256:480a9b5c640886b8171757f3ca3dee3df74e25469df8ffbf8cc23a780ae17f0e
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
$ docker pull traefik@sha256:a9115bd64291c28569b4da6603043fe5c5f77b67ac16c9573a639842d19f55f6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.0 MB (21049536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa32dfeccdefca2de2d0b79a80eed77609a1a3e53683324ce24ccb1eec093cb0`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 05 Oct 2021 00:02:38 GMT
COPY file:c8f727cb8b17c5a8735e609a9b9f333f20765e36c457d0557ed48693a6694880 in /etc/ssl/certs/ 
# Tue, 05 Oct 2021 00:02:40 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 07 Oct 2021 19:31:28 GMT
COPY file:37d0f8b70c5da3bdf158098e422d0bfc00d82405c51ca41ee81a5e564433a943 in / 
# Thu, 07 Oct 2021 19:31:29 GMT
EXPOSE 80
# Thu, 07 Oct 2021 19:31:29 GMT
VOLUME [/tmp]
# Thu, 07 Oct 2021 19:31:30 GMT
ENTRYPOINT ["/traefik"]
# Thu, 07 Oct 2021 19:31:30 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:611185932e68f8b41b94235c966a6c2d26bb4a0f053993c6e49edc01123213f9`  
		Last Modified: Tue, 05 Oct 2021 00:04:56 GMT  
		Size: 122.4 KB (122407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07230710ce3c527700e0de335b44592e9a29b741a0fd3b5c78768beb4d5378e`  
		Last Modified: Tue, 05 Oct 2021 00:04:56 GMT  
		Size: 308.9 KB (308869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58879bf3ff90c00bf7b32d71c06d81a17679e973ce7bf8c2e6cdaac88ab37518`  
		Last Modified: Thu, 07 Oct 2021 19:33:51 GMT  
		Size: 20.6 MB (20618260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9d7e644bda91d73cdc6d25422b9b1fa9bc078f7af84afda4950854bb14e9dc8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20555472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c43fb1698cff19b134d727d7575eb7850b10576ee52b6c8987baa9af24ae2b2`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Mon, 04 Oct 2021 23:44:22 GMT
COPY file:c8f727cb8b17c5a8735e609a9b9f333f20765e36c457d0557ed48693a6694880 in /etc/ssl/certs/ 
# Mon, 04 Oct 2021 23:44:23 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 07 Oct 2021 19:39:58 GMT
COPY file:cd6a95e409278a374fb6ef69098a37f7bc0c8d4eddd3ac751de25d783adf1227 in / 
# Thu, 07 Oct 2021 19:39:58 GMT
EXPOSE 80
# Thu, 07 Oct 2021 19:39:58 GMT
VOLUME [/tmp]
# Thu, 07 Oct 2021 19:39:58 GMT
ENTRYPOINT ["/traefik"]
# Thu, 07 Oct 2021 19:39:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:3c562953a5524a25157fc08c1e7009693f341518b2dcfdcab8ae04d990438254`  
		Last Modified: Mon, 04 Oct 2021 23:45:36 GMT  
		Size: 122.4 KB (122408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086b385acba426fecb8a1f24e7e5b29c5b3dfdf54524653104e29d181dcbcd5b`  
		Last Modified: Mon, 04 Oct 2021 23:45:36 GMT  
		Size: 308.9 KB (308866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baba49691f4c4477b848e632ac02b60345178820d53252af24c6e0100ae6f1ee`  
		Last Modified: Thu, 07 Oct 2021 19:41:12 GMT  
		Size: 20.1 MB (20124198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.33`

```console
$ docker pull traefik@sha256:480a9b5c640886b8171757f3ca3dee3df74e25469df8ffbf8cc23a780ae17f0e
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
$ docker pull traefik@sha256:a9115bd64291c28569b4da6603043fe5c5f77b67ac16c9573a639842d19f55f6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.0 MB (21049536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa32dfeccdefca2de2d0b79a80eed77609a1a3e53683324ce24ccb1eec093cb0`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 05 Oct 2021 00:02:38 GMT
COPY file:c8f727cb8b17c5a8735e609a9b9f333f20765e36c457d0557ed48693a6694880 in /etc/ssl/certs/ 
# Tue, 05 Oct 2021 00:02:40 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 07 Oct 2021 19:31:28 GMT
COPY file:37d0f8b70c5da3bdf158098e422d0bfc00d82405c51ca41ee81a5e564433a943 in / 
# Thu, 07 Oct 2021 19:31:29 GMT
EXPOSE 80
# Thu, 07 Oct 2021 19:31:29 GMT
VOLUME [/tmp]
# Thu, 07 Oct 2021 19:31:30 GMT
ENTRYPOINT ["/traefik"]
# Thu, 07 Oct 2021 19:31:30 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:611185932e68f8b41b94235c966a6c2d26bb4a0f053993c6e49edc01123213f9`  
		Last Modified: Tue, 05 Oct 2021 00:04:56 GMT  
		Size: 122.4 KB (122407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07230710ce3c527700e0de335b44592e9a29b741a0fd3b5c78768beb4d5378e`  
		Last Modified: Tue, 05 Oct 2021 00:04:56 GMT  
		Size: 308.9 KB (308869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58879bf3ff90c00bf7b32d71c06d81a17679e973ce7bf8c2e6cdaac88ab37518`  
		Last Modified: Thu, 07 Oct 2021 19:33:51 GMT  
		Size: 20.6 MB (20618260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.33` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9d7e644bda91d73cdc6d25422b9b1fa9bc078f7af84afda4950854bb14e9dc8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20555472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c43fb1698cff19b134d727d7575eb7850b10576ee52b6c8987baa9af24ae2b2`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Mon, 04 Oct 2021 23:44:22 GMT
COPY file:c8f727cb8b17c5a8735e609a9b9f333f20765e36c457d0557ed48693a6694880 in /etc/ssl/certs/ 
# Mon, 04 Oct 2021 23:44:23 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 07 Oct 2021 19:39:58 GMT
COPY file:cd6a95e409278a374fb6ef69098a37f7bc0c8d4eddd3ac751de25d783adf1227 in / 
# Thu, 07 Oct 2021 19:39:58 GMT
EXPOSE 80
# Thu, 07 Oct 2021 19:39:58 GMT
VOLUME [/tmp]
# Thu, 07 Oct 2021 19:39:58 GMT
ENTRYPOINT ["/traefik"]
# Thu, 07 Oct 2021 19:39:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:3c562953a5524a25157fc08c1e7009693f341518b2dcfdcab8ae04d990438254`  
		Last Modified: Mon, 04 Oct 2021 23:45:36 GMT  
		Size: 122.4 KB (122408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086b385acba426fecb8a1f24e7e5b29c5b3dfdf54524653104e29d181dcbcd5b`  
		Last Modified: Mon, 04 Oct 2021 23:45:36 GMT  
		Size: 308.9 KB (308866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baba49691f4c4477b848e632ac02b60345178820d53252af24c6e0100ae6f1ee`  
		Last Modified: Thu, 07 Oct 2021 19:41:12 GMT  
		Size: 20.1 MB (20124198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.33-alpine`

```console
$ docker pull traefik@sha256:fb358034c340794bd43c591002c926382820df7205e65c0879f3e70385e51322
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
$ docker pull traefik@sha256:14c6316a9d20558e4d28e13d6a6eb4e6f3199cc47e1d5287ef8d482849b4ec52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23908243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:629912e245f4d430278f3e14ef32be01ea70c04ae40e131d7d39bf0042d00c63`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 18:16:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 07 Oct 2021 19:31:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 07 Oct 2021 19:31:06 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 07 Oct 2021 19:31:06 GMT
EXPOSE 80
# Thu, 07 Oct 2021 19:31:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Oct 2021 19:31:07 GMT
CMD ["traefik"]
# Thu, 07 Oct 2021 19:31:08 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac532a93bbc80e8fcf54dcb6ef0229a94aa4f2c94f0e9afec75226cfd91451c`  
		Last Modified: Thu, 02 Sep 2021 18:17:59 GMT  
		Size: 662.0 KB (661991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62b9cbace357f1af4892553b0e7d5985c60f32d1401fe4991432ec1028bd2ae`  
		Last Modified: Thu, 07 Oct 2021 19:33:14 GMT  
		Size: 20.6 MB (20618436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a3411058b7ed63da77792b8c2e2ccf0bc0ff03528e597a3c75e6ee529ff4b9`  
		Last Modified: Thu, 07 Oct 2021 19:33:00 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.33-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:4d46f44cb8f6e923a789bce72bb21ac3e3f17b1bb1c0afeae696d111b68ae0a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23495299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a99fbda519f3c0712c4582233fe0106e3cf17204799fdda7b18ec7b7be27f9b9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:46:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 07 Oct 2021 19:39:44 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 07 Oct 2021 19:39:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 07 Oct 2021 19:39:44 GMT
EXPOSE 80
# Thu, 07 Oct 2021 19:39:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Oct 2021 19:39:44 GMT
CMD ["traefik"]
# Thu, 07 Oct 2021 19:39:45 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55b5f395e28da206554aa30d5732a9b9a134cb909215e47a12301afbb1dba15`  
		Last Modified: Thu, 02 Sep 2021 17:47:55 GMT  
		Size: 658.9 KB (658858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814fda492f8bb5f7a9175b058062dc3347924a09e9d05326d780c86ff219ddf1`  
		Last Modified: Thu, 07 Oct 2021 19:40:47 GMT  
		Size: 20.1 MB (20124247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf21937c0359e10bf99379e506ad7dfe0e56dc2fd8911234b935558480ff38e0`  
		Last Modified: Thu, 07 Oct 2021 19:40:44 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.33-windowsservercore-1809`

```console
$ docker pull traefik@sha256:1b2705448077d8cc37f49f9185485d7d77f7872a8ca1bd5569c6e447d1ccd83f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `traefik:v1.7.33-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull traefik@sha256:437bb3298f50ba92370d44507a0810b57791e10056e7968d99287bc9957bb366
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2709549668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12bf5af8e35c139620f26df2edcc883c7c6add7c30d9601fac329bc574e62a92`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 07 Oct 2021 19:18:36 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 07 Oct 2021 19:18:37 GMT
EXPOSE 80
# Thu, 07 Oct 2021 19:18:38 GMT
ENTRYPOINT ["/traefik"]
# Thu, 07 Oct 2021 19:18:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e6a78c2cc1b3b87f01fe5643ca6635c8d84211449dcdbca2f40485cc4d0732`  
		Last Modified: Thu, 07 Oct 2021 19:19:14 GMT  
		Size: 22.8 MB (22846068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c1b67f1976804b7e4436fca932b868aefafab88a428c407fedd2a158ee7fc1`  
		Last Modified: Thu, 07 Oct 2021 19:19:08 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f02d143ace29a045b87e7c7d8166bfce2e26c53563e6267847323f67779d86`  
		Last Modified: Thu, 07 Oct 2021 19:19:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364f6175eb5c6e45ec71345b85c48e45bc32fd0d18dab39a71d8eb5bc8df1161`  
		Last Modified: Thu, 07 Oct 2021 19:19:08 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-alpine`

```console
$ docker pull traefik@sha256:fb358034c340794bd43c591002c926382820df7205e65c0879f3e70385e51322
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
$ docker pull traefik@sha256:14c6316a9d20558e4d28e13d6a6eb4e6f3199cc47e1d5287ef8d482849b4ec52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23908243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:629912e245f4d430278f3e14ef32be01ea70c04ae40e131d7d39bf0042d00c63`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 18:16:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 07 Oct 2021 19:31:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 07 Oct 2021 19:31:06 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 07 Oct 2021 19:31:06 GMT
EXPOSE 80
# Thu, 07 Oct 2021 19:31:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Oct 2021 19:31:07 GMT
CMD ["traefik"]
# Thu, 07 Oct 2021 19:31:08 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac532a93bbc80e8fcf54dcb6ef0229a94aa4f2c94f0e9afec75226cfd91451c`  
		Last Modified: Thu, 02 Sep 2021 18:17:59 GMT  
		Size: 662.0 KB (661991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62b9cbace357f1af4892553b0e7d5985c60f32d1401fe4991432ec1028bd2ae`  
		Last Modified: Thu, 07 Oct 2021 19:33:14 GMT  
		Size: 20.6 MB (20618436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a3411058b7ed63da77792b8c2e2ccf0bc0ff03528e597a3c75e6ee529ff4b9`  
		Last Modified: Thu, 07 Oct 2021 19:33:00 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:4d46f44cb8f6e923a789bce72bb21ac3e3f17b1bb1c0afeae696d111b68ae0a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23495299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a99fbda519f3c0712c4582233fe0106e3cf17204799fdda7b18ec7b7be27f9b9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:46:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 07 Oct 2021 19:39:44 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 07 Oct 2021 19:39:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 07 Oct 2021 19:39:44 GMT
EXPOSE 80
# Thu, 07 Oct 2021 19:39:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Oct 2021 19:39:44 GMT
CMD ["traefik"]
# Thu, 07 Oct 2021 19:39:45 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55b5f395e28da206554aa30d5732a9b9a134cb909215e47a12301afbb1dba15`  
		Last Modified: Thu, 02 Sep 2021 17:47:55 GMT  
		Size: 658.9 KB (658858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814fda492f8bb5f7a9175b058062dc3347924a09e9d05326d780c86ff219ddf1`  
		Last Modified: Thu, 07 Oct 2021 19:40:47 GMT  
		Size: 20.1 MB (20124247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf21937c0359e10bf99379e506ad7dfe0e56dc2fd8911234b935558480ff38e0`  
		Last Modified: Thu, 07 Oct 2021 19:40:44 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:1b2705448077d8cc37f49f9185485d7d77f7872a8ca1bd5569c6e447d1ccd83f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `traefik:v1.7-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull traefik@sha256:437bb3298f50ba92370d44507a0810b57791e10056e7968d99287bc9957bb366
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2709549668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12bf5af8e35c139620f26df2edcc883c7c6add7c30d9601fac329bc574e62a92`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 07 Oct 2021 19:18:36 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.33/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 07 Oct 2021 19:18:37 GMT
EXPOSE 80
# Thu, 07 Oct 2021 19:18:38 GMT
ENTRYPOINT ["/traefik"]
# Thu, 07 Oct 2021 19:18:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.33 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e6a78c2cc1b3b87f01fe5643ca6635c8d84211449dcdbca2f40485cc4d0732`  
		Last Modified: Thu, 07 Oct 2021 19:19:14 GMT  
		Size: 22.8 MB (22846068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c1b67f1976804b7e4436fca932b868aefafab88a428c407fedd2a158ee7fc1`  
		Last Modified: Thu, 07 Oct 2021 19:19:08 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f02d143ace29a045b87e7c7d8166bfce2e26c53563e6267847323f67779d86`  
		Last Modified: Thu, 07 Oct 2021 19:19:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364f6175eb5c6e45ec71345b85c48e45bc32fd0d18dab39a71d8eb5bc8df1161`  
		Last Modified: Thu, 07 Oct 2021 19:19:08 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.5`

```console
$ docker pull traefik@sha256:f40028d9771cb29a35392b4cbdd655625596a319b915061e306c503059d0b6f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.5` - linux; amd64

```console
$ docker pull traefik@sha256:b3f4abc5706a00dc886b8b8483dbadf691314d6000f7f2f8736bfe9158cfddbf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29057668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d933d21fd8a09022ca5cf067fb195fbfccf0f5c2b5d750d2d1d6eb562b6a8b23`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:28:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Sep 2021 22:33:57 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.3/traefik_v2.5.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Sep 2021 22:33:57 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Sep 2021 22:33:57 GMT
EXPOSE 80
# Mon, 20 Sep 2021 22:33:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Sep 2021 22:33:58 GMT
CMD ["traefik"]
# Mon, 20 Sep 2021 22:33:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:709a291a928e2c186dfda0482997e46082d5f3f59ece15af68d716daaece906a`  
		Last Modified: Mon, 20 Sep 2021 22:34:29 GMT  
		Size: 25.6 MB (25586499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2367d83d5091433850e079372929625c34f7297930b7c5853c4af8740df8c470`  
		Last Modified: Mon, 20 Sep 2021 22:34:24 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.5` - linux; arm variant v6

```console
$ docker pull traefik@sha256:e12c0a18cae5675bbc0c133f445b96489fbf6617c66ebf254aa4499b5e4bce04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27303193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:439f235df3e981ae502eea1719af18b8fdf666ff7adf6602fd7522a02428fe2d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 18:16:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Sep 2021 23:02:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.3/traefik_v2.5.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Sep 2021 23:02:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Sep 2021 23:02:06 GMT
EXPOSE 80
# Mon, 20 Sep 2021 23:02:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Sep 2021 23:02:06 GMT
CMD ["traefik"]
# Mon, 20 Sep 2021 23:02:07 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac532a93bbc80e8fcf54dcb6ef0229a94aa4f2c94f0e9afec75226cfd91451c`  
		Last Modified: Thu, 02 Sep 2021 18:17:59 GMT  
		Size: 662.0 KB (661991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06452c3a5e8e127597025204daab5d7e08fd26a9604e469bffead7c88192f263`  
		Last Modified: Mon, 20 Sep 2021 23:04:10 GMT  
		Size: 24.0 MB (24013387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c9059e1c58be06e68f3ff3d92f20dc6295e8bbd7a588693346718bf872ee57`  
		Last Modified: Mon, 20 Sep 2021 23:03:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.5` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:642ea446082cd3cd29a00d89447be819f0e1226e0c2643cb5ecfc9259c2d85e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26720590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:026ae4c43ba7bf101b11c8a12d09e3a0bc6858ac98433c5b9c0133b379b6c36b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:46:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Sep 2021 22:44:57 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.3/traefik_v2.5.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Sep 2021 22:44:58 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Sep 2021 22:44:58 GMT
EXPOSE 80
# Mon, 20 Sep 2021 22:44:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Sep 2021 22:44:58 GMT
CMD ["traefik"]
# Mon, 20 Sep 2021 22:44:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55b5f395e28da206554aa30d5732a9b9a134cb909215e47a12301afbb1dba15`  
		Last Modified: Thu, 02 Sep 2021 17:47:55 GMT  
		Size: 658.9 KB (658858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef03ca17e72ecae6b44198d22bbcbf2a29c03bfdc2e63a0083dc77967bbd8b9`  
		Last Modified: Mon, 20 Sep 2021 22:45:57 GMT  
		Size: 23.3 MB (23349537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267983b7cc1765fa911ad76ce5d7d6c3ff57cf87ae52ff4a8cf79bd810aa8ce3`  
		Last Modified: Mon, 20 Sep 2021 22:45:53 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.5.3`

```console
$ docker pull traefik@sha256:f40028d9771cb29a35392b4cbdd655625596a319b915061e306c503059d0b6f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.5.3` - linux; amd64

```console
$ docker pull traefik@sha256:b3f4abc5706a00dc886b8b8483dbadf691314d6000f7f2f8736bfe9158cfddbf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29057668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d933d21fd8a09022ca5cf067fb195fbfccf0f5c2b5d750d2d1d6eb562b6a8b23`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:28:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Sep 2021 22:33:57 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.3/traefik_v2.5.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Sep 2021 22:33:57 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Sep 2021 22:33:57 GMT
EXPOSE 80
# Mon, 20 Sep 2021 22:33:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Sep 2021 22:33:58 GMT
CMD ["traefik"]
# Mon, 20 Sep 2021 22:33:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:709a291a928e2c186dfda0482997e46082d5f3f59ece15af68d716daaece906a`  
		Last Modified: Mon, 20 Sep 2021 22:34:29 GMT  
		Size: 25.6 MB (25586499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2367d83d5091433850e079372929625c34f7297930b7c5853c4af8740df8c470`  
		Last Modified: Mon, 20 Sep 2021 22:34:24 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.5.3` - linux; arm variant v6

```console
$ docker pull traefik@sha256:e12c0a18cae5675bbc0c133f445b96489fbf6617c66ebf254aa4499b5e4bce04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27303193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:439f235df3e981ae502eea1719af18b8fdf666ff7adf6602fd7522a02428fe2d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 18:16:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Sep 2021 23:02:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.3/traefik_v2.5.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Sep 2021 23:02:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Sep 2021 23:02:06 GMT
EXPOSE 80
# Mon, 20 Sep 2021 23:02:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Sep 2021 23:02:06 GMT
CMD ["traefik"]
# Mon, 20 Sep 2021 23:02:07 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac532a93bbc80e8fcf54dcb6ef0229a94aa4f2c94f0e9afec75226cfd91451c`  
		Last Modified: Thu, 02 Sep 2021 18:17:59 GMT  
		Size: 662.0 KB (661991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06452c3a5e8e127597025204daab5d7e08fd26a9604e469bffead7c88192f263`  
		Last Modified: Mon, 20 Sep 2021 23:04:10 GMT  
		Size: 24.0 MB (24013387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c9059e1c58be06e68f3ff3d92f20dc6295e8bbd7a588693346718bf872ee57`  
		Last Modified: Mon, 20 Sep 2021 23:03:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.5.3` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:642ea446082cd3cd29a00d89447be819f0e1226e0c2643cb5ecfc9259c2d85e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26720590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:026ae4c43ba7bf101b11c8a12d09e3a0bc6858ac98433c5b9c0133b379b6c36b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:46:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Sep 2021 22:44:57 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.3/traefik_v2.5.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Sep 2021 22:44:58 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Sep 2021 22:44:58 GMT
EXPOSE 80
# Mon, 20 Sep 2021 22:44:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Sep 2021 22:44:58 GMT
CMD ["traefik"]
# Mon, 20 Sep 2021 22:44:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55b5f395e28da206554aa30d5732a9b9a134cb909215e47a12301afbb1dba15`  
		Last Modified: Thu, 02 Sep 2021 17:47:55 GMT  
		Size: 658.9 KB (658858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef03ca17e72ecae6b44198d22bbcbf2a29c03bfdc2e63a0083dc77967bbd8b9`  
		Last Modified: Mon, 20 Sep 2021 22:45:57 GMT  
		Size: 23.3 MB (23349537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267983b7cc1765fa911ad76ce5d7d6c3ff57cf87ae52ff4a8cf79bd810aa8ce3`  
		Last Modified: Mon, 20 Sep 2021 22:45:53 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.5.3-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f477c676d05e5445ca0a7dfd08f2b46de13a95d760f27704cc2352970b7c1e36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `traefik:v2.5.3-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull traefik@sha256:83ba3ec6a46a9674e26043fe76cad156bf41d997f816b29a2744dbee81f998c2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2712907530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4ed3ac6db10312765b3172f418f0b2e08d33e8a0427fd1521e61911c3353dbf`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 20 Sep 2021 23:09:34 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.5.3/traefik_v2.5.3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 20 Sep 2021 23:09:35 GMT
EXPOSE 80
# Mon, 20 Sep 2021 23:09:36 GMT
ENTRYPOINT ["/traefik"]
# Mon, 20 Sep 2021 23:09:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ade23375ad0841426448992a4f25970f6534b0cb39834cecbdab93bed1ef17`  
		Last Modified: Mon, 20 Sep 2021 23:10:38 GMT  
		Size: 26.2 MB (26204294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbf980003c9648a4ed498899b26dd4fcd5fd3ec2e195a6c9c977a5c8696c4f8`  
		Last Modified: Mon, 20 Sep 2021 23:10:11 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28328bfa6a8a6ec8758c589337295e05e5b6ed23e701cc6c77d3132e962505e7`  
		Last Modified: Mon, 20 Sep 2021 23:10:11 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9408aeb13ffb205eebfce6da260fffa9bc5949eee4ca3e5d208a2e097d290933`  
		Last Modified: Mon, 20 Sep 2021 23:10:11 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.5-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f477c676d05e5445ca0a7dfd08f2b46de13a95d760f27704cc2352970b7c1e36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `traefik:v2.5-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull traefik@sha256:83ba3ec6a46a9674e26043fe76cad156bf41d997f816b29a2744dbee81f998c2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2712907530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4ed3ac6db10312765b3172f418f0b2e08d33e8a0427fd1521e61911c3353dbf`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 20 Sep 2021 23:09:34 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.5.3/traefik_v2.5.3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 20 Sep 2021 23:09:35 GMT
EXPOSE 80
# Mon, 20 Sep 2021 23:09:36 GMT
ENTRYPOINT ["/traefik"]
# Mon, 20 Sep 2021 23:09:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ade23375ad0841426448992a4f25970f6534b0cb39834cecbdab93bed1ef17`  
		Last Modified: Mon, 20 Sep 2021 23:10:38 GMT  
		Size: 26.2 MB (26204294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbf980003c9648a4ed498899b26dd4fcd5fd3ec2e195a6c9c977a5c8696c4f8`  
		Last Modified: Mon, 20 Sep 2021 23:10:11 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28328bfa6a8a6ec8758c589337295e05e5b6ed23e701cc6c77d3132e962505e7`  
		Last Modified: Mon, 20 Sep 2021 23:10:11 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9408aeb13ffb205eebfce6da260fffa9bc5949eee4ca3e5d208a2e097d290933`  
		Last Modified: Mon, 20 Sep 2021 23:10:11 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:f477c676d05e5445ca0a7dfd08f2b46de13a95d760f27704cc2352970b7c1e36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull traefik@sha256:83ba3ec6a46a9674e26043fe76cad156bf41d997f816b29a2744dbee81f998c2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2712907530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4ed3ac6db10312765b3172f418f0b2e08d33e8a0427fd1521e61911c3353dbf`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 20 Sep 2021 23:09:34 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.5.3/traefik_v2.5.3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 20 Sep 2021 23:09:35 GMT
EXPOSE 80
# Mon, 20 Sep 2021 23:09:36 GMT
ENTRYPOINT ["/traefik"]
# Mon, 20 Sep 2021 23:09:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ade23375ad0841426448992a4f25970f6534b0cb39834cecbdab93bed1ef17`  
		Last Modified: Mon, 20 Sep 2021 23:10:38 GMT  
		Size: 26.2 MB (26204294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbf980003c9648a4ed498899b26dd4fcd5fd3ec2e195a6c9c977a5c8696c4f8`  
		Last Modified: Mon, 20 Sep 2021 23:10:11 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28328bfa6a8a6ec8758c589337295e05e5b6ed23e701cc6c77d3132e962505e7`  
		Last Modified: Mon, 20 Sep 2021 23:10:11 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9408aeb13ffb205eebfce6da260fffa9bc5949eee4ca3e5d208a2e097d290933`  
		Last Modified: Mon, 20 Sep 2021 23:10:11 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
