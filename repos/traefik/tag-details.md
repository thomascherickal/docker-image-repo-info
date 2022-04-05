<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:1.7`](#traefik17)
-	[`traefik:1.7-alpine`](#traefik17-alpine)
-	[`traefik:1.7-windowsservercore-1809`](#traefik17-windowsservercore-1809)
-	[`traefik:1.7.34`](#traefik1734)
-	[`traefik:1.7.34-alpine`](#traefik1734-alpine)
-	[`traefik:1.7.34-windowsservercore-1809`](#traefik1734-windowsservercore-1809)
-	[`traefik:2.6`](#traefik26)
-	[`traefik:2.6-windowsservercore-1809`](#traefik26-windowsservercore-1809)
-	[`traefik:2.6.3`](#traefik263)
-	[`traefik:2.6.3-windowsservercore-1809`](#traefik263-windowsservercore-1809)
-	[`traefik:2.7`](#traefik27)
-	[`traefik:2.7-windowsservercore-1809`](#traefik27-windowsservercore-1809)
-	[`traefik:2.7.0-rc2`](#traefik270-rc2)
-	[`traefik:2.7.0-rc2-windowsservercore-1809`](#traefik270-rc2-windowsservercore-1809)
-	[`traefik:epoisses`](#traefikepoisses)
-	[`traefik:epoisses-windowsservercore-1809`](#traefikepoisses-windowsservercore-1809)
-	[`traefik:latest`](#traefiklatest)
-	[`traefik:maroilles`](#traefikmaroilles)
-	[`traefik:maroilles-alpine`](#traefikmaroilles-alpine)
-	[`traefik:maroilles-windowsservercore-1809`](#traefikmaroilles-windowsservercore-1809)
-	[`traefik:rocamadour`](#traefikrocamadour)
-	[`traefik:rocamadour-windowsservercore-1809`](#traefikrocamadour-windowsservercore-1809)
-	[`traefik:v1.7`](#traefikv17)
-	[`traefik:v1.7-alpine`](#traefikv17-alpine)
-	[`traefik:v1.7-windowsservercore-1809`](#traefikv17-windowsservercore-1809)
-	[`traefik:v1.7.34`](#traefikv1734)
-	[`traefik:v1.7.34-alpine`](#traefikv1734-alpine)
-	[`traefik:v1.7.34-windowsservercore-1809`](#traefikv1734-windowsservercore-1809)
-	[`traefik:v2.6`](#traefikv26)
-	[`traefik:v2.6-windowsservercore-1809`](#traefikv26-windowsservercore-1809)
-	[`traefik:v2.6.3`](#traefikv263)
-	[`traefik:v2.6.3-windowsservercore-1809`](#traefikv263-windowsservercore-1809)
-	[`traefik:v2.7`](#traefikv27)
-	[`traefik:v2.7-windowsservercore-1809`](#traefikv27-windowsservercore-1809)
-	[`traefik:v2.7.0-rc2`](#traefikv270-rc2)
-	[`traefik:v2.7.0-rc2-windowsservercore-1809`](#traefikv270-rc2-windowsservercore-1809)
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
$ docker pull traefik@sha256:2536d87a206f10723c87604304bd3355cf36757de6599917cd9e8e77a03ba612
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:00b854b023b6ad2775a64b9a3c191420d2e5ee28902906b6e38ea3db6e9ee826
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25647457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bdaefa287d6893b1f23c7f069a71f95a7d520c4000d37330654a30402867e02`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:43:11 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 29 Mar 2022 11:43:30 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 29 Mar 2022 11:43:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 29 Mar 2022 11:43:31 GMT
EXPOSE 80
# Tue, 29 Mar 2022 11:43:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 11:43:31 GMT
CMD ["traefik"]
# Tue, 29 Mar 2022 11:43:31 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491249faa733d19d2c4f479860df3563c3f269d08d4c70b53926670b486092d5`  
		Last Modified: Tue, 29 Mar 2022 11:44:20 GMT  
		Size: 666.7 KB (666674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa40b07000dff13e47f89c1a98d9c91348c57a3d63e217a6048ca837818b8dfe`  
		Last Modified: Tue, 29 Mar 2022 11:45:06 GMT  
		Size: 22.2 MB (22162061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df6217935f5fada8326229f327ccbf2417b11aa70f4f7d01c3ff7b5c793d747`  
		Last Modified: Tue, 29 Mar 2022 11:45:02 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:faf9be547dc6180e313c055b4a7f2da1a2eb1b4a62f2215ca4712ffbfef5dd83
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23922329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d09ca9a761d0f863bf5aff1b51e985ecf319d9821a5cfd67aadbc17743780b5f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:46 GMT
ADD file:9670f4f7de6a9b8eb844e418daedd0dbad90009126790eb65e246b29cac5ea47 in / 
# Tue, 29 Mar 2022 00:49:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 13:21:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 29 Mar 2022 13:22:23 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 29 Mar 2022 13:22:24 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 29 Mar 2022 13:22:24 GMT
EXPOSE 80
# Tue, 29 Mar 2022 13:22:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 13:22:25 GMT
CMD ["traefik"]
# Tue, 29 Mar 2022 13:22:25 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79f5c9df0b90097bae07a9861e9e0e3f52a16b0bfde2793c4e14ad033cfb47f4`  
		Last Modified: Tue, 29 Mar 2022 00:51:45 GMT  
		Size: 2.6 MB (2626017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10449722d0e221d9f2d76fded7a3856b1e5da5de38e926c9dbde9dfeb95c67c8`  
		Last Modified: Tue, 29 Mar 2022 13:24:24 GMT  
		Size: 672.5 KB (672526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4783ae6cdd5ea4a521c85fdafa8b39c172173886b178ef7c9d456018198f20bc`  
		Last Modified: Tue, 29 Mar 2022 13:26:02 GMT  
		Size: 20.6 MB (20623419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99f4630a8f43bea8e6dd2b3cd39639e77fa3d52cd95e84593a545ddff84bcfe`  
		Last Modified: Tue, 29 Mar 2022 13:25:48 GMT  
		Size: 367.0 B  
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
$ docker pull traefik@sha256:85ffe3d43fd4929a0e48d226e018af240fbbd8ea9a03685f74f1c78c432f85b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:1.7-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:67d210fa3d7dcb1ebc3b3b5f3bfdaac7d18195e1bb2b83fa2c1b1f48d09b08dd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2738303983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6ebd04310fbdd68b4e7225310f8a6f2dec3a0330af0d02b74a9a0e35b79945b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:53:09 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 09 Mar 2022 18:53:10 GMT
EXPOSE 80
# Wed, 09 Mar 2022 18:53:11 GMT
ENTRYPOINT ["/traefik"]
# Wed, 09 Mar 2022 18:53:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd63edc5d2bde654b771ee58c8e9bb78539127758e862053223f402d3eaea68`  
		Last Modified: Wed, 09 Mar 2022 18:54:50 GMT  
		Size: 22.8 MB (22845783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cefe3e1f9703a33ffdf92a9c03b8a4738222fe08ea99aded6416f848aa300e9`  
		Last Modified: Wed, 09 Mar 2022 18:54:27 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939f3b18eb0ddb1cb4c6b01a2abc4127403c6a67c630a8c05c6be5f43ab74acc`  
		Last Modified: Wed, 09 Mar 2022 18:54:26 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bcba10ab84d161e2dc32a48f6bc15da23d8aabdb22bbf4a89499ce18583d46`  
		Last Modified: Wed, 09 Mar 2022 18:54:26 GMT  
		Size: 1.4 KB (1389 bytes)  
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
$ docker pull traefik@sha256:2536d87a206f10723c87604304bd3355cf36757de6599917cd9e8e77a03ba612
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.34-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:00b854b023b6ad2775a64b9a3c191420d2e5ee28902906b6e38ea3db6e9ee826
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25647457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bdaefa287d6893b1f23c7f069a71f95a7d520c4000d37330654a30402867e02`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:43:11 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 29 Mar 2022 11:43:30 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 29 Mar 2022 11:43:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 29 Mar 2022 11:43:31 GMT
EXPOSE 80
# Tue, 29 Mar 2022 11:43:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 11:43:31 GMT
CMD ["traefik"]
# Tue, 29 Mar 2022 11:43:31 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491249faa733d19d2c4f479860df3563c3f269d08d4c70b53926670b486092d5`  
		Last Modified: Tue, 29 Mar 2022 11:44:20 GMT  
		Size: 666.7 KB (666674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa40b07000dff13e47f89c1a98d9c91348c57a3d63e217a6048ca837818b8dfe`  
		Last Modified: Tue, 29 Mar 2022 11:45:06 GMT  
		Size: 22.2 MB (22162061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df6217935f5fada8326229f327ccbf2417b11aa70f4f7d01c3ff7b5c793d747`  
		Last Modified: Tue, 29 Mar 2022 11:45:02 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.34-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:faf9be547dc6180e313c055b4a7f2da1a2eb1b4a62f2215ca4712ffbfef5dd83
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23922329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d09ca9a761d0f863bf5aff1b51e985ecf319d9821a5cfd67aadbc17743780b5f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:46 GMT
ADD file:9670f4f7de6a9b8eb844e418daedd0dbad90009126790eb65e246b29cac5ea47 in / 
# Tue, 29 Mar 2022 00:49:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 13:21:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 29 Mar 2022 13:22:23 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 29 Mar 2022 13:22:24 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 29 Mar 2022 13:22:24 GMT
EXPOSE 80
# Tue, 29 Mar 2022 13:22:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 13:22:25 GMT
CMD ["traefik"]
# Tue, 29 Mar 2022 13:22:25 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79f5c9df0b90097bae07a9861e9e0e3f52a16b0bfde2793c4e14ad033cfb47f4`  
		Last Modified: Tue, 29 Mar 2022 00:51:45 GMT  
		Size: 2.6 MB (2626017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10449722d0e221d9f2d76fded7a3856b1e5da5de38e926c9dbde9dfeb95c67c8`  
		Last Modified: Tue, 29 Mar 2022 13:24:24 GMT  
		Size: 672.5 KB (672526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4783ae6cdd5ea4a521c85fdafa8b39c172173886b178ef7c9d456018198f20bc`  
		Last Modified: Tue, 29 Mar 2022 13:26:02 GMT  
		Size: 20.6 MB (20623419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99f4630a8f43bea8e6dd2b3cd39639e77fa3d52cd95e84593a545ddff84bcfe`  
		Last Modified: Tue, 29 Mar 2022 13:25:48 GMT  
		Size: 367.0 B  
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
$ docker pull traefik@sha256:85ffe3d43fd4929a0e48d226e018af240fbbd8ea9a03685f74f1c78c432f85b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:1.7.34-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:67d210fa3d7dcb1ebc3b3b5f3bfdaac7d18195e1bb2b83fa2c1b1f48d09b08dd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2738303983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6ebd04310fbdd68b4e7225310f8a6f2dec3a0330af0d02b74a9a0e35b79945b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:53:09 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 09 Mar 2022 18:53:10 GMT
EXPOSE 80
# Wed, 09 Mar 2022 18:53:11 GMT
ENTRYPOINT ["/traefik"]
# Wed, 09 Mar 2022 18:53:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd63edc5d2bde654b771ee58c8e9bb78539127758e862053223f402d3eaea68`  
		Last Modified: Wed, 09 Mar 2022 18:54:50 GMT  
		Size: 22.8 MB (22845783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cefe3e1f9703a33ffdf92a9c03b8a4738222fe08ea99aded6416f848aa300e9`  
		Last Modified: Wed, 09 Mar 2022 18:54:27 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939f3b18eb0ddb1cb4c6b01a2abc4127403c6a67c630a8c05c6be5f43ab74acc`  
		Last Modified: Wed, 09 Mar 2022 18:54:26 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bcba10ab84d161e2dc32a48f6bc15da23d8aabdb22bbf4a89499ce18583d46`  
		Last Modified: Wed, 09 Mar 2022 18:54:26 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.6`

```console
$ docker pull traefik@sha256:67d4020f130982992b0864ad714f90f79c12899229a8573612cb3047dc79a308
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.6` - linux; amd64

```console
$ docker pull traefik@sha256:a1219f2ba73f764ee9c550f3c13045a9264c6b78bdd0b0db6e956a7f96972f48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.3 MB (30339348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3325c6dd7f244fcdc7729819792ee0e0483f58f6ac34baabcd7bd374b7c067e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:43:11 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 31 Mar 2022 02:24:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 31 Mar 2022 02:24:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 31 Mar 2022 02:24:27 GMT
EXPOSE 80
# Thu, 31 Mar 2022 02:24:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 31 Mar 2022 02:24:27 GMT
CMD ["traefik"]
# Thu, 31 Mar 2022 02:24:27 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491249faa733d19d2c4f479860df3563c3f269d08d4c70b53926670b486092d5`  
		Last Modified: Tue, 29 Mar 2022 11:44:20 GMT  
		Size: 666.7 KB (666674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7660e64df1e00fb3bbfae87703ee37e1b01bf9352d6d5bf05dd11b9701a773`  
		Last Modified: Thu, 31 Mar 2022 02:25:23 GMT  
		Size: 26.9 MB (26853953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080a3ffe94e58283fb36ef270c6d19f0ef82fe40354fb2131023d1efbd951592`  
		Last Modified: Thu, 31 Mar 2022 02:25:18 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.6` - linux; arm variant v6

```console
$ docker pull traefik@sha256:2a6e91644420e884a47301e5719349eb6a1c6c36d044c7fcfac6789aeb4b0475
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28508633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53d4c7eeb0769e066b9a8fb8fe3463393dc695230d928b19ddc768a90f265ee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:46 GMT
ADD file:9670f4f7de6a9b8eb844e418daedd0dbad90009126790eb65e246b29cac5ea47 in / 
# Tue, 29 Mar 2022 00:49:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 13:21:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 29 Mar 2022 20:15:02 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 29 Mar 2022 20:15:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 29 Mar 2022 20:15:03 GMT
EXPOSE 80
# Tue, 29 Mar 2022 20:15:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 20:15:04 GMT
CMD ["traefik"]
# Tue, 29 Mar 2022 20:15:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79f5c9df0b90097bae07a9861e9e0e3f52a16b0bfde2793c4e14ad033cfb47f4`  
		Last Modified: Tue, 29 Mar 2022 00:51:45 GMT  
		Size: 2.6 MB (2626017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10449722d0e221d9f2d76fded7a3856b1e5da5de38e926c9dbde9dfeb95c67c8`  
		Last Modified: Tue, 29 Mar 2022 13:24:24 GMT  
		Size: 672.5 KB (672526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b16455b7f19741086604a735e590e982fa72a4f8419eebac2e4b93a6dded9e`  
		Last Modified: Tue, 29 Mar 2022 20:18:07 GMT  
		Size: 25.2 MB (25209721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ea9ec0719c1f9245fcee9072b0a02747793e15bec07885cade6befb6fa13b3`  
		Last Modified: Tue, 29 Mar 2022 20:17:50 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.6` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:abcf0f8ace901dc06a7db4b9ab761ed79d084f8a0f1fcb8d5b630fd4b6487bb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27882793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cebe76258a556250464b66a64aa1fe8af5aa375fbf74efa560d5cca5bfe4d84`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:27:04 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 07:27:22 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 07:27:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 07:27:23 GMT
EXPOSE 80
# Tue, 05 Apr 2022 07:27:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 07:27:25 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 07:27:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:1f34d16123c581d2614d26cbcd1618aa3bec385321f1b5d361be3a9d0cf3edd0`  
		Last Modified: Tue, 05 Apr 2022 07:29:03 GMT  
		Size: 24.5 MB (24496745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fb8900c64102e15429a227ea22db387e3f73f305e5b3a07ba46ef030aa6913`  
		Last Modified: Tue, 05 Apr 2022 07:28:59 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.6` - linux; s390x

```console
$ docker pull traefik@sha256:7664483ac7f02aed931da58072699fd842463c6ed0838dd77d1c9063ca373424
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29133529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9effa158d8a7eb4de0dc5ef0f9e5068b916010a030594833ffeee4229ce787`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:47 GMT
ADD file:0f70e0f0075bee67acb44e5ef01bf6b9df1f69a25b7aa6fd15bd5bb6ec5bcc9f in / 
# Mon, 04 Apr 2022 23:41:48 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:14:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 06:15:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 06:15:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 06:15:16 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:15:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 06:15:16 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 06:15:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6f6a6c77b1bd5dfb3e759efaa292f964f197ae4b96be74d80ef059f87317997a`  
		Last Modified: Mon, 04 Apr 2022 23:42:47 GMT  
		Size: 2.6 MB (2604075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd299e72e5dfb969cf246832a04767813018867ef4e23d3cd39e9ed53fbb2e2`  
		Last Modified: Tue, 05 Apr 2022 06:15:50 GMT  
		Size: 672.5 KB (672500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d058aad59a877e33e73441ea4d8bc9339a3cf057ba559b89a6403e9ad67d344`  
		Last Modified: Tue, 05 Apr 2022 06:16:11 GMT  
		Size: 25.9 MB (25856586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b401ac447e5e18e7baee3f9bc3f6e782878325212d2ef6cb51213203f7b7958`  
		Last Modified: Tue, 05 Apr 2022 06:16:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.6-windowsservercore-1809`

```console
$ docker pull traefik@sha256:8c6d3723194f2b09c6b7e6f1c65c00573ed8a86fb030871f472f15b7f68b6ff2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:2.6-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:47d24eaf1b6b706e5de58ce11e2cbebf3a0f9575a61fec03a4c861e4438807a9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2742898776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5706e325ee2ad18345e4fe2fd1dc42a027366b1f9c1ddfc6a3e3542f918ece9c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 29 Mar 2022 19:33:53 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 29 Mar 2022 19:33:54 GMT
EXPOSE 80
# Tue, 29 Mar 2022 19:33:55 GMT
ENTRYPOINT ["/traefik"]
# Tue, 29 Mar 2022 19:33:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a79b9a00328456358c525859928802742529204e1d520ec9f3f68f3fe63ee9`  
		Last Modified: Tue, 29 Mar 2022 19:35:24 GMT  
		Size: 27.4 MB (27440577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfbef29f86d1cb8156adb9e83f62919091b87ae19d8b49027e53e32207378a1`  
		Last Modified: Tue, 29 Mar 2022 19:35:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81861a2761b14e5cf1801456272bdb3de1fc16f0d8724c6df47a371f20478091`  
		Last Modified: Tue, 29 Mar 2022 19:35:17 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779ed28a5abfc5c391b359a30b2b6fccee48c70fdc42d2a44a77a31b1d4c3e4d`  
		Last Modified: Tue, 29 Mar 2022 19:35:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.6.3`

```console
$ docker pull traefik@sha256:67d4020f130982992b0864ad714f90f79c12899229a8573612cb3047dc79a308
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.6.3` - linux; amd64

```console
$ docker pull traefik@sha256:a1219f2ba73f764ee9c550f3c13045a9264c6b78bdd0b0db6e956a7f96972f48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.3 MB (30339348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3325c6dd7f244fcdc7729819792ee0e0483f58f6ac34baabcd7bd374b7c067e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:43:11 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 31 Mar 2022 02:24:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 31 Mar 2022 02:24:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 31 Mar 2022 02:24:27 GMT
EXPOSE 80
# Thu, 31 Mar 2022 02:24:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 31 Mar 2022 02:24:27 GMT
CMD ["traefik"]
# Thu, 31 Mar 2022 02:24:27 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491249faa733d19d2c4f479860df3563c3f269d08d4c70b53926670b486092d5`  
		Last Modified: Tue, 29 Mar 2022 11:44:20 GMT  
		Size: 666.7 KB (666674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7660e64df1e00fb3bbfae87703ee37e1b01bf9352d6d5bf05dd11b9701a773`  
		Last Modified: Thu, 31 Mar 2022 02:25:23 GMT  
		Size: 26.9 MB (26853953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080a3ffe94e58283fb36ef270c6d19f0ef82fe40354fb2131023d1efbd951592`  
		Last Modified: Thu, 31 Mar 2022 02:25:18 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.6.3` - linux; arm variant v6

```console
$ docker pull traefik@sha256:2a6e91644420e884a47301e5719349eb6a1c6c36d044c7fcfac6789aeb4b0475
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28508633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53d4c7eeb0769e066b9a8fb8fe3463393dc695230d928b19ddc768a90f265ee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:46 GMT
ADD file:9670f4f7de6a9b8eb844e418daedd0dbad90009126790eb65e246b29cac5ea47 in / 
# Tue, 29 Mar 2022 00:49:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 13:21:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 29 Mar 2022 20:15:02 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 29 Mar 2022 20:15:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 29 Mar 2022 20:15:03 GMT
EXPOSE 80
# Tue, 29 Mar 2022 20:15:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 20:15:04 GMT
CMD ["traefik"]
# Tue, 29 Mar 2022 20:15:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79f5c9df0b90097bae07a9861e9e0e3f52a16b0bfde2793c4e14ad033cfb47f4`  
		Last Modified: Tue, 29 Mar 2022 00:51:45 GMT  
		Size: 2.6 MB (2626017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10449722d0e221d9f2d76fded7a3856b1e5da5de38e926c9dbde9dfeb95c67c8`  
		Last Modified: Tue, 29 Mar 2022 13:24:24 GMT  
		Size: 672.5 KB (672526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b16455b7f19741086604a735e590e982fa72a4f8419eebac2e4b93a6dded9e`  
		Last Modified: Tue, 29 Mar 2022 20:18:07 GMT  
		Size: 25.2 MB (25209721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ea9ec0719c1f9245fcee9072b0a02747793e15bec07885cade6befb6fa13b3`  
		Last Modified: Tue, 29 Mar 2022 20:17:50 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.6.3` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:abcf0f8ace901dc06a7db4b9ab761ed79d084f8a0f1fcb8d5b630fd4b6487bb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27882793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cebe76258a556250464b66a64aa1fe8af5aa375fbf74efa560d5cca5bfe4d84`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:27:04 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 07:27:22 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 07:27:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 07:27:23 GMT
EXPOSE 80
# Tue, 05 Apr 2022 07:27:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 07:27:25 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 07:27:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:1f34d16123c581d2614d26cbcd1618aa3bec385321f1b5d361be3a9d0cf3edd0`  
		Last Modified: Tue, 05 Apr 2022 07:29:03 GMT  
		Size: 24.5 MB (24496745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fb8900c64102e15429a227ea22db387e3f73f305e5b3a07ba46ef030aa6913`  
		Last Modified: Tue, 05 Apr 2022 07:28:59 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.6.3` - linux; s390x

```console
$ docker pull traefik@sha256:7664483ac7f02aed931da58072699fd842463c6ed0838dd77d1c9063ca373424
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29133529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9effa158d8a7eb4de0dc5ef0f9e5068b916010a030594833ffeee4229ce787`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:47 GMT
ADD file:0f70e0f0075bee67acb44e5ef01bf6b9df1f69a25b7aa6fd15bd5bb6ec5bcc9f in / 
# Mon, 04 Apr 2022 23:41:48 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:14:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 06:15:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 06:15:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 06:15:16 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:15:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 06:15:16 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 06:15:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6f6a6c77b1bd5dfb3e759efaa292f964f197ae4b96be74d80ef059f87317997a`  
		Last Modified: Mon, 04 Apr 2022 23:42:47 GMT  
		Size: 2.6 MB (2604075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd299e72e5dfb969cf246832a04767813018867ef4e23d3cd39e9ed53fbb2e2`  
		Last Modified: Tue, 05 Apr 2022 06:15:50 GMT  
		Size: 672.5 KB (672500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d058aad59a877e33e73441ea4d8bc9339a3cf057ba559b89a6403e9ad67d344`  
		Last Modified: Tue, 05 Apr 2022 06:16:11 GMT  
		Size: 25.9 MB (25856586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b401ac447e5e18e7baee3f9bc3f6e782878325212d2ef6cb51213203f7b7958`  
		Last Modified: Tue, 05 Apr 2022 06:16:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.6.3-windowsservercore-1809`

```console
$ docker pull traefik@sha256:8c6d3723194f2b09c6b7e6f1c65c00573ed8a86fb030871f472f15b7f68b6ff2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:2.6.3-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:47d24eaf1b6b706e5de58ce11e2cbebf3a0f9575a61fec03a4c861e4438807a9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2742898776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5706e325ee2ad18345e4fe2fd1dc42a027366b1f9c1ddfc6a3e3542f918ece9c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 29 Mar 2022 19:33:53 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 29 Mar 2022 19:33:54 GMT
EXPOSE 80
# Tue, 29 Mar 2022 19:33:55 GMT
ENTRYPOINT ["/traefik"]
# Tue, 29 Mar 2022 19:33:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a79b9a00328456358c525859928802742529204e1d520ec9f3f68f3fe63ee9`  
		Last Modified: Tue, 29 Mar 2022 19:35:24 GMT  
		Size: 27.4 MB (27440577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfbef29f86d1cb8156adb9e83f62919091b87ae19d8b49027e53e32207378a1`  
		Last Modified: Tue, 29 Mar 2022 19:35:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81861a2761b14e5cf1801456272bdb3de1fc16f0d8724c6df47a371f20478091`  
		Last Modified: Tue, 29 Mar 2022 19:35:17 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779ed28a5abfc5c391b359a30b2b6fccee48c70fdc42d2a44a77a31b1d4c3e4d`  
		Last Modified: Tue, 29 Mar 2022 19:35:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.7`

```console
$ docker pull traefik@sha256:13b2dabb45da3611d756bf9b1e26d8c530e12d6edb6d182fb9cbe4847d552c0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.7` - linux; amd64

```console
$ docker pull traefik@sha256:0f179eab7150d8c8eabd7ca596d98603e420b84c78d0a8023eee1c06ee3ff545
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30884413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a4db61886791f13225c2845cd57d60ff8a5a0720eccb889e7c7341ffe1b9594`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:43:11 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 31 Mar 2022 02:24:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.0-rc2/traefik_v2.7.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 31 Mar 2022 02:24:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 31 Mar 2022 02:24:20 GMT
EXPOSE 80
# Thu, 31 Mar 2022 02:24:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 31 Mar 2022 02:24:20 GMT
CMD ["traefik"]
# Thu, 31 Mar 2022 02:24:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491249faa733d19d2c4f479860df3563c3f269d08d4c70b53926670b486092d5`  
		Last Modified: Tue, 29 Mar 2022 11:44:20 GMT  
		Size: 666.7 KB (666674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150f61256352f339798457a33bd19e97a2c486d649ab99d14e8ccc1b9c0aab4c`  
		Last Modified: Thu, 31 Mar 2022 02:25:02 GMT  
		Size: 27.4 MB (27399018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d9192a4e45679a6fe98f98a61976527914a4344b8b8126ba5e9ae401d7c37c`  
		Last Modified: Thu, 31 Mar 2022 02:24:57 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:1aee5e27fbc6358f097fa0fecd790f97972a5d860b39dd15c5c0746b7cae529a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (28982492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5067b6791686be1a6a27d9bb0fead0ff84404cf74a87b0cb709692e22117837c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:46 GMT
ADD file:9670f4f7de6a9b8eb844e418daedd0dbad90009126790eb65e246b29cac5ea47 in / 
# Tue, 29 Mar 2022 00:49:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 13:21:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 29 Mar 2022 20:14:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.0-rc2/traefik_v2.7.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 29 Mar 2022 20:14:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 29 Mar 2022 20:14:39 GMT
EXPOSE 80
# Tue, 29 Mar 2022 20:14:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 20:14:40 GMT
CMD ["traefik"]
# Tue, 29 Mar 2022 20:14:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79f5c9df0b90097bae07a9861e9e0e3f52a16b0bfde2793c4e14ad033cfb47f4`  
		Last Modified: Tue, 29 Mar 2022 00:51:45 GMT  
		Size: 2.6 MB (2626017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10449722d0e221d9f2d76fded7a3856b1e5da5de38e926c9dbde9dfeb95c67c8`  
		Last Modified: Tue, 29 Mar 2022 13:24:24 GMT  
		Size: 672.5 KB (672526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c35bed17508c434cf42b82887ab060852475c4e374ab4927382d30577e3ff1f`  
		Last Modified: Tue, 29 Mar 2022 20:17:27 GMT  
		Size: 25.7 MB (25683580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db18cf51e2278ee816fbc5b729a8cb8148229542f5993ccef454c8599eb551e`  
		Last Modified: Tue, 29 Mar 2022 20:17:10 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:cbc72e60f32f55ba66d1a5be7993d663006d2283f3b52202af99971e5c355ea2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28364421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ef4096bf04746212cf88c9a0795877622ff1ba98808ecb03b7ffe933c5ebd46`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:27:04 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 07:27:07 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.0-rc2/traefik_v2.7.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 07:27:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 07:27:08 GMT
EXPOSE 80
# Tue, 05 Apr 2022 07:27:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 07:27:10 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 07:27:11 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:ff858383c840c4b97834e60774329c49bf3fea922085ae31d8165402d4b9f5ea`  
		Last Modified: Tue, 05 Apr 2022 07:28:40 GMT  
		Size: 25.0 MB (24978372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04abccc9cf218d0e24ff784807a2c3570b5ed2a7183fbf08517b4fc4221c813e`  
		Last Modified: Tue, 05 Apr 2022 07:28:36 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.7` - linux; s390x

```console
$ docker pull traefik@sha256:7569039608d54d25f8a85c29da7151f2e16732547c169e96de3d8377bc945831
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29653216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e16a4ac48877da270277f281f90230f4a9638f791a4fe3a5e04e49c9e23235a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:47 GMT
ADD file:0f70e0f0075bee67acb44e5ef01bf6b9df1f69a25b7aa6fd15bd5bb6ec5bcc9f in / 
# Mon, 04 Apr 2022 23:41:48 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:14:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 06:15:02 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.0-rc2/traefik_v2.7.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 06:15:03 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 06:15:03 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:15:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 06:15:04 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 06:15:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6f6a6c77b1bd5dfb3e759efaa292f964f197ae4b96be74d80ef059f87317997a`  
		Last Modified: Mon, 04 Apr 2022 23:42:47 GMT  
		Size: 2.6 MB (2604075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd299e72e5dfb969cf246832a04767813018867ef4e23d3cd39e9ed53fbb2e2`  
		Last Modified: Tue, 05 Apr 2022 06:15:50 GMT  
		Size: 672.5 KB (672500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9565ee21a342064cf700d9474883f1f743b295fc38f1a934caec7c014c19a39`  
		Last Modified: Tue, 05 Apr 2022 06:15:54 GMT  
		Size: 26.4 MB (26376273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0ffd87278d72e40d22211cb05d509dbac1628f7a1a59d0e65d8b8a260db1c3`  
		Last Modified: Tue, 05 Apr 2022 06:15:50 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:fe30fb1edd24cb35ed73084221b49fd145c789c540a1a10e2e76aad943673a66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:2.7-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:b10e4f877aebabb1734135b2646cb64cc5d70727f9964b4b764f6f1e749decc3
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2743448944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf2840916230e28221e266704780ab0cf47a706724fd322280cc72c40af2d0d6`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 29 Mar 2022 19:32:51 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.7.0-rc2/traefik_v2.7.0-rc2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 29 Mar 2022 19:32:52 GMT
EXPOSE 80
# Tue, 29 Mar 2022 19:32:53 GMT
ENTRYPOINT ["/traefik"]
# Tue, 29 Mar 2022 19:32:54 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e322088afb1a013924e6a53963322f66b3b52751ccaeb821099765b4ddc569ae`  
		Last Modified: Tue, 29 Mar 2022 19:35:00 GMT  
		Size: 28.0 MB (27991054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68de6a12e36621523a032635b4054a09a9c5898b8e50c091d7170ca3f0926544`  
		Last Modified: Tue, 29 Mar 2022 19:34:29 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcece30b93b7bbc58f5afe87698f87c2dc34b5aae3311c71ebf03339c1b0fec`  
		Last Modified: Tue, 29 Mar 2022 19:34:29 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99b616e8af959eea48003b4cf3217d9c66250b599e93b4cc5496bfeea62699c`  
		Last Modified: Tue, 29 Mar 2022 19:34:29 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.7.0-rc2`

```console
$ docker pull traefik@sha256:13b2dabb45da3611d756bf9b1e26d8c530e12d6edb6d182fb9cbe4847d552c0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.7.0-rc2` - linux; amd64

```console
$ docker pull traefik@sha256:0f179eab7150d8c8eabd7ca596d98603e420b84c78d0a8023eee1c06ee3ff545
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30884413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a4db61886791f13225c2845cd57d60ff8a5a0720eccb889e7c7341ffe1b9594`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:43:11 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 31 Mar 2022 02:24:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.0-rc2/traefik_v2.7.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 31 Mar 2022 02:24:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 31 Mar 2022 02:24:20 GMT
EXPOSE 80
# Thu, 31 Mar 2022 02:24:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 31 Mar 2022 02:24:20 GMT
CMD ["traefik"]
# Thu, 31 Mar 2022 02:24:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491249faa733d19d2c4f479860df3563c3f269d08d4c70b53926670b486092d5`  
		Last Modified: Tue, 29 Mar 2022 11:44:20 GMT  
		Size: 666.7 KB (666674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150f61256352f339798457a33bd19e97a2c486d649ab99d14e8ccc1b9c0aab4c`  
		Last Modified: Thu, 31 Mar 2022 02:25:02 GMT  
		Size: 27.4 MB (27399018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d9192a4e45679a6fe98f98a61976527914a4344b8b8126ba5e9ae401d7c37c`  
		Last Modified: Thu, 31 Mar 2022 02:24:57 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.7.0-rc2` - linux; arm variant v6

```console
$ docker pull traefik@sha256:1aee5e27fbc6358f097fa0fecd790f97972a5d860b39dd15c5c0746b7cae529a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (28982492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5067b6791686be1a6a27d9bb0fead0ff84404cf74a87b0cb709692e22117837c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:46 GMT
ADD file:9670f4f7de6a9b8eb844e418daedd0dbad90009126790eb65e246b29cac5ea47 in / 
# Tue, 29 Mar 2022 00:49:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 13:21:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 29 Mar 2022 20:14:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.0-rc2/traefik_v2.7.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 29 Mar 2022 20:14:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 29 Mar 2022 20:14:39 GMT
EXPOSE 80
# Tue, 29 Mar 2022 20:14:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 20:14:40 GMT
CMD ["traefik"]
# Tue, 29 Mar 2022 20:14:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79f5c9df0b90097bae07a9861e9e0e3f52a16b0bfde2793c4e14ad033cfb47f4`  
		Last Modified: Tue, 29 Mar 2022 00:51:45 GMT  
		Size: 2.6 MB (2626017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10449722d0e221d9f2d76fded7a3856b1e5da5de38e926c9dbde9dfeb95c67c8`  
		Last Modified: Tue, 29 Mar 2022 13:24:24 GMT  
		Size: 672.5 KB (672526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c35bed17508c434cf42b82887ab060852475c4e374ab4927382d30577e3ff1f`  
		Last Modified: Tue, 29 Mar 2022 20:17:27 GMT  
		Size: 25.7 MB (25683580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db18cf51e2278ee816fbc5b729a8cb8148229542f5993ccef454c8599eb551e`  
		Last Modified: Tue, 29 Mar 2022 20:17:10 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.7.0-rc2` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:cbc72e60f32f55ba66d1a5be7993d663006d2283f3b52202af99971e5c355ea2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28364421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ef4096bf04746212cf88c9a0795877622ff1ba98808ecb03b7ffe933c5ebd46`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:27:04 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 07:27:07 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.0-rc2/traefik_v2.7.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 07:27:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 07:27:08 GMT
EXPOSE 80
# Tue, 05 Apr 2022 07:27:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 07:27:10 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 07:27:11 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:ff858383c840c4b97834e60774329c49bf3fea922085ae31d8165402d4b9f5ea`  
		Last Modified: Tue, 05 Apr 2022 07:28:40 GMT  
		Size: 25.0 MB (24978372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04abccc9cf218d0e24ff784807a2c3570b5ed2a7183fbf08517b4fc4221c813e`  
		Last Modified: Tue, 05 Apr 2022 07:28:36 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.7.0-rc2` - linux; s390x

```console
$ docker pull traefik@sha256:7569039608d54d25f8a85c29da7151f2e16732547c169e96de3d8377bc945831
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29653216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e16a4ac48877da270277f281f90230f4a9638f791a4fe3a5e04e49c9e23235a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:47 GMT
ADD file:0f70e0f0075bee67acb44e5ef01bf6b9df1f69a25b7aa6fd15bd5bb6ec5bcc9f in / 
# Mon, 04 Apr 2022 23:41:48 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:14:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 06:15:02 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.0-rc2/traefik_v2.7.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 06:15:03 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 06:15:03 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:15:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 06:15:04 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 06:15:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6f6a6c77b1bd5dfb3e759efaa292f964f197ae4b96be74d80ef059f87317997a`  
		Last Modified: Mon, 04 Apr 2022 23:42:47 GMT  
		Size: 2.6 MB (2604075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd299e72e5dfb969cf246832a04767813018867ef4e23d3cd39e9ed53fbb2e2`  
		Last Modified: Tue, 05 Apr 2022 06:15:50 GMT  
		Size: 672.5 KB (672500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9565ee21a342064cf700d9474883f1f743b295fc38f1a934caec7c014c19a39`  
		Last Modified: Tue, 05 Apr 2022 06:15:54 GMT  
		Size: 26.4 MB (26376273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0ffd87278d72e40d22211cb05d509dbac1628f7a1a59d0e65d8b8a260db1c3`  
		Last Modified: Tue, 05 Apr 2022 06:15:50 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.7.0-rc2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:fe30fb1edd24cb35ed73084221b49fd145c789c540a1a10e2e76aad943673a66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:2.7.0-rc2-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:b10e4f877aebabb1734135b2646cb64cc5d70727f9964b4b764f6f1e749decc3
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2743448944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf2840916230e28221e266704780ab0cf47a706724fd322280cc72c40af2d0d6`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 29 Mar 2022 19:32:51 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.7.0-rc2/traefik_v2.7.0-rc2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 29 Mar 2022 19:32:52 GMT
EXPOSE 80
# Tue, 29 Mar 2022 19:32:53 GMT
ENTRYPOINT ["/traefik"]
# Tue, 29 Mar 2022 19:32:54 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e322088afb1a013924e6a53963322f66b3b52751ccaeb821099765b4ddc569ae`  
		Last Modified: Tue, 29 Mar 2022 19:35:00 GMT  
		Size: 28.0 MB (27991054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68de6a12e36621523a032635b4054a09a9c5898b8e50c091d7170ca3f0926544`  
		Last Modified: Tue, 29 Mar 2022 19:34:29 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcece30b93b7bbc58f5afe87698f87c2dc34b5aae3311c71ebf03339c1b0fec`  
		Last Modified: Tue, 29 Mar 2022 19:34:29 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99b616e8af959eea48003b4cf3217d9c66250b599e93b4cc5496bfeea62699c`  
		Last Modified: Tue, 29 Mar 2022 19:34:29 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:epoisses`

```console
$ docker pull traefik@sha256:13b2dabb45da3611d756bf9b1e26d8c530e12d6edb6d182fb9cbe4847d552c0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:epoisses` - linux; amd64

```console
$ docker pull traefik@sha256:0f179eab7150d8c8eabd7ca596d98603e420b84c78d0a8023eee1c06ee3ff545
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30884413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a4db61886791f13225c2845cd57d60ff8a5a0720eccb889e7c7341ffe1b9594`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:43:11 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 31 Mar 2022 02:24:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.0-rc2/traefik_v2.7.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 31 Mar 2022 02:24:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 31 Mar 2022 02:24:20 GMT
EXPOSE 80
# Thu, 31 Mar 2022 02:24:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 31 Mar 2022 02:24:20 GMT
CMD ["traefik"]
# Thu, 31 Mar 2022 02:24:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491249faa733d19d2c4f479860df3563c3f269d08d4c70b53926670b486092d5`  
		Last Modified: Tue, 29 Mar 2022 11:44:20 GMT  
		Size: 666.7 KB (666674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150f61256352f339798457a33bd19e97a2c486d649ab99d14e8ccc1b9c0aab4c`  
		Last Modified: Thu, 31 Mar 2022 02:25:02 GMT  
		Size: 27.4 MB (27399018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d9192a4e45679a6fe98f98a61976527914a4344b8b8126ba5e9ae401d7c37c`  
		Last Modified: Thu, 31 Mar 2022 02:24:57 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:epoisses` - linux; arm variant v6

```console
$ docker pull traefik@sha256:1aee5e27fbc6358f097fa0fecd790f97972a5d860b39dd15c5c0746b7cae529a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (28982492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5067b6791686be1a6a27d9bb0fead0ff84404cf74a87b0cb709692e22117837c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:46 GMT
ADD file:9670f4f7de6a9b8eb844e418daedd0dbad90009126790eb65e246b29cac5ea47 in / 
# Tue, 29 Mar 2022 00:49:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 13:21:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 29 Mar 2022 20:14:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.0-rc2/traefik_v2.7.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 29 Mar 2022 20:14:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 29 Mar 2022 20:14:39 GMT
EXPOSE 80
# Tue, 29 Mar 2022 20:14:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 20:14:40 GMT
CMD ["traefik"]
# Tue, 29 Mar 2022 20:14:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79f5c9df0b90097bae07a9861e9e0e3f52a16b0bfde2793c4e14ad033cfb47f4`  
		Last Modified: Tue, 29 Mar 2022 00:51:45 GMT  
		Size: 2.6 MB (2626017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10449722d0e221d9f2d76fded7a3856b1e5da5de38e926c9dbde9dfeb95c67c8`  
		Last Modified: Tue, 29 Mar 2022 13:24:24 GMT  
		Size: 672.5 KB (672526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c35bed17508c434cf42b82887ab060852475c4e374ab4927382d30577e3ff1f`  
		Last Modified: Tue, 29 Mar 2022 20:17:27 GMT  
		Size: 25.7 MB (25683580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db18cf51e2278ee816fbc5b729a8cb8148229542f5993ccef454c8599eb551e`  
		Last Modified: Tue, 29 Mar 2022 20:17:10 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:epoisses` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:cbc72e60f32f55ba66d1a5be7993d663006d2283f3b52202af99971e5c355ea2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28364421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ef4096bf04746212cf88c9a0795877622ff1ba98808ecb03b7ffe933c5ebd46`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:27:04 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 07:27:07 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.0-rc2/traefik_v2.7.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 07:27:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 07:27:08 GMT
EXPOSE 80
# Tue, 05 Apr 2022 07:27:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 07:27:10 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 07:27:11 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:ff858383c840c4b97834e60774329c49bf3fea922085ae31d8165402d4b9f5ea`  
		Last Modified: Tue, 05 Apr 2022 07:28:40 GMT  
		Size: 25.0 MB (24978372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04abccc9cf218d0e24ff784807a2c3570b5ed2a7183fbf08517b4fc4221c813e`  
		Last Modified: Tue, 05 Apr 2022 07:28:36 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:epoisses` - linux; s390x

```console
$ docker pull traefik@sha256:7569039608d54d25f8a85c29da7151f2e16732547c169e96de3d8377bc945831
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29653216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e16a4ac48877da270277f281f90230f4a9638f791a4fe3a5e04e49c9e23235a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:47 GMT
ADD file:0f70e0f0075bee67acb44e5ef01bf6b9df1f69a25b7aa6fd15bd5bb6ec5bcc9f in / 
# Mon, 04 Apr 2022 23:41:48 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:14:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 06:15:02 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.0-rc2/traefik_v2.7.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 06:15:03 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 06:15:03 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:15:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 06:15:04 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 06:15:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6f6a6c77b1bd5dfb3e759efaa292f964f197ae4b96be74d80ef059f87317997a`  
		Last Modified: Mon, 04 Apr 2022 23:42:47 GMT  
		Size: 2.6 MB (2604075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd299e72e5dfb969cf246832a04767813018867ef4e23d3cd39e9ed53fbb2e2`  
		Last Modified: Tue, 05 Apr 2022 06:15:50 GMT  
		Size: 672.5 KB (672500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9565ee21a342064cf700d9474883f1f743b295fc38f1a934caec7c014c19a39`  
		Last Modified: Tue, 05 Apr 2022 06:15:54 GMT  
		Size: 26.4 MB (26376273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0ffd87278d72e40d22211cb05d509dbac1628f7a1a59d0e65d8b8a260db1c3`  
		Last Modified: Tue, 05 Apr 2022 06:15:50 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:epoisses-windowsservercore-1809`

```console
$ docker pull traefik@sha256:fe30fb1edd24cb35ed73084221b49fd145c789c540a1a10e2e76aad943673a66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:epoisses-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:b10e4f877aebabb1734135b2646cb64cc5d70727f9964b4b764f6f1e749decc3
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2743448944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf2840916230e28221e266704780ab0cf47a706724fd322280cc72c40af2d0d6`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 29 Mar 2022 19:32:51 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.7.0-rc2/traefik_v2.7.0-rc2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 29 Mar 2022 19:32:52 GMT
EXPOSE 80
# Tue, 29 Mar 2022 19:32:53 GMT
ENTRYPOINT ["/traefik"]
# Tue, 29 Mar 2022 19:32:54 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e322088afb1a013924e6a53963322f66b3b52751ccaeb821099765b4ddc569ae`  
		Last Modified: Tue, 29 Mar 2022 19:35:00 GMT  
		Size: 28.0 MB (27991054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68de6a12e36621523a032635b4054a09a9c5898b8e50c091d7170ca3f0926544`  
		Last Modified: Tue, 29 Mar 2022 19:34:29 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcece30b93b7bbc58f5afe87698f87c2dc34b5aae3311c71ebf03339c1b0fec`  
		Last Modified: Tue, 29 Mar 2022 19:34:29 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99b616e8af959eea48003b4cf3217d9c66250b599e93b4cc5496bfeea62699c`  
		Last Modified: Tue, 29 Mar 2022 19:34:29 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:67d4020f130982992b0864ad714f90f79c12899229a8573612cb3047dc79a308
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:a1219f2ba73f764ee9c550f3c13045a9264c6b78bdd0b0db6e956a7f96972f48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.3 MB (30339348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3325c6dd7f244fcdc7729819792ee0e0483f58f6ac34baabcd7bd374b7c067e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:43:11 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 31 Mar 2022 02:24:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 31 Mar 2022 02:24:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 31 Mar 2022 02:24:27 GMT
EXPOSE 80
# Thu, 31 Mar 2022 02:24:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 31 Mar 2022 02:24:27 GMT
CMD ["traefik"]
# Thu, 31 Mar 2022 02:24:27 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491249faa733d19d2c4f479860df3563c3f269d08d4c70b53926670b486092d5`  
		Last Modified: Tue, 29 Mar 2022 11:44:20 GMT  
		Size: 666.7 KB (666674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7660e64df1e00fb3bbfae87703ee37e1b01bf9352d6d5bf05dd11b9701a773`  
		Last Modified: Thu, 31 Mar 2022 02:25:23 GMT  
		Size: 26.9 MB (26853953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080a3ffe94e58283fb36ef270c6d19f0ef82fe40354fb2131023d1efbd951592`  
		Last Modified: Thu, 31 Mar 2022 02:25:18 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:2a6e91644420e884a47301e5719349eb6a1c6c36d044c7fcfac6789aeb4b0475
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28508633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53d4c7eeb0769e066b9a8fb8fe3463393dc695230d928b19ddc768a90f265ee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:46 GMT
ADD file:9670f4f7de6a9b8eb844e418daedd0dbad90009126790eb65e246b29cac5ea47 in / 
# Tue, 29 Mar 2022 00:49:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 13:21:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 29 Mar 2022 20:15:02 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 29 Mar 2022 20:15:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 29 Mar 2022 20:15:03 GMT
EXPOSE 80
# Tue, 29 Mar 2022 20:15:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 20:15:04 GMT
CMD ["traefik"]
# Tue, 29 Mar 2022 20:15:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79f5c9df0b90097bae07a9861e9e0e3f52a16b0bfde2793c4e14ad033cfb47f4`  
		Last Modified: Tue, 29 Mar 2022 00:51:45 GMT  
		Size: 2.6 MB (2626017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10449722d0e221d9f2d76fded7a3856b1e5da5de38e926c9dbde9dfeb95c67c8`  
		Last Modified: Tue, 29 Mar 2022 13:24:24 GMT  
		Size: 672.5 KB (672526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b16455b7f19741086604a735e590e982fa72a4f8419eebac2e4b93a6dded9e`  
		Last Modified: Tue, 29 Mar 2022 20:18:07 GMT  
		Size: 25.2 MB (25209721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ea9ec0719c1f9245fcee9072b0a02747793e15bec07885cade6befb6fa13b3`  
		Last Modified: Tue, 29 Mar 2022 20:17:50 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:abcf0f8ace901dc06a7db4b9ab761ed79d084f8a0f1fcb8d5b630fd4b6487bb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27882793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cebe76258a556250464b66a64aa1fe8af5aa375fbf74efa560d5cca5bfe4d84`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:27:04 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 07:27:22 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 07:27:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 07:27:23 GMT
EXPOSE 80
# Tue, 05 Apr 2022 07:27:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 07:27:25 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 07:27:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:1f34d16123c581d2614d26cbcd1618aa3bec385321f1b5d361be3a9d0cf3edd0`  
		Last Modified: Tue, 05 Apr 2022 07:29:03 GMT  
		Size: 24.5 MB (24496745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fb8900c64102e15429a227ea22db387e3f73f305e5b3a07ba46ef030aa6913`  
		Last Modified: Tue, 05 Apr 2022 07:28:59 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; s390x

```console
$ docker pull traefik@sha256:7664483ac7f02aed931da58072699fd842463c6ed0838dd77d1c9063ca373424
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29133529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9effa158d8a7eb4de0dc5ef0f9e5068b916010a030594833ffeee4229ce787`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:47 GMT
ADD file:0f70e0f0075bee67acb44e5ef01bf6b9df1f69a25b7aa6fd15bd5bb6ec5bcc9f in / 
# Mon, 04 Apr 2022 23:41:48 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:14:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 06:15:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 06:15:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 06:15:16 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:15:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 06:15:16 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 06:15:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6f6a6c77b1bd5dfb3e759efaa292f964f197ae4b96be74d80ef059f87317997a`  
		Last Modified: Mon, 04 Apr 2022 23:42:47 GMT  
		Size: 2.6 MB (2604075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd299e72e5dfb969cf246832a04767813018867ef4e23d3cd39e9ed53fbb2e2`  
		Last Modified: Tue, 05 Apr 2022 06:15:50 GMT  
		Size: 672.5 KB (672500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d058aad59a877e33e73441ea4d8bc9339a3cf057ba559b89a6403e9ad67d344`  
		Last Modified: Tue, 05 Apr 2022 06:16:11 GMT  
		Size: 25.9 MB (25856586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b401ac447e5e18e7baee3f9bc3f6e782878325212d2ef6cb51213203f7b7958`  
		Last Modified: Tue, 05 Apr 2022 06:16:07 GMT  
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
$ docker pull traefik@sha256:2536d87a206f10723c87604304bd3355cf36757de6599917cd9e8e77a03ba612
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:00b854b023b6ad2775a64b9a3c191420d2e5ee28902906b6e38ea3db6e9ee826
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25647457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bdaefa287d6893b1f23c7f069a71f95a7d520c4000d37330654a30402867e02`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:43:11 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 29 Mar 2022 11:43:30 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 29 Mar 2022 11:43:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 29 Mar 2022 11:43:31 GMT
EXPOSE 80
# Tue, 29 Mar 2022 11:43:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 11:43:31 GMT
CMD ["traefik"]
# Tue, 29 Mar 2022 11:43:31 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491249faa733d19d2c4f479860df3563c3f269d08d4c70b53926670b486092d5`  
		Last Modified: Tue, 29 Mar 2022 11:44:20 GMT  
		Size: 666.7 KB (666674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa40b07000dff13e47f89c1a98d9c91348c57a3d63e217a6048ca837818b8dfe`  
		Last Modified: Tue, 29 Mar 2022 11:45:06 GMT  
		Size: 22.2 MB (22162061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df6217935f5fada8326229f327ccbf2417b11aa70f4f7d01c3ff7b5c793d747`  
		Last Modified: Tue, 29 Mar 2022 11:45:02 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:faf9be547dc6180e313c055b4a7f2da1a2eb1b4a62f2215ca4712ffbfef5dd83
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23922329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d09ca9a761d0f863bf5aff1b51e985ecf319d9821a5cfd67aadbc17743780b5f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:46 GMT
ADD file:9670f4f7de6a9b8eb844e418daedd0dbad90009126790eb65e246b29cac5ea47 in / 
# Tue, 29 Mar 2022 00:49:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 13:21:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 29 Mar 2022 13:22:23 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 29 Mar 2022 13:22:24 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 29 Mar 2022 13:22:24 GMT
EXPOSE 80
# Tue, 29 Mar 2022 13:22:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 13:22:25 GMT
CMD ["traefik"]
# Tue, 29 Mar 2022 13:22:25 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79f5c9df0b90097bae07a9861e9e0e3f52a16b0bfde2793c4e14ad033cfb47f4`  
		Last Modified: Tue, 29 Mar 2022 00:51:45 GMT  
		Size: 2.6 MB (2626017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10449722d0e221d9f2d76fded7a3856b1e5da5de38e926c9dbde9dfeb95c67c8`  
		Last Modified: Tue, 29 Mar 2022 13:24:24 GMT  
		Size: 672.5 KB (672526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4783ae6cdd5ea4a521c85fdafa8b39c172173886b178ef7c9d456018198f20bc`  
		Last Modified: Tue, 29 Mar 2022 13:26:02 GMT  
		Size: 20.6 MB (20623419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99f4630a8f43bea8e6dd2b3cd39639e77fa3d52cd95e84593a545ddff84bcfe`  
		Last Modified: Tue, 29 Mar 2022 13:25:48 GMT  
		Size: 367.0 B  
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
$ docker pull traefik@sha256:85ffe3d43fd4929a0e48d226e018af240fbbd8ea9a03685f74f1c78c432f85b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:67d210fa3d7dcb1ebc3b3b5f3bfdaac7d18195e1bb2b83fa2c1b1f48d09b08dd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2738303983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6ebd04310fbdd68b4e7225310f8a6f2dec3a0330af0d02b74a9a0e35b79945b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:53:09 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 09 Mar 2022 18:53:10 GMT
EXPOSE 80
# Wed, 09 Mar 2022 18:53:11 GMT
ENTRYPOINT ["/traefik"]
# Wed, 09 Mar 2022 18:53:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd63edc5d2bde654b771ee58c8e9bb78539127758e862053223f402d3eaea68`  
		Last Modified: Wed, 09 Mar 2022 18:54:50 GMT  
		Size: 22.8 MB (22845783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cefe3e1f9703a33ffdf92a9c03b8a4738222fe08ea99aded6416f848aa300e9`  
		Last Modified: Wed, 09 Mar 2022 18:54:27 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939f3b18eb0ddb1cb4c6b01a2abc4127403c6a67c630a8c05c6be5f43ab74acc`  
		Last Modified: Wed, 09 Mar 2022 18:54:26 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bcba10ab84d161e2dc32a48f6bc15da23d8aabdb22bbf4a89499ce18583d46`  
		Last Modified: Wed, 09 Mar 2022 18:54:26 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:rocamadour`

```console
$ docker pull traefik@sha256:67d4020f130982992b0864ad714f90f79c12899229a8573612cb3047dc79a308
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:rocamadour` - linux; amd64

```console
$ docker pull traefik@sha256:a1219f2ba73f764ee9c550f3c13045a9264c6b78bdd0b0db6e956a7f96972f48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.3 MB (30339348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3325c6dd7f244fcdc7729819792ee0e0483f58f6ac34baabcd7bd374b7c067e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:43:11 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 31 Mar 2022 02:24:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 31 Mar 2022 02:24:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 31 Mar 2022 02:24:27 GMT
EXPOSE 80
# Thu, 31 Mar 2022 02:24:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 31 Mar 2022 02:24:27 GMT
CMD ["traefik"]
# Thu, 31 Mar 2022 02:24:27 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491249faa733d19d2c4f479860df3563c3f269d08d4c70b53926670b486092d5`  
		Last Modified: Tue, 29 Mar 2022 11:44:20 GMT  
		Size: 666.7 KB (666674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7660e64df1e00fb3bbfae87703ee37e1b01bf9352d6d5bf05dd11b9701a773`  
		Last Modified: Thu, 31 Mar 2022 02:25:23 GMT  
		Size: 26.9 MB (26853953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080a3ffe94e58283fb36ef270c6d19f0ef82fe40354fb2131023d1efbd951592`  
		Last Modified: Thu, 31 Mar 2022 02:25:18 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:rocamadour` - linux; arm variant v6

```console
$ docker pull traefik@sha256:2a6e91644420e884a47301e5719349eb6a1c6c36d044c7fcfac6789aeb4b0475
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28508633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53d4c7eeb0769e066b9a8fb8fe3463393dc695230d928b19ddc768a90f265ee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:46 GMT
ADD file:9670f4f7de6a9b8eb844e418daedd0dbad90009126790eb65e246b29cac5ea47 in / 
# Tue, 29 Mar 2022 00:49:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 13:21:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 29 Mar 2022 20:15:02 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 29 Mar 2022 20:15:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 29 Mar 2022 20:15:03 GMT
EXPOSE 80
# Tue, 29 Mar 2022 20:15:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 20:15:04 GMT
CMD ["traefik"]
# Tue, 29 Mar 2022 20:15:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79f5c9df0b90097bae07a9861e9e0e3f52a16b0bfde2793c4e14ad033cfb47f4`  
		Last Modified: Tue, 29 Mar 2022 00:51:45 GMT  
		Size: 2.6 MB (2626017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10449722d0e221d9f2d76fded7a3856b1e5da5de38e926c9dbde9dfeb95c67c8`  
		Last Modified: Tue, 29 Mar 2022 13:24:24 GMT  
		Size: 672.5 KB (672526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b16455b7f19741086604a735e590e982fa72a4f8419eebac2e4b93a6dded9e`  
		Last Modified: Tue, 29 Mar 2022 20:18:07 GMT  
		Size: 25.2 MB (25209721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ea9ec0719c1f9245fcee9072b0a02747793e15bec07885cade6befb6fa13b3`  
		Last Modified: Tue, 29 Mar 2022 20:17:50 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:rocamadour` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:abcf0f8ace901dc06a7db4b9ab761ed79d084f8a0f1fcb8d5b630fd4b6487bb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27882793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cebe76258a556250464b66a64aa1fe8af5aa375fbf74efa560d5cca5bfe4d84`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:27:04 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 07:27:22 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 07:27:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 07:27:23 GMT
EXPOSE 80
# Tue, 05 Apr 2022 07:27:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 07:27:25 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 07:27:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:1f34d16123c581d2614d26cbcd1618aa3bec385321f1b5d361be3a9d0cf3edd0`  
		Last Modified: Tue, 05 Apr 2022 07:29:03 GMT  
		Size: 24.5 MB (24496745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fb8900c64102e15429a227ea22db387e3f73f305e5b3a07ba46ef030aa6913`  
		Last Modified: Tue, 05 Apr 2022 07:28:59 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:rocamadour` - linux; s390x

```console
$ docker pull traefik@sha256:7664483ac7f02aed931da58072699fd842463c6ed0838dd77d1c9063ca373424
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29133529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9effa158d8a7eb4de0dc5ef0f9e5068b916010a030594833ffeee4229ce787`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:47 GMT
ADD file:0f70e0f0075bee67acb44e5ef01bf6b9df1f69a25b7aa6fd15bd5bb6ec5bcc9f in / 
# Mon, 04 Apr 2022 23:41:48 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:14:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 06:15:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 06:15:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 06:15:16 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:15:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 06:15:16 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 06:15:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6f6a6c77b1bd5dfb3e759efaa292f964f197ae4b96be74d80ef059f87317997a`  
		Last Modified: Mon, 04 Apr 2022 23:42:47 GMT  
		Size: 2.6 MB (2604075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd299e72e5dfb969cf246832a04767813018867ef4e23d3cd39e9ed53fbb2e2`  
		Last Modified: Tue, 05 Apr 2022 06:15:50 GMT  
		Size: 672.5 KB (672500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d058aad59a877e33e73441ea4d8bc9339a3cf057ba559b89a6403e9ad67d344`  
		Last Modified: Tue, 05 Apr 2022 06:16:11 GMT  
		Size: 25.9 MB (25856586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b401ac447e5e18e7baee3f9bc3f6e782878325212d2ef6cb51213203f7b7958`  
		Last Modified: Tue, 05 Apr 2022 06:16:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:rocamadour-windowsservercore-1809`

```console
$ docker pull traefik@sha256:8c6d3723194f2b09c6b7e6f1c65c00573ed8a86fb030871f472f15b7f68b6ff2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:rocamadour-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:47d24eaf1b6b706e5de58ce11e2cbebf3a0f9575a61fec03a4c861e4438807a9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2742898776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5706e325ee2ad18345e4fe2fd1dc42a027366b1f9c1ddfc6a3e3542f918ece9c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 29 Mar 2022 19:33:53 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 29 Mar 2022 19:33:54 GMT
EXPOSE 80
# Tue, 29 Mar 2022 19:33:55 GMT
ENTRYPOINT ["/traefik"]
# Tue, 29 Mar 2022 19:33:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a79b9a00328456358c525859928802742529204e1d520ec9f3f68f3fe63ee9`  
		Last Modified: Tue, 29 Mar 2022 19:35:24 GMT  
		Size: 27.4 MB (27440577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfbef29f86d1cb8156adb9e83f62919091b87ae19d8b49027e53e32207378a1`  
		Last Modified: Tue, 29 Mar 2022 19:35:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81861a2761b14e5cf1801456272bdb3de1fc16f0d8724c6df47a371f20478091`  
		Last Modified: Tue, 29 Mar 2022 19:35:17 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779ed28a5abfc5c391b359a30b2b6fccee48c70fdc42d2a44a77a31b1d4c3e4d`  
		Last Modified: Tue, 29 Mar 2022 19:35:17 GMT  
		Size: 1.4 KB (1435 bytes)  
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
$ docker pull traefik@sha256:2536d87a206f10723c87604304bd3355cf36757de6599917cd9e8e77a03ba612
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:00b854b023b6ad2775a64b9a3c191420d2e5ee28902906b6e38ea3db6e9ee826
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25647457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bdaefa287d6893b1f23c7f069a71f95a7d520c4000d37330654a30402867e02`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:43:11 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 29 Mar 2022 11:43:30 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 29 Mar 2022 11:43:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 29 Mar 2022 11:43:31 GMT
EXPOSE 80
# Tue, 29 Mar 2022 11:43:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 11:43:31 GMT
CMD ["traefik"]
# Tue, 29 Mar 2022 11:43:31 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491249faa733d19d2c4f479860df3563c3f269d08d4c70b53926670b486092d5`  
		Last Modified: Tue, 29 Mar 2022 11:44:20 GMT  
		Size: 666.7 KB (666674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa40b07000dff13e47f89c1a98d9c91348c57a3d63e217a6048ca837818b8dfe`  
		Last Modified: Tue, 29 Mar 2022 11:45:06 GMT  
		Size: 22.2 MB (22162061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df6217935f5fada8326229f327ccbf2417b11aa70f4f7d01c3ff7b5c793d747`  
		Last Modified: Tue, 29 Mar 2022 11:45:02 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:faf9be547dc6180e313c055b4a7f2da1a2eb1b4a62f2215ca4712ffbfef5dd83
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23922329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d09ca9a761d0f863bf5aff1b51e985ecf319d9821a5cfd67aadbc17743780b5f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:46 GMT
ADD file:9670f4f7de6a9b8eb844e418daedd0dbad90009126790eb65e246b29cac5ea47 in / 
# Tue, 29 Mar 2022 00:49:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 13:21:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 29 Mar 2022 13:22:23 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 29 Mar 2022 13:22:24 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 29 Mar 2022 13:22:24 GMT
EXPOSE 80
# Tue, 29 Mar 2022 13:22:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 13:22:25 GMT
CMD ["traefik"]
# Tue, 29 Mar 2022 13:22:25 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79f5c9df0b90097bae07a9861e9e0e3f52a16b0bfde2793c4e14ad033cfb47f4`  
		Last Modified: Tue, 29 Mar 2022 00:51:45 GMT  
		Size: 2.6 MB (2626017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10449722d0e221d9f2d76fded7a3856b1e5da5de38e926c9dbde9dfeb95c67c8`  
		Last Modified: Tue, 29 Mar 2022 13:24:24 GMT  
		Size: 672.5 KB (672526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4783ae6cdd5ea4a521c85fdafa8b39c172173886b178ef7c9d456018198f20bc`  
		Last Modified: Tue, 29 Mar 2022 13:26:02 GMT  
		Size: 20.6 MB (20623419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99f4630a8f43bea8e6dd2b3cd39639e77fa3d52cd95e84593a545ddff84bcfe`  
		Last Modified: Tue, 29 Mar 2022 13:25:48 GMT  
		Size: 367.0 B  
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
$ docker pull traefik@sha256:85ffe3d43fd4929a0e48d226e018af240fbbd8ea9a03685f74f1c78c432f85b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:v1.7-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:67d210fa3d7dcb1ebc3b3b5f3bfdaac7d18195e1bb2b83fa2c1b1f48d09b08dd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2738303983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6ebd04310fbdd68b4e7225310f8a6f2dec3a0330af0d02b74a9a0e35b79945b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:53:09 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 09 Mar 2022 18:53:10 GMT
EXPOSE 80
# Wed, 09 Mar 2022 18:53:11 GMT
ENTRYPOINT ["/traefik"]
# Wed, 09 Mar 2022 18:53:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd63edc5d2bde654b771ee58c8e9bb78539127758e862053223f402d3eaea68`  
		Last Modified: Wed, 09 Mar 2022 18:54:50 GMT  
		Size: 22.8 MB (22845783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cefe3e1f9703a33ffdf92a9c03b8a4738222fe08ea99aded6416f848aa300e9`  
		Last Modified: Wed, 09 Mar 2022 18:54:27 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939f3b18eb0ddb1cb4c6b01a2abc4127403c6a67c630a8c05c6be5f43ab74acc`  
		Last Modified: Wed, 09 Mar 2022 18:54:26 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bcba10ab84d161e2dc32a48f6bc15da23d8aabdb22bbf4a89499ce18583d46`  
		Last Modified: Wed, 09 Mar 2022 18:54:26 GMT  
		Size: 1.4 KB (1389 bytes)  
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
$ docker pull traefik@sha256:2536d87a206f10723c87604304bd3355cf36757de6599917cd9e8e77a03ba612
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.34-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:00b854b023b6ad2775a64b9a3c191420d2e5ee28902906b6e38ea3db6e9ee826
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25647457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bdaefa287d6893b1f23c7f069a71f95a7d520c4000d37330654a30402867e02`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:43:11 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 29 Mar 2022 11:43:30 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 29 Mar 2022 11:43:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 29 Mar 2022 11:43:31 GMT
EXPOSE 80
# Tue, 29 Mar 2022 11:43:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 11:43:31 GMT
CMD ["traefik"]
# Tue, 29 Mar 2022 11:43:31 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491249faa733d19d2c4f479860df3563c3f269d08d4c70b53926670b486092d5`  
		Last Modified: Tue, 29 Mar 2022 11:44:20 GMT  
		Size: 666.7 KB (666674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa40b07000dff13e47f89c1a98d9c91348c57a3d63e217a6048ca837818b8dfe`  
		Last Modified: Tue, 29 Mar 2022 11:45:06 GMT  
		Size: 22.2 MB (22162061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df6217935f5fada8326229f327ccbf2417b11aa70f4f7d01c3ff7b5c793d747`  
		Last Modified: Tue, 29 Mar 2022 11:45:02 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.34-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:faf9be547dc6180e313c055b4a7f2da1a2eb1b4a62f2215ca4712ffbfef5dd83
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23922329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d09ca9a761d0f863bf5aff1b51e985ecf319d9821a5cfd67aadbc17743780b5f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:46 GMT
ADD file:9670f4f7de6a9b8eb844e418daedd0dbad90009126790eb65e246b29cac5ea47 in / 
# Tue, 29 Mar 2022 00:49:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 13:21:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 29 Mar 2022 13:22:23 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 29 Mar 2022 13:22:24 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 29 Mar 2022 13:22:24 GMT
EXPOSE 80
# Tue, 29 Mar 2022 13:22:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 13:22:25 GMT
CMD ["traefik"]
# Tue, 29 Mar 2022 13:22:25 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79f5c9df0b90097bae07a9861e9e0e3f52a16b0bfde2793c4e14ad033cfb47f4`  
		Last Modified: Tue, 29 Mar 2022 00:51:45 GMT  
		Size: 2.6 MB (2626017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10449722d0e221d9f2d76fded7a3856b1e5da5de38e926c9dbde9dfeb95c67c8`  
		Last Modified: Tue, 29 Mar 2022 13:24:24 GMT  
		Size: 672.5 KB (672526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4783ae6cdd5ea4a521c85fdafa8b39c172173886b178ef7c9d456018198f20bc`  
		Last Modified: Tue, 29 Mar 2022 13:26:02 GMT  
		Size: 20.6 MB (20623419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99f4630a8f43bea8e6dd2b3cd39639e77fa3d52cd95e84593a545ddff84bcfe`  
		Last Modified: Tue, 29 Mar 2022 13:25:48 GMT  
		Size: 367.0 B  
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
$ docker pull traefik@sha256:85ffe3d43fd4929a0e48d226e018af240fbbd8ea9a03685f74f1c78c432f85b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:v1.7.34-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:67d210fa3d7dcb1ebc3b3b5f3bfdaac7d18195e1bb2b83fa2c1b1f48d09b08dd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2738303983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6ebd04310fbdd68b4e7225310f8a6f2dec3a0330af0d02b74a9a0e35b79945b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:53:09 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 09 Mar 2022 18:53:10 GMT
EXPOSE 80
# Wed, 09 Mar 2022 18:53:11 GMT
ENTRYPOINT ["/traefik"]
# Wed, 09 Mar 2022 18:53:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd63edc5d2bde654b771ee58c8e9bb78539127758e862053223f402d3eaea68`  
		Last Modified: Wed, 09 Mar 2022 18:54:50 GMT  
		Size: 22.8 MB (22845783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cefe3e1f9703a33ffdf92a9c03b8a4738222fe08ea99aded6416f848aa300e9`  
		Last Modified: Wed, 09 Mar 2022 18:54:27 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939f3b18eb0ddb1cb4c6b01a2abc4127403c6a67c630a8c05c6be5f43ab74acc`  
		Last Modified: Wed, 09 Mar 2022 18:54:26 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bcba10ab84d161e2dc32a48f6bc15da23d8aabdb22bbf4a89499ce18583d46`  
		Last Modified: Wed, 09 Mar 2022 18:54:26 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.6`

```console
$ docker pull traefik@sha256:67d4020f130982992b0864ad714f90f79c12899229a8573612cb3047dc79a308
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.6` - linux; amd64

```console
$ docker pull traefik@sha256:a1219f2ba73f764ee9c550f3c13045a9264c6b78bdd0b0db6e956a7f96972f48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.3 MB (30339348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3325c6dd7f244fcdc7729819792ee0e0483f58f6ac34baabcd7bd374b7c067e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:43:11 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 31 Mar 2022 02:24:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 31 Mar 2022 02:24:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 31 Mar 2022 02:24:27 GMT
EXPOSE 80
# Thu, 31 Mar 2022 02:24:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 31 Mar 2022 02:24:27 GMT
CMD ["traefik"]
# Thu, 31 Mar 2022 02:24:27 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491249faa733d19d2c4f479860df3563c3f269d08d4c70b53926670b486092d5`  
		Last Modified: Tue, 29 Mar 2022 11:44:20 GMT  
		Size: 666.7 KB (666674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7660e64df1e00fb3bbfae87703ee37e1b01bf9352d6d5bf05dd11b9701a773`  
		Last Modified: Thu, 31 Mar 2022 02:25:23 GMT  
		Size: 26.9 MB (26853953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080a3ffe94e58283fb36ef270c6d19f0ef82fe40354fb2131023d1efbd951592`  
		Last Modified: Thu, 31 Mar 2022 02:25:18 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.6` - linux; arm variant v6

```console
$ docker pull traefik@sha256:2a6e91644420e884a47301e5719349eb6a1c6c36d044c7fcfac6789aeb4b0475
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28508633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53d4c7eeb0769e066b9a8fb8fe3463393dc695230d928b19ddc768a90f265ee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:46 GMT
ADD file:9670f4f7de6a9b8eb844e418daedd0dbad90009126790eb65e246b29cac5ea47 in / 
# Tue, 29 Mar 2022 00:49:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 13:21:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 29 Mar 2022 20:15:02 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 29 Mar 2022 20:15:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 29 Mar 2022 20:15:03 GMT
EXPOSE 80
# Tue, 29 Mar 2022 20:15:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 20:15:04 GMT
CMD ["traefik"]
# Tue, 29 Mar 2022 20:15:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79f5c9df0b90097bae07a9861e9e0e3f52a16b0bfde2793c4e14ad033cfb47f4`  
		Last Modified: Tue, 29 Mar 2022 00:51:45 GMT  
		Size: 2.6 MB (2626017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10449722d0e221d9f2d76fded7a3856b1e5da5de38e926c9dbde9dfeb95c67c8`  
		Last Modified: Tue, 29 Mar 2022 13:24:24 GMT  
		Size: 672.5 KB (672526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b16455b7f19741086604a735e590e982fa72a4f8419eebac2e4b93a6dded9e`  
		Last Modified: Tue, 29 Mar 2022 20:18:07 GMT  
		Size: 25.2 MB (25209721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ea9ec0719c1f9245fcee9072b0a02747793e15bec07885cade6befb6fa13b3`  
		Last Modified: Tue, 29 Mar 2022 20:17:50 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.6` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:abcf0f8ace901dc06a7db4b9ab761ed79d084f8a0f1fcb8d5b630fd4b6487bb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27882793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cebe76258a556250464b66a64aa1fe8af5aa375fbf74efa560d5cca5bfe4d84`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:27:04 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 07:27:22 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 07:27:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 07:27:23 GMT
EXPOSE 80
# Tue, 05 Apr 2022 07:27:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 07:27:25 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 07:27:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:1f34d16123c581d2614d26cbcd1618aa3bec385321f1b5d361be3a9d0cf3edd0`  
		Last Modified: Tue, 05 Apr 2022 07:29:03 GMT  
		Size: 24.5 MB (24496745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fb8900c64102e15429a227ea22db387e3f73f305e5b3a07ba46ef030aa6913`  
		Last Modified: Tue, 05 Apr 2022 07:28:59 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.6` - linux; s390x

```console
$ docker pull traefik@sha256:7664483ac7f02aed931da58072699fd842463c6ed0838dd77d1c9063ca373424
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29133529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9effa158d8a7eb4de0dc5ef0f9e5068b916010a030594833ffeee4229ce787`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:47 GMT
ADD file:0f70e0f0075bee67acb44e5ef01bf6b9df1f69a25b7aa6fd15bd5bb6ec5bcc9f in / 
# Mon, 04 Apr 2022 23:41:48 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:14:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 06:15:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 06:15:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 06:15:16 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:15:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 06:15:16 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 06:15:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6f6a6c77b1bd5dfb3e759efaa292f964f197ae4b96be74d80ef059f87317997a`  
		Last Modified: Mon, 04 Apr 2022 23:42:47 GMT  
		Size: 2.6 MB (2604075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd299e72e5dfb969cf246832a04767813018867ef4e23d3cd39e9ed53fbb2e2`  
		Last Modified: Tue, 05 Apr 2022 06:15:50 GMT  
		Size: 672.5 KB (672500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d058aad59a877e33e73441ea4d8bc9339a3cf057ba559b89a6403e9ad67d344`  
		Last Modified: Tue, 05 Apr 2022 06:16:11 GMT  
		Size: 25.9 MB (25856586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b401ac447e5e18e7baee3f9bc3f6e782878325212d2ef6cb51213203f7b7958`  
		Last Modified: Tue, 05 Apr 2022 06:16:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.6-windowsservercore-1809`

```console
$ docker pull traefik@sha256:8c6d3723194f2b09c6b7e6f1c65c00573ed8a86fb030871f472f15b7f68b6ff2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:v2.6-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:47d24eaf1b6b706e5de58ce11e2cbebf3a0f9575a61fec03a4c861e4438807a9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2742898776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5706e325ee2ad18345e4fe2fd1dc42a027366b1f9c1ddfc6a3e3542f918ece9c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 29 Mar 2022 19:33:53 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 29 Mar 2022 19:33:54 GMT
EXPOSE 80
# Tue, 29 Mar 2022 19:33:55 GMT
ENTRYPOINT ["/traefik"]
# Tue, 29 Mar 2022 19:33:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a79b9a00328456358c525859928802742529204e1d520ec9f3f68f3fe63ee9`  
		Last Modified: Tue, 29 Mar 2022 19:35:24 GMT  
		Size: 27.4 MB (27440577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfbef29f86d1cb8156adb9e83f62919091b87ae19d8b49027e53e32207378a1`  
		Last Modified: Tue, 29 Mar 2022 19:35:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81861a2761b14e5cf1801456272bdb3de1fc16f0d8724c6df47a371f20478091`  
		Last Modified: Tue, 29 Mar 2022 19:35:17 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779ed28a5abfc5c391b359a30b2b6fccee48c70fdc42d2a44a77a31b1d4c3e4d`  
		Last Modified: Tue, 29 Mar 2022 19:35:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.6.3`

```console
$ docker pull traefik@sha256:67d4020f130982992b0864ad714f90f79c12899229a8573612cb3047dc79a308
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.6.3` - linux; amd64

```console
$ docker pull traefik@sha256:a1219f2ba73f764ee9c550f3c13045a9264c6b78bdd0b0db6e956a7f96972f48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.3 MB (30339348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3325c6dd7f244fcdc7729819792ee0e0483f58f6ac34baabcd7bd374b7c067e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:43:11 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 31 Mar 2022 02:24:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 31 Mar 2022 02:24:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 31 Mar 2022 02:24:27 GMT
EXPOSE 80
# Thu, 31 Mar 2022 02:24:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 31 Mar 2022 02:24:27 GMT
CMD ["traefik"]
# Thu, 31 Mar 2022 02:24:27 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491249faa733d19d2c4f479860df3563c3f269d08d4c70b53926670b486092d5`  
		Last Modified: Tue, 29 Mar 2022 11:44:20 GMT  
		Size: 666.7 KB (666674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7660e64df1e00fb3bbfae87703ee37e1b01bf9352d6d5bf05dd11b9701a773`  
		Last Modified: Thu, 31 Mar 2022 02:25:23 GMT  
		Size: 26.9 MB (26853953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080a3ffe94e58283fb36ef270c6d19f0ef82fe40354fb2131023d1efbd951592`  
		Last Modified: Thu, 31 Mar 2022 02:25:18 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.6.3` - linux; arm variant v6

```console
$ docker pull traefik@sha256:2a6e91644420e884a47301e5719349eb6a1c6c36d044c7fcfac6789aeb4b0475
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28508633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53d4c7eeb0769e066b9a8fb8fe3463393dc695230d928b19ddc768a90f265ee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:46 GMT
ADD file:9670f4f7de6a9b8eb844e418daedd0dbad90009126790eb65e246b29cac5ea47 in / 
# Tue, 29 Mar 2022 00:49:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 13:21:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 29 Mar 2022 20:15:02 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 29 Mar 2022 20:15:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 29 Mar 2022 20:15:03 GMT
EXPOSE 80
# Tue, 29 Mar 2022 20:15:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 20:15:04 GMT
CMD ["traefik"]
# Tue, 29 Mar 2022 20:15:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79f5c9df0b90097bae07a9861e9e0e3f52a16b0bfde2793c4e14ad033cfb47f4`  
		Last Modified: Tue, 29 Mar 2022 00:51:45 GMT  
		Size: 2.6 MB (2626017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10449722d0e221d9f2d76fded7a3856b1e5da5de38e926c9dbde9dfeb95c67c8`  
		Last Modified: Tue, 29 Mar 2022 13:24:24 GMT  
		Size: 672.5 KB (672526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b16455b7f19741086604a735e590e982fa72a4f8419eebac2e4b93a6dded9e`  
		Last Modified: Tue, 29 Mar 2022 20:18:07 GMT  
		Size: 25.2 MB (25209721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ea9ec0719c1f9245fcee9072b0a02747793e15bec07885cade6befb6fa13b3`  
		Last Modified: Tue, 29 Mar 2022 20:17:50 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.6.3` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:abcf0f8ace901dc06a7db4b9ab761ed79d084f8a0f1fcb8d5b630fd4b6487bb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27882793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cebe76258a556250464b66a64aa1fe8af5aa375fbf74efa560d5cca5bfe4d84`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:27:04 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 07:27:22 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 07:27:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 07:27:23 GMT
EXPOSE 80
# Tue, 05 Apr 2022 07:27:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 07:27:25 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 07:27:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:1f34d16123c581d2614d26cbcd1618aa3bec385321f1b5d361be3a9d0cf3edd0`  
		Last Modified: Tue, 05 Apr 2022 07:29:03 GMT  
		Size: 24.5 MB (24496745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fb8900c64102e15429a227ea22db387e3f73f305e5b3a07ba46ef030aa6913`  
		Last Modified: Tue, 05 Apr 2022 07:28:59 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.6.3` - linux; s390x

```console
$ docker pull traefik@sha256:7664483ac7f02aed931da58072699fd842463c6ed0838dd77d1c9063ca373424
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29133529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9effa158d8a7eb4de0dc5ef0f9e5068b916010a030594833ffeee4229ce787`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:47 GMT
ADD file:0f70e0f0075bee67acb44e5ef01bf6b9df1f69a25b7aa6fd15bd5bb6ec5bcc9f in / 
# Mon, 04 Apr 2022 23:41:48 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:14:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 06:15:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 06:15:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 06:15:16 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:15:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 06:15:16 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 06:15:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6f6a6c77b1bd5dfb3e759efaa292f964f197ae4b96be74d80ef059f87317997a`  
		Last Modified: Mon, 04 Apr 2022 23:42:47 GMT  
		Size: 2.6 MB (2604075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd299e72e5dfb969cf246832a04767813018867ef4e23d3cd39e9ed53fbb2e2`  
		Last Modified: Tue, 05 Apr 2022 06:15:50 GMT  
		Size: 672.5 KB (672500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d058aad59a877e33e73441ea4d8bc9339a3cf057ba559b89a6403e9ad67d344`  
		Last Modified: Tue, 05 Apr 2022 06:16:11 GMT  
		Size: 25.9 MB (25856586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b401ac447e5e18e7baee3f9bc3f6e782878325212d2ef6cb51213203f7b7958`  
		Last Modified: Tue, 05 Apr 2022 06:16:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.6.3-windowsservercore-1809`

```console
$ docker pull traefik@sha256:8c6d3723194f2b09c6b7e6f1c65c00573ed8a86fb030871f472f15b7f68b6ff2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:v2.6.3-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:47d24eaf1b6b706e5de58ce11e2cbebf3a0f9575a61fec03a4c861e4438807a9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2742898776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5706e325ee2ad18345e4fe2fd1dc42a027366b1f9c1ddfc6a3e3542f918ece9c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 29 Mar 2022 19:33:53 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 29 Mar 2022 19:33:54 GMT
EXPOSE 80
# Tue, 29 Mar 2022 19:33:55 GMT
ENTRYPOINT ["/traefik"]
# Tue, 29 Mar 2022 19:33:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a79b9a00328456358c525859928802742529204e1d520ec9f3f68f3fe63ee9`  
		Last Modified: Tue, 29 Mar 2022 19:35:24 GMT  
		Size: 27.4 MB (27440577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfbef29f86d1cb8156adb9e83f62919091b87ae19d8b49027e53e32207378a1`  
		Last Modified: Tue, 29 Mar 2022 19:35:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81861a2761b14e5cf1801456272bdb3de1fc16f0d8724c6df47a371f20478091`  
		Last Modified: Tue, 29 Mar 2022 19:35:17 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779ed28a5abfc5c391b359a30b2b6fccee48c70fdc42d2a44a77a31b1d4c3e4d`  
		Last Modified: Tue, 29 Mar 2022 19:35:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.7`

```console
$ docker pull traefik@sha256:13b2dabb45da3611d756bf9b1e26d8c530e12d6edb6d182fb9cbe4847d552c0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.7` - linux; amd64

```console
$ docker pull traefik@sha256:0f179eab7150d8c8eabd7ca596d98603e420b84c78d0a8023eee1c06ee3ff545
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30884413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a4db61886791f13225c2845cd57d60ff8a5a0720eccb889e7c7341ffe1b9594`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:43:11 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 31 Mar 2022 02:24:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.0-rc2/traefik_v2.7.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 31 Mar 2022 02:24:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 31 Mar 2022 02:24:20 GMT
EXPOSE 80
# Thu, 31 Mar 2022 02:24:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 31 Mar 2022 02:24:20 GMT
CMD ["traefik"]
# Thu, 31 Mar 2022 02:24:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491249faa733d19d2c4f479860df3563c3f269d08d4c70b53926670b486092d5`  
		Last Modified: Tue, 29 Mar 2022 11:44:20 GMT  
		Size: 666.7 KB (666674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150f61256352f339798457a33bd19e97a2c486d649ab99d14e8ccc1b9c0aab4c`  
		Last Modified: Thu, 31 Mar 2022 02:25:02 GMT  
		Size: 27.4 MB (27399018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d9192a4e45679a6fe98f98a61976527914a4344b8b8126ba5e9ae401d7c37c`  
		Last Modified: Thu, 31 Mar 2022 02:24:57 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:1aee5e27fbc6358f097fa0fecd790f97972a5d860b39dd15c5c0746b7cae529a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (28982492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5067b6791686be1a6a27d9bb0fead0ff84404cf74a87b0cb709692e22117837c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:46 GMT
ADD file:9670f4f7de6a9b8eb844e418daedd0dbad90009126790eb65e246b29cac5ea47 in / 
# Tue, 29 Mar 2022 00:49:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 13:21:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 29 Mar 2022 20:14:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.0-rc2/traefik_v2.7.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 29 Mar 2022 20:14:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 29 Mar 2022 20:14:39 GMT
EXPOSE 80
# Tue, 29 Mar 2022 20:14:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 20:14:40 GMT
CMD ["traefik"]
# Tue, 29 Mar 2022 20:14:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79f5c9df0b90097bae07a9861e9e0e3f52a16b0bfde2793c4e14ad033cfb47f4`  
		Last Modified: Tue, 29 Mar 2022 00:51:45 GMT  
		Size: 2.6 MB (2626017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10449722d0e221d9f2d76fded7a3856b1e5da5de38e926c9dbde9dfeb95c67c8`  
		Last Modified: Tue, 29 Mar 2022 13:24:24 GMT  
		Size: 672.5 KB (672526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c35bed17508c434cf42b82887ab060852475c4e374ab4927382d30577e3ff1f`  
		Last Modified: Tue, 29 Mar 2022 20:17:27 GMT  
		Size: 25.7 MB (25683580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db18cf51e2278ee816fbc5b729a8cb8148229542f5993ccef454c8599eb551e`  
		Last Modified: Tue, 29 Mar 2022 20:17:10 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:cbc72e60f32f55ba66d1a5be7993d663006d2283f3b52202af99971e5c355ea2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28364421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ef4096bf04746212cf88c9a0795877622ff1ba98808ecb03b7ffe933c5ebd46`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:27:04 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 07:27:07 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.0-rc2/traefik_v2.7.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 07:27:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 07:27:08 GMT
EXPOSE 80
# Tue, 05 Apr 2022 07:27:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 07:27:10 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 07:27:11 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:ff858383c840c4b97834e60774329c49bf3fea922085ae31d8165402d4b9f5ea`  
		Last Modified: Tue, 05 Apr 2022 07:28:40 GMT  
		Size: 25.0 MB (24978372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04abccc9cf218d0e24ff784807a2c3570b5ed2a7183fbf08517b4fc4221c813e`  
		Last Modified: Tue, 05 Apr 2022 07:28:36 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.7` - linux; s390x

```console
$ docker pull traefik@sha256:7569039608d54d25f8a85c29da7151f2e16732547c169e96de3d8377bc945831
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29653216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e16a4ac48877da270277f281f90230f4a9638f791a4fe3a5e04e49c9e23235a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:47 GMT
ADD file:0f70e0f0075bee67acb44e5ef01bf6b9df1f69a25b7aa6fd15bd5bb6ec5bcc9f in / 
# Mon, 04 Apr 2022 23:41:48 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:14:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 06:15:02 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.0-rc2/traefik_v2.7.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 06:15:03 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 06:15:03 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:15:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 06:15:04 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 06:15:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6f6a6c77b1bd5dfb3e759efaa292f964f197ae4b96be74d80ef059f87317997a`  
		Last Modified: Mon, 04 Apr 2022 23:42:47 GMT  
		Size: 2.6 MB (2604075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd299e72e5dfb969cf246832a04767813018867ef4e23d3cd39e9ed53fbb2e2`  
		Last Modified: Tue, 05 Apr 2022 06:15:50 GMT  
		Size: 672.5 KB (672500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9565ee21a342064cf700d9474883f1f743b295fc38f1a934caec7c014c19a39`  
		Last Modified: Tue, 05 Apr 2022 06:15:54 GMT  
		Size: 26.4 MB (26376273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0ffd87278d72e40d22211cb05d509dbac1628f7a1a59d0e65d8b8a260db1c3`  
		Last Modified: Tue, 05 Apr 2022 06:15:50 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:fe30fb1edd24cb35ed73084221b49fd145c789c540a1a10e2e76aad943673a66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:v2.7-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:b10e4f877aebabb1734135b2646cb64cc5d70727f9964b4b764f6f1e749decc3
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2743448944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf2840916230e28221e266704780ab0cf47a706724fd322280cc72c40af2d0d6`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 29 Mar 2022 19:32:51 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.7.0-rc2/traefik_v2.7.0-rc2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 29 Mar 2022 19:32:52 GMT
EXPOSE 80
# Tue, 29 Mar 2022 19:32:53 GMT
ENTRYPOINT ["/traefik"]
# Tue, 29 Mar 2022 19:32:54 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e322088afb1a013924e6a53963322f66b3b52751ccaeb821099765b4ddc569ae`  
		Last Modified: Tue, 29 Mar 2022 19:35:00 GMT  
		Size: 28.0 MB (27991054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68de6a12e36621523a032635b4054a09a9c5898b8e50c091d7170ca3f0926544`  
		Last Modified: Tue, 29 Mar 2022 19:34:29 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcece30b93b7bbc58f5afe87698f87c2dc34b5aae3311c71ebf03339c1b0fec`  
		Last Modified: Tue, 29 Mar 2022 19:34:29 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99b616e8af959eea48003b4cf3217d9c66250b599e93b4cc5496bfeea62699c`  
		Last Modified: Tue, 29 Mar 2022 19:34:29 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.7.0-rc2`

```console
$ docker pull traefik@sha256:13b2dabb45da3611d756bf9b1e26d8c530e12d6edb6d182fb9cbe4847d552c0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.7.0-rc2` - linux; amd64

```console
$ docker pull traefik@sha256:0f179eab7150d8c8eabd7ca596d98603e420b84c78d0a8023eee1c06ee3ff545
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30884413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a4db61886791f13225c2845cd57d60ff8a5a0720eccb889e7c7341ffe1b9594`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:43:11 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 31 Mar 2022 02:24:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.0-rc2/traefik_v2.7.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 31 Mar 2022 02:24:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 31 Mar 2022 02:24:20 GMT
EXPOSE 80
# Thu, 31 Mar 2022 02:24:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 31 Mar 2022 02:24:20 GMT
CMD ["traefik"]
# Thu, 31 Mar 2022 02:24:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491249faa733d19d2c4f479860df3563c3f269d08d4c70b53926670b486092d5`  
		Last Modified: Tue, 29 Mar 2022 11:44:20 GMT  
		Size: 666.7 KB (666674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150f61256352f339798457a33bd19e97a2c486d649ab99d14e8ccc1b9c0aab4c`  
		Last Modified: Thu, 31 Mar 2022 02:25:02 GMT  
		Size: 27.4 MB (27399018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d9192a4e45679a6fe98f98a61976527914a4344b8b8126ba5e9ae401d7c37c`  
		Last Modified: Thu, 31 Mar 2022 02:24:57 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.7.0-rc2` - linux; arm variant v6

```console
$ docker pull traefik@sha256:1aee5e27fbc6358f097fa0fecd790f97972a5d860b39dd15c5c0746b7cae529a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (28982492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5067b6791686be1a6a27d9bb0fead0ff84404cf74a87b0cb709692e22117837c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:46 GMT
ADD file:9670f4f7de6a9b8eb844e418daedd0dbad90009126790eb65e246b29cac5ea47 in / 
# Tue, 29 Mar 2022 00:49:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 13:21:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 29 Mar 2022 20:14:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.0-rc2/traefik_v2.7.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 29 Mar 2022 20:14:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 29 Mar 2022 20:14:39 GMT
EXPOSE 80
# Tue, 29 Mar 2022 20:14:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 20:14:40 GMT
CMD ["traefik"]
# Tue, 29 Mar 2022 20:14:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79f5c9df0b90097bae07a9861e9e0e3f52a16b0bfde2793c4e14ad033cfb47f4`  
		Last Modified: Tue, 29 Mar 2022 00:51:45 GMT  
		Size: 2.6 MB (2626017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10449722d0e221d9f2d76fded7a3856b1e5da5de38e926c9dbde9dfeb95c67c8`  
		Last Modified: Tue, 29 Mar 2022 13:24:24 GMT  
		Size: 672.5 KB (672526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c35bed17508c434cf42b82887ab060852475c4e374ab4927382d30577e3ff1f`  
		Last Modified: Tue, 29 Mar 2022 20:17:27 GMT  
		Size: 25.7 MB (25683580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db18cf51e2278ee816fbc5b729a8cb8148229542f5993ccef454c8599eb551e`  
		Last Modified: Tue, 29 Mar 2022 20:17:10 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.7.0-rc2` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:cbc72e60f32f55ba66d1a5be7993d663006d2283f3b52202af99971e5c355ea2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28364421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ef4096bf04746212cf88c9a0795877622ff1ba98808ecb03b7ffe933c5ebd46`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:27:04 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 07:27:07 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.0-rc2/traefik_v2.7.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 07:27:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 07:27:08 GMT
EXPOSE 80
# Tue, 05 Apr 2022 07:27:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 07:27:10 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 07:27:11 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:ff858383c840c4b97834e60774329c49bf3fea922085ae31d8165402d4b9f5ea`  
		Last Modified: Tue, 05 Apr 2022 07:28:40 GMT  
		Size: 25.0 MB (24978372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04abccc9cf218d0e24ff784807a2c3570b5ed2a7183fbf08517b4fc4221c813e`  
		Last Modified: Tue, 05 Apr 2022 07:28:36 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.7.0-rc2` - linux; s390x

```console
$ docker pull traefik@sha256:7569039608d54d25f8a85c29da7151f2e16732547c169e96de3d8377bc945831
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29653216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e16a4ac48877da270277f281f90230f4a9638f791a4fe3a5e04e49c9e23235a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:47 GMT
ADD file:0f70e0f0075bee67acb44e5ef01bf6b9df1f69a25b7aa6fd15bd5bb6ec5bcc9f in / 
# Mon, 04 Apr 2022 23:41:48 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:14:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 05 Apr 2022 06:15:02 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.7.0-rc2/traefik_v2.7.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 05 Apr 2022 06:15:03 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 05 Apr 2022 06:15:03 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:15:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 06:15:04 GMT
CMD ["traefik"]
# Tue, 05 Apr 2022 06:15:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6f6a6c77b1bd5dfb3e759efaa292f964f197ae4b96be74d80ef059f87317997a`  
		Last Modified: Mon, 04 Apr 2022 23:42:47 GMT  
		Size: 2.6 MB (2604075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd299e72e5dfb969cf246832a04767813018867ef4e23d3cd39e9ed53fbb2e2`  
		Last Modified: Tue, 05 Apr 2022 06:15:50 GMT  
		Size: 672.5 KB (672500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9565ee21a342064cf700d9474883f1f743b295fc38f1a934caec7c014c19a39`  
		Last Modified: Tue, 05 Apr 2022 06:15:54 GMT  
		Size: 26.4 MB (26376273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0ffd87278d72e40d22211cb05d509dbac1628f7a1a59d0e65d8b8a260db1c3`  
		Last Modified: Tue, 05 Apr 2022 06:15:50 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.7.0-rc2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:fe30fb1edd24cb35ed73084221b49fd145c789c540a1a10e2e76aad943673a66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:v2.7.0-rc2-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:b10e4f877aebabb1734135b2646cb64cc5d70727f9964b4b764f6f1e749decc3
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2743448944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf2840916230e28221e266704780ab0cf47a706724fd322280cc72c40af2d0d6`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 29 Mar 2022 19:32:51 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.7.0-rc2/traefik_v2.7.0-rc2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 29 Mar 2022 19:32:52 GMT
EXPOSE 80
# Tue, 29 Mar 2022 19:32:53 GMT
ENTRYPOINT ["/traefik"]
# Tue, 29 Mar 2022 19:32:54 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e322088afb1a013924e6a53963322f66b3b52751ccaeb821099765b4ddc569ae`  
		Last Modified: Tue, 29 Mar 2022 19:35:00 GMT  
		Size: 28.0 MB (27991054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68de6a12e36621523a032635b4054a09a9c5898b8e50c091d7170ca3f0926544`  
		Last Modified: Tue, 29 Mar 2022 19:34:29 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcece30b93b7bbc58f5afe87698f87c2dc34b5aae3311c71ebf03339c1b0fec`  
		Last Modified: Tue, 29 Mar 2022 19:34:29 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99b616e8af959eea48003b4cf3217d9c66250b599e93b4cc5496bfeea62699c`  
		Last Modified: Tue, 29 Mar 2022 19:34:29 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:8c6d3723194f2b09c6b7e6f1c65c00573ed8a86fb030871f472f15b7f68b6ff2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:47d24eaf1b6b706e5de58ce11e2cbebf3a0f9575a61fec03a4c861e4438807a9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2742898776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5706e325ee2ad18345e4fe2fd1dc42a027366b1f9c1ddfc6a3e3542f918ece9c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 29 Mar 2022 19:33:53 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.6.3/traefik_v2.6.3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 29 Mar 2022 19:33:54 GMT
EXPOSE 80
# Tue, 29 Mar 2022 19:33:55 GMT
ENTRYPOINT ["/traefik"]
# Tue, 29 Mar 2022 19:33:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a79b9a00328456358c525859928802742529204e1d520ec9f3f68f3fe63ee9`  
		Last Modified: Tue, 29 Mar 2022 19:35:24 GMT  
		Size: 27.4 MB (27440577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfbef29f86d1cb8156adb9e83f62919091b87ae19d8b49027e53e32207378a1`  
		Last Modified: Tue, 29 Mar 2022 19:35:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81861a2761b14e5cf1801456272bdb3de1fc16f0d8724c6df47a371f20478091`  
		Last Modified: Tue, 29 Mar 2022 19:35:17 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779ed28a5abfc5c391b359a30b2b6fccee48c70fdc42d2a44a77a31b1d4c3e4d`  
		Last Modified: Tue, 29 Mar 2022 19:35:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
