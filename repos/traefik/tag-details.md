<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:1.7`](#traefik17)
-	[`traefik:1.7.21`](#traefik1721)
-	[`traefik:1.7.21-alpine`](#traefik1721-alpine)
-	[`traefik:1.7.21-windowsservercore-1809`](#traefik1721-windowsservercore-1809)
-	[`traefik:1.7-alpine`](#traefik17-alpine)
-	[`traefik:1.7-windowsservercore-1809`](#traefik17-windowsservercore-1809)
-	[`traefik:2.1`](#traefik21)
-	[`traefik:2.1.4`](#traefik214)
-	[`traefik:2.1.4-windowsservercore-1809`](#traefik214-windowsservercore-1809)
-	[`traefik:2.1-windowsservercore-1809`](#traefik21-windowsservercore-1809)
-	[`traefik:cantal`](#traefikcantal)
-	[`traefik:cantal-windowsservercore-1809`](#traefikcantal-windowsservercore-1809)
-	[`traefik:latest`](#traefiklatest)
-	[`traefik:maroilles`](#traefikmaroilles)
-	[`traefik:maroilles-alpine`](#traefikmaroilles-alpine)
-	[`traefik:maroilles-windowsservercore-1809`](#traefikmaroilles-windowsservercore-1809)
-	[`traefik:v1.7`](#traefikv17)
-	[`traefik:v1.7.21`](#traefikv1721)
-	[`traefik:v1.7.21-alpine`](#traefikv1721-alpine)
-	[`traefik:v1.7.21-windowsservercore-1809`](#traefikv1721-windowsservercore-1809)
-	[`traefik:v1.7-alpine`](#traefikv17-alpine)
-	[`traefik:v1.7-windowsservercore-1809`](#traefikv17-windowsservercore-1809)
-	[`traefik:v2.1`](#traefikv21)
-	[`traefik:v2.1.4`](#traefikv214)
-	[`traefik:v2.1.4-windowsservercore-1809`](#traefikv214-windowsservercore-1809)
-	[`traefik:v2.1-windowsservercore-1809`](#traefikv21-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:1.7`

```console
$ docker pull traefik@sha256:5ec34caf19d114f8f0ed76f9bc3dad6ba8cf6d13a1575c4294b59b77709def39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7` - linux; amd64

```console
$ docker pull traefik@sha256:3b1c4d57c57d125a5d949d463d41882fefc957ce117db226aace4e7314e82d5c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.0 MB (24005352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96c63a7d3e502fcbbd8937a2523368c22d0edd1788b8389af095f64038318834`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 27 Aug 2019 01:00:22 GMT
COPY file:091d2a65366d205fc0db557b2f495da40adb5a33c9d656d02c3ea08bb22f6c4d in /etc/ssl/certs/ 
# Mon, 21 Oct 2019 22:26:52 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 10 Dec 2019 22:31:38 GMT
COPY file:be1ea92a6d3f63051c9ae787ca41c986b81a56ce7f8b8347b97c3ddc3b4471f5 in / 
# Tue, 10 Dec 2019 22:31:38 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:31:38 GMT
VOLUME [/tmp]
# Tue, 10 Dec 2019 22:31:38 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 22:31:39 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:42e7d26ec3785f8ce0f20e327cf72404ee054ba022ce9068ad2d28c52e82db2a`  
		Last Modified: Tue, 27 Aug 2019 01:00:52 GMT  
		Size: 132.0 KB (132022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a753f02eeffef33e5e071a6feac9e12fffb36330fc7ef5441f378d0ce67c528`  
		Last Modified: Mon, 21 Oct 2019 22:27:25 GMT  
		Size: 327.3 KB (327346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab927d94d255c72862c3e7ada3f6cdb36f90926b7a8913a080062b17d73f186b`  
		Last Modified: Tue, 10 Dec 2019 22:32:27 GMT  
		Size: 23.5 MB (23545984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:3a32e589b7d538f688f0a4d5777ab21dc2e946e22a1b08872aaad72b4192976e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.5 MB (22491539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:099411d81ac7bf28b232625f19ecc6590f39c3920418958b3056caa4f85815c4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Mon, 26 Aug 2019 23:54:26 GMT
COPY file:091d2a65366d205fc0db557b2f495da40adb5a33c9d656d02c3ea08bb22f6c4d in /etc/ssl/certs/ 
# Mon, 21 Oct 2019 20:27:55 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 10 Dec 2019 21:57:12 GMT
COPY file:ad6d99c4dea9edfff1bf18494e1c85b8a82b1a74f77a8bf3f437bd05222fbf79 in / 
# Tue, 10 Dec 2019 21:57:14 GMT
EXPOSE 80
# Tue, 10 Dec 2019 21:57:15 GMT
VOLUME [/tmp]
# Tue, 10 Dec 2019 21:57:16 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 21:57:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:506698346e0f5f486b919abaa7bc72252b3dc553cb28e0d1a5e2b6f3708cf4c0`  
		Last Modified: Mon, 26 Aug 2019 23:55:08 GMT  
		Size: 132.0 KB (132026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46037320e6487ea40f4dfb2c29d120090739bc20051bca67eb5e64a072973136`  
		Last Modified: Mon, 21 Oct 2019 20:28:50 GMT  
		Size: 327.4 KB (327388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0d7ab9d9ce392bdaa622a30db2df3963e7ac8b19c846fddc788b2f7fd3f890`  
		Last Modified: Tue, 10 Dec 2019 21:58:07 GMT  
		Size: 22.0 MB (22032125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3a587a9647aca9d58c237389157512cf349f00e99afc0f33959501bc5366b489
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.2 MB (22219190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:843151930dcd29bc722fa2e9949bcecfcb0020d961037b85983f47017aa38a58`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 27 Aug 2019 00:16:41 GMT
COPY file:091d2a65366d205fc0db557b2f495da40adb5a33c9d656d02c3ea08bb22f6c4d in /etc/ssl/certs/ 
# Mon, 21 Oct 2019 23:22:44 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 10 Dec 2019 22:39:48 GMT
COPY file:2548a09c5388b09356e8109d52a2261b02b840df1156718406457af4ef9eedcd in / 
# Tue, 10 Dec 2019 22:39:50 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:39:50 GMT
VOLUME [/tmp]
# Tue, 10 Dec 2019 22:39:51 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 22:39:51 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f07a1cd6fb05ab2fb5b66f5326144f82e52f5580df40a42e400637f8a8f9c6d8`  
		Last Modified: Tue, 27 Aug 2019 00:17:31 GMT  
		Size: 132.0 KB (132021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2afd881e5b94f57a79b2f6bcd9d637c2f7a6aa910f4013045b8653ebe29fdb`  
		Last Modified: Mon, 21 Oct 2019 23:23:36 GMT  
		Size: 327.4 KB (327378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b05c8936168a3f333423ce8dca6ed7e5ad1890ce50b95da487f61aa83440e26`  
		Last Modified: Tue, 10 Dec 2019 22:40:39 GMT  
		Size: 21.8 MB (21759791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.21`

```console
$ docker pull traefik@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `traefik:1.7.21-alpine`

```console
$ docker pull traefik@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `traefik:1.7.21-windowsservercore-1809`

```console
$ docker pull traefik@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `traefik:1.7-alpine`

```console
$ docker pull traefik@sha256:710a1f7845f02e1f1d694a83bf41042c6dbe47eb9ee3b2bf0cf35b3eaa6c2b4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:8fa8c4faa799bf8f632fe4af56768e3e1f302bf2d63fc1cd7c7752a36ee364a3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27028116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee8378e05f99d815e7131d19af5863e997f0b35d694fe4e6298995a8342b4aca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 06:13:00 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 24 Jan 2020 06:13:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 24 Jan 2020 06:13:11 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 24 Jan 2020 06:13:11 GMT
EXPOSE 80
# Fri, 24 Jan 2020 06:13:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Jan 2020 06:13:11 GMT
CMD ["traefik"]
# Fri, 24 Jan 2020 06:13:12 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0520ea16e7f6377da620429123e1719b05706a467405f9f0e316903e8e1e3115`  
		Last Modified: Fri, 24 Jan 2020 06:13:50 GMT  
		Size: 694.5 KB (694516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5fe297ffea46a9bc6c4835ba3be1f448489b318393b4e21359be110bfbb8c6`  
		Last Modified: Fri, 24 Jan 2020 06:14:27 GMT  
		Size: 23.5 MB (23546270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b709b3720f84d639406bffe2c590c3ca2a41f646204f2dbb712a92bbd372b778`  
		Last Modified: Fri, 24 Jan 2020 06:14:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:59849962d6b994b67dc7fbc511912c5a1b87944e9b1fda436acb6502c53506a8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.3 MB (25301946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5307869ccfa13af9d37cbe35f32b4bfa91f47eb7cb00bad6cfdfbac45293e452`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 20:52:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 23 Jan 2020 20:52:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 23 Jan 2020 20:52:38 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 23 Jan 2020 20:52:39 GMT
EXPOSE 80
# Thu, 23 Jan 2020 20:52:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jan 2020 20:52:42 GMT
CMD ["traefik"]
# Thu, 23 Jan 2020 20:52:43 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cce0b3f7bff62be2da6a6ad84b3c9f19602e97675f95f1f29a72440b8e0de2`  
		Last Modified: Thu, 23 Jan 2020 20:53:14 GMT  
		Size: 697.8 KB (697843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d03b0a042ba73cfa9ff088a916bb4dd22cec09c6862278e94c8f4445863f12`  
		Last Modified: Thu, 23 Jan 2020 20:54:01 GMT  
		Size: 22.0 MB (22032328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c7026f34a4d522e997bb9203822966f0365b1d11745be187098906406a66e3`  
		Last Modified: Thu, 23 Jan 2020 20:53:49 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:c8fb04d8e9dc6d90c50f0aef2fb297e6f60eb5b3dfbf7e54c867f529d2e9e921
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25175660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb79bfa9ac897ef9b92d59e867f29384b4de2dd09b4661d3bbed24db2c24c49f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 23:06:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 23 Jan 2020 23:06:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 23 Jan 2020 23:06:54 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 23 Jan 2020 23:06:55 GMT
EXPOSE 80
# Thu, 23 Jan 2020 23:06:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jan 2020 23:06:56 GMT
CMD ["traefik"]
# Thu, 23 Jan 2020 23:06:57 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5302a139894873055677d3d78220a84bb6ac687403a19e1a6ad9d6b5cac436f`  
		Last Modified: Thu, 23 Jan 2020 23:07:28 GMT  
		Size: 697.9 KB (697891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b113fe6a3e0b2cd5c0ae54f9c7e91772e63de10e3c3de56637e5fc424eebeb`  
		Last Modified: Thu, 23 Jan 2020 23:07:56 GMT  
		Size: 21.8 MB (21759669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015c2eeb7e6dd0f5cfc02d219ff8d92d377955247e328fba478afb0851411309`  
		Last Modified: Thu, 23 Jan 2020 23:07:43 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:ddafd02e86095ada31c578c9381a2fb4564f06249b27582851b42933360f3fda
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1040; amd64

### `traefik:1.7-windowsservercore-1809` - windows version 10.0.17763.1040; amd64

```console
$ docker pull traefik@sha256:d9a86f1c028465d0386b6bcdcb7f0406e4b869b4c3bdb4072bb2324e3e8a5f6d
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2258629762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeaa5ea7b49d391defe940491cabea16b107869e8280058c96ec19780b6500d3`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 17 Feb 2020 06:57:13 GMT
RUN Install update 1809-amd64
# Thu, 20 Feb 2020 01:13:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 20 Feb 2020 04:10:58 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 20 Feb 2020 04:11:03 GMT
EXPOSE 80
# Thu, 20 Feb 2020 04:11:04 GMT
ENTRYPOINT ["/traefik"]
# Thu, 20 Feb 2020 04:11:06 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5405b7580792436b60c664b5fa766ea57f5a60c1d9a8c522cf53e99e4813355`  
		Size: 695.8 MB (695818606 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2061e035d6ba931d9f00238104b970d3410f4ef0d9603b4f074c7052858e01e3`  
		Last Modified: Thu, 20 Feb 2020 03:03:21 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e408e0468affea1e08f6b2f042cb317a049e054facb40203890f92a9c949a2a`  
		Last Modified: Thu, 20 Feb 2020 04:13:13 GMT  
		Size: 28.1 MB (28121068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8135def4596c3617f986272ab36a30c1b326c7958af0692f2385ba06fa14b41f`  
		Last Modified: Thu, 20 Feb 2020 04:13:06 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572b8adabe49a3ea8bc39655c4c84c2e935403b1d1912bc256db7e8197862ca9`  
		Last Modified: Thu, 20 Feb 2020 04:13:06 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc029e15049ca8e469f3bf092d9f1b6e22adce0b04a5ea52dc457c05036ae3f`  
		Last Modified: Thu, 20 Feb 2020 04:13:06 GMT  
		Size: 1.2 KB (1217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.1`

```console
$ docker pull traefik@sha256:0b55d2ea61610454d36c0309c8b63ef5ca3d0e03fd075bbd888dbb52271a7500
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.1` - linux; amd64

```console
$ docker pull traefik@sha256:f44bc748fa7e63a526b34ded810d1c3eb0eff4d85d3a756d3504ad8bb1f15cc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.0 MB (23035783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:651438efd845b3eebc67b9d8f8fa1a472ff7d6b6335d708361dd5e8eb13ba4a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Feb 2020 23:43:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.4/traefik_v2.1.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Feb 2020 23:43:00 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Feb 2020 23:43:01 GMT
EXPOSE 80
# Thu, 06 Feb 2020 23:43:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Feb 2020 23:43:01 GMT
CMD ["traefik"]
# Thu, 06 Feb 2020 23:43:02 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c141e361698e17a696b4b6bccfed69dc1eb931474405e31a0c907c01f4e272a6`  
		Last Modified: Thu, 06 Feb 2020 23:44:04 GMT  
		Size: 694.2 KB (694182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79168d1112b903e1741ab90b5aedcd760811b4de9d8971d4d4fa81f71a540659`  
		Last Modified: Thu, 06 Feb 2020 23:44:09 GMT  
		Size: 19.5 MB (19538278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d494c7ddd01f20eed6faefdb17e356f86de35fba80c674f675ef8af14b88e33`  
		Last Modified: Thu, 06 Feb 2020 23:44:03 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.1` - linux; arm variant v6

```console
$ docker pull traefik@sha256:8874d5dcb885073dc662c3205ae35984ae552a2db1673030bdb9ba537cc7d307
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21620174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba70568d5b80052e457a3058c2067512e2c5adfd92b5c9389644fa9f4830551b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Feb 2020 22:49:45 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.4/traefik_v2.1.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Feb 2020 22:49:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Feb 2020 22:49:46 GMT
EXPOSE 80
# Thu, 06 Feb 2020 22:49:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Feb 2020 22:49:47 GMT
CMD ["traefik"]
# Thu, 06 Feb 2020 22:49:48 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a045f3facd048d78ccec1317c0b8d3aa5e1b76f175b643f80c704ec2aa89f8`  
		Last Modified: Thu, 06 Feb 2020 22:51:40 GMT  
		Size: 698.0 KB (698013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9745c2a4ff5d2bfcd64252391c39fa81b12e6b88cabbc57384a3dea3b2d4222`  
		Last Modified: Thu, 06 Feb 2020 22:51:51 GMT  
		Size: 18.3 MB (18304232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e4d0ccb0157397196b8cf9cb3914252dc11ff9e26cecef56daa5e722d20104`  
		Last Modified: Thu, 06 Feb 2020 22:51:38 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:a87d68c5513f8449083099aecc1015397c7cd9e4c9941907f41fa82bc6dfa9ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21411878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0512a89fe17b4ad94d0f6439d0ec527c45e0ac985fa4dd0fd571b5c3875301ea`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Feb 2020 22:44:30 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.4/traefik_v2.1.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Feb 2020 22:44:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Feb 2020 22:44:31 GMT
EXPOSE 80
# Thu, 06 Feb 2020 22:44:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Feb 2020 22:44:32 GMT
CMD ["traefik"]
# Thu, 06 Feb 2020 22:44:33 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5c788179332343fbcbc8b97673406752232ca36894176cc87ece20ee279754`  
		Last Modified: Thu, 06 Feb 2020 22:47:56 GMT  
		Size: 696.0 KB (696043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c407d1e0b29391431bfef58f5bc2a55eaecbfdb70a55b5f9c8ef92e83ebf3b13`  
		Last Modified: Thu, 06 Feb 2020 22:48:08 GMT  
		Size: 18.0 MB (17992393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609ef9e236c8bf18f9a1bfef77c2b60092d81692ff465610c8c5ce4eef7bffc8`  
		Last Modified: Thu, 06 Feb 2020 22:47:55 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.1.4`

```console
$ docker pull traefik@sha256:0b55d2ea61610454d36c0309c8b63ef5ca3d0e03fd075bbd888dbb52271a7500
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.1.4` - linux; amd64

```console
$ docker pull traefik@sha256:f44bc748fa7e63a526b34ded810d1c3eb0eff4d85d3a756d3504ad8bb1f15cc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.0 MB (23035783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:651438efd845b3eebc67b9d8f8fa1a472ff7d6b6335d708361dd5e8eb13ba4a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Feb 2020 23:43:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.4/traefik_v2.1.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Feb 2020 23:43:00 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Feb 2020 23:43:01 GMT
EXPOSE 80
# Thu, 06 Feb 2020 23:43:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Feb 2020 23:43:01 GMT
CMD ["traefik"]
# Thu, 06 Feb 2020 23:43:02 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c141e361698e17a696b4b6bccfed69dc1eb931474405e31a0c907c01f4e272a6`  
		Last Modified: Thu, 06 Feb 2020 23:44:04 GMT  
		Size: 694.2 KB (694182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79168d1112b903e1741ab90b5aedcd760811b4de9d8971d4d4fa81f71a540659`  
		Last Modified: Thu, 06 Feb 2020 23:44:09 GMT  
		Size: 19.5 MB (19538278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d494c7ddd01f20eed6faefdb17e356f86de35fba80c674f675ef8af14b88e33`  
		Last Modified: Thu, 06 Feb 2020 23:44:03 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.1.4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:8874d5dcb885073dc662c3205ae35984ae552a2db1673030bdb9ba537cc7d307
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21620174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba70568d5b80052e457a3058c2067512e2c5adfd92b5c9389644fa9f4830551b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Feb 2020 22:49:45 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.4/traefik_v2.1.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Feb 2020 22:49:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Feb 2020 22:49:46 GMT
EXPOSE 80
# Thu, 06 Feb 2020 22:49:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Feb 2020 22:49:47 GMT
CMD ["traefik"]
# Thu, 06 Feb 2020 22:49:48 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a045f3facd048d78ccec1317c0b8d3aa5e1b76f175b643f80c704ec2aa89f8`  
		Last Modified: Thu, 06 Feb 2020 22:51:40 GMT  
		Size: 698.0 KB (698013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9745c2a4ff5d2bfcd64252391c39fa81b12e6b88cabbc57384a3dea3b2d4222`  
		Last Modified: Thu, 06 Feb 2020 22:51:51 GMT  
		Size: 18.3 MB (18304232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e4d0ccb0157397196b8cf9cb3914252dc11ff9e26cecef56daa5e722d20104`  
		Last Modified: Thu, 06 Feb 2020 22:51:38 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.1.4` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:a87d68c5513f8449083099aecc1015397c7cd9e4c9941907f41fa82bc6dfa9ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21411878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0512a89fe17b4ad94d0f6439d0ec527c45e0ac985fa4dd0fd571b5c3875301ea`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Feb 2020 22:44:30 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.4/traefik_v2.1.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Feb 2020 22:44:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Feb 2020 22:44:31 GMT
EXPOSE 80
# Thu, 06 Feb 2020 22:44:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Feb 2020 22:44:32 GMT
CMD ["traefik"]
# Thu, 06 Feb 2020 22:44:33 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5c788179332343fbcbc8b97673406752232ca36894176cc87ece20ee279754`  
		Last Modified: Thu, 06 Feb 2020 22:47:56 GMT  
		Size: 696.0 KB (696043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c407d1e0b29391431bfef58f5bc2a55eaecbfdb70a55b5f9c8ef92e83ebf3b13`  
		Last Modified: Thu, 06 Feb 2020 22:48:08 GMT  
		Size: 18.0 MB (17992393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609ef9e236c8bf18f9a1bfef77c2b60092d81692ff465610c8c5ce4eef7bffc8`  
		Last Modified: Thu, 06 Feb 2020 22:47:55 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.1.4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:0259147e1c2948488566cce22add60c4c9d015c0ab83c0cad5326369207ffdb2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1040; amd64

### `traefik:2.1.4-windowsservercore-1809` - windows version 10.0.17763.1040; amd64

```console
$ docker pull traefik@sha256:0d8a4d21a3ead1268dda0b75994711ed4a9e1442b7c360fb4b0b72bcb737cbd0
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2254614482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89f4d9bbba7707130be947cacf6d7bf25d0c0fa309e0bc57a1c01d2c56a14580`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 17 Feb 2020 06:57:13 GMT
RUN Install update 1809-amd64
# Thu, 20 Feb 2020 01:13:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 20 Feb 2020 04:09:34 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.4/traefik_v2.1.4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 20 Feb 2020 04:09:38 GMT
EXPOSE 80
# Thu, 20 Feb 2020 04:09:40 GMT
ENTRYPOINT ["/traefik"]
# Thu, 20 Feb 2020 04:09:41 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5405b7580792436b60c664b5fa766ea57f5a60c1d9a8c522cf53e99e4813355`  
		Size: 695.8 MB (695818606 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2061e035d6ba931d9f00238104b970d3410f4ef0d9603b4f074c7052858e01e3`  
		Last Modified: Thu, 20 Feb 2020 03:03:21 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c60a73e575d57222e8843fb64304b2ad26e626f1a8e630b96eb634b4084ec2`  
		Last Modified: Thu, 20 Feb 2020 04:12:03 GMT  
		Size: 24.1 MB (24105807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b74827fa03828ff650d42ccbd438a71c76f21f75d808d9a4edc1d49c98f6ce`  
		Last Modified: Thu, 20 Feb 2020 04:11:38 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1325439ba377e72162df98641f409c9d49c72bb29a932bdf9fe3faae9898aa2`  
		Last Modified: Thu, 20 Feb 2020 04:11:38 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c08705395bfeaf239a907f9b9241976a6a7fd77a367b4d3d3523f86a735ca4a`  
		Last Modified: Thu, 20 Feb 2020 04:11:39 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:0259147e1c2948488566cce22add60c4c9d015c0ab83c0cad5326369207ffdb2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1040; amd64

### `traefik:2.1-windowsservercore-1809` - windows version 10.0.17763.1040; amd64

```console
$ docker pull traefik@sha256:0d8a4d21a3ead1268dda0b75994711ed4a9e1442b7c360fb4b0b72bcb737cbd0
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2254614482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89f4d9bbba7707130be947cacf6d7bf25d0c0fa309e0bc57a1c01d2c56a14580`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 17 Feb 2020 06:57:13 GMT
RUN Install update 1809-amd64
# Thu, 20 Feb 2020 01:13:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 20 Feb 2020 04:09:34 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.4/traefik_v2.1.4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 20 Feb 2020 04:09:38 GMT
EXPOSE 80
# Thu, 20 Feb 2020 04:09:40 GMT
ENTRYPOINT ["/traefik"]
# Thu, 20 Feb 2020 04:09:41 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5405b7580792436b60c664b5fa766ea57f5a60c1d9a8c522cf53e99e4813355`  
		Size: 695.8 MB (695818606 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2061e035d6ba931d9f00238104b970d3410f4ef0d9603b4f074c7052858e01e3`  
		Last Modified: Thu, 20 Feb 2020 03:03:21 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c60a73e575d57222e8843fb64304b2ad26e626f1a8e630b96eb634b4084ec2`  
		Last Modified: Thu, 20 Feb 2020 04:12:03 GMT  
		Size: 24.1 MB (24105807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b74827fa03828ff650d42ccbd438a71c76f21f75d808d9a4edc1d49c98f6ce`  
		Last Modified: Thu, 20 Feb 2020 04:11:38 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1325439ba377e72162df98641f409c9d49c72bb29a932bdf9fe3faae9898aa2`  
		Last Modified: Thu, 20 Feb 2020 04:11:38 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c08705395bfeaf239a907f9b9241976a6a7fd77a367b4d3d3523f86a735ca4a`  
		Last Modified: Thu, 20 Feb 2020 04:11:39 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:cantal`

```console
$ docker pull traefik@sha256:0b55d2ea61610454d36c0309c8b63ef5ca3d0e03fd075bbd888dbb52271a7500
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:cantal` - linux; amd64

```console
$ docker pull traefik@sha256:f44bc748fa7e63a526b34ded810d1c3eb0eff4d85d3a756d3504ad8bb1f15cc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.0 MB (23035783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:651438efd845b3eebc67b9d8f8fa1a472ff7d6b6335d708361dd5e8eb13ba4a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Feb 2020 23:43:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.4/traefik_v2.1.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Feb 2020 23:43:00 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Feb 2020 23:43:01 GMT
EXPOSE 80
# Thu, 06 Feb 2020 23:43:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Feb 2020 23:43:01 GMT
CMD ["traefik"]
# Thu, 06 Feb 2020 23:43:02 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c141e361698e17a696b4b6bccfed69dc1eb931474405e31a0c907c01f4e272a6`  
		Last Modified: Thu, 06 Feb 2020 23:44:04 GMT  
		Size: 694.2 KB (694182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79168d1112b903e1741ab90b5aedcd760811b4de9d8971d4d4fa81f71a540659`  
		Last Modified: Thu, 06 Feb 2020 23:44:09 GMT  
		Size: 19.5 MB (19538278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d494c7ddd01f20eed6faefdb17e356f86de35fba80c674f675ef8af14b88e33`  
		Last Modified: Thu, 06 Feb 2020 23:44:03 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:cantal` - linux; arm variant v6

```console
$ docker pull traefik@sha256:8874d5dcb885073dc662c3205ae35984ae552a2db1673030bdb9ba537cc7d307
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21620174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba70568d5b80052e457a3058c2067512e2c5adfd92b5c9389644fa9f4830551b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Feb 2020 22:49:45 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.4/traefik_v2.1.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Feb 2020 22:49:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Feb 2020 22:49:46 GMT
EXPOSE 80
# Thu, 06 Feb 2020 22:49:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Feb 2020 22:49:47 GMT
CMD ["traefik"]
# Thu, 06 Feb 2020 22:49:48 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a045f3facd048d78ccec1317c0b8d3aa5e1b76f175b643f80c704ec2aa89f8`  
		Last Modified: Thu, 06 Feb 2020 22:51:40 GMT  
		Size: 698.0 KB (698013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9745c2a4ff5d2bfcd64252391c39fa81b12e6b88cabbc57384a3dea3b2d4222`  
		Last Modified: Thu, 06 Feb 2020 22:51:51 GMT  
		Size: 18.3 MB (18304232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e4d0ccb0157397196b8cf9cb3914252dc11ff9e26cecef56daa5e722d20104`  
		Last Modified: Thu, 06 Feb 2020 22:51:38 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:cantal` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:a87d68c5513f8449083099aecc1015397c7cd9e4c9941907f41fa82bc6dfa9ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21411878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0512a89fe17b4ad94d0f6439d0ec527c45e0ac985fa4dd0fd571b5c3875301ea`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Feb 2020 22:44:30 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.4/traefik_v2.1.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Feb 2020 22:44:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Feb 2020 22:44:31 GMT
EXPOSE 80
# Thu, 06 Feb 2020 22:44:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Feb 2020 22:44:32 GMT
CMD ["traefik"]
# Thu, 06 Feb 2020 22:44:33 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5c788179332343fbcbc8b97673406752232ca36894176cc87ece20ee279754`  
		Last Modified: Thu, 06 Feb 2020 22:47:56 GMT  
		Size: 696.0 KB (696043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c407d1e0b29391431bfef58f5bc2a55eaecbfdb70a55b5f9c8ef92e83ebf3b13`  
		Last Modified: Thu, 06 Feb 2020 22:48:08 GMT  
		Size: 18.0 MB (17992393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609ef9e236c8bf18f9a1bfef77c2b60092d81692ff465610c8c5ce4eef7bffc8`  
		Last Modified: Thu, 06 Feb 2020 22:47:55 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:cantal-windowsservercore-1809`

```console
$ docker pull traefik@sha256:0259147e1c2948488566cce22add60c4c9d015c0ab83c0cad5326369207ffdb2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1040; amd64

### `traefik:cantal-windowsservercore-1809` - windows version 10.0.17763.1040; amd64

```console
$ docker pull traefik@sha256:0d8a4d21a3ead1268dda0b75994711ed4a9e1442b7c360fb4b0b72bcb737cbd0
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2254614482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89f4d9bbba7707130be947cacf6d7bf25d0c0fa309e0bc57a1c01d2c56a14580`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 17 Feb 2020 06:57:13 GMT
RUN Install update 1809-amd64
# Thu, 20 Feb 2020 01:13:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 20 Feb 2020 04:09:34 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.4/traefik_v2.1.4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 20 Feb 2020 04:09:38 GMT
EXPOSE 80
# Thu, 20 Feb 2020 04:09:40 GMT
ENTRYPOINT ["/traefik"]
# Thu, 20 Feb 2020 04:09:41 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5405b7580792436b60c664b5fa766ea57f5a60c1d9a8c522cf53e99e4813355`  
		Size: 695.8 MB (695818606 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2061e035d6ba931d9f00238104b970d3410f4ef0d9603b4f074c7052858e01e3`  
		Last Modified: Thu, 20 Feb 2020 03:03:21 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c60a73e575d57222e8843fb64304b2ad26e626f1a8e630b96eb634b4084ec2`  
		Last Modified: Thu, 20 Feb 2020 04:12:03 GMT  
		Size: 24.1 MB (24105807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b74827fa03828ff650d42ccbd438a71c76f21f75d808d9a4edc1d49c98f6ce`  
		Last Modified: Thu, 20 Feb 2020 04:11:38 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1325439ba377e72162df98641f409c9d49c72bb29a932bdf9fe3faae9898aa2`  
		Last Modified: Thu, 20 Feb 2020 04:11:38 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c08705395bfeaf239a907f9b9241976a6a7fd77a367b4d3d3523f86a735ca4a`  
		Last Modified: Thu, 20 Feb 2020 04:11:39 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:0b55d2ea61610454d36c0309c8b63ef5ca3d0e03fd075bbd888dbb52271a7500
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:f44bc748fa7e63a526b34ded810d1c3eb0eff4d85d3a756d3504ad8bb1f15cc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.0 MB (23035783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:651438efd845b3eebc67b9d8f8fa1a472ff7d6b6335d708361dd5e8eb13ba4a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Feb 2020 23:43:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.4/traefik_v2.1.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Feb 2020 23:43:00 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Feb 2020 23:43:01 GMT
EXPOSE 80
# Thu, 06 Feb 2020 23:43:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Feb 2020 23:43:01 GMT
CMD ["traefik"]
# Thu, 06 Feb 2020 23:43:02 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c141e361698e17a696b4b6bccfed69dc1eb931474405e31a0c907c01f4e272a6`  
		Last Modified: Thu, 06 Feb 2020 23:44:04 GMT  
		Size: 694.2 KB (694182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79168d1112b903e1741ab90b5aedcd760811b4de9d8971d4d4fa81f71a540659`  
		Last Modified: Thu, 06 Feb 2020 23:44:09 GMT  
		Size: 19.5 MB (19538278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d494c7ddd01f20eed6faefdb17e356f86de35fba80c674f675ef8af14b88e33`  
		Last Modified: Thu, 06 Feb 2020 23:44:03 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:8874d5dcb885073dc662c3205ae35984ae552a2db1673030bdb9ba537cc7d307
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21620174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba70568d5b80052e457a3058c2067512e2c5adfd92b5c9389644fa9f4830551b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Feb 2020 22:49:45 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.4/traefik_v2.1.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Feb 2020 22:49:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Feb 2020 22:49:46 GMT
EXPOSE 80
# Thu, 06 Feb 2020 22:49:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Feb 2020 22:49:47 GMT
CMD ["traefik"]
# Thu, 06 Feb 2020 22:49:48 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a045f3facd048d78ccec1317c0b8d3aa5e1b76f175b643f80c704ec2aa89f8`  
		Last Modified: Thu, 06 Feb 2020 22:51:40 GMT  
		Size: 698.0 KB (698013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9745c2a4ff5d2bfcd64252391c39fa81b12e6b88cabbc57384a3dea3b2d4222`  
		Last Modified: Thu, 06 Feb 2020 22:51:51 GMT  
		Size: 18.3 MB (18304232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e4d0ccb0157397196b8cf9cb3914252dc11ff9e26cecef56daa5e722d20104`  
		Last Modified: Thu, 06 Feb 2020 22:51:38 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:a87d68c5513f8449083099aecc1015397c7cd9e4c9941907f41fa82bc6dfa9ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21411878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0512a89fe17b4ad94d0f6439d0ec527c45e0ac985fa4dd0fd571b5c3875301ea`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Feb 2020 22:44:30 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.4/traefik_v2.1.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Feb 2020 22:44:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Feb 2020 22:44:31 GMT
EXPOSE 80
# Thu, 06 Feb 2020 22:44:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Feb 2020 22:44:32 GMT
CMD ["traefik"]
# Thu, 06 Feb 2020 22:44:33 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5c788179332343fbcbc8b97673406752232ca36894176cc87ece20ee279754`  
		Last Modified: Thu, 06 Feb 2020 22:47:56 GMT  
		Size: 696.0 KB (696043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c407d1e0b29391431bfef58f5bc2a55eaecbfdb70a55b5f9c8ef92e83ebf3b13`  
		Last Modified: Thu, 06 Feb 2020 22:48:08 GMT  
		Size: 18.0 MB (17992393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609ef9e236c8bf18f9a1bfef77c2b60092d81692ff465610c8c5ce4eef7bffc8`  
		Last Modified: Thu, 06 Feb 2020 22:47:55 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles`

```console
$ docker pull traefik@sha256:5ec34caf19d114f8f0ed76f9bc3dad6ba8cf6d13a1575c4294b59b77709def39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles` - linux; amd64

```console
$ docker pull traefik@sha256:3b1c4d57c57d125a5d949d463d41882fefc957ce117db226aace4e7314e82d5c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.0 MB (24005352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96c63a7d3e502fcbbd8937a2523368c22d0edd1788b8389af095f64038318834`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 27 Aug 2019 01:00:22 GMT
COPY file:091d2a65366d205fc0db557b2f495da40adb5a33c9d656d02c3ea08bb22f6c4d in /etc/ssl/certs/ 
# Mon, 21 Oct 2019 22:26:52 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 10 Dec 2019 22:31:38 GMT
COPY file:be1ea92a6d3f63051c9ae787ca41c986b81a56ce7f8b8347b97c3ddc3b4471f5 in / 
# Tue, 10 Dec 2019 22:31:38 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:31:38 GMT
VOLUME [/tmp]
# Tue, 10 Dec 2019 22:31:38 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 22:31:39 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:42e7d26ec3785f8ce0f20e327cf72404ee054ba022ce9068ad2d28c52e82db2a`  
		Last Modified: Tue, 27 Aug 2019 01:00:52 GMT  
		Size: 132.0 KB (132022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a753f02eeffef33e5e071a6feac9e12fffb36330fc7ef5441f378d0ce67c528`  
		Last Modified: Mon, 21 Oct 2019 22:27:25 GMT  
		Size: 327.3 KB (327346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab927d94d255c72862c3e7ada3f6cdb36f90926b7a8913a080062b17d73f186b`  
		Last Modified: Tue, 10 Dec 2019 22:32:27 GMT  
		Size: 23.5 MB (23545984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm variant v6

```console
$ docker pull traefik@sha256:3a32e589b7d538f688f0a4d5777ab21dc2e946e22a1b08872aaad72b4192976e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.5 MB (22491539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:099411d81ac7bf28b232625f19ecc6590f39c3920418958b3056caa4f85815c4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Mon, 26 Aug 2019 23:54:26 GMT
COPY file:091d2a65366d205fc0db557b2f495da40adb5a33c9d656d02c3ea08bb22f6c4d in /etc/ssl/certs/ 
# Mon, 21 Oct 2019 20:27:55 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 10 Dec 2019 21:57:12 GMT
COPY file:ad6d99c4dea9edfff1bf18494e1c85b8a82b1a74f77a8bf3f437bd05222fbf79 in / 
# Tue, 10 Dec 2019 21:57:14 GMT
EXPOSE 80
# Tue, 10 Dec 2019 21:57:15 GMT
VOLUME [/tmp]
# Tue, 10 Dec 2019 21:57:16 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 21:57:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:506698346e0f5f486b919abaa7bc72252b3dc553cb28e0d1a5e2b6f3708cf4c0`  
		Last Modified: Mon, 26 Aug 2019 23:55:08 GMT  
		Size: 132.0 KB (132026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46037320e6487ea40f4dfb2c29d120090739bc20051bca67eb5e64a072973136`  
		Last Modified: Mon, 21 Oct 2019 20:28:50 GMT  
		Size: 327.4 KB (327388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0d7ab9d9ce392bdaa622a30db2df3963e7ac8b19c846fddc788b2f7fd3f890`  
		Last Modified: Tue, 10 Dec 2019 21:58:07 GMT  
		Size: 22.0 MB (22032125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3a587a9647aca9d58c237389157512cf349f00e99afc0f33959501bc5366b489
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.2 MB (22219190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:843151930dcd29bc722fa2e9949bcecfcb0020d961037b85983f47017aa38a58`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 27 Aug 2019 00:16:41 GMT
COPY file:091d2a65366d205fc0db557b2f495da40adb5a33c9d656d02c3ea08bb22f6c4d in /etc/ssl/certs/ 
# Mon, 21 Oct 2019 23:22:44 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 10 Dec 2019 22:39:48 GMT
COPY file:2548a09c5388b09356e8109d52a2261b02b840df1156718406457af4ef9eedcd in / 
# Tue, 10 Dec 2019 22:39:50 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:39:50 GMT
VOLUME [/tmp]
# Tue, 10 Dec 2019 22:39:51 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 22:39:51 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f07a1cd6fb05ab2fb5b66f5326144f82e52f5580df40a42e400637f8a8f9c6d8`  
		Last Modified: Tue, 27 Aug 2019 00:17:31 GMT  
		Size: 132.0 KB (132021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2afd881e5b94f57a79b2f6bcd9d637c2f7a6aa910f4013045b8653ebe29fdb`  
		Last Modified: Mon, 21 Oct 2019 23:23:36 GMT  
		Size: 327.4 KB (327378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b05c8936168a3f333423ce8dca6ed7e5ad1890ce50b95da487f61aa83440e26`  
		Last Modified: Tue, 10 Dec 2019 22:40:39 GMT  
		Size: 21.8 MB (21759791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-alpine`

```console
$ docker pull traefik@sha256:710a1f7845f02e1f1d694a83bf41042c6dbe47eb9ee3b2bf0cf35b3eaa6c2b4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:8fa8c4faa799bf8f632fe4af56768e3e1f302bf2d63fc1cd7c7752a36ee364a3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27028116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee8378e05f99d815e7131d19af5863e997f0b35d694fe4e6298995a8342b4aca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 06:13:00 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 24 Jan 2020 06:13:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 24 Jan 2020 06:13:11 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 24 Jan 2020 06:13:11 GMT
EXPOSE 80
# Fri, 24 Jan 2020 06:13:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Jan 2020 06:13:11 GMT
CMD ["traefik"]
# Fri, 24 Jan 2020 06:13:12 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0520ea16e7f6377da620429123e1719b05706a467405f9f0e316903e8e1e3115`  
		Last Modified: Fri, 24 Jan 2020 06:13:50 GMT  
		Size: 694.5 KB (694516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5fe297ffea46a9bc6c4835ba3be1f448489b318393b4e21359be110bfbb8c6`  
		Last Modified: Fri, 24 Jan 2020 06:14:27 GMT  
		Size: 23.5 MB (23546270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b709b3720f84d639406bffe2c590c3ca2a41f646204f2dbb712a92bbd372b778`  
		Last Modified: Fri, 24 Jan 2020 06:14:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:59849962d6b994b67dc7fbc511912c5a1b87944e9b1fda436acb6502c53506a8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.3 MB (25301946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5307869ccfa13af9d37cbe35f32b4bfa91f47eb7cb00bad6cfdfbac45293e452`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 20:52:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 23 Jan 2020 20:52:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 23 Jan 2020 20:52:38 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 23 Jan 2020 20:52:39 GMT
EXPOSE 80
# Thu, 23 Jan 2020 20:52:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jan 2020 20:52:42 GMT
CMD ["traefik"]
# Thu, 23 Jan 2020 20:52:43 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cce0b3f7bff62be2da6a6ad84b3c9f19602e97675f95f1f29a72440b8e0de2`  
		Last Modified: Thu, 23 Jan 2020 20:53:14 GMT  
		Size: 697.8 KB (697843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d03b0a042ba73cfa9ff088a916bb4dd22cec09c6862278e94c8f4445863f12`  
		Last Modified: Thu, 23 Jan 2020 20:54:01 GMT  
		Size: 22.0 MB (22032328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c7026f34a4d522e997bb9203822966f0365b1d11745be187098906406a66e3`  
		Last Modified: Thu, 23 Jan 2020 20:53:49 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:c8fb04d8e9dc6d90c50f0aef2fb297e6f60eb5b3dfbf7e54c867f529d2e9e921
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25175660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb79bfa9ac897ef9b92d59e867f29384b4de2dd09b4661d3bbed24db2c24c49f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 23:06:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 23 Jan 2020 23:06:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 23 Jan 2020 23:06:54 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 23 Jan 2020 23:06:55 GMT
EXPOSE 80
# Thu, 23 Jan 2020 23:06:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jan 2020 23:06:56 GMT
CMD ["traefik"]
# Thu, 23 Jan 2020 23:06:57 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5302a139894873055677d3d78220a84bb6ac687403a19e1a6ad9d6b5cac436f`  
		Last Modified: Thu, 23 Jan 2020 23:07:28 GMT  
		Size: 697.9 KB (697891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b113fe6a3e0b2cd5c0ae54f9c7e91772e63de10e3c3de56637e5fc424eebeb`  
		Last Modified: Thu, 23 Jan 2020 23:07:56 GMT  
		Size: 21.8 MB (21759669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015c2eeb7e6dd0f5cfc02d219ff8d92d377955247e328fba478afb0851411309`  
		Last Modified: Thu, 23 Jan 2020 23:07:43 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-windowsservercore-1809`

```console
$ docker pull traefik@sha256:ddafd02e86095ada31c578c9381a2fb4564f06249b27582851b42933360f3fda
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1040; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.1040; amd64

```console
$ docker pull traefik@sha256:d9a86f1c028465d0386b6bcdcb7f0406e4b869b4c3bdb4072bb2324e3e8a5f6d
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2258629762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeaa5ea7b49d391defe940491cabea16b107869e8280058c96ec19780b6500d3`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 17 Feb 2020 06:57:13 GMT
RUN Install update 1809-amd64
# Thu, 20 Feb 2020 01:13:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 20 Feb 2020 04:10:58 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 20 Feb 2020 04:11:03 GMT
EXPOSE 80
# Thu, 20 Feb 2020 04:11:04 GMT
ENTRYPOINT ["/traefik"]
# Thu, 20 Feb 2020 04:11:06 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5405b7580792436b60c664b5fa766ea57f5a60c1d9a8c522cf53e99e4813355`  
		Size: 695.8 MB (695818606 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2061e035d6ba931d9f00238104b970d3410f4ef0d9603b4f074c7052858e01e3`  
		Last Modified: Thu, 20 Feb 2020 03:03:21 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e408e0468affea1e08f6b2f042cb317a049e054facb40203890f92a9c949a2a`  
		Last Modified: Thu, 20 Feb 2020 04:13:13 GMT  
		Size: 28.1 MB (28121068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8135def4596c3617f986272ab36a30c1b326c7958af0692f2385ba06fa14b41f`  
		Last Modified: Thu, 20 Feb 2020 04:13:06 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572b8adabe49a3ea8bc39655c4c84c2e935403b1d1912bc256db7e8197862ca9`  
		Last Modified: Thu, 20 Feb 2020 04:13:06 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc029e15049ca8e469f3bf092d9f1b6e22adce0b04a5ea52dc457c05036ae3f`  
		Last Modified: Thu, 20 Feb 2020 04:13:06 GMT  
		Size: 1.2 KB (1217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7`

```console
$ docker pull traefik@sha256:5ec34caf19d114f8f0ed76f9bc3dad6ba8cf6d13a1575c4294b59b77709def39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7` - linux; amd64

```console
$ docker pull traefik@sha256:3b1c4d57c57d125a5d949d463d41882fefc957ce117db226aace4e7314e82d5c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.0 MB (24005352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96c63a7d3e502fcbbd8937a2523368c22d0edd1788b8389af095f64038318834`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 27 Aug 2019 01:00:22 GMT
COPY file:091d2a65366d205fc0db557b2f495da40adb5a33c9d656d02c3ea08bb22f6c4d in /etc/ssl/certs/ 
# Mon, 21 Oct 2019 22:26:52 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 10 Dec 2019 22:31:38 GMT
COPY file:be1ea92a6d3f63051c9ae787ca41c986b81a56ce7f8b8347b97c3ddc3b4471f5 in / 
# Tue, 10 Dec 2019 22:31:38 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:31:38 GMT
VOLUME [/tmp]
# Tue, 10 Dec 2019 22:31:38 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 22:31:39 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:42e7d26ec3785f8ce0f20e327cf72404ee054ba022ce9068ad2d28c52e82db2a`  
		Last Modified: Tue, 27 Aug 2019 01:00:52 GMT  
		Size: 132.0 KB (132022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a753f02eeffef33e5e071a6feac9e12fffb36330fc7ef5441f378d0ce67c528`  
		Last Modified: Mon, 21 Oct 2019 22:27:25 GMT  
		Size: 327.3 KB (327346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab927d94d255c72862c3e7ada3f6cdb36f90926b7a8913a080062b17d73f186b`  
		Last Modified: Tue, 10 Dec 2019 22:32:27 GMT  
		Size: 23.5 MB (23545984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:3a32e589b7d538f688f0a4d5777ab21dc2e946e22a1b08872aaad72b4192976e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.5 MB (22491539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:099411d81ac7bf28b232625f19ecc6590f39c3920418958b3056caa4f85815c4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Mon, 26 Aug 2019 23:54:26 GMT
COPY file:091d2a65366d205fc0db557b2f495da40adb5a33c9d656d02c3ea08bb22f6c4d in /etc/ssl/certs/ 
# Mon, 21 Oct 2019 20:27:55 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 10 Dec 2019 21:57:12 GMT
COPY file:ad6d99c4dea9edfff1bf18494e1c85b8a82b1a74f77a8bf3f437bd05222fbf79 in / 
# Tue, 10 Dec 2019 21:57:14 GMT
EXPOSE 80
# Tue, 10 Dec 2019 21:57:15 GMT
VOLUME [/tmp]
# Tue, 10 Dec 2019 21:57:16 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 21:57:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:506698346e0f5f486b919abaa7bc72252b3dc553cb28e0d1a5e2b6f3708cf4c0`  
		Last Modified: Mon, 26 Aug 2019 23:55:08 GMT  
		Size: 132.0 KB (132026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46037320e6487ea40f4dfb2c29d120090739bc20051bca67eb5e64a072973136`  
		Last Modified: Mon, 21 Oct 2019 20:28:50 GMT  
		Size: 327.4 KB (327388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0d7ab9d9ce392bdaa622a30db2df3963e7ac8b19c846fddc788b2f7fd3f890`  
		Last Modified: Tue, 10 Dec 2019 21:58:07 GMT  
		Size: 22.0 MB (22032125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3a587a9647aca9d58c237389157512cf349f00e99afc0f33959501bc5366b489
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.2 MB (22219190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:843151930dcd29bc722fa2e9949bcecfcb0020d961037b85983f47017aa38a58`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 27 Aug 2019 00:16:41 GMT
COPY file:091d2a65366d205fc0db557b2f495da40adb5a33c9d656d02c3ea08bb22f6c4d in /etc/ssl/certs/ 
# Mon, 21 Oct 2019 23:22:44 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 10 Dec 2019 22:39:48 GMT
COPY file:2548a09c5388b09356e8109d52a2261b02b840df1156718406457af4ef9eedcd in / 
# Tue, 10 Dec 2019 22:39:50 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:39:50 GMT
VOLUME [/tmp]
# Tue, 10 Dec 2019 22:39:51 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 22:39:51 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f07a1cd6fb05ab2fb5b66f5326144f82e52f5580df40a42e400637f8a8f9c6d8`  
		Last Modified: Tue, 27 Aug 2019 00:17:31 GMT  
		Size: 132.0 KB (132021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2afd881e5b94f57a79b2f6bcd9d637c2f7a6aa910f4013045b8653ebe29fdb`  
		Last Modified: Mon, 21 Oct 2019 23:23:36 GMT  
		Size: 327.4 KB (327378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b05c8936168a3f333423ce8dca6ed7e5ad1890ce50b95da487f61aa83440e26`  
		Last Modified: Tue, 10 Dec 2019 22:40:39 GMT  
		Size: 21.8 MB (21759791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.21`

```console
$ docker pull traefik@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `traefik:v1.7.21-alpine`

```console
$ docker pull traefik@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `traefik:v1.7.21-windowsservercore-1809`

```console
$ docker pull traefik@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `traefik:v1.7-alpine`

```console
$ docker pull traefik@sha256:710a1f7845f02e1f1d694a83bf41042c6dbe47eb9ee3b2bf0cf35b3eaa6c2b4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:8fa8c4faa799bf8f632fe4af56768e3e1f302bf2d63fc1cd7c7752a36ee364a3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27028116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee8378e05f99d815e7131d19af5863e997f0b35d694fe4e6298995a8342b4aca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 06:13:00 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 24 Jan 2020 06:13:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 24 Jan 2020 06:13:11 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 24 Jan 2020 06:13:11 GMT
EXPOSE 80
# Fri, 24 Jan 2020 06:13:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Jan 2020 06:13:11 GMT
CMD ["traefik"]
# Fri, 24 Jan 2020 06:13:12 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0520ea16e7f6377da620429123e1719b05706a467405f9f0e316903e8e1e3115`  
		Last Modified: Fri, 24 Jan 2020 06:13:50 GMT  
		Size: 694.5 KB (694516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5fe297ffea46a9bc6c4835ba3be1f448489b318393b4e21359be110bfbb8c6`  
		Last Modified: Fri, 24 Jan 2020 06:14:27 GMT  
		Size: 23.5 MB (23546270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b709b3720f84d639406bffe2c590c3ca2a41f646204f2dbb712a92bbd372b778`  
		Last Modified: Fri, 24 Jan 2020 06:14:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:59849962d6b994b67dc7fbc511912c5a1b87944e9b1fda436acb6502c53506a8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.3 MB (25301946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5307869ccfa13af9d37cbe35f32b4bfa91f47eb7cb00bad6cfdfbac45293e452`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 20:52:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 23 Jan 2020 20:52:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 23 Jan 2020 20:52:38 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 23 Jan 2020 20:52:39 GMT
EXPOSE 80
# Thu, 23 Jan 2020 20:52:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jan 2020 20:52:42 GMT
CMD ["traefik"]
# Thu, 23 Jan 2020 20:52:43 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cce0b3f7bff62be2da6a6ad84b3c9f19602e97675f95f1f29a72440b8e0de2`  
		Last Modified: Thu, 23 Jan 2020 20:53:14 GMT  
		Size: 697.8 KB (697843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d03b0a042ba73cfa9ff088a916bb4dd22cec09c6862278e94c8f4445863f12`  
		Last Modified: Thu, 23 Jan 2020 20:54:01 GMT  
		Size: 22.0 MB (22032328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c7026f34a4d522e997bb9203822966f0365b1d11745be187098906406a66e3`  
		Last Modified: Thu, 23 Jan 2020 20:53:49 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:c8fb04d8e9dc6d90c50f0aef2fb297e6f60eb5b3dfbf7e54c867f529d2e9e921
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25175660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb79bfa9ac897ef9b92d59e867f29384b4de2dd09b4661d3bbed24db2c24c49f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 23:06:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 23 Jan 2020 23:06:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 23 Jan 2020 23:06:54 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 23 Jan 2020 23:06:55 GMT
EXPOSE 80
# Thu, 23 Jan 2020 23:06:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jan 2020 23:06:56 GMT
CMD ["traefik"]
# Thu, 23 Jan 2020 23:06:57 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5302a139894873055677d3d78220a84bb6ac687403a19e1a6ad9d6b5cac436f`  
		Last Modified: Thu, 23 Jan 2020 23:07:28 GMT  
		Size: 697.9 KB (697891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b113fe6a3e0b2cd5c0ae54f9c7e91772e63de10e3c3de56637e5fc424eebeb`  
		Last Modified: Thu, 23 Jan 2020 23:07:56 GMT  
		Size: 21.8 MB (21759669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015c2eeb7e6dd0f5cfc02d219ff8d92d377955247e328fba478afb0851411309`  
		Last Modified: Thu, 23 Jan 2020 23:07:43 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:ddafd02e86095ada31c578c9381a2fb4564f06249b27582851b42933360f3fda
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1040; amd64

### `traefik:v1.7-windowsservercore-1809` - windows version 10.0.17763.1040; amd64

```console
$ docker pull traefik@sha256:d9a86f1c028465d0386b6bcdcb7f0406e4b869b4c3bdb4072bb2324e3e8a5f6d
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2258629762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeaa5ea7b49d391defe940491cabea16b107869e8280058c96ec19780b6500d3`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 17 Feb 2020 06:57:13 GMT
RUN Install update 1809-amd64
# Thu, 20 Feb 2020 01:13:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 20 Feb 2020 04:10:58 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 20 Feb 2020 04:11:03 GMT
EXPOSE 80
# Thu, 20 Feb 2020 04:11:04 GMT
ENTRYPOINT ["/traefik"]
# Thu, 20 Feb 2020 04:11:06 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5405b7580792436b60c664b5fa766ea57f5a60c1d9a8c522cf53e99e4813355`  
		Size: 695.8 MB (695818606 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2061e035d6ba931d9f00238104b970d3410f4ef0d9603b4f074c7052858e01e3`  
		Last Modified: Thu, 20 Feb 2020 03:03:21 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e408e0468affea1e08f6b2f042cb317a049e054facb40203890f92a9c949a2a`  
		Last Modified: Thu, 20 Feb 2020 04:13:13 GMT  
		Size: 28.1 MB (28121068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8135def4596c3617f986272ab36a30c1b326c7958af0692f2385ba06fa14b41f`  
		Last Modified: Thu, 20 Feb 2020 04:13:06 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572b8adabe49a3ea8bc39655c4c84c2e935403b1d1912bc256db7e8197862ca9`  
		Last Modified: Thu, 20 Feb 2020 04:13:06 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc029e15049ca8e469f3bf092d9f1b6e22adce0b04a5ea52dc457c05036ae3f`  
		Last Modified: Thu, 20 Feb 2020 04:13:06 GMT  
		Size: 1.2 KB (1217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.1`

```console
$ docker pull traefik@sha256:0b55d2ea61610454d36c0309c8b63ef5ca3d0e03fd075bbd888dbb52271a7500
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.1` - linux; amd64

```console
$ docker pull traefik@sha256:f44bc748fa7e63a526b34ded810d1c3eb0eff4d85d3a756d3504ad8bb1f15cc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.0 MB (23035783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:651438efd845b3eebc67b9d8f8fa1a472ff7d6b6335d708361dd5e8eb13ba4a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Feb 2020 23:43:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.4/traefik_v2.1.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Feb 2020 23:43:00 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Feb 2020 23:43:01 GMT
EXPOSE 80
# Thu, 06 Feb 2020 23:43:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Feb 2020 23:43:01 GMT
CMD ["traefik"]
# Thu, 06 Feb 2020 23:43:02 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c141e361698e17a696b4b6bccfed69dc1eb931474405e31a0c907c01f4e272a6`  
		Last Modified: Thu, 06 Feb 2020 23:44:04 GMT  
		Size: 694.2 KB (694182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79168d1112b903e1741ab90b5aedcd760811b4de9d8971d4d4fa81f71a540659`  
		Last Modified: Thu, 06 Feb 2020 23:44:09 GMT  
		Size: 19.5 MB (19538278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d494c7ddd01f20eed6faefdb17e356f86de35fba80c674f675ef8af14b88e33`  
		Last Modified: Thu, 06 Feb 2020 23:44:03 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.1` - linux; arm variant v6

```console
$ docker pull traefik@sha256:8874d5dcb885073dc662c3205ae35984ae552a2db1673030bdb9ba537cc7d307
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21620174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba70568d5b80052e457a3058c2067512e2c5adfd92b5c9389644fa9f4830551b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Feb 2020 22:49:45 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.4/traefik_v2.1.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Feb 2020 22:49:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Feb 2020 22:49:46 GMT
EXPOSE 80
# Thu, 06 Feb 2020 22:49:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Feb 2020 22:49:47 GMT
CMD ["traefik"]
# Thu, 06 Feb 2020 22:49:48 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a045f3facd048d78ccec1317c0b8d3aa5e1b76f175b643f80c704ec2aa89f8`  
		Last Modified: Thu, 06 Feb 2020 22:51:40 GMT  
		Size: 698.0 KB (698013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9745c2a4ff5d2bfcd64252391c39fa81b12e6b88cabbc57384a3dea3b2d4222`  
		Last Modified: Thu, 06 Feb 2020 22:51:51 GMT  
		Size: 18.3 MB (18304232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e4d0ccb0157397196b8cf9cb3914252dc11ff9e26cecef56daa5e722d20104`  
		Last Modified: Thu, 06 Feb 2020 22:51:38 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:a87d68c5513f8449083099aecc1015397c7cd9e4c9941907f41fa82bc6dfa9ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21411878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0512a89fe17b4ad94d0f6439d0ec527c45e0ac985fa4dd0fd571b5c3875301ea`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Feb 2020 22:44:30 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.4/traefik_v2.1.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Feb 2020 22:44:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Feb 2020 22:44:31 GMT
EXPOSE 80
# Thu, 06 Feb 2020 22:44:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Feb 2020 22:44:32 GMT
CMD ["traefik"]
# Thu, 06 Feb 2020 22:44:33 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5c788179332343fbcbc8b97673406752232ca36894176cc87ece20ee279754`  
		Last Modified: Thu, 06 Feb 2020 22:47:56 GMT  
		Size: 696.0 KB (696043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c407d1e0b29391431bfef58f5bc2a55eaecbfdb70a55b5f9c8ef92e83ebf3b13`  
		Last Modified: Thu, 06 Feb 2020 22:48:08 GMT  
		Size: 18.0 MB (17992393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609ef9e236c8bf18f9a1bfef77c2b60092d81692ff465610c8c5ce4eef7bffc8`  
		Last Modified: Thu, 06 Feb 2020 22:47:55 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.1.4`

```console
$ docker pull traefik@sha256:0b55d2ea61610454d36c0309c8b63ef5ca3d0e03fd075bbd888dbb52271a7500
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.1.4` - linux; amd64

```console
$ docker pull traefik@sha256:f44bc748fa7e63a526b34ded810d1c3eb0eff4d85d3a756d3504ad8bb1f15cc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.0 MB (23035783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:651438efd845b3eebc67b9d8f8fa1a472ff7d6b6335d708361dd5e8eb13ba4a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Feb 2020 23:43:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.4/traefik_v2.1.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Feb 2020 23:43:00 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Feb 2020 23:43:01 GMT
EXPOSE 80
# Thu, 06 Feb 2020 23:43:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Feb 2020 23:43:01 GMT
CMD ["traefik"]
# Thu, 06 Feb 2020 23:43:02 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c141e361698e17a696b4b6bccfed69dc1eb931474405e31a0c907c01f4e272a6`  
		Last Modified: Thu, 06 Feb 2020 23:44:04 GMT  
		Size: 694.2 KB (694182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79168d1112b903e1741ab90b5aedcd760811b4de9d8971d4d4fa81f71a540659`  
		Last Modified: Thu, 06 Feb 2020 23:44:09 GMT  
		Size: 19.5 MB (19538278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d494c7ddd01f20eed6faefdb17e356f86de35fba80c674f675ef8af14b88e33`  
		Last Modified: Thu, 06 Feb 2020 23:44:03 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.1.4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:8874d5dcb885073dc662c3205ae35984ae552a2db1673030bdb9ba537cc7d307
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21620174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba70568d5b80052e457a3058c2067512e2c5adfd92b5c9389644fa9f4830551b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Feb 2020 22:49:45 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.4/traefik_v2.1.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Feb 2020 22:49:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Feb 2020 22:49:46 GMT
EXPOSE 80
# Thu, 06 Feb 2020 22:49:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Feb 2020 22:49:47 GMT
CMD ["traefik"]
# Thu, 06 Feb 2020 22:49:48 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a045f3facd048d78ccec1317c0b8d3aa5e1b76f175b643f80c704ec2aa89f8`  
		Last Modified: Thu, 06 Feb 2020 22:51:40 GMT  
		Size: 698.0 KB (698013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9745c2a4ff5d2bfcd64252391c39fa81b12e6b88cabbc57384a3dea3b2d4222`  
		Last Modified: Thu, 06 Feb 2020 22:51:51 GMT  
		Size: 18.3 MB (18304232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e4d0ccb0157397196b8cf9cb3914252dc11ff9e26cecef56daa5e722d20104`  
		Last Modified: Thu, 06 Feb 2020 22:51:38 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.1.4` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:a87d68c5513f8449083099aecc1015397c7cd9e4c9941907f41fa82bc6dfa9ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21411878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0512a89fe17b4ad94d0f6439d0ec527c45e0ac985fa4dd0fd571b5c3875301ea`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Feb 2020 22:44:30 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.4/traefik_v2.1.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Feb 2020 22:44:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Feb 2020 22:44:31 GMT
EXPOSE 80
# Thu, 06 Feb 2020 22:44:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Feb 2020 22:44:32 GMT
CMD ["traefik"]
# Thu, 06 Feb 2020 22:44:33 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5c788179332343fbcbc8b97673406752232ca36894176cc87ece20ee279754`  
		Last Modified: Thu, 06 Feb 2020 22:47:56 GMT  
		Size: 696.0 KB (696043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c407d1e0b29391431bfef58f5bc2a55eaecbfdb70a55b5f9c8ef92e83ebf3b13`  
		Last Modified: Thu, 06 Feb 2020 22:48:08 GMT  
		Size: 18.0 MB (17992393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609ef9e236c8bf18f9a1bfef77c2b60092d81692ff465610c8c5ce4eef7bffc8`  
		Last Modified: Thu, 06 Feb 2020 22:47:55 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.1.4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:0259147e1c2948488566cce22add60c4c9d015c0ab83c0cad5326369207ffdb2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1040; amd64

### `traefik:v2.1.4-windowsservercore-1809` - windows version 10.0.17763.1040; amd64

```console
$ docker pull traefik@sha256:0d8a4d21a3ead1268dda0b75994711ed4a9e1442b7c360fb4b0b72bcb737cbd0
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2254614482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89f4d9bbba7707130be947cacf6d7bf25d0c0fa309e0bc57a1c01d2c56a14580`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 17 Feb 2020 06:57:13 GMT
RUN Install update 1809-amd64
# Thu, 20 Feb 2020 01:13:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 20 Feb 2020 04:09:34 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.4/traefik_v2.1.4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 20 Feb 2020 04:09:38 GMT
EXPOSE 80
# Thu, 20 Feb 2020 04:09:40 GMT
ENTRYPOINT ["/traefik"]
# Thu, 20 Feb 2020 04:09:41 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5405b7580792436b60c664b5fa766ea57f5a60c1d9a8c522cf53e99e4813355`  
		Size: 695.8 MB (695818606 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2061e035d6ba931d9f00238104b970d3410f4ef0d9603b4f074c7052858e01e3`  
		Last Modified: Thu, 20 Feb 2020 03:03:21 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c60a73e575d57222e8843fb64304b2ad26e626f1a8e630b96eb634b4084ec2`  
		Last Modified: Thu, 20 Feb 2020 04:12:03 GMT  
		Size: 24.1 MB (24105807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b74827fa03828ff650d42ccbd438a71c76f21f75d808d9a4edc1d49c98f6ce`  
		Last Modified: Thu, 20 Feb 2020 04:11:38 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1325439ba377e72162df98641f409c9d49c72bb29a932bdf9fe3faae9898aa2`  
		Last Modified: Thu, 20 Feb 2020 04:11:38 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c08705395bfeaf239a907f9b9241976a6a7fd77a367b4d3d3523f86a735ca4a`  
		Last Modified: Thu, 20 Feb 2020 04:11:39 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:0259147e1c2948488566cce22add60c4c9d015c0ab83c0cad5326369207ffdb2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1040; amd64

### `traefik:v2.1-windowsservercore-1809` - windows version 10.0.17763.1040; amd64

```console
$ docker pull traefik@sha256:0d8a4d21a3ead1268dda0b75994711ed4a9e1442b7c360fb4b0b72bcb737cbd0
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2254614482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89f4d9bbba7707130be947cacf6d7bf25d0c0fa309e0bc57a1c01d2c56a14580`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 17 Feb 2020 06:57:13 GMT
RUN Install update 1809-amd64
# Thu, 20 Feb 2020 01:13:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 20 Feb 2020 04:09:34 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.4/traefik_v2.1.4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 20 Feb 2020 04:09:38 GMT
EXPOSE 80
# Thu, 20 Feb 2020 04:09:40 GMT
ENTRYPOINT ["/traefik"]
# Thu, 20 Feb 2020 04:09:41 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5405b7580792436b60c664b5fa766ea57f5a60c1d9a8c522cf53e99e4813355`  
		Size: 695.8 MB (695818606 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2061e035d6ba931d9f00238104b970d3410f4ef0d9603b4f074c7052858e01e3`  
		Last Modified: Thu, 20 Feb 2020 03:03:21 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c60a73e575d57222e8843fb64304b2ad26e626f1a8e630b96eb634b4084ec2`  
		Last Modified: Thu, 20 Feb 2020 04:12:03 GMT  
		Size: 24.1 MB (24105807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b74827fa03828ff650d42ccbd438a71c76f21f75d808d9a4edc1d49c98f6ce`  
		Last Modified: Thu, 20 Feb 2020 04:11:38 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1325439ba377e72162df98641f409c9d49c72bb29a932bdf9fe3faae9898aa2`  
		Last Modified: Thu, 20 Feb 2020 04:11:38 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c08705395bfeaf239a907f9b9241976a6a7fd77a367b4d3d3523f86a735ca4a`  
		Last Modified: Thu, 20 Feb 2020 04:11:39 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:0259147e1c2948488566cce22add60c4c9d015c0ab83c0cad5326369207ffdb2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1040; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.1040; amd64

```console
$ docker pull traefik@sha256:0d8a4d21a3ead1268dda0b75994711ed4a9e1442b7c360fb4b0b72bcb737cbd0
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2254614482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89f4d9bbba7707130be947cacf6d7bf25d0c0fa309e0bc57a1c01d2c56a14580`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 17 Feb 2020 06:57:13 GMT
RUN Install update 1809-amd64
# Thu, 20 Feb 2020 01:13:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 20 Feb 2020 04:09:34 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.4/traefik_v2.1.4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 20 Feb 2020 04:09:38 GMT
EXPOSE 80
# Thu, 20 Feb 2020 04:09:40 GMT
ENTRYPOINT ["/traefik"]
# Thu, 20 Feb 2020 04:09:41 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5405b7580792436b60c664b5fa766ea57f5a60c1d9a8c522cf53e99e4813355`  
		Size: 695.8 MB (695818606 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2061e035d6ba931d9f00238104b970d3410f4ef0d9603b4f074c7052858e01e3`  
		Last Modified: Thu, 20 Feb 2020 03:03:21 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c60a73e575d57222e8843fb64304b2ad26e626f1a8e630b96eb634b4084ec2`  
		Last Modified: Thu, 20 Feb 2020 04:12:03 GMT  
		Size: 24.1 MB (24105807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b74827fa03828ff650d42ccbd438a71c76f21f75d808d9a4edc1d49c98f6ce`  
		Last Modified: Thu, 20 Feb 2020 04:11:38 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1325439ba377e72162df98641f409c9d49c72bb29a932bdf9fe3faae9898aa2`  
		Last Modified: Thu, 20 Feb 2020 04:11:38 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c08705395bfeaf239a907f9b9241976a6a7fd77a367b4d3d3523f86a735ca4a`  
		Last Modified: Thu, 20 Feb 2020 04:11:39 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
