<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:1.7`](#traefik17)
-	[`traefik:1.7-alpine`](#traefik17-alpine)
-	[`traefik:1.7-windowsservercore-1809`](#traefik17-windowsservercore-1809)
-	[`traefik:1.7.34`](#traefik1734)
-	[`traefik:1.7.34-alpine`](#traefik1734-alpine)
-	[`traefik:1.7.34-windowsservercore-1809`](#traefik1734-windowsservercore-1809)
-	[`traefik:2.7`](#traefik27)
-	[`traefik:2.7-windowsservercore-1809`](#traefik27-windowsservercore-1809)
-	[`traefik:2.7.1`](#traefik271)
-	[`traefik:2.7.1-windowsservercore-1809`](#traefik271-windowsservercore-1809)
-	[`traefik:2.8`](#traefik28)
-	[`traefik:2.8-windowsservercore-1809`](#traefik28-windowsservercore-1809)
-	[`traefik:2.8.0-rc1`](#traefik280-rc1)
-	[`traefik:2.8.0-rc1-windowsservercore-1809`](#traefik280-rc1-windowsservercore-1809)
-	[`traefik:epoisses`](#traefikepoisses)
-	[`traefik:epoisses-windowsservercore-1809`](#traefikepoisses-windowsservercore-1809)
-	[`traefik:latest`](#traefiklatest)
-	[`traefik:maroilles`](#traefikmaroilles)
-	[`traefik:maroilles-alpine`](#traefikmaroilles-alpine)
-	[`traefik:maroilles-windowsservercore-1809`](#traefikmaroilles-windowsservercore-1809)
-	[`traefik:v1.7`](#traefikv17)
-	[`traefik:v1.7-alpine`](#traefikv17-alpine)
-	[`traefik:v1.7-windowsservercore-1809`](#traefikv17-windowsservercore-1809)
-	[`traefik:v1.7.34`](#traefikv1734)
-	[`traefik:v1.7.34-alpine`](#traefikv1734-alpine)
-	[`traefik:v1.7.34-windowsservercore-1809`](#traefikv1734-windowsservercore-1809)
-	[`traefik:v2.7`](#traefikv27)
-	[`traefik:v2.7-windowsservercore-1809`](#traefikv27-windowsservercore-1809)
-	[`traefik:v2.7.1`](#traefikv271)
-	[`traefik:v2.7.1-windowsservercore-1809`](#traefikv271-windowsservercore-1809)
-	[`traefik:v2.8`](#traefikv28)
-	[`traefik:v2.8-windowsservercore-1809`](#traefikv28-windowsservercore-1809)
-	[`traefik:v2.8.0-rc1`](#traefikv280-rc1)
-	[`traefik:v2.8.0-rc1-windowsservercore-1809`](#traefikv280-rc1-windowsservercore-1809)
-	[`traefik:vacherin`](#traefikvacherin)
-	[`traefik:vacherin-windowsservercore-1809`](#traefikvacherin-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:1.7`

```console
$ docker pull traefik@sha256:1d8a41ae1bd54c9e9a5e0cc8da9002638932c53cc3d50c6f0c172238374ebe8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7` - linux; amd64

```console
$ docker pull traefik@sha256:f705216279431ed8ab470318736acd767794a847acda2db325e3e159574bd03c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22607863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43de28b34d397393ca2d0ec8bd6923735fab787f8c3bd3dab0719cd256fcc010`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 18 Mar 2022 06:23:36 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Fri, 18 Mar 2022 06:23:37 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Fri, 18 Mar 2022 06:23:38 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Fri, 18 Mar 2022 06:23:39 GMT
EXPOSE 80
# Fri, 18 Mar 2022 06:23:39 GMT
VOLUME [/tmp]
# Fri, 18 Mar 2022 06:23:39 GMT
ENTRYPOINT ["/traefik"]
# Fri, 18 Mar 2022 06:23:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:903e84870d1b7b581b2c6c362c74751a258cb8e2dbb443bddcd36fe8f29a20ab`  
		Last Modified: Fri, 18 Mar 2022 06:24:59 GMT  
		Size: 117.4 KB (117389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914ae7a2b8652023026596365a1dfe88e317d16b1cc8099ee03c20357c95716e`  
		Last Modified: Fri, 18 Mar 2022 06:25:00 GMT  
		Size: 328.5 KB (328522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f483c7bcad16f6ac0813c7a4704d4dc9319bfd6533f10c888b5e2ca21c72dc44`  
		Last Modified: Fri, 18 Mar 2022 06:25:05 GMT  
		Size: 22.2 MB (22161952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:fe6bde6e9349ec036bc3aaec90c095006425bface50ee2f449e0d196cb5850c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21069186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a5c3451377ef5e2379e4bc19691fb6c14b1a2215326833336e1db9e16cc5ca3`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Mar 2022 22:45:25 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Thu, 17 Mar 2022 22:45:27 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Thu, 17 Mar 2022 22:45:32 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Thu, 17 Mar 2022 22:45:33 GMT
EXPOSE 80
# Thu, 17 Mar 2022 22:45:33 GMT
VOLUME [/tmp]
# Thu, 17 Mar 2022 22:45:34 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Mar 2022 22:45:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:27b61c1d4effca5c7137bfe0c8b6a3a228418ef37998781ad6cc7372c6f7e98f`  
		Last Modified: Thu, 17 Mar 2022 22:48:17 GMT  
		Size: 117.4 KB (117390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98aae3b48a316f885b1d485fee6b2ffffb3c2c7dea49cea01019d4c103b204da`  
		Last Modified: Thu, 17 Mar 2022 22:48:18 GMT  
		Size: 328.5 KB (328514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82873a2be1cc2b2dfbc565c4bf9960f32b61892f49f0911ec1ac7e310210c3d`  
		Last Modified: Thu, 17 Mar 2022 22:48:34 GMT  
		Size: 20.6 MB (20623282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:c2930d3e36f7feb98470b85e8bc9fce0016fc5eadbc805249e63d6a458eb2323
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20577242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7338e148255e82dd93286a1f87db35f499d4e391d7f5f3e1bfb6c71ed4ec2d4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Mar 2022 21:07:07 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Thu, 17 Mar 2022 21:07:08 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Thu, 17 Mar 2022 21:07:09 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Thu, 17 Mar 2022 21:07:09 GMT
EXPOSE 80
# Thu, 17 Mar 2022 21:07:10 GMT
VOLUME [/tmp]
# Thu, 17 Mar 2022 21:07:11 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Mar 2022 21:07:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:86cd07830d2730c0aa24f0e47380af5ef760945b5049a2e72a8ebe0675ed6d34`  
		Last Modified: Thu, 17 Mar 2022 21:08:41 GMT  
		Size: 117.4 KB (117390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135b9e65a5ea0b642df02ea2cf73c74a353d1cbfa3b95d048a4adbf0bacf9653`  
		Last Modified: Thu, 17 Mar 2022 21:08:41 GMT  
		Size: 328.5 KB (328505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee8fa09b05c38fc9116b1446ac3d204200577fd9bfb1801d684657dc722b74b`  
		Last Modified: Thu, 17 Mar 2022 21:08:45 GMT  
		Size: 20.1 MB (20131347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-alpine`

```console
$ docker pull traefik@sha256:eb08a301bd06b8e71a7dfb44c829e593e6aaa24b0ea6a90cfb09488587911fe3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:437693178563fbe5e9d51a163f9c5507cfcaf5a52569b7e5814f6ccd71e53ee4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25647491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e98bf8d6e3fea93acd477a953dd3276b9ac3a285a9b7cdf1613f806e73a61f7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:53:36 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 10:53:56 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 10:53:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 10:53:56 GMT
EXPOSE 80
# Tue, 05 Apr 2022 10:53:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 10:53:56 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 10:53:56 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6b5dadc224e5464ecd6b4217323f15e90e06847ef61af9132dc606b1a9863a`  
		Last Modified: Tue, 05 Apr 2022 10:54:28 GMT  
		Size: 666.7 KB (666681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae84b4a436968a2d3e0c2d1d3f62ad7c56a1e0a20f0c6e00a8f76f646de636d4`  
		Last Modified: Tue, 05 Apr 2022 10:55:14 GMT  
		Size: 22.2 MB (22162072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7beb865e347fb64ada1ea356e11aa7f4e81221b6b589b618abf86188a9d3719a`  
		Last Modified: Tue, 05 Apr 2022 10:55:10 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:6907e0a9c3e242920fb2102a261b41864c3d8bf697efa46b6a09596b59c5300e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23922383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5db7d675647f8f59a02cd5915f6fd2afab456fbb1716db05032b9111a469f9b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:55 GMT
ADD file:2e4db0cea3f5eecfbb82c5abd09eb100749fed0189fc30d2c51980d2560e3ccb in / 
# Mon, 04 Apr 2022 23:49:56 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 14:40:53 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 14:41:48 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 14:41:49 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 14:41:49 GMT
EXPOSE 80
# Tue, 05 Apr 2022 14:41:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 14:41:50 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 14:41:50 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f9f2e4e531ad51ee917e8311e91a223a4893c1d754acb8246af87375ea60c6aa`  
		Last Modified: Mon, 04 Apr 2022 23:51:47 GMT  
		Size: 2.6 MB (2626056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a1618fdbb5f9b720d159d71fa3326e20a38c9bba9feb9392f897ab456d07f4`  
		Last Modified: Tue, 05 Apr 2022 14:43:49 GMT  
		Size: 672.5 KB (672528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2aba3d211189b35b7f9d6160aa51d316bde615e058a83996627fcb7dfdca0d0`  
		Last Modified: Tue, 05 Apr 2022 14:45:28 GMT  
		Size: 20.6 MB (20623431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ff4f0661732ea1e9661f9d94015bc7b5fcf85d6674fb173e88c50a23840d40`  
		Last Modified: Tue, 05 Apr 2022 14:45:13 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7bca8f9f0aebebc3c7c5e968e03474b479420b55a77f33683c435fead3366e18
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23517412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd43ec235cafac033220e63f50aaf33544f0f719f1a51e4d8be83109763738d7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:27:04 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 07:27:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 07:27:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 07:27:39 GMT
EXPOSE 80
# Tue, 05 Apr 2022 07:27:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 07:27:41 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 07:27:42 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a873ae44592179453bfc8ffe686a6faef6bae9b61f4465e8844d31d37b4a74`  
		Last Modified: Tue, 05 Apr 2022 07:28:36 GMT  
		Size: 668.3 KB (668291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1f2f70dadc3bc4f06bfc6c0eff12d88e357f1a8c8ee2876e16278cb07571b3`  
		Last Modified: Tue, 05 Apr 2022 07:29:28 GMT  
		Size: 20.1 MB (20131364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c24699415b41c9daba64f440481479635163834c11c1cb770c1e56ed677d840`  
		Last Modified: Tue, 05 Apr 2022 07:29:24 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:a07bc9e1c23a8aea5a3aba48bbc075c3da3c5808aec1b177ff02686e407a7e86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `traefik:1.7-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull traefik@sha256:409130d91fbc0358647a6c76902bdbb381917458dbba5e1b708d2cf349165982
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2527038215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ba63f98fa60e151dbfa2aeeb320019986a8644a21dbe1aaa3271db5d30b1a59`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 18:44:13 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 11 May 2022 18:44:14 GMT
EXPOSE 80
# Wed, 11 May 2022 18:44:15 GMT
ENTRYPOINT ["/traefik"]
# Wed, 11 May 2022 18:44:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4855f4a147e4a46d47f2c6fd99b86646844ad214cf11ba9cd365f0f17f0826`  
		Last Modified: Wed, 11 May 2022 18:46:23 GMT  
		Size: 23.0 MB (22976712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a1c70612f452f4df618632922a10afa962409fa89a5730cccb22cabb054ae5`  
		Last Modified: Wed, 11 May 2022 18:46:17 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857221245c4f0e2826adbe4632333050cb275e3798b22c512e6a05227cfaecdd`  
		Last Modified: Wed, 11 May 2022 18:46:17 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903aa8403bd64b1d753c81fcd69f266fa3e4298268cce3e3b1255ccbee1ee9dc`  
		Last Modified: Wed, 11 May 2022 18:46:17 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.34`

```console
$ docker pull traefik@sha256:1d8a41ae1bd54c9e9a5e0cc8da9002638932c53cc3d50c6f0c172238374ebe8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.34` - linux; amd64

```console
$ docker pull traefik@sha256:f705216279431ed8ab470318736acd767794a847acda2db325e3e159574bd03c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22607863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43de28b34d397393ca2d0ec8bd6923735fab787f8c3bd3dab0719cd256fcc010`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 18 Mar 2022 06:23:36 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Fri, 18 Mar 2022 06:23:37 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Fri, 18 Mar 2022 06:23:38 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Fri, 18 Mar 2022 06:23:39 GMT
EXPOSE 80
# Fri, 18 Mar 2022 06:23:39 GMT
VOLUME [/tmp]
# Fri, 18 Mar 2022 06:23:39 GMT
ENTRYPOINT ["/traefik"]
# Fri, 18 Mar 2022 06:23:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:903e84870d1b7b581b2c6c362c74751a258cb8e2dbb443bddcd36fe8f29a20ab`  
		Last Modified: Fri, 18 Mar 2022 06:24:59 GMT  
		Size: 117.4 KB (117389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914ae7a2b8652023026596365a1dfe88e317d16b1cc8099ee03c20357c95716e`  
		Last Modified: Fri, 18 Mar 2022 06:25:00 GMT  
		Size: 328.5 KB (328522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f483c7bcad16f6ac0813c7a4704d4dc9319bfd6533f10c888b5e2ca21c72dc44`  
		Last Modified: Fri, 18 Mar 2022 06:25:05 GMT  
		Size: 22.2 MB (22161952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.34` - linux; arm variant v6

```console
$ docker pull traefik@sha256:fe6bde6e9349ec036bc3aaec90c095006425bface50ee2f449e0d196cb5850c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21069186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a5c3451377ef5e2379e4bc19691fb6c14b1a2215326833336e1db9e16cc5ca3`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Mar 2022 22:45:25 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Thu, 17 Mar 2022 22:45:27 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Thu, 17 Mar 2022 22:45:32 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Thu, 17 Mar 2022 22:45:33 GMT
EXPOSE 80
# Thu, 17 Mar 2022 22:45:33 GMT
VOLUME [/tmp]
# Thu, 17 Mar 2022 22:45:34 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Mar 2022 22:45:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:27b61c1d4effca5c7137bfe0c8b6a3a228418ef37998781ad6cc7372c6f7e98f`  
		Last Modified: Thu, 17 Mar 2022 22:48:17 GMT  
		Size: 117.4 KB (117390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98aae3b48a316f885b1d485fee6b2ffffb3c2c7dea49cea01019d4c103b204da`  
		Last Modified: Thu, 17 Mar 2022 22:48:18 GMT  
		Size: 328.5 KB (328514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82873a2be1cc2b2dfbc565c4bf9960f32b61892f49f0911ec1ac7e310210c3d`  
		Last Modified: Thu, 17 Mar 2022 22:48:34 GMT  
		Size: 20.6 MB (20623282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.34` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:c2930d3e36f7feb98470b85e8bc9fce0016fc5eadbc805249e63d6a458eb2323
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20577242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7338e148255e82dd93286a1f87db35f499d4e391d7f5f3e1bfb6c71ed4ec2d4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Mar 2022 21:07:07 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Thu, 17 Mar 2022 21:07:08 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Thu, 17 Mar 2022 21:07:09 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Thu, 17 Mar 2022 21:07:09 GMT
EXPOSE 80
# Thu, 17 Mar 2022 21:07:10 GMT
VOLUME [/tmp]
# Thu, 17 Mar 2022 21:07:11 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Mar 2022 21:07:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:86cd07830d2730c0aa24f0e47380af5ef760945b5049a2e72a8ebe0675ed6d34`  
		Last Modified: Thu, 17 Mar 2022 21:08:41 GMT  
		Size: 117.4 KB (117390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135b9e65a5ea0b642df02ea2cf73c74a353d1cbfa3b95d048a4adbf0bacf9653`  
		Last Modified: Thu, 17 Mar 2022 21:08:41 GMT  
		Size: 328.5 KB (328505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee8fa09b05c38fc9116b1446ac3d204200577fd9bfb1801d684657dc722b74b`  
		Last Modified: Thu, 17 Mar 2022 21:08:45 GMT  
		Size: 20.1 MB (20131347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.34-alpine`

```console
$ docker pull traefik@sha256:eb08a301bd06b8e71a7dfb44c829e593e6aaa24b0ea6a90cfb09488587911fe3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.34-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:437693178563fbe5e9d51a163f9c5507cfcaf5a52569b7e5814f6ccd71e53ee4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25647491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e98bf8d6e3fea93acd477a953dd3276b9ac3a285a9b7cdf1613f806e73a61f7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:53:36 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 10:53:56 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 10:53:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 10:53:56 GMT
EXPOSE 80
# Tue, 05 Apr 2022 10:53:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 10:53:56 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 10:53:56 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6b5dadc224e5464ecd6b4217323f15e90e06847ef61af9132dc606b1a9863a`  
		Last Modified: Tue, 05 Apr 2022 10:54:28 GMT  
		Size: 666.7 KB (666681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae84b4a436968a2d3e0c2d1d3f62ad7c56a1e0a20f0c6e00a8f76f646de636d4`  
		Last Modified: Tue, 05 Apr 2022 10:55:14 GMT  
		Size: 22.2 MB (22162072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7beb865e347fb64ada1ea356e11aa7f4e81221b6b589b618abf86188a9d3719a`  
		Last Modified: Tue, 05 Apr 2022 10:55:10 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.34-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:6907e0a9c3e242920fb2102a261b41864c3d8bf697efa46b6a09596b59c5300e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23922383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5db7d675647f8f59a02cd5915f6fd2afab456fbb1716db05032b9111a469f9b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:55 GMT
ADD file:2e4db0cea3f5eecfbb82c5abd09eb100749fed0189fc30d2c51980d2560e3ccb in / 
# Mon, 04 Apr 2022 23:49:56 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 14:40:53 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 14:41:48 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 14:41:49 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 14:41:49 GMT
EXPOSE 80
# Tue, 05 Apr 2022 14:41:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 14:41:50 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 14:41:50 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f9f2e4e531ad51ee917e8311e91a223a4893c1d754acb8246af87375ea60c6aa`  
		Last Modified: Mon, 04 Apr 2022 23:51:47 GMT  
		Size: 2.6 MB (2626056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a1618fdbb5f9b720d159d71fa3326e20a38c9bba9feb9392f897ab456d07f4`  
		Last Modified: Tue, 05 Apr 2022 14:43:49 GMT  
		Size: 672.5 KB (672528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2aba3d211189b35b7f9d6160aa51d316bde615e058a83996627fcb7dfdca0d0`  
		Last Modified: Tue, 05 Apr 2022 14:45:28 GMT  
		Size: 20.6 MB (20623431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ff4f0661732ea1e9661f9d94015bc7b5fcf85d6674fb173e88c50a23840d40`  
		Last Modified: Tue, 05 Apr 2022 14:45:13 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.34-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7bca8f9f0aebebc3c7c5e968e03474b479420b55a77f33683c435fead3366e18
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23517412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd43ec235cafac033220e63f50aaf33544f0f719f1a51e4d8be83109763738d7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:27:04 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 07:27:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 07:27:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 07:27:39 GMT
EXPOSE 80
# Tue, 05 Apr 2022 07:27:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 07:27:41 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 07:27:42 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a873ae44592179453bfc8ffe686a6faef6bae9b61f4465e8844d31d37b4a74`  
		Last Modified: Tue, 05 Apr 2022 07:28:36 GMT  
		Size: 668.3 KB (668291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1f2f70dadc3bc4f06bfc6c0eff12d88e357f1a8c8ee2876e16278cb07571b3`  
		Last Modified: Tue, 05 Apr 2022 07:29:28 GMT  
		Size: 20.1 MB (20131364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c24699415b41c9daba64f440481479635163834c11c1cb770c1e56ed677d840`  
		Last Modified: Tue, 05 Apr 2022 07:29:24 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.34-windowsservercore-1809`

```console
$ docker pull traefik@sha256:a07bc9e1c23a8aea5a3aba48bbc075c3da3c5808aec1b177ff02686e407a7e86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `traefik:1.7.34-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull traefik@sha256:409130d91fbc0358647a6c76902bdbb381917458dbba5e1b708d2cf349165982
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2527038215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ba63f98fa60e151dbfa2aeeb320019986a8644a21dbe1aaa3271db5d30b1a59`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 18:44:13 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 11 May 2022 18:44:14 GMT
EXPOSE 80
# Wed, 11 May 2022 18:44:15 GMT
ENTRYPOINT ["/traefik"]
# Wed, 11 May 2022 18:44:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4855f4a147e4a46d47f2c6fd99b86646844ad214cf11ba9cd365f0f17f0826`  
		Last Modified: Wed, 11 May 2022 18:46:23 GMT  
		Size: 23.0 MB (22976712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a1c70612f452f4df618632922a10afa962409fa89a5730cccb22cabb054ae5`  
		Last Modified: Wed, 11 May 2022 18:46:17 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857221245c4f0e2826adbe4632333050cb275e3798b22c512e6a05227cfaecdd`  
		Last Modified: Wed, 11 May 2022 18:46:17 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903aa8403bd64b1d753c81fcd69f266fa3e4298268cce3e3b1255ccbee1ee9dc`  
		Last Modified: Wed, 11 May 2022 18:46:17 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.7`

```console
$ docker pull traefik@sha256:fdff55caa91ac7ff217ff03b93f3673844b3b88ad993e023ab43f6004021697c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.7` - linux; amd64

```console
$ docker pull traefik@sha256:6354bfe99cf39164514ecca33ef4189361f0bf4eca8c16ffc1bae3623b99e8c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31023311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8345b2e8bee0c824835af0881cfdc602bbb351637c205cbebc76e7b74f813597`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:09:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:34:49 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:34:50 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:34:50 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:34:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:34:50 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:34:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07cb125bb766321ae78c2a558eb61358ea0c322871a963cc343f07b19a5dfe9f`  
		Last Modified: Tue, 24 May 2022 20:09:52 GMT  
		Size: 667.0 KB (667045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7643a4c688aef051e331797b6a1c3cf5a493b95e95e9a90502f34bb69543cf`  
		Last Modified: Mon, 13 Jun 2022 18:35:44 GMT  
		Size: 27.5 MB (27541339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5730b5ba9047bdf67c081e949f31b562532504f42b183afab9b38e82692c6a03`  
		Last Modified: Mon, 13 Jun 2022 18:35:39 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:b8e54b077cf2ffb132203d201519c7dae5dd885ea8cf6eb4b24f3bdd37eb0a6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29110783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc0175d61827f26689cebc311c086e4998894cb2370fa203eb6b0fc54626b7b9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:16:34 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:01:07 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:01:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:01:08 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:01:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:01:09 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:01:10 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ca500a6585c4382a3d0562172788318c2044142456377fdbf2c4b279334e26`  
		Last Modified: Tue, 24 May 2022 20:19:13 GMT  
		Size: 672.6 KB (672642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c97f5f8fa2680bd0e85b1838bc88a1b3bad8ea5a158b18383f007e4c6b398e52`  
		Last Modified: Mon, 13 Jun 2022 18:04:09 GMT  
		Size: 25.8 MB (25815800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a11e8a929d0ad2e555c58f324df02cde6c468d2662ecf5414979893c990664`  
		Last Modified: Mon, 13 Jun 2022 18:03:52 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:f65b5a3b0de3d895385f85c41a180573a59d7dc4890d24e1b21c3fedd699ddf2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28492564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d1d1d829b444cff7a651cd13bdc6b2a66de794c8f21f75c5b7f204da37fdcb4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 21:18:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:19:33 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:19:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:19:35 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:19:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:19:37 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:19:38 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdde6df9c5c8f6328c1ce3fe2ca88cea0a7799584b83cafec0322b4d7235d0b7`  
		Last Modified: Tue, 24 May 2022 21:20:14 GMT  
		Size: 668.4 KB (668397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed46ebeb3f061a6426a51c9ce5d729ffe5bc2f3d8353303c30c35bff93ed4232`  
		Last Modified: Mon, 13 Jun 2022 18:21:04 GMT  
		Size: 25.1 MB (25107322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8683e30306089877837d12d61eaf9cc16d7ad0b3313d5b38dbff4cbc1685b057`  
		Last Modified: Mon, 13 Jun 2022 18:21:00 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.7` - linux; s390x

```console
$ docker pull traefik@sha256:9d7c6aa60ebe18d8257b0a02296eb18ac01e047675e48f4c20272c849c98669d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29788377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11de775752a6ad32f36bb166122916f9c84d52645b1d8c4274acb265af05d91`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:28:44 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:15:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:15:21 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:15:22 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:15:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:15:22 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:15:22 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f52582da22b0abbdbb4590735229191759cc22a1119ccdf5af9cd472103ffd`  
		Last Modified: Tue, 24 May 2022 20:29:51 GMT  
		Size: 672.6 KB (672603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0a8dab5f416aa3abd40293a95475c0df50231b6c94cf0b9c4fdbe5d2088c03`  
		Last Modified: Mon, 13 Jun 2022 18:16:12 GMT  
		Size: 26.5 MB (26515031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1cc2efd66f301007736aaf33dcba85abe0fd187a08d11ce716f925b49440b20`  
		Last Modified: Mon, 13 Jun 2022 18:16:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b813d64a5c1eb3498986d5a316fa433df682acfa3038a9467f72232655fe3d59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `traefik:2.7-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull traefik@sha256:7d454bf6f16177192750790acdbde2230a4d390a06b36683e92e5fc276a7f7b2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2532336814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aef3d6aed360b6013f3eac849ed76ff75eeaca4fd73dfec990b913776e8a164e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 13 Jun 2022 18:17:16 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 13 Jun 2022 18:17:17 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:17:18 GMT
ENTRYPOINT ["/traefik"]
# Mon, 13 Jun 2022 18:17:19 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc81fc68b4bd26ace09cac1f9e156a7f10c4a01fb84c1bd61156bf85efeac85`  
		Last Modified: Mon, 13 Jun 2022 18:18:58 GMT  
		Size: 28.3 MB (28275302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2b74c1667e6fd86372a21e937c532e1aa5a02c0c5590cdf2990e82bb1e6caa`  
		Last Modified: Mon, 13 Jun 2022 18:18:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5ec0fd7a47d0f100d28be14844121e6ef46f7d279f9365d6f4c5ae34833395`  
		Last Modified: Mon, 13 Jun 2022 18:18:27 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613e0863856475e19f15fbdf6bcf5516e0962a80fa16605d3ae57f8c2d4e2334`  
		Last Modified: Mon, 13 Jun 2022 18:18:27 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.7.1`

```console
$ docker pull traefik@sha256:fdff55caa91ac7ff217ff03b93f3673844b3b88ad993e023ab43f6004021697c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.7.1` - linux; amd64

```console
$ docker pull traefik@sha256:6354bfe99cf39164514ecca33ef4189361f0bf4eca8c16ffc1bae3623b99e8c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31023311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8345b2e8bee0c824835af0881cfdc602bbb351637c205cbebc76e7b74f813597`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:09:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:34:49 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:34:50 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:34:50 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:34:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:34:50 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:34:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07cb125bb766321ae78c2a558eb61358ea0c322871a963cc343f07b19a5dfe9f`  
		Last Modified: Tue, 24 May 2022 20:09:52 GMT  
		Size: 667.0 KB (667045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7643a4c688aef051e331797b6a1c3cf5a493b95e95e9a90502f34bb69543cf`  
		Last Modified: Mon, 13 Jun 2022 18:35:44 GMT  
		Size: 27.5 MB (27541339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5730b5ba9047bdf67c081e949f31b562532504f42b183afab9b38e82692c6a03`  
		Last Modified: Mon, 13 Jun 2022 18:35:39 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.7.1` - linux; arm variant v6

```console
$ docker pull traefik@sha256:b8e54b077cf2ffb132203d201519c7dae5dd885ea8cf6eb4b24f3bdd37eb0a6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29110783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc0175d61827f26689cebc311c086e4998894cb2370fa203eb6b0fc54626b7b9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:16:34 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:01:07 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:01:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:01:08 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:01:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:01:09 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:01:10 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ca500a6585c4382a3d0562172788318c2044142456377fdbf2c4b279334e26`  
		Last Modified: Tue, 24 May 2022 20:19:13 GMT  
		Size: 672.6 KB (672642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c97f5f8fa2680bd0e85b1838bc88a1b3bad8ea5a158b18383f007e4c6b398e52`  
		Last Modified: Mon, 13 Jun 2022 18:04:09 GMT  
		Size: 25.8 MB (25815800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a11e8a929d0ad2e555c58f324df02cde6c468d2662ecf5414979893c990664`  
		Last Modified: Mon, 13 Jun 2022 18:03:52 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.7.1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:f65b5a3b0de3d895385f85c41a180573a59d7dc4890d24e1b21c3fedd699ddf2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28492564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d1d1d829b444cff7a651cd13bdc6b2a66de794c8f21f75c5b7f204da37fdcb4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 21:18:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:19:33 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:19:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:19:35 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:19:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:19:37 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:19:38 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdde6df9c5c8f6328c1ce3fe2ca88cea0a7799584b83cafec0322b4d7235d0b7`  
		Last Modified: Tue, 24 May 2022 21:20:14 GMT  
		Size: 668.4 KB (668397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed46ebeb3f061a6426a51c9ce5d729ffe5bc2f3d8353303c30c35bff93ed4232`  
		Last Modified: Mon, 13 Jun 2022 18:21:04 GMT  
		Size: 25.1 MB (25107322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8683e30306089877837d12d61eaf9cc16d7ad0b3313d5b38dbff4cbc1685b057`  
		Last Modified: Mon, 13 Jun 2022 18:21:00 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.7.1` - linux; s390x

```console
$ docker pull traefik@sha256:9d7c6aa60ebe18d8257b0a02296eb18ac01e047675e48f4c20272c849c98669d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29788377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11de775752a6ad32f36bb166122916f9c84d52645b1d8c4274acb265af05d91`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:28:44 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:15:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:15:21 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:15:22 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:15:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:15:22 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:15:22 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f52582da22b0abbdbb4590735229191759cc22a1119ccdf5af9cd472103ffd`  
		Last Modified: Tue, 24 May 2022 20:29:51 GMT  
		Size: 672.6 KB (672603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0a8dab5f416aa3abd40293a95475c0df50231b6c94cf0b9c4fdbe5d2088c03`  
		Last Modified: Mon, 13 Jun 2022 18:16:12 GMT  
		Size: 26.5 MB (26515031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1cc2efd66f301007736aaf33dcba85abe0fd187a08d11ce716f925b49440b20`  
		Last Modified: Mon, 13 Jun 2022 18:16:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.7.1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b813d64a5c1eb3498986d5a316fa433df682acfa3038a9467f72232655fe3d59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `traefik:2.7.1-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull traefik@sha256:7d454bf6f16177192750790acdbde2230a4d390a06b36683e92e5fc276a7f7b2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2532336814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aef3d6aed360b6013f3eac849ed76ff75eeaca4fd73dfec990b913776e8a164e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 13 Jun 2022 18:17:16 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 13 Jun 2022 18:17:17 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:17:18 GMT
ENTRYPOINT ["/traefik"]
# Mon, 13 Jun 2022 18:17:19 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc81fc68b4bd26ace09cac1f9e156a7f10c4a01fb84c1bd61156bf85efeac85`  
		Last Modified: Mon, 13 Jun 2022 18:18:58 GMT  
		Size: 28.3 MB (28275302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2b74c1667e6fd86372a21e937c532e1aa5a02c0c5590cdf2990e82bb1e6caa`  
		Last Modified: Mon, 13 Jun 2022 18:18:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5ec0fd7a47d0f100d28be14844121e6ef46f7d279f9365d6f4c5ae34833395`  
		Last Modified: Mon, 13 Jun 2022 18:18:27 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613e0863856475e19f15fbdf6bcf5516e0962a80fa16605d3ae57f8c2d4e2334`  
		Last Modified: Mon, 13 Jun 2022 18:18:27 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.8`

```console
$ docker pull traefik@sha256:0856f146dfbc67612de10b8776b735b3e903e0fb62d15710982a53c53b67a3b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.8` - linux; amd64

```console
$ docker pull traefik@sha256:5e1798198129ebf84fec2b5e3aae4576abade055a3e1429147a7f66184501209
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31269784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dca842284774841bc00b1ee58d6c51086de47ff42311872db4f2750cc4195de`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:09:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:34:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.0-rc1/traefik_v2.8.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:34:43 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:34:43 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:34:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:34:43 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:34:43 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07cb125bb766321ae78c2a558eb61358ea0c322871a963cc343f07b19a5dfe9f`  
		Last Modified: Tue, 24 May 2022 20:09:52 GMT  
		Size: 667.0 KB (667045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d0aa7bd10b0837b5951891be0343aae1e2b18ef9fe46a7af0b1379288a5088`  
		Last Modified: Mon, 13 Jun 2022 18:35:23 GMT  
		Size: 27.8 MB (27787812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a603c8fd0afaba7471e72f9ff316ae88170561fd4e0b0f31ae7a42d771b379`  
		Last Modified: Mon, 13 Jun 2022 18:35:18 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.8` - linux; arm variant v6

```console
$ docker pull traefik@sha256:dbb784ff502f912465406439ee9df419405fe6dff2402b414240587d7945bbfc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.3 MB (29334407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7f41f140507e568077e956e176d79728114b4e5e81875f37ddabcf3c0bd9916`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:16:34 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:00:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.0-rc1/traefik_v2.8.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:00:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:00:44 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:00:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:00:45 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:00:46 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ca500a6585c4382a3d0562172788318c2044142456377fdbf2c4b279334e26`  
		Last Modified: Tue, 24 May 2022 20:19:13 GMT  
		Size: 672.6 KB (672642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9fd4dbb43f6693d731fc04a307864de55084a8aae49ba713c346b8b2609de3`  
		Last Modified: Mon, 13 Jun 2022 18:03:31 GMT  
		Size: 26.0 MB (26039425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4d398d59c3345b33011af9a19eea0681c6eed32ec39bb226fbf4e13728afb3`  
		Last Modified: Mon, 13 Jun 2022 18:03:14 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.8` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:0d6a87b45a3e97b4718d724fed6b60de6396b9379f7aafe8ba1f84311a12470c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28719767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a284f06f2207f2f09b33871cbc6854d984a4dc3ce5fbae9292fef6273d34347b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 21:18:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:19:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.0-rc1/traefik_v2.8.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:19:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:19:20 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:19:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:19:22 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:19:23 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdde6df9c5c8f6328c1ce3fe2ca88cea0a7799584b83cafec0322b4d7235d0b7`  
		Last Modified: Tue, 24 May 2022 21:20:14 GMT  
		Size: 668.4 KB (668397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32682e72e2fb3405355907ebe27456de8196b3869606c0282e33d87f6456800d`  
		Last Modified: Mon, 13 Jun 2022 18:20:40 GMT  
		Size: 25.3 MB (25334525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d930e8e440833d01453b05b786f093dd51000881521fc92a87f2375d888bc4d`  
		Last Modified: Mon, 13 Jun 2022 18:20:36 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.8` - linux; s390x

```console
$ docker pull traefik@sha256:d2e42180e7790c806f17c7b7d07d6738803dca07ea4e11bc161f43e79055dcd2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.0 MB (30026181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99c5ab9d7a4ad3bc5511585018c91cada5addf9b0599e1fb9109608ec5c74a5a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:28:44 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:15:07 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.0-rc1/traefik_v2.8.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:15:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:15:08 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:15:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:15:09 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:15:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f52582da22b0abbdbb4590735229191759cc22a1119ccdf5af9cd472103ffd`  
		Last Modified: Tue, 24 May 2022 20:29:51 GMT  
		Size: 672.6 KB (672603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba97cee16ef49e268621c22e0b2c3da5dc7914b67bb92367c1473169047af63`  
		Last Modified: Mon, 13 Jun 2022 18:15:57 GMT  
		Size: 26.8 MB (26752834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c61301d344682dd15f4d3092db668cdb3562084ca343ead49f47d118201425`  
		Last Modified: Mon, 13 Jun 2022 18:15:53 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.8-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e2cc222f17256cab7d03feacf5c2f7aa2a0034fcdaab0019545703be359e59e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `traefik:2.8-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull traefik@sha256:8963ee086a8a32c8458e64da5888d044e5b5dd7737918b8ae56dc51beb03cc75
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2532588939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8038611223da84ee443ca21bdc0a5febfe709064148bdcf22f66d836c19ef9a`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 13 Jun 2022 18:15:47 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.8.0-rc1/traefik_v2.8.0-rc1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 13 Jun 2022 18:15:48 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:15:49 GMT
ENTRYPOINT ["/traefik"]
# Mon, 13 Jun 2022 18:15:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16db0b20ba12318f4f238f69199c29e73928f90b9650bb3578d1a9b182a2d985`  
		Last Modified: Mon, 13 Jun 2022 18:18:11 GMT  
		Size: 28.5 MB (28527375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71918551829e1bfe9f5df15be61a91f9a4432268933fcd3cb7b261305b39e13b`  
		Last Modified: Mon, 13 Jun 2022 18:18:03 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534cd28bde041060e9269066e8ca5ebad28e153a233c215a335a9de34c393944`  
		Last Modified: Mon, 13 Jun 2022 18:18:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92059b5c9612669718297746abced06cbd9bc03ee2e89f97225102e27847a8d8`  
		Last Modified: Mon, 13 Jun 2022 18:18:03 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.8.0-rc1`

```console
$ docker pull traefik@sha256:0856f146dfbc67612de10b8776b735b3e903e0fb62d15710982a53c53b67a3b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.8.0-rc1` - linux; amd64

```console
$ docker pull traefik@sha256:5e1798198129ebf84fec2b5e3aae4576abade055a3e1429147a7f66184501209
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31269784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dca842284774841bc00b1ee58d6c51086de47ff42311872db4f2750cc4195de`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:09:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:34:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.0-rc1/traefik_v2.8.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:34:43 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:34:43 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:34:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:34:43 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:34:43 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07cb125bb766321ae78c2a558eb61358ea0c322871a963cc343f07b19a5dfe9f`  
		Last Modified: Tue, 24 May 2022 20:09:52 GMT  
		Size: 667.0 KB (667045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d0aa7bd10b0837b5951891be0343aae1e2b18ef9fe46a7af0b1379288a5088`  
		Last Modified: Mon, 13 Jun 2022 18:35:23 GMT  
		Size: 27.8 MB (27787812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a603c8fd0afaba7471e72f9ff316ae88170561fd4e0b0f31ae7a42d771b379`  
		Last Modified: Mon, 13 Jun 2022 18:35:18 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.8.0-rc1` - linux; arm variant v6

```console
$ docker pull traefik@sha256:dbb784ff502f912465406439ee9df419405fe6dff2402b414240587d7945bbfc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.3 MB (29334407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7f41f140507e568077e956e176d79728114b4e5e81875f37ddabcf3c0bd9916`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:16:34 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:00:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.0-rc1/traefik_v2.8.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:00:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:00:44 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:00:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:00:45 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:00:46 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ca500a6585c4382a3d0562172788318c2044142456377fdbf2c4b279334e26`  
		Last Modified: Tue, 24 May 2022 20:19:13 GMT  
		Size: 672.6 KB (672642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9fd4dbb43f6693d731fc04a307864de55084a8aae49ba713c346b8b2609de3`  
		Last Modified: Mon, 13 Jun 2022 18:03:31 GMT  
		Size: 26.0 MB (26039425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4d398d59c3345b33011af9a19eea0681c6eed32ec39bb226fbf4e13728afb3`  
		Last Modified: Mon, 13 Jun 2022 18:03:14 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.8.0-rc1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:0d6a87b45a3e97b4718d724fed6b60de6396b9379f7aafe8ba1f84311a12470c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28719767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a284f06f2207f2f09b33871cbc6854d984a4dc3ce5fbae9292fef6273d34347b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 21:18:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:19:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.0-rc1/traefik_v2.8.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:19:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:19:20 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:19:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:19:22 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:19:23 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdde6df9c5c8f6328c1ce3fe2ca88cea0a7799584b83cafec0322b4d7235d0b7`  
		Last Modified: Tue, 24 May 2022 21:20:14 GMT  
		Size: 668.4 KB (668397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32682e72e2fb3405355907ebe27456de8196b3869606c0282e33d87f6456800d`  
		Last Modified: Mon, 13 Jun 2022 18:20:40 GMT  
		Size: 25.3 MB (25334525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d930e8e440833d01453b05b786f093dd51000881521fc92a87f2375d888bc4d`  
		Last Modified: Mon, 13 Jun 2022 18:20:36 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.8.0-rc1` - linux; s390x

```console
$ docker pull traefik@sha256:d2e42180e7790c806f17c7b7d07d6738803dca07ea4e11bc161f43e79055dcd2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.0 MB (30026181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99c5ab9d7a4ad3bc5511585018c91cada5addf9b0599e1fb9109608ec5c74a5a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:28:44 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:15:07 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.0-rc1/traefik_v2.8.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:15:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:15:08 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:15:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:15:09 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:15:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f52582da22b0abbdbb4590735229191759cc22a1119ccdf5af9cd472103ffd`  
		Last Modified: Tue, 24 May 2022 20:29:51 GMT  
		Size: 672.6 KB (672603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba97cee16ef49e268621c22e0b2c3da5dc7914b67bb92367c1473169047af63`  
		Last Modified: Mon, 13 Jun 2022 18:15:57 GMT  
		Size: 26.8 MB (26752834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c61301d344682dd15f4d3092db668cdb3562084ca343ead49f47d118201425`  
		Last Modified: Mon, 13 Jun 2022 18:15:53 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.8.0-rc1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e2cc222f17256cab7d03feacf5c2f7aa2a0034fcdaab0019545703be359e59e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `traefik:2.8.0-rc1-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull traefik@sha256:8963ee086a8a32c8458e64da5888d044e5b5dd7737918b8ae56dc51beb03cc75
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2532588939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8038611223da84ee443ca21bdc0a5febfe709064148bdcf22f66d836c19ef9a`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 13 Jun 2022 18:15:47 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.8.0-rc1/traefik_v2.8.0-rc1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 13 Jun 2022 18:15:48 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:15:49 GMT
ENTRYPOINT ["/traefik"]
# Mon, 13 Jun 2022 18:15:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16db0b20ba12318f4f238f69199c29e73928f90b9650bb3578d1a9b182a2d985`  
		Last Modified: Mon, 13 Jun 2022 18:18:11 GMT  
		Size: 28.5 MB (28527375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71918551829e1bfe9f5df15be61a91f9a4432268933fcd3cb7b261305b39e13b`  
		Last Modified: Mon, 13 Jun 2022 18:18:03 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534cd28bde041060e9269066e8ca5ebad28e153a233c215a335a9de34c393944`  
		Last Modified: Mon, 13 Jun 2022 18:18:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92059b5c9612669718297746abced06cbd9bc03ee2e89f97225102e27847a8d8`  
		Last Modified: Mon, 13 Jun 2022 18:18:03 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:epoisses`

```console
$ docker pull traefik@sha256:fdff55caa91ac7ff217ff03b93f3673844b3b88ad993e023ab43f6004021697c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:epoisses` - linux; amd64

```console
$ docker pull traefik@sha256:6354bfe99cf39164514ecca33ef4189361f0bf4eca8c16ffc1bae3623b99e8c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31023311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8345b2e8bee0c824835af0881cfdc602bbb351637c205cbebc76e7b74f813597`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:09:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:34:49 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:34:50 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:34:50 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:34:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:34:50 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:34:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07cb125bb766321ae78c2a558eb61358ea0c322871a963cc343f07b19a5dfe9f`  
		Last Modified: Tue, 24 May 2022 20:09:52 GMT  
		Size: 667.0 KB (667045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7643a4c688aef051e331797b6a1c3cf5a493b95e95e9a90502f34bb69543cf`  
		Last Modified: Mon, 13 Jun 2022 18:35:44 GMT  
		Size: 27.5 MB (27541339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5730b5ba9047bdf67c081e949f31b562532504f42b183afab9b38e82692c6a03`  
		Last Modified: Mon, 13 Jun 2022 18:35:39 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:epoisses` - linux; arm variant v6

```console
$ docker pull traefik@sha256:b8e54b077cf2ffb132203d201519c7dae5dd885ea8cf6eb4b24f3bdd37eb0a6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29110783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc0175d61827f26689cebc311c086e4998894cb2370fa203eb6b0fc54626b7b9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:16:34 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:01:07 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:01:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:01:08 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:01:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:01:09 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:01:10 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ca500a6585c4382a3d0562172788318c2044142456377fdbf2c4b279334e26`  
		Last Modified: Tue, 24 May 2022 20:19:13 GMT  
		Size: 672.6 KB (672642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c97f5f8fa2680bd0e85b1838bc88a1b3bad8ea5a158b18383f007e4c6b398e52`  
		Last Modified: Mon, 13 Jun 2022 18:04:09 GMT  
		Size: 25.8 MB (25815800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a11e8a929d0ad2e555c58f324df02cde6c468d2662ecf5414979893c990664`  
		Last Modified: Mon, 13 Jun 2022 18:03:52 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:epoisses` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:f65b5a3b0de3d895385f85c41a180573a59d7dc4890d24e1b21c3fedd699ddf2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28492564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d1d1d829b444cff7a651cd13bdc6b2a66de794c8f21f75c5b7f204da37fdcb4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 21:18:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:19:33 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:19:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:19:35 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:19:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:19:37 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:19:38 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdde6df9c5c8f6328c1ce3fe2ca88cea0a7799584b83cafec0322b4d7235d0b7`  
		Last Modified: Tue, 24 May 2022 21:20:14 GMT  
		Size: 668.4 KB (668397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed46ebeb3f061a6426a51c9ce5d729ffe5bc2f3d8353303c30c35bff93ed4232`  
		Last Modified: Mon, 13 Jun 2022 18:21:04 GMT  
		Size: 25.1 MB (25107322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8683e30306089877837d12d61eaf9cc16d7ad0b3313d5b38dbff4cbc1685b057`  
		Last Modified: Mon, 13 Jun 2022 18:21:00 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:epoisses` - linux; s390x

```console
$ docker pull traefik@sha256:9d7c6aa60ebe18d8257b0a02296eb18ac01e047675e48f4c20272c849c98669d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29788377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11de775752a6ad32f36bb166122916f9c84d52645b1d8c4274acb265af05d91`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:28:44 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:15:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:15:21 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:15:22 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:15:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:15:22 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:15:22 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f52582da22b0abbdbb4590735229191759cc22a1119ccdf5af9cd472103ffd`  
		Last Modified: Tue, 24 May 2022 20:29:51 GMT  
		Size: 672.6 KB (672603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0a8dab5f416aa3abd40293a95475c0df50231b6c94cf0b9c4fdbe5d2088c03`  
		Last Modified: Mon, 13 Jun 2022 18:16:12 GMT  
		Size: 26.5 MB (26515031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1cc2efd66f301007736aaf33dcba85abe0fd187a08d11ce716f925b49440b20`  
		Last Modified: Mon, 13 Jun 2022 18:16:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:epoisses-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b813d64a5c1eb3498986d5a316fa433df682acfa3038a9467f72232655fe3d59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `traefik:epoisses-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull traefik@sha256:7d454bf6f16177192750790acdbde2230a4d390a06b36683e92e5fc276a7f7b2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2532336814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aef3d6aed360b6013f3eac849ed76ff75eeaca4fd73dfec990b913776e8a164e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 13 Jun 2022 18:17:16 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 13 Jun 2022 18:17:17 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:17:18 GMT
ENTRYPOINT ["/traefik"]
# Mon, 13 Jun 2022 18:17:19 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc81fc68b4bd26ace09cac1f9e156a7f10c4a01fb84c1bd61156bf85efeac85`  
		Last Modified: Mon, 13 Jun 2022 18:18:58 GMT  
		Size: 28.3 MB (28275302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2b74c1667e6fd86372a21e937c532e1aa5a02c0c5590cdf2990e82bb1e6caa`  
		Last Modified: Mon, 13 Jun 2022 18:18:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5ec0fd7a47d0f100d28be14844121e6ef46f7d279f9365d6f4c5ae34833395`  
		Last Modified: Mon, 13 Jun 2022 18:18:27 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613e0863856475e19f15fbdf6bcf5516e0962a80fa16605d3ae57f8c2d4e2334`  
		Last Modified: Mon, 13 Jun 2022 18:18:27 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:fdff55caa91ac7ff217ff03b93f3673844b3b88ad993e023ab43f6004021697c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:6354bfe99cf39164514ecca33ef4189361f0bf4eca8c16ffc1bae3623b99e8c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31023311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8345b2e8bee0c824835af0881cfdc602bbb351637c205cbebc76e7b74f813597`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:09:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:34:49 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:34:50 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:34:50 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:34:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:34:50 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:34:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07cb125bb766321ae78c2a558eb61358ea0c322871a963cc343f07b19a5dfe9f`  
		Last Modified: Tue, 24 May 2022 20:09:52 GMT  
		Size: 667.0 KB (667045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7643a4c688aef051e331797b6a1c3cf5a493b95e95e9a90502f34bb69543cf`  
		Last Modified: Mon, 13 Jun 2022 18:35:44 GMT  
		Size: 27.5 MB (27541339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5730b5ba9047bdf67c081e949f31b562532504f42b183afab9b38e82692c6a03`  
		Last Modified: Mon, 13 Jun 2022 18:35:39 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:b8e54b077cf2ffb132203d201519c7dae5dd885ea8cf6eb4b24f3bdd37eb0a6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29110783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc0175d61827f26689cebc311c086e4998894cb2370fa203eb6b0fc54626b7b9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:16:34 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:01:07 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:01:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:01:08 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:01:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:01:09 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:01:10 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ca500a6585c4382a3d0562172788318c2044142456377fdbf2c4b279334e26`  
		Last Modified: Tue, 24 May 2022 20:19:13 GMT  
		Size: 672.6 KB (672642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c97f5f8fa2680bd0e85b1838bc88a1b3bad8ea5a158b18383f007e4c6b398e52`  
		Last Modified: Mon, 13 Jun 2022 18:04:09 GMT  
		Size: 25.8 MB (25815800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a11e8a929d0ad2e555c58f324df02cde6c468d2662ecf5414979893c990664`  
		Last Modified: Mon, 13 Jun 2022 18:03:52 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:f65b5a3b0de3d895385f85c41a180573a59d7dc4890d24e1b21c3fedd699ddf2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28492564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d1d1d829b444cff7a651cd13bdc6b2a66de794c8f21f75c5b7f204da37fdcb4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 21:18:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:19:33 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:19:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:19:35 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:19:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:19:37 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:19:38 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdde6df9c5c8f6328c1ce3fe2ca88cea0a7799584b83cafec0322b4d7235d0b7`  
		Last Modified: Tue, 24 May 2022 21:20:14 GMT  
		Size: 668.4 KB (668397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed46ebeb3f061a6426a51c9ce5d729ffe5bc2f3d8353303c30c35bff93ed4232`  
		Last Modified: Mon, 13 Jun 2022 18:21:04 GMT  
		Size: 25.1 MB (25107322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8683e30306089877837d12d61eaf9cc16d7ad0b3313d5b38dbff4cbc1685b057`  
		Last Modified: Mon, 13 Jun 2022 18:21:00 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; s390x

```console
$ docker pull traefik@sha256:9d7c6aa60ebe18d8257b0a02296eb18ac01e047675e48f4c20272c849c98669d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29788377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11de775752a6ad32f36bb166122916f9c84d52645b1d8c4274acb265af05d91`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:28:44 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:15:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:15:21 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:15:22 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:15:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:15:22 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:15:22 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f52582da22b0abbdbb4590735229191759cc22a1119ccdf5af9cd472103ffd`  
		Last Modified: Tue, 24 May 2022 20:29:51 GMT  
		Size: 672.6 KB (672603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0a8dab5f416aa3abd40293a95475c0df50231b6c94cf0b9c4fdbe5d2088c03`  
		Last Modified: Mon, 13 Jun 2022 18:16:12 GMT  
		Size: 26.5 MB (26515031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1cc2efd66f301007736aaf33dcba85abe0fd187a08d11ce716f925b49440b20`  
		Last Modified: Mon, 13 Jun 2022 18:16:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles`

```console
$ docker pull traefik@sha256:1d8a41ae1bd54c9e9a5e0cc8da9002638932c53cc3d50c6f0c172238374ebe8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles` - linux; amd64

```console
$ docker pull traefik@sha256:f705216279431ed8ab470318736acd767794a847acda2db325e3e159574bd03c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22607863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43de28b34d397393ca2d0ec8bd6923735fab787f8c3bd3dab0719cd256fcc010`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 18 Mar 2022 06:23:36 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Fri, 18 Mar 2022 06:23:37 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Fri, 18 Mar 2022 06:23:38 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Fri, 18 Mar 2022 06:23:39 GMT
EXPOSE 80
# Fri, 18 Mar 2022 06:23:39 GMT
VOLUME [/tmp]
# Fri, 18 Mar 2022 06:23:39 GMT
ENTRYPOINT ["/traefik"]
# Fri, 18 Mar 2022 06:23:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:903e84870d1b7b581b2c6c362c74751a258cb8e2dbb443bddcd36fe8f29a20ab`  
		Last Modified: Fri, 18 Mar 2022 06:24:59 GMT  
		Size: 117.4 KB (117389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914ae7a2b8652023026596365a1dfe88e317d16b1cc8099ee03c20357c95716e`  
		Last Modified: Fri, 18 Mar 2022 06:25:00 GMT  
		Size: 328.5 KB (328522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f483c7bcad16f6ac0813c7a4704d4dc9319bfd6533f10c888b5e2ca21c72dc44`  
		Last Modified: Fri, 18 Mar 2022 06:25:05 GMT  
		Size: 22.2 MB (22161952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm variant v6

```console
$ docker pull traefik@sha256:fe6bde6e9349ec036bc3aaec90c095006425bface50ee2f449e0d196cb5850c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21069186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a5c3451377ef5e2379e4bc19691fb6c14b1a2215326833336e1db9e16cc5ca3`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Mar 2022 22:45:25 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Thu, 17 Mar 2022 22:45:27 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Thu, 17 Mar 2022 22:45:32 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Thu, 17 Mar 2022 22:45:33 GMT
EXPOSE 80
# Thu, 17 Mar 2022 22:45:33 GMT
VOLUME [/tmp]
# Thu, 17 Mar 2022 22:45:34 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Mar 2022 22:45:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:27b61c1d4effca5c7137bfe0c8b6a3a228418ef37998781ad6cc7372c6f7e98f`  
		Last Modified: Thu, 17 Mar 2022 22:48:17 GMT  
		Size: 117.4 KB (117390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98aae3b48a316f885b1d485fee6b2ffffb3c2c7dea49cea01019d4c103b204da`  
		Last Modified: Thu, 17 Mar 2022 22:48:18 GMT  
		Size: 328.5 KB (328514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82873a2be1cc2b2dfbc565c4bf9960f32b61892f49f0911ec1ac7e310210c3d`  
		Last Modified: Thu, 17 Mar 2022 22:48:34 GMT  
		Size: 20.6 MB (20623282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:c2930d3e36f7feb98470b85e8bc9fce0016fc5eadbc805249e63d6a458eb2323
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20577242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7338e148255e82dd93286a1f87db35f499d4e391d7f5f3e1bfb6c71ed4ec2d4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Mar 2022 21:07:07 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Thu, 17 Mar 2022 21:07:08 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Thu, 17 Mar 2022 21:07:09 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Thu, 17 Mar 2022 21:07:09 GMT
EXPOSE 80
# Thu, 17 Mar 2022 21:07:10 GMT
VOLUME [/tmp]
# Thu, 17 Mar 2022 21:07:11 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Mar 2022 21:07:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:86cd07830d2730c0aa24f0e47380af5ef760945b5049a2e72a8ebe0675ed6d34`  
		Last Modified: Thu, 17 Mar 2022 21:08:41 GMT  
		Size: 117.4 KB (117390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135b9e65a5ea0b642df02ea2cf73c74a353d1cbfa3b95d048a4adbf0bacf9653`  
		Last Modified: Thu, 17 Mar 2022 21:08:41 GMT  
		Size: 328.5 KB (328505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee8fa09b05c38fc9116b1446ac3d204200577fd9bfb1801d684657dc722b74b`  
		Last Modified: Thu, 17 Mar 2022 21:08:45 GMT  
		Size: 20.1 MB (20131347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-alpine`

```console
$ docker pull traefik@sha256:eb08a301bd06b8e71a7dfb44c829e593e6aaa24b0ea6a90cfb09488587911fe3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:437693178563fbe5e9d51a163f9c5507cfcaf5a52569b7e5814f6ccd71e53ee4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25647491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e98bf8d6e3fea93acd477a953dd3276b9ac3a285a9b7cdf1613f806e73a61f7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:53:36 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 10:53:56 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 10:53:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 10:53:56 GMT
EXPOSE 80
# Tue, 05 Apr 2022 10:53:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 10:53:56 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 10:53:56 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6b5dadc224e5464ecd6b4217323f15e90e06847ef61af9132dc606b1a9863a`  
		Last Modified: Tue, 05 Apr 2022 10:54:28 GMT  
		Size: 666.7 KB (666681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae84b4a436968a2d3e0c2d1d3f62ad7c56a1e0a20f0c6e00a8f76f646de636d4`  
		Last Modified: Tue, 05 Apr 2022 10:55:14 GMT  
		Size: 22.2 MB (22162072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7beb865e347fb64ada1ea356e11aa7f4e81221b6b589b618abf86188a9d3719a`  
		Last Modified: Tue, 05 Apr 2022 10:55:10 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:6907e0a9c3e242920fb2102a261b41864c3d8bf697efa46b6a09596b59c5300e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23922383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5db7d675647f8f59a02cd5915f6fd2afab456fbb1716db05032b9111a469f9b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:55 GMT
ADD file:2e4db0cea3f5eecfbb82c5abd09eb100749fed0189fc30d2c51980d2560e3ccb in / 
# Mon, 04 Apr 2022 23:49:56 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 14:40:53 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 14:41:48 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 14:41:49 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 14:41:49 GMT
EXPOSE 80
# Tue, 05 Apr 2022 14:41:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 14:41:50 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 14:41:50 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f9f2e4e531ad51ee917e8311e91a223a4893c1d754acb8246af87375ea60c6aa`  
		Last Modified: Mon, 04 Apr 2022 23:51:47 GMT  
		Size: 2.6 MB (2626056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a1618fdbb5f9b720d159d71fa3326e20a38c9bba9feb9392f897ab456d07f4`  
		Last Modified: Tue, 05 Apr 2022 14:43:49 GMT  
		Size: 672.5 KB (672528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2aba3d211189b35b7f9d6160aa51d316bde615e058a83996627fcb7dfdca0d0`  
		Last Modified: Tue, 05 Apr 2022 14:45:28 GMT  
		Size: 20.6 MB (20623431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ff4f0661732ea1e9661f9d94015bc7b5fcf85d6674fb173e88c50a23840d40`  
		Last Modified: Tue, 05 Apr 2022 14:45:13 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7bca8f9f0aebebc3c7c5e968e03474b479420b55a77f33683c435fead3366e18
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23517412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd43ec235cafac033220e63f50aaf33544f0f719f1a51e4d8be83109763738d7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:27:04 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 07:27:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 07:27:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 07:27:39 GMT
EXPOSE 80
# Tue, 05 Apr 2022 07:27:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 07:27:41 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 07:27:42 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a873ae44592179453bfc8ffe686a6faef6bae9b61f4465e8844d31d37b4a74`  
		Last Modified: Tue, 05 Apr 2022 07:28:36 GMT  
		Size: 668.3 KB (668291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1f2f70dadc3bc4f06bfc6c0eff12d88e357f1a8c8ee2876e16278cb07571b3`  
		Last Modified: Tue, 05 Apr 2022 07:29:28 GMT  
		Size: 20.1 MB (20131364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c24699415b41c9daba64f440481479635163834c11c1cb770c1e56ed677d840`  
		Last Modified: Tue, 05 Apr 2022 07:29:24 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-windowsservercore-1809`

```console
$ docker pull traefik@sha256:a07bc9e1c23a8aea5a3aba48bbc075c3da3c5808aec1b177ff02686e407a7e86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull traefik@sha256:409130d91fbc0358647a6c76902bdbb381917458dbba5e1b708d2cf349165982
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2527038215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ba63f98fa60e151dbfa2aeeb320019986a8644a21dbe1aaa3271db5d30b1a59`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 18:44:13 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 11 May 2022 18:44:14 GMT
EXPOSE 80
# Wed, 11 May 2022 18:44:15 GMT
ENTRYPOINT ["/traefik"]
# Wed, 11 May 2022 18:44:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4855f4a147e4a46d47f2c6fd99b86646844ad214cf11ba9cd365f0f17f0826`  
		Last Modified: Wed, 11 May 2022 18:46:23 GMT  
		Size: 23.0 MB (22976712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a1c70612f452f4df618632922a10afa962409fa89a5730cccb22cabb054ae5`  
		Last Modified: Wed, 11 May 2022 18:46:17 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857221245c4f0e2826adbe4632333050cb275e3798b22c512e6a05227cfaecdd`  
		Last Modified: Wed, 11 May 2022 18:46:17 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903aa8403bd64b1d753c81fcd69f266fa3e4298268cce3e3b1255ccbee1ee9dc`  
		Last Modified: Wed, 11 May 2022 18:46:17 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7`

```console
$ docker pull traefik@sha256:1d8a41ae1bd54c9e9a5e0cc8da9002638932c53cc3d50c6f0c172238374ebe8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7` - linux; amd64

```console
$ docker pull traefik@sha256:f705216279431ed8ab470318736acd767794a847acda2db325e3e159574bd03c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22607863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43de28b34d397393ca2d0ec8bd6923735fab787f8c3bd3dab0719cd256fcc010`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 18 Mar 2022 06:23:36 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Fri, 18 Mar 2022 06:23:37 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Fri, 18 Mar 2022 06:23:38 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Fri, 18 Mar 2022 06:23:39 GMT
EXPOSE 80
# Fri, 18 Mar 2022 06:23:39 GMT
VOLUME [/tmp]
# Fri, 18 Mar 2022 06:23:39 GMT
ENTRYPOINT ["/traefik"]
# Fri, 18 Mar 2022 06:23:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:903e84870d1b7b581b2c6c362c74751a258cb8e2dbb443bddcd36fe8f29a20ab`  
		Last Modified: Fri, 18 Mar 2022 06:24:59 GMT  
		Size: 117.4 KB (117389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914ae7a2b8652023026596365a1dfe88e317d16b1cc8099ee03c20357c95716e`  
		Last Modified: Fri, 18 Mar 2022 06:25:00 GMT  
		Size: 328.5 KB (328522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f483c7bcad16f6ac0813c7a4704d4dc9319bfd6533f10c888b5e2ca21c72dc44`  
		Last Modified: Fri, 18 Mar 2022 06:25:05 GMT  
		Size: 22.2 MB (22161952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:fe6bde6e9349ec036bc3aaec90c095006425bface50ee2f449e0d196cb5850c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21069186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a5c3451377ef5e2379e4bc19691fb6c14b1a2215326833336e1db9e16cc5ca3`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Mar 2022 22:45:25 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Thu, 17 Mar 2022 22:45:27 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Thu, 17 Mar 2022 22:45:32 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Thu, 17 Mar 2022 22:45:33 GMT
EXPOSE 80
# Thu, 17 Mar 2022 22:45:33 GMT
VOLUME [/tmp]
# Thu, 17 Mar 2022 22:45:34 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Mar 2022 22:45:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:27b61c1d4effca5c7137bfe0c8b6a3a228418ef37998781ad6cc7372c6f7e98f`  
		Last Modified: Thu, 17 Mar 2022 22:48:17 GMT  
		Size: 117.4 KB (117390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98aae3b48a316f885b1d485fee6b2ffffb3c2c7dea49cea01019d4c103b204da`  
		Last Modified: Thu, 17 Mar 2022 22:48:18 GMT  
		Size: 328.5 KB (328514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82873a2be1cc2b2dfbc565c4bf9960f32b61892f49f0911ec1ac7e310210c3d`  
		Last Modified: Thu, 17 Mar 2022 22:48:34 GMT  
		Size: 20.6 MB (20623282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:c2930d3e36f7feb98470b85e8bc9fce0016fc5eadbc805249e63d6a458eb2323
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20577242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7338e148255e82dd93286a1f87db35f499d4e391d7f5f3e1bfb6c71ed4ec2d4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Mar 2022 21:07:07 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Thu, 17 Mar 2022 21:07:08 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Thu, 17 Mar 2022 21:07:09 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Thu, 17 Mar 2022 21:07:09 GMT
EXPOSE 80
# Thu, 17 Mar 2022 21:07:10 GMT
VOLUME [/tmp]
# Thu, 17 Mar 2022 21:07:11 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Mar 2022 21:07:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:86cd07830d2730c0aa24f0e47380af5ef760945b5049a2e72a8ebe0675ed6d34`  
		Last Modified: Thu, 17 Mar 2022 21:08:41 GMT  
		Size: 117.4 KB (117390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135b9e65a5ea0b642df02ea2cf73c74a353d1cbfa3b95d048a4adbf0bacf9653`  
		Last Modified: Thu, 17 Mar 2022 21:08:41 GMT  
		Size: 328.5 KB (328505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee8fa09b05c38fc9116b1446ac3d204200577fd9bfb1801d684657dc722b74b`  
		Last Modified: Thu, 17 Mar 2022 21:08:45 GMT  
		Size: 20.1 MB (20131347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-alpine`

```console
$ docker pull traefik@sha256:eb08a301bd06b8e71a7dfb44c829e593e6aaa24b0ea6a90cfb09488587911fe3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:437693178563fbe5e9d51a163f9c5507cfcaf5a52569b7e5814f6ccd71e53ee4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25647491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e98bf8d6e3fea93acd477a953dd3276b9ac3a285a9b7cdf1613f806e73a61f7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:53:36 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 10:53:56 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 10:53:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 10:53:56 GMT
EXPOSE 80
# Tue, 05 Apr 2022 10:53:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 10:53:56 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 10:53:56 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6b5dadc224e5464ecd6b4217323f15e90e06847ef61af9132dc606b1a9863a`  
		Last Modified: Tue, 05 Apr 2022 10:54:28 GMT  
		Size: 666.7 KB (666681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae84b4a436968a2d3e0c2d1d3f62ad7c56a1e0a20f0c6e00a8f76f646de636d4`  
		Last Modified: Tue, 05 Apr 2022 10:55:14 GMT  
		Size: 22.2 MB (22162072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7beb865e347fb64ada1ea356e11aa7f4e81221b6b589b618abf86188a9d3719a`  
		Last Modified: Tue, 05 Apr 2022 10:55:10 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:6907e0a9c3e242920fb2102a261b41864c3d8bf697efa46b6a09596b59c5300e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23922383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5db7d675647f8f59a02cd5915f6fd2afab456fbb1716db05032b9111a469f9b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:55 GMT
ADD file:2e4db0cea3f5eecfbb82c5abd09eb100749fed0189fc30d2c51980d2560e3ccb in / 
# Mon, 04 Apr 2022 23:49:56 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 14:40:53 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 14:41:48 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 14:41:49 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 14:41:49 GMT
EXPOSE 80
# Tue, 05 Apr 2022 14:41:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 14:41:50 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 14:41:50 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f9f2e4e531ad51ee917e8311e91a223a4893c1d754acb8246af87375ea60c6aa`  
		Last Modified: Mon, 04 Apr 2022 23:51:47 GMT  
		Size: 2.6 MB (2626056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a1618fdbb5f9b720d159d71fa3326e20a38c9bba9feb9392f897ab456d07f4`  
		Last Modified: Tue, 05 Apr 2022 14:43:49 GMT  
		Size: 672.5 KB (672528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2aba3d211189b35b7f9d6160aa51d316bde615e058a83996627fcb7dfdca0d0`  
		Last Modified: Tue, 05 Apr 2022 14:45:28 GMT  
		Size: 20.6 MB (20623431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ff4f0661732ea1e9661f9d94015bc7b5fcf85d6674fb173e88c50a23840d40`  
		Last Modified: Tue, 05 Apr 2022 14:45:13 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7bca8f9f0aebebc3c7c5e968e03474b479420b55a77f33683c435fead3366e18
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23517412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd43ec235cafac033220e63f50aaf33544f0f719f1a51e4d8be83109763738d7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:27:04 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 07:27:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 07:27:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 07:27:39 GMT
EXPOSE 80
# Tue, 05 Apr 2022 07:27:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 07:27:41 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 07:27:42 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a873ae44592179453bfc8ffe686a6faef6bae9b61f4465e8844d31d37b4a74`  
		Last Modified: Tue, 05 Apr 2022 07:28:36 GMT  
		Size: 668.3 KB (668291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1f2f70dadc3bc4f06bfc6c0eff12d88e357f1a8c8ee2876e16278cb07571b3`  
		Last Modified: Tue, 05 Apr 2022 07:29:28 GMT  
		Size: 20.1 MB (20131364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c24699415b41c9daba64f440481479635163834c11c1cb770c1e56ed677d840`  
		Last Modified: Tue, 05 Apr 2022 07:29:24 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:a07bc9e1c23a8aea5a3aba48bbc075c3da3c5808aec1b177ff02686e407a7e86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `traefik:v1.7-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull traefik@sha256:409130d91fbc0358647a6c76902bdbb381917458dbba5e1b708d2cf349165982
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2527038215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ba63f98fa60e151dbfa2aeeb320019986a8644a21dbe1aaa3271db5d30b1a59`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 18:44:13 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 11 May 2022 18:44:14 GMT
EXPOSE 80
# Wed, 11 May 2022 18:44:15 GMT
ENTRYPOINT ["/traefik"]
# Wed, 11 May 2022 18:44:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4855f4a147e4a46d47f2c6fd99b86646844ad214cf11ba9cd365f0f17f0826`  
		Last Modified: Wed, 11 May 2022 18:46:23 GMT  
		Size: 23.0 MB (22976712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a1c70612f452f4df618632922a10afa962409fa89a5730cccb22cabb054ae5`  
		Last Modified: Wed, 11 May 2022 18:46:17 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857221245c4f0e2826adbe4632333050cb275e3798b22c512e6a05227cfaecdd`  
		Last Modified: Wed, 11 May 2022 18:46:17 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903aa8403bd64b1d753c81fcd69f266fa3e4298268cce3e3b1255ccbee1ee9dc`  
		Last Modified: Wed, 11 May 2022 18:46:17 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.34`

```console
$ docker pull traefik@sha256:1d8a41ae1bd54c9e9a5e0cc8da9002638932c53cc3d50c6f0c172238374ebe8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.34` - linux; amd64

```console
$ docker pull traefik@sha256:f705216279431ed8ab470318736acd767794a847acda2db325e3e159574bd03c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22607863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43de28b34d397393ca2d0ec8bd6923735fab787f8c3bd3dab0719cd256fcc010`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 18 Mar 2022 06:23:36 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Fri, 18 Mar 2022 06:23:37 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Fri, 18 Mar 2022 06:23:38 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Fri, 18 Mar 2022 06:23:39 GMT
EXPOSE 80
# Fri, 18 Mar 2022 06:23:39 GMT
VOLUME [/tmp]
# Fri, 18 Mar 2022 06:23:39 GMT
ENTRYPOINT ["/traefik"]
# Fri, 18 Mar 2022 06:23:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:903e84870d1b7b581b2c6c362c74751a258cb8e2dbb443bddcd36fe8f29a20ab`  
		Last Modified: Fri, 18 Mar 2022 06:24:59 GMT  
		Size: 117.4 KB (117389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914ae7a2b8652023026596365a1dfe88e317d16b1cc8099ee03c20357c95716e`  
		Last Modified: Fri, 18 Mar 2022 06:25:00 GMT  
		Size: 328.5 KB (328522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f483c7bcad16f6ac0813c7a4704d4dc9319bfd6533f10c888b5e2ca21c72dc44`  
		Last Modified: Fri, 18 Mar 2022 06:25:05 GMT  
		Size: 22.2 MB (22161952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.34` - linux; arm variant v6

```console
$ docker pull traefik@sha256:fe6bde6e9349ec036bc3aaec90c095006425bface50ee2f449e0d196cb5850c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21069186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a5c3451377ef5e2379e4bc19691fb6c14b1a2215326833336e1db9e16cc5ca3`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Mar 2022 22:45:25 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Thu, 17 Mar 2022 22:45:27 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Thu, 17 Mar 2022 22:45:32 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Thu, 17 Mar 2022 22:45:33 GMT
EXPOSE 80
# Thu, 17 Mar 2022 22:45:33 GMT
VOLUME [/tmp]
# Thu, 17 Mar 2022 22:45:34 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Mar 2022 22:45:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:27b61c1d4effca5c7137bfe0c8b6a3a228418ef37998781ad6cc7372c6f7e98f`  
		Last Modified: Thu, 17 Mar 2022 22:48:17 GMT  
		Size: 117.4 KB (117390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98aae3b48a316f885b1d485fee6b2ffffb3c2c7dea49cea01019d4c103b204da`  
		Last Modified: Thu, 17 Mar 2022 22:48:18 GMT  
		Size: 328.5 KB (328514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82873a2be1cc2b2dfbc565c4bf9960f32b61892f49f0911ec1ac7e310210c3d`  
		Last Modified: Thu, 17 Mar 2022 22:48:34 GMT  
		Size: 20.6 MB (20623282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.34` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:c2930d3e36f7feb98470b85e8bc9fce0016fc5eadbc805249e63d6a458eb2323
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20577242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7338e148255e82dd93286a1f87db35f499d4e391d7f5f3e1bfb6c71ed4ec2d4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Mar 2022 21:07:07 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Thu, 17 Mar 2022 21:07:08 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Thu, 17 Mar 2022 21:07:09 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Thu, 17 Mar 2022 21:07:09 GMT
EXPOSE 80
# Thu, 17 Mar 2022 21:07:10 GMT
VOLUME [/tmp]
# Thu, 17 Mar 2022 21:07:11 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Mar 2022 21:07:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:86cd07830d2730c0aa24f0e47380af5ef760945b5049a2e72a8ebe0675ed6d34`  
		Last Modified: Thu, 17 Mar 2022 21:08:41 GMT  
		Size: 117.4 KB (117390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135b9e65a5ea0b642df02ea2cf73c74a353d1cbfa3b95d048a4adbf0bacf9653`  
		Last Modified: Thu, 17 Mar 2022 21:08:41 GMT  
		Size: 328.5 KB (328505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee8fa09b05c38fc9116b1446ac3d204200577fd9bfb1801d684657dc722b74b`  
		Last Modified: Thu, 17 Mar 2022 21:08:45 GMT  
		Size: 20.1 MB (20131347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.34-alpine`

```console
$ docker pull traefik@sha256:eb08a301bd06b8e71a7dfb44c829e593e6aaa24b0ea6a90cfb09488587911fe3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.34-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:437693178563fbe5e9d51a163f9c5507cfcaf5a52569b7e5814f6ccd71e53ee4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25647491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e98bf8d6e3fea93acd477a953dd3276b9ac3a285a9b7cdf1613f806e73a61f7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:53:36 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 10:53:56 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 10:53:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 10:53:56 GMT
EXPOSE 80
# Tue, 05 Apr 2022 10:53:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 10:53:56 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 10:53:56 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6b5dadc224e5464ecd6b4217323f15e90e06847ef61af9132dc606b1a9863a`  
		Last Modified: Tue, 05 Apr 2022 10:54:28 GMT  
		Size: 666.7 KB (666681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae84b4a436968a2d3e0c2d1d3f62ad7c56a1e0a20f0c6e00a8f76f646de636d4`  
		Last Modified: Tue, 05 Apr 2022 10:55:14 GMT  
		Size: 22.2 MB (22162072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7beb865e347fb64ada1ea356e11aa7f4e81221b6b589b618abf86188a9d3719a`  
		Last Modified: Tue, 05 Apr 2022 10:55:10 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.34-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:6907e0a9c3e242920fb2102a261b41864c3d8bf697efa46b6a09596b59c5300e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23922383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5db7d675647f8f59a02cd5915f6fd2afab456fbb1716db05032b9111a469f9b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:55 GMT
ADD file:2e4db0cea3f5eecfbb82c5abd09eb100749fed0189fc30d2c51980d2560e3ccb in / 
# Mon, 04 Apr 2022 23:49:56 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 14:40:53 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 14:41:48 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 14:41:49 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 14:41:49 GMT
EXPOSE 80
# Tue, 05 Apr 2022 14:41:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 14:41:50 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 14:41:50 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f9f2e4e531ad51ee917e8311e91a223a4893c1d754acb8246af87375ea60c6aa`  
		Last Modified: Mon, 04 Apr 2022 23:51:47 GMT  
		Size: 2.6 MB (2626056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a1618fdbb5f9b720d159d71fa3326e20a38c9bba9feb9392f897ab456d07f4`  
		Last Modified: Tue, 05 Apr 2022 14:43:49 GMT  
		Size: 672.5 KB (672528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2aba3d211189b35b7f9d6160aa51d316bde615e058a83996627fcb7dfdca0d0`  
		Last Modified: Tue, 05 Apr 2022 14:45:28 GMT  
		Size: 20.6 MB (20623431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ff4f0661732ea1e9661f9d94015bc7b5fcf85d6674fb173e88c50a23840d40`  
		Last Modified: Tue, 05 Apr 2022 14:45:13 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.34-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7bca8f9f0aebebc3c7c5e968e03474b479420b55a77f33683c435fead3366e18
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23517412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd43ec235cafac033220e63f50aaf33544f0f719f1a51e4d8be83109763738d7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:27:04 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 07:27:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 07:27:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 07:27:39 GMT
EXPOSE 80
# Tue, 05 Apr 2022 07:27:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 07:27:41 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 07:27:42 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a873ae44592179453bfc8ffe686a6faef6bae9b61f4465e8844d31d37b4a74`  
		Last Modified: Tue, 05 Apr 2022 07:28:36 GMT  
		Size: 668.3 KB (668291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1f2f70dadc3bc4f06bfc6c0eff12d88e357f1a8c8ee2876e16278cb07571b3`  
		Last Modified: Tue, 05 Apr 2022 07:29:28 GMT  
		Size: 20.1 MB (20131364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c24699415b41c9daba64f440481479635163834c11c1cb770c1e56ed677d840`  
		Last Modified: Tue, 05 Apr 2022 07:29:24 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.34-windowsservercore-1809`

```console
$ docker pull traefik@sha256:a07bc9e1c23a8aea5a3aba48bbc075c3da3c5808aec1b177ff02686e407a7e86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `traefik:v1.7.34-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull traefik@sha256:409130d91fbc0358647a6c76902bdbb381917458dbba5e1b708d2cf349165982
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2527038215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ba63f98fa60e151dbfa2aeeb320019986a8644a21dbe1aaa3271db5d30b1a59`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 18:44:13 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 11 May 2022 18:44:14 GMT
EXPOSE 80
# Wed, 11 May 2022 18:44:15 GMT
ENTRYPOINT ["/traefik"]
# Wed, 11 May 2022 18:44:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4855f4a147e4a46d47f2c6fd99b86646844ad214cf11ba9cd365f0f17f0826`  
		Last Modified: Wed, 11 May 2022 18:46:23 GMT  
		Size: 23.0 MB (22976712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a1c70612f452f4df618632922a10afa962409fa89a5730cccb22cabb054ae5`  
		Last Modified: Wed, 11 May 2022 18:46:17 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857221245c4f0e2826adbe4632333050cb275e3798b22c512e6a05227cfaecdd`  
		Last Modified: Wed, 11 May 2022 18:46:17 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903aa8403bd64b1d753c81fcd69f266fa3e4298268cce3e3b1255ccbee1ee9dc`  
		Last Modified: Wed, 11 May 2022 18:46:17 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.7`

```console
$ docker pull traefik@sha256:fdff55caa91ac7ff217ff03b93f3673844b3b88ad993e023ab43f6004021697c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.7` - linux; amd64

```console
$ docker pull traefik@sha256:6354bfe99cf39164514ecca33ef4189361f0bf4eca8c16ffc1bae3623b99e8c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31023311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8345b2e8bee0c824835af0881cfdc602bbb351637c205cbebc76e7b74f813597`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:09:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:34:49 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:34:50 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:34:50 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:34:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:34:50 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:34:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07cb125bb766321ae78c2a558eb61358ea0c322871a963cc343f07b19a5dfe9f`  
		Last Modified: Tue, 24 May 2022 20:09:52 GMT  
		Size: 667.0 KB (667045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7643a4c688aef051e331797b6a1c3cf5a493b95e95e9a90502f34bb69543cf`  
		Last Modified: Mon, 13 Jun 2022 18:35:44 GMT  
		Size: 27.5 MB (27541339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5730b5ba9047bdf67c081e949f31b562532504f42b183afab9b38e82692c6a03`  
		Last Modified: Mon, 13 Jun 2022 18:35:39 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:b8e54b077cf2ffb132203d201519c7dae5dd885ea8cf6eb4b24f3bdd37eb0a6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29110783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc0175d61827f26689cebc311c086e4998894cb2370fa203eb6b0fc54626b7b9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:16:34 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:01:07 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:01:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:01:08 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:01:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:01:09 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:01:10 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ca500a6585c4382a3d0562172788318c2044142456377fdbf2c4b279334e26`  
		Last Modified: Tue, 24 May 2022 20:19:13 GMT  
		Size: 672.6 KB (672642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c97f5f8fa2680bd0e85b1838bc88a1b3bad8ea5a158b18383f007e4c6b398e52`  
		Last Modified: Mon, 13 Jun 2022 18:04:09 GMT  
		Size: 25.8 MB (25815800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a11e8a929d0ad2e555c58f324df02cde6c468d2662ecf5414979893c990664`  
		Last Modified: Mon, 13 Jun 2022 18:03:52 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:f65b5a3b0de3d895385f85c41a180573a59d7dc4890d24e1b21c3fedd699ddf2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28492564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d1d1d829b444cff7a651cd13bdc6b2a66de794c8f21f75c5b7f204da37fdcb4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 21:18:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:19:33 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:19:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:19:35 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:19:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:19:37 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:19:38 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdde6df9c5c8f6328c1ce3fe2ca88cea0a7799584b83cafec0322b4d7235d0b7`  
		Last Modified: Tue, 24 May 2022 21:20:14 GMT  
		Size: 668.4 KB (668397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed46ebeb3f061a6426a51c9ce5d729ffe5bc2f3d8353303c30c35bff93ed4232`  
		Last Modified: Mon, 13 Jun 2022 18:21:04 GMT  
		Size: 25.1 MB (25107322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8683e30306089877837d12d61eaf9cc16d7ad0b3313d5b38dbff4cbc1685b057`  
		Last Modified: Mon, 13 Jun 2022 18:21:00 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.7` - linux; s390x

```console
$ docker pull traefik@sha256:9d7c6aa60ebe18d8257b0a02296eb18ac01e047675e48f4c20272c849c98669d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29788377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11de775752a6ad32f36bb166122916f9c84d52645b1d8c4274acb265af05d91`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:28:44 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:15:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:15:21 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:15:22 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:15:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:15:22 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:15:22 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f52582da22b0abbdbb4590735229191759cc22a1119ccdf5af9cd472103ffd`  
		Last Modified: Tue, 24 May 2022 20:29:51 GMT  
		Size: 672.6 KB (672603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0a8dab5f416aa3abd40293a95475c0df50231b6c94cf0b9c4fdbe5d2088c03`  
		Last Modified: Mon, 13 Jun 2022 18:16:12 GMT  
		Size: 26.5 MB (26515031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1cc2efd66f301007736aaf33dcba85abe0fd187a08d11ce716f925b49440b20`  
		Last Modified: Mon, 13 Jun 2022 18:16:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b813d64a5c1eb3498986d5a316fa433df682acfa3038a9467f72232655fe3d59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `traefik:v2.7-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull traefik@sha256:7d454bf6f16177192750790acdbde2230a4d390a06b36683e92e5fc276a7f7b2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2532336814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aef3d6aed360b6013f3eac849ed76ff75eeaca4fd73dfec990b913776e8a164e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 13 Jun 2022 18:17:16 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 13 Jun 2022 18:17:17 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:17:18 GMT
ENTRYPOINT ["/traefik"]
# Mon, 13 Jun 2022 18:17:19 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc81fc68b4bd26ace09cac1f9e156a7f10c4a01fb84c1bd61156bf85efeac85`  
		Last Modified: Mon, 13 Jun 2022 18:18:58 GMT  
		Size: 28.3 MB (28275302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2b74c1667e6fd86372a21e937c532e1aa5a02c0c5590cdf2990e82bb1e6caa`  
		Last Modified: Mon, 13 Jun 2022 18:18:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5ec0fd7a47d0f100d28be14844121e6ef46f7d279f9365d6f4c5ae34833395`  
		Last Modified: Mon, 13 Jun 2022 18:18:27 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613e0863856475e19f15fbdf6bcf5516e0962a80fa16605d3ae57f8c2d4e2334`  
		Last Modified: Mon, 13 Jun 2022 18:18:27 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.7.1`

```console
$ docker pull traefik@sha256:fdff55caa91ac7ff217ff03b93f3673844b3b88ad993e023ab43f6004021697c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.7.1` - linux; amd64

```console
$ docker pull traefik@sha256:6354bfe99cf39164514ecca33ef4189361f0bf4eca8c16ffc1bae3623b99e8c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31023311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8345b2e8bee0c824835af0881cfdc602bbb351637c205cbebc76e7b74f813597`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:09:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:34:49 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:34:50 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:34:50 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:34:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:34:50 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:34:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07cb125bb766321ae78c2a558eb61358ea0c322871a963cc343f07b19a5dfe9f`  
		Last Modified: Tue, 24 May 2022 20:09:52 GMT  
		Size: 667.0 KB (667045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7643a4c688aef051e331797b6a1c3cf5a493b95e95e9a90502f34bb69543cf`  
		Last Modified: Mon, 13 Jun 2022 18:35:44 GMT  
		Size: 27.5 MB (27541339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5730b5ba9047bdf67c081e949f31b562532504f42b183afab9b38e82692c6a03`  
		Last Modified: Mon, 13 Jun 2022 18:35:39 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.7.1` - linux; arm variant v6

```console
$ docker pull traefik@sha256:b8e54b077cf2ffb132203d201519c7dae5dd885ea8cf6eb4b24f3bdd37eb0a6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29110783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc0175d61827f26689cebc311c086e4998894cb2370fa203eb6b0fc54626b7b9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:16:34 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:01:07 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:01:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:01:08 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:01:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:01:09 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:01:10 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ca500a6585c4382a3d0562172788318c2044142456377fdbf2c4b279334e26`  
		Last Modified: Tue, 24 May 2022 20:19:13 GMT  
		Size: 672.6 KB (672642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c97f5f8fa2680bd0e85b1838bc88a1b3bad8ea5a158b18383f007e4c6b398e52`  
		Last Modified: Mon, 13 Jun 2022 18:04:09 GMT  
		Size: 25.8 MB (25815800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a11e8a929d0ad2e555c58f324df02cde6c468d2662ecf5414979893c990664`  
		Last Modified: Mon, 13 Jun 2022 18:03:52 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.7.1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:f65b5a3b0de3d895385f85c41a180573a59d7dc4890d24e1b21c3fedd699ddf2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28492564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d1d1d829b444cff7a651cd13bdc6b2a66de794c8f21f75c5b7f204da37fdcb4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 21:18:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:19:33 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:19:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:19:35 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:19:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:19:37 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:19:38 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdde6df9c5c8f6328c1ce3fe2ca88cea0a7799584b83cafec0322b4d7235d0b7`  
		Last Modified: Tue, 24 May 2022 21:20:14 GMT  
		Size: 668.4 KB (668397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed46ebeb3f061a6426a51c9ce5d729ffe5bc2f3d8353303c30c35bff93ed4232`  
		Last Modified: Mon, 13 Jun 2022 18:21:04 GMT  
		Size: 25.1 MB (25107322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8683e30306089877837d12d61eaf9cc16d7ad0b3313d5b38dbff4cbc1685b057`  
		Last Modified: Mon, 13 Jun 2022 18:21:00 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.7.1` - linux; s390x

```console
$ docker pull traefik@sha256:9d7c6aa60ebe18d8257b0a02296eb18ac01e047675e48f4c20272c849c98669d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29788377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11de775752a6ad32f36bb166122916f9c84d52645b1d8c4274acb265af05d91`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:28:44 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:15:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:15:21 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:15:22 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:15:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:15:22 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:15:22 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f52582da22b0abbdbb4590735229191759cc22a1119ccdf5af9cd472103ffd`  
		Last Modified: Tue, 24 May 2022 20:29:51 GMT  
		Size: 672.6 KB (672603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0a8dab5f416aa3abd40293a95475c0df50231b6c94cf0b9c4fdbe5d2088c03`  
		Last Modified: Mon, 13 Jun 2022 18:16:12 GMT  
		Size: 26.5 MB (26515031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1cc2efd66f301007736aaf33dcba85abe0fd187a08d11ce716f925b49440b20`  
		Last Modified: Mon, 13 Jun 2022 18:16:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.7.1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b813d64a5c1eb3498986d5a316fa433df682acfa3038a9467f72232655fe3d59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `traefik:v2.7.1-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull traefik@sha256:7d454bf6f16177192750790acdbde2230a4d390a06b36683e92e5fc276a7f7b2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2532336814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aef3d6aed360b6013f3eac849ed76ff75eeaca4fd73dfec990b913776e8a164e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 13 Jun 2022 18:17:16 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 13 Jun 2022 18:17:17 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:17:18 GMT
ENTRYPOINT ["/traefik"]
# Mon, 13 Jun 2022 18:17:19 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc81fc68b4bd26ace09cac1f9e156a7f10c4a01fb84c1bd61156bf85efeac85`  
		Last Modified: Mon, 13 Jun 2022 18:18:58 GMT  
		Size: 28.3 MB (28275302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2b74c1667e6fd86372a21e937c532e1aa5a02c0c5590cdf2990e82bb1e6caa`  
		Last Modified: Mon, 13 Jun 2022 18:18:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5ec0fd7a47d0f100d28be14844121e6ef46f7d279f9365d6f4c5ae34833395`  
		Last Modified: Mon, 13 Jun 2022 18:18:27 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613e0863856475e19f15fbdf6bcf5516e0962a80fa16605d3ae57f8c2d4e2334`  
		Last Modified: Mon, 13 Jun 2022 18:18:27 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.8`

```console
$ docker pull traefik@sha256:0856f146dfbc67612de10b8776b735b3e903e0fb62d15710982a53c53b67a3b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.8` - linux; amd64

```console
$ docker pull traefik@sha256:5e1798198129ebf84fec2b5e3aae4576abade055a3e1429147a7f66184501209
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31269784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dca842284774841bc00b1ee58d6c51086de47ff42311872db4f2750cc4195de`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:09:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:34:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.0-rc1/traefik_v2.8.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:34:43 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:34:43 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:34:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:34:43 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:34:43 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07cb125bb766321ae78c2a558eb61358ea0c322871a963cc343f07b19a5dfe9f`  
		Last Modified: Tue, 24 May 2022 20:09:52 GMT  
		Size: 667.0 KB (667045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d0aa7bd10b0837b5951891be0343aae1e2b18ef9fe46a7af0b1379288a5088`  
		Last Modified: Mon, 13 Jun 2022 18:35:23 GMT  
		Size: 27.8 MB (27787812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a603c8fd0afaba7471e72f9ff316ae88170561fd4e0b0f31ae7a42d771b379`  
		Last Modified: Mon, 13 Jun 2022 18:35:18 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.8` - linux; arm variant v6

```console
$ docker pull traefik@sha256:dbb784ff502f912465406439ee9df419405fe6dff2402b414240587d7945bbfc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.3 MB (29334407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7f41f140507e568077e956e176d79728114b4e5e81875f37ddabcf3c0bd9916`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:16:34 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:00:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.0-rc1/traefik_v2.8.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:00:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:00:44 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:00:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:00:45 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:00:46 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ca500a6585c4382a3d0562172788318c2044142456377fdbf2c4b279334e26`  
		Last Modified: Tue, 24 May 2022 20:19:13 GMT  
		Size: 672.6 KB (672642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9fd4dbb43f6693d731fc04a307864de55084a8aae49ba713c346b8b2609de3`  
		Last Modified: Mon, 13 Jun 2022 18:03:31 GMT  
		Size: 26.0 MB (26039425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4d398d59c3345b33011af9a19eea0681c6eed32ec39bb226fbf4e13728afb3`  
		Last Modified: Mon, 13 Jun 2022 18:03:14 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.8` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:0d6a87b45a3e97b4718d724fed6b60de6396b9379f7aafe8ba1f84311a12470c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28719767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a284f06f2207f2f09b33871cbc6854d984a4dc3ce5fbae9292fef6273d34347b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 21:18:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:19:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.0-rc1/traefik_v2.8.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:19:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:19:20 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:19:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:19:22 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:19:23 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdde6df9c5c8f6328c1ce3fe2ca88cea0a7799584b83cafec0322b4d7235d0b7`  
		Last Modified: Tue, 24 May 2022 21:20:14 GMT  
		Size: 668.4 KB (668397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32682e72e2fb3405355907ebe27456de8196b3869606c0282e33d87f6456800d`  
		Last Modified: Mon, 13 Jun 2022 18:20:40 GMT  
		Size: 25.3 MB (25334525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d930e8e440833d01453b05b786f093dd51000881521fc92a87f2375d888bc4d`  
		Last Modified: Mon, 13 Jun 2022 18:20:36 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.8` - linux; s390x

```console
$ docker pull traefik@sha256:d2e42180e7790c806f17c7b7d07d6738803dca07ea4e11bc161f43e79055dcd2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.0 MB (30026181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99c5ab9d7a4ad3bc5511585018c91cada5addf9b0599e1fb9109608ec5c74a5a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:28:44 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:15:07 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.0-rc1/traefik_v2.8.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:15:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:15:08 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:15:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:15:09 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:15:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f52582da22b0abbdbb4590735229191759cc22a1119ccdf5af9cd472103ffd`  
		Last Modified: Tue, 24 May 2022 20:29:51 GMT  
		Size: 672.6 KB (672603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba97cee16ef49e268621c22e0b2c3da5dc7914b67bb92367c1473169047af63`  
		Last Modified: Mon, 13 Jun 2022 18:15:57 GMT  
		Size: 26.8 MB (26752834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c61301d344682dd15f4d3092db668cdb3562084ca343ead49f47d118201425`  
		Last Modified: Mon, 13 Jun 2022 18:15:53 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.8-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e2cc222f17256cab7d03feacf5c2f7aa2a0034fcdaab0019545703be359e59e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `traefik:v2.8-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull traefik@sha256:8963ee086a8a32c8458e64da5888d044e5b5dd7737918b8ae56dc51beb03cc75
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2532588939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8038611223da84ee443ca21bdc0a5febfe709064148bdcf22f66d836c19ef9a`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 13 Jun 2022 18:15:47 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.8.0-rc1/traefik_v2.8.0-rc1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 13 Jun 2022 18:15:48 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:15:49 GMT
ENTRYPOINT ["/traefik"]
# Mon, 13 Jun 2022 18:15:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16db0b20ba12318f4f238f69199c29e73928f90b9650bb3578d1a9b182a2d985`  
		Last Modified: Mon, 13 Jun 2022 18:18:11 GMT  
		Size: 28.5 MB (28527375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71918551829e1bfe9f5df15be61a91f9a4432268933fcd3cb7b261305b39e13b`  
		Last Modified: Mon, 13 Jun 2022 18:18:03 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534cd28bde041060e9269066e8ca5ebad28e153a233c215a335a9de34c393944`  
		Last Modified: Mon, 13 Jun 2022 18:18:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92059b5c9612669718297746abced06cbd9bc03ee2e89f97225102e27847a8d8`  
		Last Modified: Mon, 13 Jun 2022 18:18:03 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.8.0-rc1`

```console
$ docker pull traefik@sha256:0856f146dfbc67612de10b8776b735b3e903e0fb62d15710982a53c53b67a3b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.8.0-rc1` - linux; amd64

```console
$ docker pull traefik@sha256:5e1798198129ebf84fec2b5e3aae4576abade055a3e1429147a7f66184501209
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31269784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dca842284774841bc00b1ee58d6c51086de47ff42311872db4f2750cc4195de`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:09:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:34:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.0-rc1/traefik_v2.8.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:34:43 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:34:43 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:34:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:34:43 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:34:43 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07cb125bb766321ae78c2a558eb61358ea0c322871a963cc343f07b19a5dfe9f`  
		Last Modified: Tue, 24 May 2022 20:09:52 GMT  
		Size: 667.0 KB (667045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d0aa7bd10b0837b5951891be0343aae1e2b18ef9fe46a7af0b1379288a5088`  
		Last Modified: Mon, 13 Jun 2022 18:35:23 GMT  
		Size: 27.8 MB (27787812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a603c8fd0afaba7471e72f9ff316ae88170561fd4e0b0f31ae7a42d771b379`  
		Last Modified: Mon, 13 Jun 2022 18:35:18 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.8.0-rc1` - linux; arm variant v6

```console
$ docker pull traefik@sha256:dbb784ff502f912465406439ee9df419405fe6dff2402b414240587d7945bbfc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.3 MB (29334407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7f41f140507e568077e956e176d79728114b4e5e81875f37ddabcf3c0bd9916`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:16:34 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:00:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.0-rc1/traefik_v2.8.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:00:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:00:44 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:00:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:00:45 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:00:46 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ca500a6585c4382a3d0562172788318c2044142456377fdbf2c4b279334e26`  
		Last Modified: Tue, 24 May 2022 20:19:13 GMT  
		Size: 672.6 KB (672642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9fd4dbb43f6693d731fc04a307864de55084a8aae49ba713c346b8b2609de3`  
		Last Modified: Mon, 13 Jun 2022 18:03:31 GMT  
		Size: 26.0 MB (26039425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4d398d59c3345b33011af9a19eea0681c6eed32ec39bb226fbf4e13728afb3`  
		Last Modified: Mon, 13 Jun 2022 18:03:14 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.8.0-rc1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:0d6a87b45a3e97b4718d724fed6b60de6396b9379f7aafe8ba1f84311a12470c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28719767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a284f06f2207f2f09b33871cbc6854d984a4dc3ce5fbae9292fef6273d34347b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 21:18:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:19:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.0-rc1/traefik_v2.8.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:19:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:19:20 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:19:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:19:22 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:19:23 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdde6df9c5c8f6328c1ce3fe2ca88cea0a7799584b83cafec0322b4d7235d0b7`  
		Last Modified: Tue, 24 May 2022 21:20:14 GMT  
		Size: 668.4 KB (668397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32682e72e2fb3405355907ebe27456de8196b3869606c0282e33d87f6456800d`  
		Last Modified: Mon, 13 Jun 2022 18:20:40 GMT  
		Size: 25.3 MB (25334525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d930e8e440833d01453b05b786f093dd51000881521fc92a87f2375d888bc4d`  
		Last Modified: Mon, 13 Jun 2022 18:20:36 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.8.0-rc1` - linux; s390x

```console
$ docker pull traefik@sha256:d2e42180e7790c806f17c7b7d07d6738803dca07ea4e11bc161f43e79055dcd2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.0 MB (30026181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99c5ab9d7a4ad3bc5511585018c91cada5addf9b0599e1fb9109608ec5c74a5a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:28:44 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:15:07 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.0-rc1/traefik_v2.8.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:15:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:15:08 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:15:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:15:09 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:15:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f52582da22b0abbdbb4590735229191759cc22a1119ccdf5af9cd472103ffd`  
		Last Modified: Tue, 24 May 2022 20:29:51 GMT  
		Size: 672.6 KB (672603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba97cee16ef49e268621c22e0b2c3da5dc7914b67bb92367c1473169047af63`  
		Last Modified: Mon, 13 Jun 2022 18:15:57 GMT  
		Size: 26.8 MB (26752834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c61301d344682dd15f4d3092db668cdb3562084ca343ead49f47d118201425`  
		Last Modified: Mon, 13 Jun 2022 18:15:53 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.8.0-rc1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e2cc222f17256cab7d03feacf5c2f7aa2a0034fcdaab0019545703be359e59e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `traefik:v2.8.0-rc1-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull traefik@sha256:8963ee086a8a32c8458e64da5888d044e5b5dd7737918b8ae56dc51beb03cc75
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2532588939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8038611223da84ee443ca21bdc0a5febfe709064148bdcf22f66d836c19ef9a`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 13 Jun 2022 18:15:47 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.8.0-rc1/traefik_v2.8.0-rc1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 13 Jun 2022 18:15:48 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:15:49 GMT
ENTRYPOINT ["/traefik"]
# Mon, 13 Jun 2022 18:15:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16db0b20ba12318f4f238f69199c29e73928f90b9650bb3578d1a9b182a2d985`  
		Last Modified: Mon, 13 Jun 2022 18:18:11 GMT  
		Size: 28.5 MB (28527375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71918551829e1bfe9f5df15be61a91f9a4432268933fcd3cb7b261305b39e13b`  
		Last Modified: Mon, 13 Jun 2022 18:18:03 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534cd28bde041060e9269066e8ca5ebad28e153a233c215a335a9de34c393944`  
		Last Modified: Mon, 13 Jun 2022 18:18:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92059b5c9612669718297746abced06cbd9bc03ee2e89f97225102e27847a8d8`  
		Last Modified: Mon, 13 Jun 2022 18:18:03 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:vacherin`

```console
$ docker pull traefik@sha256:0856f146dfbc67612de10b8776b735b3e903e0fb62d15710982a53c53b67a3b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:vacherin` - linux; amd64

```console
$ docker pull traefik@sha256:5e1798198129ebf84fec2b5e3aae4576abade055a3e1429147a7f66184501209
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31269784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dca842284774841bc00b1ee58d6c51086de47ff42311872db4f2750cc4195de`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:09:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:34:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.0-rc1/traefik_v2.8.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:34:43 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:34:43 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:34:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:34:43 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:34:43 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07cb125bb766321ae78c2a558eb61358ea0c322871a963cc343f07b19a5dfe9f`  
		Last Modified: Tue, 24 May 2022 20:09:52 GMT  
		Size: 667.0 KB (667045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d0aa7bd10b0837b5951891be0343aae1e2b18ef9fe46a7af0b1379288a5088`  
		Last Modified: Mon, 13 Jun 2022 18:35:23 GMT  
		Size: 27.8 MB (27787812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a603c8fd0afaba7471e72f9ff316ae88170561fd4e0b0f31ae7a42d771b379`  
		Last Modified: Mon, 13 Jun 2022 18:35:18 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:vacherin` - linux; arm variant v6

```console
$ docker pull traefik@sha256:dbb784ff502f912465406439ee9df419405fe6dff2402b414240587d7945bbfc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.3 MB (29334407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7f41f140507e568077e956e176d79728114b4e5e81875f37ddabcf3c0bd9916`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:16:34 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:00:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.0-rc1/traefik_v2.8.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:00:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:00:44 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:00:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:00:45 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:00:46 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ca500a6585c4382a3d0562172788318c2044142456377fdbf2c4b279334e26`  
		Last Modified: Tue, 24 May 2022 20:19:13 GMT  
		Size: 672.6 KB (672642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9fd4dbb43f6693d731fc04a307864de55084a8aae49ba713c346b8b2609de3`  
		Last Modified: Mon, 13 Jun 2022 18:03:31 GMT  
		Size: 26.0 MB (26039425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4d398d59c3345b33011af9a19eea0681c6eed32ec39bb226fbf4e13728afb3`  
		Last Modified: Mon, 13 Jun 2022 18:03:14 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:vacherin` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:0d6a87b45a3e97b4718d724fed6b60de6396b9379f7aafe8ba1f84311a12470c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28719767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a284f06f2207f2f09b33871cbc6854d984a4dc3ce5fbae9292fef6273d34347b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 21:18:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:19:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.0-rc1/traefik_v2.8.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:19:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:19:20 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:19:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:19:22 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:19:23 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdde6df9c5c8f6328c1ce3fe2ca88cea0a7799584b83cafec0322b4d7235d0b7`  
		Last Modified: Tue, 24 May 2022 21:20:14 GMT  
		Size: 668.4 KB (668397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32682e72e2fb3405355907ebe27456de8196b3869606c0282e33d87f6456800d`  
		Last Modified: Mon, 13 Jun 2022 18:20:40 GMT  
		Size: 25.3 MB (25334525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d930e8e440833d01453b05b786f093dd51000881521fc92a87f2375d888bc4d`  
		Last Modified: Mon, 13 Jun 2022 18:20:36 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:vacherin` - linux; s390x

```console
$ docker pull traefik@sha256:d2e42180e7790c806f17c7b7d07d6738803dca07ea4e11bc161f43e79055dcd2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.0 MB (30026181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99c5ab9d7a4ad3bc5511585018c91cada5addf9b0599e1fb9109608ec5c74a5a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:28:44 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 13 Jun 2022 18:15:07 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.0-rc1/traefik_v2.8.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 13 Jun 2022 18:15:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 13 Jun 2022 18:15:08 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:15:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Jun 2022 18:15:09 GMT
CMD ["traefik"]
# Mon, 13 Jun 2022 18:15:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f52582da22b0abbdbb4590735229191759cc22a1119ccdf5af9cd472103ffd`  
		Last Modified: Tue, 24 May 2022 20:29:51 GMT  
		Size: 672.6 KB (672603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba97cee16ef49e268621c22e0b2c3da5dc7914b67bb92367c1473169047af63`  
		Last Modified: Mon, 13 Jun 2022 18:15:57 GMT  
		Size: 26.8 MB (26752834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c61301d344682dd15f4d3092db668cdb3562084ca343ead49f47d118201425`  
		Last Modified: Mon, 13 Jun 2022 18:15:53 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:vacherin-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e2cc222f17256cab7d03feacf5c2f7aa2a0034fcdaab0019545703be359e59e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `traefik:vacherin-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull traefik@sha256:8963ee086a8a32c8458e64da5888d044e5b5dd7737918b8ae56dc51beb03cc75
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2532588939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8038611223da84ee443ca21bdc0a5febfe709064148bdcf22f66d836c19ef9a`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 13 Jun 2022 18:15:47 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.8.0-rc1/traefik_v2.8.0-rc1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 13 Jun 2022 18:15:48 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:15:49 GMT
ENTRYPOINT ["/traefik"]
# Mon, 13 Jun 2022 18:15:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16db0b20ba12318f4f238f69199c29e73928f90b9650bb3578d1a9b182a2d985`  
		Last Modified: Mon, 13 Jun 2022 18:18:11 GMT  
		Size: 28.5 MB (28527375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71918551829e1bfe9f5df15be61a91f9a4432268933fcd3cb7b261305b39e13b`  
		Last Modified: Mon, 13 Jun 2022 18:18:03 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534cd28bde041060e9269066e8ca5ebad28e153a233c215a335a9de34c393944`  
		Last Modified: Mon, 13 Jun 2022 18:18:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92059b5c9612669718297746abced06cbd9bc03ee2e89f97225102e27847a8d8`  
		Last Modified: Mon, 13 Jun 2022 18:18:03 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:b813d64a5c1eb3498986d5a316fa433df682acfa3038a9467f72232655fe3d59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull traefik@sha256:7d454bf6f16177192750790acdbde2230a4d390a06b36683e92e5fc276a7f7b2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2532336814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aef3d6aed360b6013f3eac849ed76ff75eeaca4fd73dfec990b913776e8a164e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 13 Jun 2022 18:17:16 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 13 Jun 2022 18:17:17 GMT
EXPOSE 80
# Mon, 13 Jun 2022 18:17:18 GMT
ENTRYPOINT ["/traefik"]
# Mon, 13 Jun 2022 18:17:19 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc81fc68b4bd26ace09cac1f9e156a7f10c4a01fb84c1bd61156bf85efeac85`  
		Last Modified: Mon, 13 Jun 2022 18:18:58 GMT  
		Size: 28.3 MB (28275302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2b74c1667e6fd86372a21e937c532e1aa5a02c0c5590cdf2990e82bb1e6caa`  
		Last Modified: Mon, 13 Jun 2022 18:18:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5ec0fd7a47d0f100d28be14844121e6ef46f7d279f9365d6f4c5ae34833395`  
		Last Modified: Mon, 13 Jun 2022 18:18:27 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613e0863856475e19f15fbdf6bcf5516e0962a80fa16605d3ae57f8c2d4e2334`  
		Last Modified: Mon, 13 Jun 2022 18:18:27 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
