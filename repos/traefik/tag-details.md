<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:1.7`](#traefik17)
-	[`traefik:1.7-alpine`](#traefik17-alpine)
-	[`traefik:1.7-windowsservercore-1809`](#traefik17-windowsservercore-1809)
-	[`traefik:1.7.34`](#traefik1734)
-	[`traefik:1.7.34-alpine`](#traefik1734-alpine)
-	[`traefik:1.7.34-windowsservercore-1809`](#traefik1734-windowsservercore-1809)
-	[`traefik:2.10`](#traefik210)
-	[`traefik:2.10-windowsservercore-1809`](#traefik210-windowsservercore-1809)
-	[`traefik:2.10.0-rc2`](#traefik2100-rc2)
-	[`traefik:2.10.0-rc2-windowsservercore-1809`](#traefik2100-rc2-windowsservercore-1809)
-	[`traefik:2.9`](#traefik29)
-	[`traefik:2.9-windowsservercore-1809`](#traefik29-windowsservercore-1809)
-	[`traefik:2.9.10`](#traefik2910)
-	[`traefik:2.9.10-windowsservercore-1809`](#traefik2910-windowsservercore-1809)
-	[`traefik:3.0`](#traefik30)
-	[`traefik:3.0-windowsservercore-1809`](#traefik30-windowsservercore-1809)
-	[`traefik:3.0.0-beta2`](#traefik300-beta2)
-	[`traefik:3.0.0-beta2-windowsservercore-1809`](#traefik300-beta2-windowsservercore-1809)
-	[`traefik:banon`](#traefikbanon)
-	[`traefik:banon-windowsservercore-1809`](#traefikbanon-windowsservercore-1809)
-	[`traefik:beaufort`](#traefikbeaufort)
-	[`traefik:beaufort-windowsservercore-1809`](#traefikbeaufort-windowsservercore-1809)
-	[`traefik:latest`](#traefiklatest)
-	[`traefik:maroilles`](#traefikmaroilles)
-	[`traefik:maroilles-alpine`](#traefikmaroilles-alpine)
-	[`traefik:maroilles-windowsservercore-1809`](#traefikmaroilles-windowsservercore-1809)
-	[`traefik:saintmarcelin`](#traefiksaintmarcelin)
-	[`traefik:saintmarcelin-windowsservercore-1809`](#traefiksaintmarcelin-windowsservercore-1809)
-	[`traefik:v1.7`](#traefikv17)
-	[`traefik:v1.7-alpine`](#traefikv17-alpine)
-	[`traefik:v1.7-windowsservercore-1809`](#traefikv17-windowsservercore-1809)
-	[`traefik:v1.7.34`](#traefikv1734)
-	[`traefik:v1.7.34-alpine`](#traefikv1734-alpine)
-	[`traefik:v1.7.34-windowsservercore-1809`](#traefikv1734-windowsservercore-1809)
-	[`traefik:v2.10`](#traefikv210)
-	[`traefik:v2.10-windowsservercore-1809`](#traefikv210-windowsservercore-1809)
-	[`traefik:v2.10.0-rc2`](#traefikv2100-rc2)
-	[`traefik:v2.10.0-rc2-windowsservercore-1809`](#traefikv2100-rc2-windowsservercore-1809)
-	[`traefik:v2.9`](#traefikv29)
-	[`traefik:v2.9-windowsservercore-1809`](#traefikv29-windowsservercore-1809)
-	[`traefik:v2.9.10`](#traefikv2910)
-	[`traefik:v2.9.10-windowsservercore-1809`](#traefikv2910-windowsservercore-1809)
-	[`traefik:v3.0`](#traefikv30)
-	[`traefik:v3.0-windowsservercore-1809`](#traefikv30-windowsservercore-1809)
-	[`traefik:v3.0.0-beta2`](#traefikv300-beta2)
-	[`traefik:v3.0.0-beta2-windowsservercore-1809`](#traefikv300-beta2-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:1.7`

```console
$ docker pull traefik@sha256:5d47b7bb25467dbc27ab2b260e496a7f9e1232511af369cdcc98daefba7979c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7` - linux; amd64

```console
$ docker pull traefik@sha256:d7bacaf9ca8d59b0e7c304920629d98bb98a545127ca4b10e16c8b252b9351b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22593766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aae4b2c164f286aeee70180f0b85a66a5a3652a07d87cc658851db5e53c9b59a`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 07 Oct 2022 04:21:33 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Thu, 30 Mar 2023 02:37:59 GMT
COPY dir:fcb1de0a76c41fc3dff8d6ca27f999d211e86842b0843ac2ebdecb15ff8e0492 in /usr/share/ 
# Thu, 30 Mar 2023 02:38:00 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Thu, 30 Mar 2023 02:38:01 GMT
EXPOSE 80
# Thu, 30 Mar 2023 02:38:01 GMT
VOLUME [/tmp]
# Thu, 30 Mar 2023 02:38:01 GMT
ENTRYPOINT ["/traefik"]
# Thu, 30 Mar 2023 02:38:01 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:39006e619508cd8a1ace2dcb57ecaa3a206fc01c9b72018e30b538ba58b0f45a`  
		Last Modified: Fri, 07 Oct 2022 04:22:39 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ed5475338aea0040268938cdb4cf5e6d08120622d034f2fe282ade7fb88f34`  
		Last Modified: Thu, 30 Mar 2023 02:39:32 GMT  
		Size: 308.3 KB (308275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62941aba458e9caf3e4a66617f7b97e463e427c1ee961fbc3b0a37b3dedaf385`  
		Last Modified: Thu, 30 Mar 2023 02:39:36 GMT  
		Size: 22.2 MB (22161951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0eba228e1865efa7bed0cd8ca41b7d6cf14dcab9f1852e3754b7815aeded5d20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21055086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79cd7b650b4ab04f4e437d8c394fb6f2190aea6b3e738817ce9f2462a9d93211`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 14 Mar 2023 01:31:59 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Thu, 30 Mar 2023 00:40:30 GMT
COPY dir:fcb1de0a76c41fc3dff8d6ca27f999d211e86842b0843ac2ebdecb15ff8e0492 in /usr/share/ 
# Thu, 30 Mar 2023 00:40:31 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Thu, 30 Mar 2023 00:40:32 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:40:32 GMT
VOLUME [/tmp]
# Thu, 30 Mar 2023 00:40:32 GMT
ENTRYPOINT ["/traefik"]
# Thu, 30 Mar 2023 00:40:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:68a2bb2e7a38ecc0a394b8fde6e116d903af0a9081c1816df304ab9a95b081da`  
		Last Modified: Tue, 14 Mar 2023 01:34:18 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae617ce90fe46cea74fe5b74b5c0b409ee3f81c32e2bb9f1aefe371e24ebccc1`  
		Last Modified: Thu, 30 Mar 2023 00:42:02 GMT  
		Size: 308.3 KB (308265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296e5dd1d0ad1bc244926e357696aac4774dcebeb52a2723b33bf9269b3df2db`  
		Last Modified: Thu, 30 Mar 2023 00:42:06 GMT  
		Size: 20.6 MB (20623281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:324f12be044568e2f6d8229c848734927a52950051372f956304692aa2ff1a58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20563152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b41da85c4671491cd2a55c06fe1efb206c993b03f2d5f02f5113268616bf0f04`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 27 Oct 2022 23:00:59 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Thu, 30 Mar 2023 03:27:00 GMT
COPY dir:fcb1de0a76c41fc3dff8d6ca27f999d211e86842b0843ac2ebdecb15ff8e0492 in /usr/share/ 
# Thu, 30 Mar 2023 03:27:01 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Thu, 30 Mar 2023 03:27:01 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:27:01 GMT
VOLUME [/tmp]
# Thu, 30 Mar 2023 03:27:01 GMT
ENTRYPOINT ["/traefik"]
# Thu, 30 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:384a668e636c3a58c260d7eacd140f07b0727673d5ba128334cbcedd184a99f2`  
		Last Modified: Thu, 27 Oct 2022 23:02:00 GMT  
		Size: 123.5 KB (123538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcae1c052addf1a94540e967bada340c12bef5e3c6fa1fd315bdc81f3e2db29b`  
		Last Modified: Thu, 30 Mar 2023 03:28:23 GMT  
		Size: 308.3 KB (308267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42d66bc2a6eaad18db8aeaaba24844b6f3fcb88954cbef25552a284d0c967de`  
		Last Modified: Thu, 30 Mar 2023 03:28:26 GMT  
		Size: 20.1 MB (20131347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-alpine`

```console
$ docker pull traefik@sha256:7fa25a5a54a44ddab4d6b5e40bf03175ae617b460c0ee4a744b859edfdf12c9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:323f96e7b93b93d1f3939c65b6c6ab4dd682087c4cc6842506e0526ba3b5ec4a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25652617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5752638b830b09f8b8d33d381e137e483de2476e8f9d7123a1c7caa0a3640575`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:37 GMT
ADD file:9663235f252e072c52b0f9e25845841e4321cce2caa7467a0d736c6003b05c00 in / 
# Wed, 29 Mar 2023 18:19:37 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 02:37:54 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 02:37:54 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 02:37:54 GMT
EXPOSE 80
# Thu, 30 Mar 2023 02:37:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 02:37:54 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 02:37:54 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f7dab3ab2d6ec29aa28769bec35331fb485b5837501b1e8556413d8b5a79c9c8`  
		Last Modified: Wed, 29 Mar 2023 18:20:25 GMT  
		Size: 2.8 MB (2829647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b336280e0077663b6ff48976dade0f4b39627828c80e6252ef3cbd195787a2`  
		Last Modified: Thu, 30 Mar 2023 02:39:15 GMT  
		Size: 660.5 KB (660537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9c0a6f6f71f1e51f885a6ef76ef507f598a8becb11334ab2eedda32ed2bf3d`  
		Last Modified: Thu, 30 Mar 2023 02:39:19 GMT  
		Size: 22.2 MB (22162065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfa1a444c49c4a20dc38ba06b91a7def26bd40e67624aaa412af8ae47e962cd`  
		Last Modified: Thu, 30 Mar 2023 02:39:15 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:7f9dabda3415134f3c6c55aa1c6d4a9714df3e6c1b17c09fa6829518be40304e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23928182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:989b6b4695cc561a8362ad5d755b293faf05ef51a2213c0f68940138fe65fd46`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:15 GMT
ADD file:1039802413c644346f599dac53a7c6dabd123027756231b9d8f64a1068c9779d in / 
# Wed, 29 Mar 2023 18:01:15 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:57 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 00:40:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 00:40:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 00:40:01 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:40:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 00:40:01 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 00:40:01 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ffeb76b9ee2f52d46487f4f9a7074ea62dea819a2dd53c9a2c6d703ca7b5aa06`  
		Last Modified: Wed, 29 Mar 2023 18:02:21 GMT  
		Size: 2.6 MB (2638259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b1182fcb4f775d878f0b8af17e60fdef00a0afb3a68f68731fdf08ca613566`  
		Last Modified: Thu, 30 Mar 2023 00:41:46 GMT  
		Size: 666.1 KB (666134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ace3e9b5f4c3d44312fca26e27d43459ab4671204cc813ae1a2d94bc295e24`  
		Last Modified: Thu, 30 Mar 2023 00:41:49 GMT  
		Size: 20.6 MB (20623422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fec87c1bbd8ed5033ef249c444c828c0d4a024613f7c067d6408df986bd229a`  
		Last Modified: Thu, 30 Mar 2023 00:41:46 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:604a02479b2cd6d49eefd5f24cc81497d3af5f7bc33c21d1cae3881779219515
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23519179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fe0b5ab962401db114bc8e05b69ff178950436ca17116fe2fd64b3189aa0acc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:25 GMT
ADD file:c3d52cc254959a9ff493e7347e6b1bc25c0ccfdcf9532dbf43173ddd182d0e4d in / 
# Wed, 29 Mar 2023 17:39:25 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:49 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 03:26:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 03:26:51 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 03:26:51 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:26:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 03:26:51 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 03:26:52 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:422ed46b1a92579f7c475c0c19fade6880a8d98f23a2b4ccfb77c265d4f72dfc`  
		Last Modified: Wed, 29 Mar 2023 17:40:13 GMT  
		Size: 2.7 MB (2725148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6752cbc5332b159f041b740aaa55aae27464ed4eccd5bef82a29db3a8910c02b`  
		Last Modified: Thu, 30 Mar 2023 03:28:09 GMT  
		Size: 662.3 KB (662304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77516a6a2e38caf662af65c73d4bed11e3775022a478ffb8c84004d4dcbc6f82`  
		Last Modified: Thu, 30 Mar 2023 03:28:11 GMT  
		Size: 20.1 MB (20131360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8cf26694e550c02564e364e7285e5830c82ec691f8de5269c861084468777b`  
		Last Modified: Thu, 30 Mar 2023 03:28:08 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f643d6e3857163a610f6ee48dcedefc4ae1c6957968b821a132c45dad295521d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:1.7-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:eb030d1415b37297490d0d042c132510d0592f8158bb80f98328bebe132c71c7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2036484756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd883fc0a81df58f398881ad9a26665e14af2ff944186704211ca53de351d281`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 08:48:48 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 16 Mar 2023 08:48:49 GMT
EXPOSE 80
# Thu, 16 Mar 2023 08:48:50 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Mar 2023 08:48:51 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c40e4a974e18ba73f3964c77bafb530b44a02b157bff67d57d80b50a37d306`  
		Last Modified: Thu, 16 Mar 2023 08:50:12 GMT  
		Size: 23.0 MB (22970100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b8a1819bca4f2eb81e780d11f83ab69e9c936aeaddbd31803a9949cf487145`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5590048d6ec03d383585a24a3e40df19cce710181b483bb92abd200c87c856`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbdbd264f1bd9f178ca6c87b2073841bac0e4226b3fed4145bbdb0c46e98ca1`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.34`

```console
$ docker pull traefik@sha256:5d47b7bb25467dbc27ab2b260e496a7f9e1232511af369cdcc98daefba7979c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.34` - linux; amd64

```console
$ docker pull traefik@sha256:d7bacaf9ca8d59b0e7c304920629d98bb98a545127ca4b10e16c8b252b9351b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22593766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aae4b2c164f286aeee70180f0b85a66a5a3652a07d87cc658851db5e53c9b59a`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 07 Oct 2022 04:21:33 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Thu, 30 Mar 2023 02:37:59 GMT
COPY dir:fcb1de0a76c41fc3dff8d6ca27f999d211e86842b0843ac2ebdecb15ff8e0492 in /usr/share/ 
# Thu, 30 Mar 2023 02:38:00 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Thu, 30 Mar 2023 02:38:01 GMT
EXPOSE 80
# Thu, 30 Mar 2023 02:38:01 GMT
VOLUME [/tmp]
# Thu, 30 Mar 2023 02:38:01 GMT
ENTRYPOINT ["/traefik"]
# Thu, 30 Mar 2023 02:38:01 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:39006e619508cd8a1ace2dcb57ecaa3a206fc01c9b72018e30b538ba58b0f45a`  
		Last Modified: Fri, 07 Oct 2022 04:22:39 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ed5475338aea0040268938cdb4cf5e6d08120622d034f2fe282ade7fb88f34`  
		Last Modified: Thu, 30 Mar 2023 02:39:32 GMT  
		Size: 308.3 KB (308275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62941aba458e9caf3e4a66617f7b97e463e427c1ee961fbc3b0a37b3dedaf385`  
		Last Modified: Thu, 30 Mar 2023 02:39:36 GMT  
		Size: 22.2 MB (22161951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.34` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0eba228e1865efa7bed0cd8ca41b7d6cf14dcab9f1852e3754b7815aeded5d20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21055086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79cd7b650b4ab04f4e437d8c394fb6f2190aea6b3e738817ce9f2462a9d93211`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 14 Mar 2023 01:31:59 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Thu, 30 Mar 2023 00:40:30 GMT
COPY dir:fcb1de0a76c41fc3dff8d6ca27f999d211e86842b0843ac2ebdecb15ff8e0492 in /usr/share/ 
# Thu, 30 Mar 2023 00:40:31 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Thu, 30 Mar 2023 00:40:32 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:40:32 GMT
VOLUME [/tmp]
# Thu, 30 Mar 2023 00:40:32 GMT
ENTRYPOINT ["/traefik"]
# Thu, 30 Mar 2023 00:40:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:68a2bb2e7a38ecc0a394b8fde6e116d903af0a9081c1816df304ab9a95b081da`  
		Last Modified: Tue, 14 Mar 2023 01:34:18 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae617ce90fe46cea74fe5b74b5c0b409ee3f81c32e2bb9f1aefe371e24ebccc1`  
		Last Modified: Thu, 30 Mar 2023 00:42:02 GMT  
		Size: 308.3 KB (308265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296e5dd1d0ad1bc244926e357696aac4774dcebeb52a2723b33bf9269b3df2db`  
		Last Modified: Thu, 30 Mar 2023 00:42:06 GMT  
		Size: 20.6 MB (20623281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.34` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:324f12be044568e2f6d8229c848734927a52950051372f956304692aa2ff1a58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20563152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b41da85c4671491cd2a55c06fe1efb206c993b03f2d5f02f5113268616bf0f04`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 27 Oct 2022 23:00:59 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Thu, 30 Mar 2023 03:27:00 GMT
COPY dir:fcb1de0a76c41fc3dff8d6ca27f999d211e86842b0843ac2ebdecb15ff8e0492 in /usr/share/ 
# Thu, 30 Mar 2023 03:27:01 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Thu, 30 Mar 2023 03:27:01 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:27:01 GMT
VOLUME [/tmp]
# Thu, 30 Mar 2023 03:27:01 GMT
ENTRYPOINT ["/traefik"]
# Thu, 30 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:384a668e636c3a58c260d7eacd140f07b0727673d5ba128334cbcedd184a99f2`  
		Last Modified: Thu, 27 Oct 2022 23:02:00 GMT  
		Size: 123.5 KB (123538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcae1c052addf1a94540e967bada340c12bef5e3c6fa1fd315bdc81f3e2db29b`  
		Last Modified: Thu, 30 Mar 2023 03:28:23 GMT  
		Size: 308.3 KB (308267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42d66bc2a6eaad18db8aeaaba24844b6f3fcb88954cbef25552a284d0c967de`  
		Last Modified: Thu, 30 Mar 2023 03:28:26 GMT  
		Size: 20.1 MB (20131347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.34-alpine`

```console
$ docker pull traefik@sha256:7fa25a5a54a44ddab4d6b5e40bf03175ae617b460c0ee4a744b859edfdf12c9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.34-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:323f96e7b93b93d1f3939c65b6c6ab4dd682087c4cc6842506e0526ba3b5ec4a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25652617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5752638b830b09f8b8d33d381e137e483de2476e8f9d7123a1c7caa0a3640575`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:37 GMT
ADD file:9663235f252e072c52b0f9e25845841e4321cce2caa7467a0d736c6003b05c00 in / 
# Wed, 29 Mar 2023 18:19:37 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 02:37:54 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 02:37:54 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 02:37:54 GMT
EXPOSE 80
# Thu, 30 Mar 2023 02:37:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 02:37:54 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 02:37:54 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f7dab3ab2d6ec29aa28769bec35331fb485b5837501b1e8556413d8b5a79c9c8`  
		Last Modified: Wed, 29 Mar 2023 18:20:25 GMT  
		Size: 2.8 MB (2829647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b336280e0077663b6ff48976dade0f4b39627828c80e6252ef3cbd195787a2`  
		Last Modified: Thu, 30 Mar 2023 02:39:15 GMT  
		Size: 660.5 KB (660537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9c0a6f6f71f1e51f885a6ef76ef507f598a8becb11334ab2eedda32ed2bf3d`  
		Last Modified: Thu, 30 Mar 2023 02:39:19 GMT  
		Size: 22.2 MB (22162065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfa1a444c49c4a20dc38ba06b91a7def26bd40e67624aaa412af8ae47e962cd`  
		Last Modified: Thu, 30 Mar 2023 02:39:15 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.34-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:7f9dabda3415134f3c6c55aa1c6d4a9714df3e6c1b17c09fa6829518be40304e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23928182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:989b6b4695cc561a8362ad5d755b293faf05ef51a2213c0f68940138fe65fd46`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:15 GMT
ADD file:1039802413c644346f599dac53a7c6dabd123027756231b9d8f64a1068c9779d in / 
# Wed, 29 Mar 2023 18:01:15 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:57 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 00:40:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 00:40:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 00:40:01 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:40:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 00:40:01 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 00:40:01 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ffeb76b9ee2f52d46487f4f9a7074ea62dea819a2dd53c9a2c6d703ca7b5aa06`  
		Last Modified: Wed, 29 Mar 2023 18:02:21 GMT  
		Size: 2.6 MB (2638259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b1182fcb4f775d878f0b8af17e60fdef00a0afb3a68f68731fdf08ca613566`  
		Last Modified: Thu, 30 Mar 2023 00:41:46 GMT  
		Size: 666.1 KB (666134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ace3e9b5f4c3d44312fca26e27d43459ab4671204cc813ae1a2d94bc295e24`  
		Last Modified: Thu, 30 Mar 2023 00:41:49 GMT  
		Size: 20.6 MB (20623422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fec87c1bbd8ed5033ef249c444c828c0d4a024613f7c067d6408df986bd229a`  
		Last Modified: Thu, 30 Mar 2023 00:41:46 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.34-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:604a02479b2cd6d49eefd5f24cc81497d3af5f7bc33c21d1cae3881779219515
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23519179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fe0b5ab962401db114bc8e05b69ff178950436ca17116fe2fd64b3189aa0acc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:25 GMT
ADD file:c3d52cc254959a9ff493e7347e6b1bc25c0ccfdcf9532dbf43173ddd182d0e4d in / 
# Wed, 29 Mar 2023 17:39:25 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:49 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 03:26:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 03:26:51 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 03:26:51 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:26:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 03:26:51 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 03:26:52 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:422ed46b1a92579f7c475c0c19fade6880a8d98f23a2b4ccfb77c265d4f72dfc`  
		Last Modified: Wed, 29 Mar 2023 17:40:13 GMT  
		Size: 2.7 MB (2725148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6752cbc5332b159f041b740aaa55aae27464ed4eccd5bef82a29db3a8910c02b`  
		Last Modified: Thu, 30 Mar 2023 03:28:09 GMT  
		Size: 662.3 KB (662304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77516a6a2e38caf662af65c73d4bed11e3775022a478ffb8c84004d4dcbc6f82`  
		Last Modified: Thu, 30 Mar 2023 03:28:11 GMT  
		Size: 20.1 MB (20131360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8cf26694e550c02564e364e7285e5830c82ec691f8de5269c861084468777b`  
		Last Modified: Thu, 30 Mar 2023 03:28:08 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.34-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f643d6e3857163a610f6ee48dcedefc4ae1c6957968b821a132c45dad295521d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:1.7.34-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:eb030d1415b37297490d0d042c132510d0592f8158bb80f98328bebe132c71c7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2036484756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd883fc0a81df58f398881ad9a26665e14af2ff944186704211ca53de351d281`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 08:48:48 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 16 Mar 2023 08:48:49 GMT
EXPOSE 80
# Thu, 16 Mar 2023 08:48:50 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Mar 2023 08:48:51 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c40e4a974e18ba73f3964c77bafb530b44a02b157bff67d57d80b50a37d306`  
		Last Modified: Thu, 16 Mar 2023 08:50:12 GMT  
		Size: 23.0 MB (22970100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b8a1819bca4f2eb81e780d11f83ab69e9c936aeaddbd31803a9949cf487145`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5590048d6ec03d383585a24a3e40df19cce710181b483bb92abd200c87c856`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbdbd264f1bd9f178ca6c87b2073841bac0e4226b3fed4145bbdb0c46e98ca1`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10`

```console
$ docker pull traefik@sha256:90f12602b0cb4df586fe90d3aacfdcf34b2e72253bcd01167ec6d670b631d39e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.10` - linux; amd64

```console
$ docker pull traefik@sha256:e740be22cd324a87119d2091a70e8c89c7f8a0f83913caa7dbc098c40ed01b44
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40979650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31d787e98af349f3ec4332f4d1cebf0555523271d40666e6d462dccec7c88872`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:38 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Apr 2023 22:20:57 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.0-rc2/traefik_v2.10.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Apr 2023 22:20:57 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Apr 2023 22:20:57 GMT
EXPOSE 80
# Fri, 07 Apr 2023 22:20:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Apr 2023 22:20:57 GMT
CMD ["traefik"]
# Fri, 07 Apr 2023 22:20:57 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d055169f9c6f7e08b88a6ef90eba203750fcc51761ecb994e40aa2aaa640ff72`  
		Last Modified: Thu, 30 Mar 2023 02:38:35 GMT  
		Size: 622.2 KB (622239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4680b9aefc39947986fb5f7d0fbb6c51f79b9fee726231e6e22799985ada11e`  
		Last Modified: Fri, 07 Apr 2023 22:21:24 GMT  
		Size: 37.0 MB (36982480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c40271a2c0502a46ca8dca99a5196da7cac0b078453a70a90877bee34cb6a45c`  
		Last Modified: Fri, 07 Apr 2023 22:21:18 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10` - linux; arm variant v6

```console
$ docker pull traefik@sha256:b45b8ce39f0f0a648e61c21b78a9a25f550969461997e9af661154f37e6c636f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37335481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:741d6b598348314376ea260c1fea9a9a81a56894b53da44daa8e972f4b6bf799`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:39 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 00:39:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.0-rc1/traefik_v2.10.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 00:39:53 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 00:39:53 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:39:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 00:39:53 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 00:39:53 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bd7901efecc8425b6d98584a9ee5d091a238a8936fb50b8aa4654afb90d05d`  
		Last Modified: Thu, 30 Mar 2023 00:41:05 GMT  
		Size: 624.4 KB (624425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc684a14f3623efaff9c3ff5a04d8dd15013918bff353a56fe64ba0ed9cc998b`  
		Last Modified: Thu, 30 Mar 2023 00:41:31 GMT  
		Size: 33.6 MB (33599887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d08a29db0e624938a5852b6f5752c900006cef7a5d8b305b400c6b9767a8e5`  
		Last Modified: Thu, 30 Mar 2023 00:41:25 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:4ac10aadbf80be52435784c32ad9fd4d80a95c949d12ff85e480ed0d0ce388ae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.6 MB (36598696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17449690bd237d6b44fdcfccf02d14b68f850e33f0476c25b6323f0f78539e30`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 03:26:45 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.0-rc1/traefik_v2.10.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 03:26:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 03:26:46 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:26:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 03:26:46 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 03:26:46 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4336eee5b1b811f9668d2251fb67e6099c4089ef7b26ade14aacd2f5f0982e06`  
		Last Modified: Thu, 30 Mar 2023 03:27:34 GMT  
		Size: 624.2 KB (624204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f80e6c463b9b292f88426c5afa82893107ee14f8f24ab7bbb5e1775e074ad7b0`  
		Last Modified: Thu, 30 Mar 2023 03:27:56 GMT  
		Size: 32.7 MB (32712271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68471cc27eba1f51573559a697edac9f1b8473bf301734e6d08d630fcb89288f`  
		Last Modified: Thu, 30 Mar 2023 03:27:52 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10` - linux; s390x

```console
$ docker pull traefik@sha256:25628239cc46999c02e0e8468645f4d310276777bc9473fd83e740ef6d3138cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38416622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fd82d431bd0f17307f89ce4d5c99653fb6f91c9f51965591d424410e6d25f9e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:38:21 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Mar 2023 22:38:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.0-rc1/traefik_v2.10.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Mar 2023 22:38:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Mar 2023 22:38:39 GMT
EXPOSE 80
# Wed, 29 Mar 2023 22:38:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 22:38:40 GMT
CMD ["traefik"]
# Wed, 29 Mar 2023 22:38:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096a495bd82a55e97c5be084787578b5b5af0321a33c70ccf19bca0dc260a981`  
		Last Modified: Wed, 29 Mar 2023 22:39:11 GMT  
		Size: 622.6 KB (622584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6483277d1e50cb2a0b9fdcebf8901f64c898d7042e19bea5f36a5982a9c262`  
		Last Modified: Wed, 29 Mar 2023 22:39:32 GMT  
		Size: 34.6 MB (34618483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f079c1b0af8d690151aa9187d4308985a20f7ac72e4916f72e429e87a3dbf9`  
		Last Modified: Wed, 29 Mar 2023 22:39:26 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e06b8c9a11f534829f3f075965ea66db0848b8c65075ac79790ab13631922a8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:2.10-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:290c74bd221d9156e894120db45f83e6c3073414ae4726b33a6c5394aad11ced
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2051118218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12766268c3909b8aea4982e046e39d57a153a1a283de0210d852fd225fb75428`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 07 Apr 2023 22:17:15 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.0-rc2/traefik_v2.10.0-rc2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Fri, 07 Apr 2023 22:17:16 GMT
EXPOSE 80
# Fri, 07 Apr 2023 22:17:17 GMT
ENTRYPOINT ["/traefik"]
# Fri, 07 Apr 2023 22:17:17 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57437d77990e17f6f1c4de8c842c9be99cc65894850bdf5fda3ce6ad610bc94`  
		Last Modified: Fri, 07 Apr 2023 22:18:11 GMT  
		Size: 37.6 MB (37603585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9b44ad239fc25c916d9b6fd60d1ee079b9827218883933725f6c452eedcb20`  
		Last Modified: Fri, 07 Apr 2023 22:18:03 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb69fbbb0a60fb6bf98cbfdfc0c3fc66801acb7bcd8c847cc43aa78fa8128a3`  
		Last Modified: Fri, 07 Apr 2023 22:18:03 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d5bdf56292275f8e72e015f1c9d64eb2d9d4ee6ddde77defa0866df6a3bbe4`  
		Last Modified: Fri, 07 Apr 2023 22:18:03 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10.0-rc2`

```console
$ docker pull traefik@sha256:f8662c6403f1b3fa10d700967241a256428241dab83d2aafab8d8c0953a4ca51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `traefik:2.10.0-rc2` - linux; amd64

```console
$ docker pull traefik@sha256:e740be22cd324a87119d2091a70e8c89c7f8a0f83913caa7dbc098c40ed01b44
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40979650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31d787e98af349f3ec4332f4d1cebf0555523271d40666e6d462dccec7c88872`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:38 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Apr 2023 22:20:57 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.0-rc2/traefik_v2.10.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Apr 2023 22:20:57 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Apr 2023 22:20:57 GMT
EXPOSE 80
# Fri, 07 Apr 2023 22:20:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Apr 2023 22:20:57 GMT
CMD ["traefik"]
# Fri, 07 Apr 2023 22:20:57 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d055169f9c6f7e08b88a6ef90eba203750fcc51761ecb994e40aa2aaa640ff72`  
		Last Modified: Thu, 30 Mar 2023 02:38:35 GMT  
		Size: 622.2 KB (622239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4680b9aefc39947986fb5f7d0fbb6c51f79b9fee726231e6e22799985ada11e`  
		Last Modified: Fri, 07 Apr 2023 22:21:24 GMT  
		Size: 37.0 MB (36982480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c40271a2c0502a46ca8dca99a5196da7cac0b078453a70a90877bee34cb6a45c`  
		Last Modified: Fri, 07 Apr 2023 22:21:18 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10.0-rc2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e06b8c9a11f534829f3f075965ea66db0848b8c65075ac79790ab13631922a8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:2.10.0-rc2-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:290c74bd221d9156e894120db45f83e6c3073414ae4726b33a6c5394aad11ced
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2051118218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12766268c3909b8aea4982e046e39d57a153a1a283de0210d852fd225fb75428`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 07 Apr 2023 22:17:15 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.0-rc2/traefik_v2.10.0-rc2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Fri, 07 Apr 2023 22:17:16 GMT
EXPOSE 80
# Fri, 07 Apr 2023 22:17:17 GMT
ENTRYPOINT ["/traefik"]
# Fri, 07 Apr 2023 22:17:17 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57437d77990e17f6f1c4de8c842c9be99cc65894850bdf5fda3ce6ad610bc94`  
		Last Modified: Fri, 07 Apr 2023 22:18:11 GMT  
		Size: 37.6 MB (37603585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9b44ad239fc25c916d9b6fd60d1ee079b9827218883933725f6c452eedcb20`  
		Last Modified: Fri, 07 Apr 2023 22:18:03 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb69fbbb0a60fb6bf98cbfdfc0c3fc66801acb7bcd8c847cc43aa78fa8128a3`  
		Last Modified: Fri, 07 Apr 2023 22:18:03 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d5bdf56292275f8e72e015f1c9d64eb2d9d4ee6ddde77defa0866df6a3bbe4`  
		Last Modified: Fri, 07 Apr 2023 22:18:03 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.9`

```console
$ docker pull traefik@sha256:8d81a9df1435f9f3d36ac9398465ef2d5d61e671059974db753faaed14b627de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.9` - linux; amd64

```console
$ docker pull traefik@sha256:6dee6938b5ebfc511a82ef4e09c80268835a2f67393e5c06c3e4ef9a14d1817b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39613072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1e26b5f8193d713eb8f39d0ab0e3d513278f86e41644b07e189e1aef536b335`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:38 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Apr 2023 18:24:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Apr 2023 18:24:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Apr 2023 18:24:44 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:24:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:24:44 GMT
CMD ["traefik"]
# Thu, 06 Apr 2023 18:24:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d055169f9c6f7e08b88a6ef90eba203750fcc51761ecb994e40aa2aaa640ff72`  
		Last Modified: Thu, 30 Mar 2023 02:38:35 GMT  
		Size: 622.2 KB (622239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afaddc85d79e665b30c4ee7ce9fc12425532f4695c6888b052086589f12aa687`  
		Last Modified: Thu, 06 Apr 2023 18:25:11 GMT  
		Size: 35.6 MB (35615902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff733a62a1272d7fe4817f1b3a8faf56c8a7f0e3808baec593378d274c1d081`  
		Last Modified: Thu, 06 Apr 2023 18:25:06 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f76a8f0c2b54429df275eb7e842171230994dc28924cb17f65ca41a3c5cb94fc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37257635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c077549480f6828d39797ca3855e6299d0c1e7daf08d67cd62320c07515ff0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:39 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Apr 2023 18:49:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Apr 2023 18:49:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Apr 2023 18:49:31 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:49:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:49:31 GMT
CMD ["traefik"]
# Thu, 06 Apr 2023 18:49:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bd7901efecc8425b6d98584a9ee5d091a238a8936fb50b8aa4654afb90d05d`  
		Last Modified: Thu, 30 Mar 2023 00:41:05 GMT  
		Size: 624.4 KB (624425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:658599efc3390617789f600a87686c808ae0c26e3a0a310ca9ad50944f5061f2`  
		Last Modified: Thu, 06 Apr 2023 18:49:58 GMT  
		Size: 33.5 MB (33522040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39827a939bd6089039662bd6dc0237923c0b6b7d177fcf7f37bdcb9dcaf831ee`  
		Last Modified: Thu, 06 Apr 2023 18:49:52 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7b1ecf3dcf9d504f037e14d060c7bfcb87ebde442eaf3c1d89e0c2e2f180a987
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.5 MB (36503424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fa39db0cea458044cad085ee32cf6bb615ccff2f3f7bbbc5e57f9b36984afb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Apr 2023 18:51:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Apr 2023 18:51:04 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Apr 2023 18:51:04 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:51:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:51:04 GMT
CMD ["traefik"]
# Thu, 06 Apr 2023 18:51:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4336eee5b1b811f9668d2251fb67e6099c4089ef7b26ade14aacd2f5f0982e06`  
		Last Modified: Thu, 30 Mar 2023 03:27:34 GMT  
		Size: 624.2 KB (624204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9cadb05aa1b060d980fd3437917259c39ca7d9fb914fccd2d05ba2c3ac9d1e`  
		Last Modified: Thu, 06 Apr 2023 18:51:28 GMT  
		Size: 32.6 MB (32616998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1371d2d81d70ec646fa25de2ef0e1ecbf8a73448a75536cdae53906746ee2605`  
		Last Modified: Thu, 06 Apr 2023 18:51:24 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9` - linux; s390x

```console
$ docker pull traefik@sha256:40c157efc3aeb2a68be807c7bd9c56058b039f5dc04ea99a2d207f5694ba3498
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38337898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ed3cb8277e480dbe2a03868fd3de6e86d2381cb25b7d4cf62ca5209a4a8f36f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:38:21 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Apr 2023 18:46:14 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Apr 2023 18:46:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Apr 2023 18:46:16 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:46:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:46:16 GMT
CMD ["traefik"]
# Thu, 06 Apr 2023 18:46:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096a495bd82a55e97c5be084787578b5b5af0321a33c70ccf19bca0dc260a981`  
		Last Modified: Wed, 29 Mar 2023 22:39:11 GMT  
		Size: 622.6 KB (622584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff0e0742f027721acb6e403cfd9c33f5035562626412821cf440ee0a0d4bd6`  
		Last Modified: Thu, 06 Apr 2023 18:46:41 GMT  
		Size: 34.5 MB (34539759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566cf6a3c532656d496f8fab7a8822e11cef4dd8c1dab24cdf229bbf359101eb`  
		Last Modified: Thu, 06 Apr 2023 18:46:36 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.9-windowsservercore-1809`

```console
$ docker pull traefik@sha256:ec994d877f87622e6e0fe82b0ea8e3b3efabf1e0d8c57fe110f822b211243c08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:2.9-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:38c71b3285dd02b9aa56ad826495f85e854606a04db526dcf7bf770ca9936a20
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2049781176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f645f991b33f438d120607abe7a2a158d8300068ceb916e0d7a6d2eaa095526e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Apr 2023 18:17:03 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 06 Apr 2023 18:17:04 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:17:05 GMT
ENTRYPOINT ["/traefik"]
# Thu, 06 Apr 2023 18:17:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b184b38bee4a888e16184a05c4770d36d87ad320077cbee08f12000fd700abed`  
		Last Modified: Thu, 06 Apr 2023 18:18:10 GMT  
		Size: 36.3 MB (36266505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32de5c550068bdd6a0e71f6aaae2c5ba100294dbb52006ca1247bc09cfb87e17`  
		Last Modified: Thu, 06 Apr 2023 18:18:00 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b65f112c430971f5c46a3133c30bd210125ddcf9493bca90d0553685871a5`  
		Last Modified: Thu, 06 Apr 2023 18:18:00 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8510431814f07a8c701f707dabf5daf9283df8769147fefe8634a06b3edf2a`  
		Last Modified: Thu, 06 Apr 2023 18:18:00 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.9.10`

```console
$ docker pull traefik@sha256:8d81a9df1435f9f3d36ac9398465ef2d5d61e671059974db753faaed14b627de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.9.10` - linux; amd64

```console
$ docker pull traefik@sha256:6dee6938b5ebfc511a82ef4e09c80268835a2f67393e5c06c3e4ef9a14d1817b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39613072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1e26b5f8193d713eb8f39d0ab0e3d513278f86e41644b07e189e1aef536b335`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:38 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Apr 2023 18:24:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Apr 2023 18:24:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Apr 2023 18:24:44 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:24:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:24:44 GMT
CMD ["traefik"]
# Thu, 06 Apr 2023 18:24:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d055169f9c6f7e08b88a6ef90eba203750fcc51761ecb994e40aa2aaa640ff72`  
		Last Modified: Thu, 30 Mar 2023 02:38:35 GMT  
		Size: 622.2 KB (622239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afaddc85d79e665b30c4ee7ce9fc12425532f4695c6888b052086589f12aa687`  
		Last Modified: Thu, 06 Apr 2023 18:25:11 GMT  
		Size: 35.6 MB (35615902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff733a62a1272d7fe4817f1b3a8faf56c8a7f0e3808baec593378d274c1d081`  
		Last Modified: Thu, 06 Apr 2023 18:25:06 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9.10` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f76a8f0c2b54429df275eb7e842171230994dc28924cb17f65ca41a3c5cb94fc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37257635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c077549480f6828d39797ca3855e6299d0c1e7daf08d67cd62320c07515ff0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:39 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Apr 2023 18:49:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Apr 2023 18:49:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Apr 2023 18:49:31 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:49:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:49:31 GMT
CMD ["traefik"]
# Thu, 06 Apr 2023 18:49:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bd7901efecc8425b6d98584a9ee5d091a238a8936fb50b8aa4654afb90d05d`  
		Last Modified: Thu, 30 Mar 2023 00:41:05 GMT  
		Size: 624.4 KB (624425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:658599efc3390617789f600a87686c808ae0c26e3a0a310ca9ad50944f5061f2`  
		Last Modified: Thu, 06 Apr 2023 18:49:58 GMT  
		Size: 33.5 MB (33522040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39827a939bd6089039662bd6dc0237923c0b6b7d177fcf7f37bdcb9dcaf831ee`  
		Last Modified: Thu, 06 Apr 2023 18:49:52 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9.10` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7b1ecf3dcf9d504f037e14d060c7bfcb87ebde442eaf3c1d89e0c2e2f180a987
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.5 MB (36503424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fa39db0cea458044cad085ee32cf6bb615ccff2f3f7bbbc5e57f9b36984afb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Apr 2023 18:51:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Apr 2023 18:51:04 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Apr 2023 18:51:04 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:51:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:51:04 GMT
CMD ["traefik"]
# Thu, 06 Apr 2023 18:51:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4336eee5b1b811f9668d2251fb67e6099c4089ef7b26ade14aacd2f5f0982e06`  
		Last Modified: Thu, 30 Mar 2023 03:27:34 GMT  
		Size: 624.2 KB (624204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9cadb05aa1b060d980fd3437917259c39ca7d9fb914fccd2d05ba2c3ac9d1e`  
		Last Modified: Thu, 06 Apr 2023 18:51:28 GMT  
		Size: 32.6 MB (32616998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1371d2d81d70ec646fa25de2ef0e1ecbf8a73448a75536cdae53906746ee2605`  
		Last Modified: Thu, 06 Apr 2023 18:51:24 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9.10` - linux; s390x

```console
$ docker pull traefik@sha256:40c157efc3aeb2a68be807c7bd9c56058b039f5dc04ea99a2d207f5694ba3498
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38337898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ed3cb8277e480dbe2a03868fd3de6e86d2381cb25b7d4cf62ca5209a4a8f36f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:38:21 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Apr 2023 18:46:14 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Apr 2023 18:46:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Apr 2023 18:46:16 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:46:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:46:16 GMT
CMD ["traefik"]
# Thu, 06 Apr 2023 18:46:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096a495bd82a55e97c5be084787578b5b5af0321a33c70ccf19bca0dc260a981`  
		Last Modified: Wed, 29 Mar 2023 22:39:11 GMT  
		Size: 622.6 KB (622584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff0e0742f027721acb6e403cfd9c33f5035562626412821cf440ee0a0d4bd6`  
		Last Modified: Thu, 06 Apr 2023 18:46:41 GMT  
		Size: 34.5 MB (34539759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566cf6a3c532656d496f8fab7a8822e11cef4dd8c1dab24cdf229bbf359101eb`  
		Last Modified: Thu, 06 Apr 2023 18:46:36 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.9.10-windowsservercore-1809`

```console
$ docker pull traefik@sha256:ec994d877f87622e6e0fe82b0ea8e3b3efabf1e0d8c57fe110f822b211243c08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:2.9.10-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:38c71b3285dd02b9aa56ad826495f85e854606a04db526dcf7bf770ca9936a20
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2049781176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f645f991b33f438d120607abe7a2a158d8300068ceb916e0d7a6d2eaa095526e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Apr 2023 18:17:03 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 06 Apr 2023 18:17:04 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:17:05 GMT
ENTRYPOINT ["/traefik"]
# Thu, 06 Apr 2023 18:17:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b184b38bee4a888e16184a05c4770d36d87ad320077cbee08f12000fd700abed`  
		Last Modified: Thu, 06 Apr 2023 18:18:10 GMT  
		Size: 36.3 MB (36266505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32de5c550068bdd6a0e71f6aaae2c5ba100294dbb52006ca1247bc09cfb87e17`  
		Last Modified: Thu, 06 Apr 2023 18:18:00 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b65f112c430971f5c46a3133c30bd210125ddcf9493bca90d0553685871a5`  
		Last Modified: Thu, 06 Apr 2023 18:18:00 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8510431814f07a8c701f707dabf5daf9283df8769147fefe8634a06b3edf2a`  
		Last Modified: Thu, 06 Apr 2023 18:18:00 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0`

```console
$ docker pull traefik@sha256:0d7e8693e44e52588366695db63512b6b7a92d34b2145c2c3c732fec27ee03e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:3.0` - linux; amd64

```console
$ docker pull traefik@sha256:a239deca1c7682fe9bb6a32e54364c7ff460205fa0e87c02bfeb66efb3f3a3d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40562953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42fc5a7c2d34a752fce6439cf3dc08ac747649d7712bc265c7dd7d1b38a2a45b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 02:37:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 02:37:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 02:37:35 GMT
EXPOSE 80
# Thu, 30 Mar 2023 02:37:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 02:37:35 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 02:37:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11624eb8d0cca298aa32848e39318bbc75ab1c404423d1d47c670fa60354e3`  
		Last Modified: Thu, 30 Mar 2023 02:38:16 GMT  
		Size: 661.1 KB (661099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9d40a9765a3ede8e4ec67030b20d484fedcea2ad98ee2b231ec3d86e6fd1b6`  
		Last Modified: Thu, 30 Mar 2023 02:38:21 GMT  
		Size: 37.1 MB (37074890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fca61e22e5a1dbbdeea08d3e394601c2c5492fc65d19af813ef66cc36a7d582`  
		Last Modified: Thu, 30 Mar 2023 02:38:15 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0` - linux; arm variant v6

```console
$ docker pull traefik@sha256:5da0026b1e1053a9bcef582853c749291cf651f2bc1e35a557d87080e78a74f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38289884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d444fca66ffd358a663e6075b1d97f53a52bd6d11aa27afa1aa0b8cf4179f67`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:13 GMT
ADD file:3fb55ad8134002858be264c3c2477d784e4a60f2f6501afa7cf3b10bfede51aa in / 
# Wed, 29 Mar 2023 18:01:13 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 00:39:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 00:39:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 00:39:31 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:39:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 00:39:31 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 00:39:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:872c99a87729fa48dce303fb615edbb1a5da837f627a0b3d28495a0400ca8335`  
		Last Modified: Wed, 29 Mar 2023 18:02:12 GMT  
		Size: 2.6 MB (2634030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb226453f567b759ad92b5db4fa1f391e1eb96232b14d006147344b993d24773`  
		Last Modified: Thu, 30 Mar 2023 00:40:46 GMT  
		Size: 666.2 KB (666166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f676a5305470c023669ddf7351410e0d65fa65bcfe24fc65a2e567699f7c00e6`  
		Last Modified: Thu, 30 Mar 2023 00:40:52 GMT  
		Size: 35.0 MB (34989322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb744443f625044ceb56795d0847c66fe1957350cdaa3a296ad67d692876d308`  
		Last Modified: Thu, 30 Mar 2023 00:40:46 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:529410986a68c6e7989a5a08afa53d087795a2f1406977d5d6b183bfdfab65dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37408212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e4bfdbd12bed1c2e46296bb16021a1eea4269055e03fdf9e30c035e5f9e8dc4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 03:26:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 03:26:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 03:26:35 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:26:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 03:26:35 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 03:26:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d019fab0470c352dfa2ff6c01be8f1d0344d43e9431a28656e78c5cabd03e67f`  
		Last Modified: Thu, 30 Mar 2023 03:27:17 GMT  
		Size: 662.3 KB (662323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82ed46bb3966bf021d56f3bfda66ada1ddde7199ee9d3446ebcbeffec692004`  
		Last Modified: Thu, 30 Mar 2023 03:27:20 GMT  
		Size: 34.0 MB (34023520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a93ddfbde23c1aa20ccac6b7cd3dcbda52d11c2b1627d41dc7fa169bd46430`  
		Last Modified: Thu, 30 Mar 2023 03:27:16 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0` - linux; s390x

```console
$ docker pull traefik@sha256:e8572896cf2369e9777be7e5ce1bce0b811642e09298039e0a9d51fa570172e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39131970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:194779f21f9e8eb09ec639ba646ce59761d5db6264648a5e162bf515e294517d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:07 GMT
ADD file:5cf392863cd9a0735de88f9e7dab93c9e74aca59ca05b792943cf3b621ea2c59 in / 
# Wed, 29 Mar 2023 17:42:07 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:38:08 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Mar 2023 22:38:14 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Mar 2023 22:38:15 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Mar 2023 22:38:16 GMT
EXPOSE 80
# Wed, 29 Mar 2023 22:38:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 22:38:16 GMT
CMD ["traefik"]
# Wed, 29 Mar 2023 22:38:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:1536575ac9c5f5fff4522c60d4610af0a52be584c36e652080c6c0ad169d4f27`  
		Last Modified: Wed, 29 Mar 2023 17:42:42 GMT  
		Size: 2.6 MB (2610636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246408072526d1b1e0fec7aaa14e46bd07b33c86c047b5d7cdce7778f992de28`  
		Last Modified: Wed, 29 Mar 2023 22:38:58 GMT  
		Size: 665.5 KB (665530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982fc64501c81b1c6a90bf3b79f669b6d16f9133509eb962541ae33f7f14c83c`  
		Last Modified: Wed, 29 Mar 2023 22:39:03 GMT  
		Size: 35.9 MB (35855437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b72fc0bf978c8423d98dc56a60760c0b3d12dbea0fd1524d98a88e3f173c6ab`  
		Last Modified: Wed, 29 Mar 2023 22:38:58 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0-windowsservercore-1809`

```console
$ docker pull traefik@sha256:2eb0d945da364a274f76288295b9120086404be2c7606fe340ac2ee6f1d64ed1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:3.0-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:62e9db8356188c92dbce1706a8c2af3702993ee762b34d398fc7921eb03a3629
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2051205802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648f7c4938c24c605c3f3cbf0b16d4a5767ce075cd407fa9c6ab93e256035917`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 08:45:29 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 16 Mar 2023 08:45:30 GMT
EXPOSE 80
# Thu, 16 Mar 2023 08:45:31 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Mar 2023 08:45:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5eafb0300ea614e208e5052cfdd0941f2ad90a341c5b337ab489e223bb31e88`  
		Last Modified: Thu, 16 Mar 2023 08:49:24 GMT  
		Size: 37.7 MB (37691161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec0dc51e5d37193b3e6ebdd21f1bb94e44f593af5691b32af00720bb4548bbc`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28da668ed65b21bb734a5ba72dd5262a27de001c56a64bebf1db5e9244aaad4c`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6138998225adfde27a93f621c64ba53c628511ce9209f16661fd0c3619ff3e3`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0.0-beta2`

```console
$ docker pull traefik@sha256:0d7e8693e44e52588366695db63512b6b7a92d34b2145c2c3c732fec27ee03e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:3.0.0-beta2` - linux; amd64

```console
$ docker pull traefik@sha256:a239deca1c7682fe9bb6a32e54364c7ff460205fa0e87c02bfeb66efb3f3a3d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40562953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42fc5a7c2d34a752fce6439cf3dc08ac747649d7712bc265c7dd7d1b38a2a45b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 02:37:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 02:37:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 02:37:35 GMT
EXPOSE 80
# Thu, 30 Mar 2023 02:37:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 02:37:35 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 02:37:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11624eb8d0cca298aa32848e39318bbc75ab1c404423d1d47c670fa60354e3`  
		Last Modified: Thu, 30 Mar 2023 02:38:16 GMT  
		Size: 661.1 KB (661099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9d40a9765a3ede8e4ec67030b20d484fedcea2ad98ee2b231ec3d86e6fd1b6`  
		Last Modified: Thu, 30 Mar 2023 02:38:21 GMT  
		Size: 37.1 MB (37074890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fca61e22e5a1dbbdeea08d3e394601c2c5492fc65d19af813ef66cc36a7d582`  
		Last Modified: Thu, 30 Mar 2023 02:38:15 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0.0-beta2` - linux; arm variant v6

```console
$ docker pull traefik@sha256:5da0026b1e1053a9bcef582853c749291cf651f2bc1e35a557d87080e78a74f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38289884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d444fca66ffd358a663e6075b1d97f53a52bd6d11aa27afa1aa0b8cf4179f67`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:13 GMT
ADD file:3fb55ad8134002858be264c3c2477d784e4a60f2f6501afa7cf3b10bfede51aa in / 
# Wed, 29 Mar 2023 18:01:13 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 00:39:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 00:39:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 00:39:31 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:39:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 00:39:31 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 00:39:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:872c99a87729fa48dce303fb615edbb1a5da837f627a0b3d28495a0400ca8335`  
		Last Modified: Wed, 29 Mar 2023 18:02:12 GMT  
		Size: 2.6 MB (2634030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb226453f567b759ad92b5db4fa1f391e1eb96232b14d006147344b993d24773`  
		Last Modified: Thu, 30 Mar 2023 00:40:46 GMT  
		Size: 666.2 KB (666166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f676a5305470c023669ddf7351410e0d65fa65bcfe24fc65a2e567699f7c00e6`  
		Last Modified: Thu, 30 Mar 2023 00:40:52 GMT  
		Size: 35.0 MB (34989322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb744443f625044ceb56795d0847c66fe1957350cdaa3a296ad67d692876d308`  
		Last Modified: Thu, 30 Mar 2023 00:40:46 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0.0-beta2` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:529410986a68c6e7989a5a08afa53d087795a2f1406977d5d6b183bfdfab65dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37408212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e4bfdbd12bed1c2e46296bb16021a1eea4269055e03fdf9e30c035e5f9e8dc4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 03:26:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 03:26:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 03:26:35 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:26:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 03:26:35 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 03:26:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d019fab0470c352dfa2ff6c01be8f1d0344d43e9431a28656e78c5cabd03e67f`  
		Last Modified: Thu, 30 Mar 2023 03:27:17 GMT  
		Size: 662.3 KB (662323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82ed46bb3966bf021d56f3bfda66ada1ddde7199ee9d3446ebcbeffec692004`  
		Last Modified: Thu, 30 Mar 2023 03:27:20 GMT  
		Size: 34.0 MB (34023520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a93ddfbde23c1aa20ccac6b7cd3dcbda52d11c2b1627d41dc7fa169bd46430`  
		Last Modified: Thu, 30 Mar 2023 03:27:16 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0.0-beta2` - linux; s390x

```console
$ docker pull traefik@sha256:e8572896cf2369e9777be7e5ce1bce0b811642e09298039e0a9d51fa570172e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39131970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:194779f21f9e8eb09ec639ba646ce59761d5db6264648a5e162bf515e294517d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:07 GMT
ADD file:5cf392863cd9a0735de88f9e7dab93c9e74aca59ca05b792943cf3b621ea2c59 in / 
# Wed, 29 Mar 2023 17:42:07 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:38:08 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Mar 2023 22:38:14 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Mar 2023 22:38:15 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Mar 2023 22:38:16 GMT
EXPOSE 80
# Wed, 29 Mar 2023 22:38:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 22:38:16 GMT
CMD ["traefik"]
# Wed, 29 Mar 2023 22:38:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:1536575ac9c5f5fff4522c60d4610af0a52be584c36e652080c6c0ad169d4f27`  
		Last Modified: Wed, 29 Mar 2023 17:42:42 GMT  
		Size: 2.6 MB (2610636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246408072526d1b1e0fec7aaa14e46bd07b33c86c047b5d7cdce7778f992de28`  
		Last Modified: Wed, 29 Mar 2023 22:38:58 GMT  
		Size: 665.5 KB (665530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982fc64501c81b1c6a90bf3b79f669b6d16f9133509eb962541ae33f7f14c83c`  
		Last Modified: Wed, 29 Mar 2023 22:39:03 GMT  
		Size: 35.9 MB (35855437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b72fc0bf978c8423d98dc56a60760c0b3d12dbea0fd1524d98a88e3f173c6ab`  
		Last Modified: Wed, 29 Mar 2023 22:38:58 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0.0-beta2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:2eb0d945da364a274f76288295b9120086404be2c7606fe340ac2ee6f1d64ed1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:3.0.0-beta2-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:62e9db8356188c92dbce1706a8c2af3702993ee762b34d398fc7921eb03a3629
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2051205802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648f7c4938c24c605c3f3cbf0b16d4a5767ce075cd407fa9c6ab93e256035917`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 08:45:29 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 16 Mar 2023 08:45:30 GMT
EXPOSE 80
# Thu, 16 Mar 2023 08:45:31 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Mar 2023 08:45:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5eafb0300ea614e208e5052cfdd0941f2ad90a341c5b337ab489e223bb31e88`  
		Last Modified: Thu, 16 Mar 2023 08:49:24 GMT  
		Size: 37.7 MB (37691161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec0dc51e5d37193b3e6ebdd21f1bb94e44f593af5691b32af00720bb4548bbc`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28da668ed65b21bb734a5ba72dd5262a27de001c56a64bebf1db5e9244aaad4c`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6138998225adfde27a93f621c64ba53c628511ce9209f16661fd0c3619ff3e3`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:banon`

```console
$ docker pull traefik@sha256:8d81a9df1435f9f3d36ac9398465ef2d5d61e671059974db753faaed14b627de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:banon` - linux; amd64

```console
$ docker pull traefik@sha256:6dee6938b5ebfc511a82ef4e09c80268835a2f67393e5c06c3e4ef9a14d1817b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39613072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1e26b5f8193d713eb8f39d0ab0e3d513278f86e41644b07e189e1aef536b335`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:38 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Apr 2023 18:24:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Apr 2023 18:24:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Apr 2023 18:24:44 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:24:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:24:44 GMT
CMD ["traefik"]
# Thu, 06 Apr 2023 18:24:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d055169f9c6f7e08b88a6ef90eba203750fcc51761ecb994e40aa2aaa640ff72`  
		Last Modified: Thu, 30 Mar 2023 02:38:35 GMT  
		Size: 622.2 KB (622239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afaddc85d79e665b30c4ee7ce9fc12425532f4695c6888b052086589f12aa687`  
		Last Modified: Thu, 06 Apr 2023 18:25:11 GMT  
		Size: 35.6 MB (35615902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff733a62a1272d7fe4817f1b3a8faf56c8a7f0e3808baec593378d274c1d081`  
		Last Modified: Thu, 06 Apr 2023 18:25:06 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:banon` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f76a8f0c2b54429df275eb7e842171230994dc28924cb17f65ca41a3c5cb94fc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37257635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c077549480f6828d39797ca3855e6299d0c1e7daf08d67cd62320c07515ff0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:39 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Apr 2023 18:49:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Apr 2023 18:49:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Apr 2023 18:49:31 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:49:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:49:31 GMT
CMD ["traefik"]
# Thu, 06 Apr 2023 18:49:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bd7901efecc8425b6d98584a9ee5d091a238a8936fb50b8aa4654afb90d05d`  
		Last Modified: Thu, 30 Mar 2023 00:41:05 GMT  
		Size: 624.4 KB (624425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:658599efc3390617789f600a87686c808ae0c26e3a0a310ca9ad50944f5061f2`  
		Last Modified: Thu, 06 Apr 2023 18:49:58 GMT  
		Size: 33.5 MB (33522040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39827a939bd6089039662bd6dc0237923c0b6b7d177fcf7f37bdcb9dcaf831ee`  
		Last Modified: Thu, 06 Apr 2023 18:49:52 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:banon` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7b1ecf3dcf9d504f037e14d060c7bfcb87ebde442eaf3c1d89e0c2e2f180a987
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.5 MB (36503424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fa39db0cea458044cad085ee32cf6bb615ccff2f3f7bbbc5e57f9b36984afb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Apr 2023 18:51:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Apr 2023 18:51:04 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Apr 2023 18:51:04 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:51:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:51:04 GMT
CMD ["traefik"]
# Thu, 06 Apr 2023 18:51:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4336eee5b1b811f9668d2251fb67e6099c4089ef7b26ade14aacd2f5f0982e06`  
		Last Modified: Thu, 30 Mar 2023 03:27:34 GMT  
		Size: 624.2 KB (624204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9cadb05aa1b060d980fd3437917259c39ca7d9fb914fccd2d05ba2c3ac9d1e`  
		Last Modified: Thu, 06 Apr 2023 18:51:28 GMT  
		Size: 32.6 MB (32616998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1371d2d81d70ec646fa25de2ef0e1ecbf8a73448a75536cdae53906746ee2605`  
		Last Modified: Thu, 06 Apr 2023 18:51:24 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:banon` - linux; s390x

```console
$ docker pull traefik@sha256:40c157efc3aeb2a68be807c7bd9c56058b039f5dc04ea99a2d207f5694ba3498
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38337898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ed3cb8277e480dbe2a03868fd3de6e86d2381cb25b7d4cf62ca5209a4a8f36f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:38:21 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Apr 2023 18:46:14 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Apr 2023 18:46:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Apr 2023 18:46:16 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:46:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:46:16 GMT
CMD ["traefik"]
# Thu, 06 Apr 2023 18:46:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096a495bd82a55e97c5be084787578b5b5af0321a33c70ccf19bca0dc260a981`  
		Last Modified: Wed, 29 Mar 2023 22:39:11 GMT  
		Size: 622.6 KB (622584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff0e0742f027721acb6e403cfd9c33f5035562626412821cf440ee0a0d4bd6`  
		Last Modified: Thu, 06 Apr 2023 18:46:41 GMT  
		Size: 34.5 MB (34539759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566cf6a3c532656d496f8fab7a8822e11cef4dd8c1dab24cdf229bbf359101eb`  
		Last Modified: Thu, 06 Apr 2023 18:46:36 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:banon-windowsservercore-1809`

```console
$ docker pull traefik@sha256:ec994d877f87622e6e0fe82b0ea8e3b3efabf1e0d8c57fe110f822b211243c08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:banon-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:38c71b3285dd02b9aa56ad826495f85e854606a04db526dcf7bf770ca9936a20
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2049781176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f645f991b33f438d120607abe7a2a158d8300068ceb916e0d7a6d2eaa095526e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Apr 2023 18:17:03 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 06 Apr 2023 18:17:04 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:17:05 GMT
ENTRYPOINT ["/traefik"]
# Thu, 06 Apr 2023 18:17:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b184b38bee4a888e16184a05c4770d36d87ad320077cbee08f12000fd700abed`  
		Last Modified: Thu, 06 Apr 2023 18:18:10 GMT  
		Size: 36.3 MB (36266505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32de5c550068bdd6a0e71f6aaae2c5ba100294dbb52006ca1247bc09cfb87e17`  
		Last Modified: Thu, 06 Apr 2023 18:18:00 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b65f112c430971f5c46a3133c30bd210125ddcf9493bca90d0553685871a5`  
		Last Modified: Thu, 06 Apr 2023 18:18:00 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8510431814f07a8c701f707dabf5daf9283df8769147fefe8634a06b3edf2a`  
		Last Modified: Thu, 06 Apr 2023 18:18:00 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:beaufort`

```console
$ docker pull traefik@sha256:0d7e8693e44e52588366695db63512b6b7a92d34b2145c2c3c732fec27ee03e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:beaufort` - linux; amd64

```console
$ docker pull traefik@sha256:a239deca1c7682fe9bb6a32e54364c7ff460205fa0e87c02bfeb66efb3f3a3d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40562953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42fc5a7c2d34a752fce6439cf3dc08ac747649d7712bc265c7dd7d1b38a2a45b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 02:37:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 02:37:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 02:37:35 GMT
EXPOSE 80
# Thu, 30 Mar 2023 02:37:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 02:37:35 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 02:37:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11624eb8d0cca298aa32848e39318bbc75ab1c404423d1d47c670fa60354e3`  
		Last Modified: Thu, 30 Mar 2023 02:38:16 GMT  
		Size: 661.1 KB (661099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9d40a9765a3ede8e4ec67030b20d484fedcea2ad98ee2b231ec3d86e6fd1b6`  
		Last Modified: Thu, 30 Mar 2023 02:38:21 GMT  
		Size: 37.1 MB (37074890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fca61e22e5a1dbbdeea08d3e394601c2c5492fc65d19af813ef66cc36a7d582`  
		Last Modified: Thu, 30 Mar 2023 02:38:15 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; arm variant v6

```console
$ docker pull traefik@sha256:5da0026b1e1053a9bcef582853c749291cf651f2bc1e35a557d87080e78a74f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38289884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d444fca66ffd358a663e6075b1d97f53a52bd6d11aa27afa1aa0b8cf4179f67`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:13 GMT
ADD file:3fb55ad8134002858be264c3c2477d784e4a60f2f6501afa7cf3b10bfede51aa in / 
# Wed, 29 Mar 2023 18:01:13 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 00:39:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 00:39:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 00:39:31 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:39:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 00:39:31 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 00:39:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:872c99a87729fa48dce303fb615edbb1a5da837f627a0b3d28495a0400ca8335`  
		Last Modified: Wed, 29 Mar 2023 18:02:12 GMT  
		Size: 2.6 MB (2634030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb226453f567b759ad92b5db4fa1f391e1eb96232b14d006147344b993d24773`  
		Last Modified: Thu, 30 Mar 2023 00:40:46 GMT  
		Size: 666.2 KB (666166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f676a5305470c023669ddf7351410e0d65fa65bcfe24fc65a2e567699f7c00e6`  
		Last Modified: Thu, 30 Mar 2023 00:40:52 GMT  
		Size: 35.0 MB (34989322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb744443f625044ceb56795d0847c66fe1957350cdaa3a296ad67d692876d308`  
		Last Modified: Thu, 30 Mar 2023 00:40:46 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:529410986a68c6e7989a5a08afa53d087795a2f1406977d5d6b183bfdfab65dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37408212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e4bfdbd12bed1c2e46296bb16021a1eea4269055e03fdf9e30c035e5f9e8dc4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 03:26:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 03:26:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 03:26:35 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:26:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 03:26:35 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 03:26:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d019fab0470c352dfa2ff6c01be8f1d0344d43e9431a28656e78c5cabd03e67f`  
		Last Modified: Thu, 30 Mar 2023 03:27:17 GMT  
		Size: 662.3 KB (662323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82ed46bb3966bf021d56f3bfda66ada1ddde7199ee9d3446ebcbeffec692004`  
		Last Modified: Thu, 30 Mar 2023 03:27:20 GMT  
		Size: 34.0 MB (34023520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a93ddfbde23c1aa20ccac6b7cd3dcbda52d11c2b1627d41dc7fa169bd46430`  
		Last Modified: Thu, 30 Mar 2023 03:27:16 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; s390x

```console
$ docker pull traefik@sha256:e8572896cf2369e9777be7e5ce1bce0b811642e09298039e0a9d51fa570172e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39131970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:194779f21f9e8eb09ec639ba646ce59761d5db6264648a5e162bf515e294517d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:07 GMT
ADD file:5cf392863cd9a0735de88f9e7dab93c9e74aca59ca05b792943cf3b621ea2c59 in / 
# Wed, 29 Mar 2023 17:42:07 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:38:08 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Mar 2023 22:38:14 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Mar 2023 22:38:15 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Mar 2023 22:38:16 GMT
EXPOSE 80
# Wed, 29 Mar 2023 22:38:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 22:38:16 GMT
CMD ["traefik"]
# Wed, 29 Mar 2023 22:38:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:1536575ac9c5f5fff4522c60d4610af0a52be584c36e652080c6c0ad169d4f27`  
		Last Modified: Wed, 29 Mar 2023 17:42:42 GMT  
		Size: 2.6 MB (2610636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246408072526d1b1e0fec7aaa14e46bd07b33c86c047b5d7cdce7778f992de28`  
		Last Modified: Wed, 29 Mar 2023 22:38:58 GMT  
		Size: 665.5 KB (665530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982fc64501c81b1c6a90bf3b79f669b6d16f9133509eb962541ae33f7f14c83c`  
		Last Modified: Wed, 29 Mar 2023 22:39:03 GMT  
		Size: 35.9 MB (35855437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b72fc0bf978c8423d98dc56a60760c0b3d12dbea0fd1524d98a88e3f173c6ab`  
		Last Modified: Wed, 29 Mar 2023 22:38:58 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:beaufort-windowsservercore-1809`

```console
$ docker pull traefik@sha256:2eb0d945da364a274f76288295b9120086404be2c7606fe340ac2ee6f1d64ed1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:beaufort-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:62e9db8356188c92dbce1706a8c2af3702993ee762b34d398fc7921eb03a3629
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2051205802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648f7c4938c24c605c3f3cbf0b16d4a5767ce075cd407fa9c6ab93e256035917`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 08:45:29 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 16 Mar 2023 08:45:30 GMT
EXPOSE 80
# Thu, 16 Mar 2023 08:45:31 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Mar 2023 08:45:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5eafb0300ea614e208e5052cfdd0941f2ad90a341c5b337ab489e223bb31e88`  
		Last Modified: Thu, 16 Mar 2023 08:49:24 GMT  
		Size: 37.7 MB (37691161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec0dc51e5d37193b3e6ebdd21f1bb94e44f593af5691b32af00720bb4548bbc`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28da668ed65b21bb734a5ba72dd5262a27de001c56a64bebf1db5e9244aaad4c`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6138998225adfde27a93f621c64ba53c628511ce9209f16661fd0c3619ff3e3`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:8d81a9df1435f9f3d36ac9398465ef2d5d61e671059974db753faaed14b627de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:6dee6938b5ebfc511a82ef4e09c80268835a2f67393e5c06c3e4ef9a14d1817b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39613072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1e26b5f8193d713eb8f39d0ab0e3d513278f86e41644b07e189e1aef536b335`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:38 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Apr 2023 18:24:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Apr 2023 18:24:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Apr 2023 18:24:44 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:24:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:24:44 GMT
CMD ["traefik"]
# Thu, 06 Apr 2023 18:24:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d055169f9c6f7e08b88a6ef90eba203750fcc51761ecb994e40aa2aaa640ff72`  
		Last Modified: Thu, 30 Mar 2023 02:38:35 GMT  
		Size: 622.2 KB (622239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afaddc85d79e665b30c4ee7ce9fc12425532f4695c6888b052086589f12aa687`  
		Last Modified: Thu, 06 Apr 2023 18:25:11 GMT  
		Size: 35.6 MB (35615902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff733a62a1272d7fe4817f1b3a8faf56c8a7f0e3808baec593378d274c1d081`  
		Last Modified: Thu, 06 Apr 2023 18:25:06 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f76a8f0c2b54429df275eb7e842171230994dc28924cb17f65ca41a3c5cb94fc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37257635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c077549480f6828d39797ca3855e6299d0c1e7daf08d67cd62320c07515ff0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:39 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Apr 2023 18:49:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Apr 2023 18:49:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Apr 2023 18:49:31 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:49:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:49:31 GMT
CMD ["traefik"]
# Thu, 06 Apr 2023 18:49:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bd7901efecc8425b6d98584a9ee5d091a238a8936fb50b8aa4654afb90d05d`  
		Last Modified: Thu, 30 Mar 2023 00:41:05 GMT  
		Size: 624.4 KB (624425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:658599efc3390617789f600a87686c808ae0c26e3a0a310ca9ad50944f5061f2`  
		Last Modified: Thu, 06 Apr 2023 18:49:58 GMT  
		Size: 33.5 MB (33522040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39827a939bd6089039662bd6dc0237923c0b6b7d177fcf7f37bdcb9dcaf831ee`  
		Last Modified: Thu, 06 Apr 2023 18:49:52 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7b1ecf3dcf9d504f037e14d060c7bfcb87ebde442eaf3c1d89e0c2e2f180a987
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.5 MB (36503424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fa39db0cea458044cad085ee32cf6bb615ccff2f3f7bbbc5e57f9b36984afb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Apr 2023 18:51:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Apr 2023 18:51:04 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Apr 2023 18:51:04 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:51:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:51:04 GMT
CMD ["traefik"]
# Thu, 06 Apr 2023 18:51:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4336eee5b1b811f9668d2251fb67e6099c4089ef7b26ade14aacd2f5f0982e06`  
		Last Modified: Thu, 30 Mar 2023 03:27:34 GMT  
		Size: 624.2 KB (624204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9cadb05aa1b060d980fd3437917259c39ca7d9fb914fccd2d05ba2c3ac9d1e`  
		Last Modified: Thu, 06 Apr 2023 18:51:28 GMT  
		Size: 32.6 MB (32616998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1371d2d81d70ec646fa25de2ef0e1ecbf8a73448a75536cdae53906746ee2605`  
		Last Modified: Thu, 06 Apr 2023 18:51:24 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; s390x

```console
$ docker pull traefik@sha256:40c157efc3aeb2a68be807c7bd9c56058b039f5dc04ea99a2d207f5694ba3498
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38337898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ed3cb8277e480dbe2a03868fd3de6e86d2381cb25b7d4cf62ca5209a4a8f36f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:38:21 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Apr 2023 18:46:14 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Apr 2023 18:46:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Apr 2023 18:46:16 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:46:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:46:16 GMT
CMD ["traefik"]
# Thu, 06 Apr 2023 18:46:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096a495bd82a55e97c5be084787578b5b5af0321a33c70ccf19bca0dc260a981`  
		Last Modified: Wed, 29 Mar 2023 22:39:11 GMT  
		Size: 622.6 KB (622584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff0e0742f027721acb6e403cfd9c33f5035562626412821cf440ee0a0d4bd6`  
		Last Modified: Thu, 06 Apr 2023 18:46:41 GMT  
		Size: 34.5 MB (34539759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566cf6a3c532656d496f8fab7a8822e11cef4dd8c1dab24cdf229bbf359101eb`  
		Last Modified: Thu, 06 Apr 2023 18:46:36 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles`

```console
$ docker pull traefik@sha256:5d47b7bb25467dbc27ab2b260e496a7f9e1232511af369cdcc98daefba7979c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles` - linux; amd64

```console
$ docker pull traefik@sha256:d7bacaf9ca8d59b0e7c304920629d98bb98a545127ca4b10e16c8b252b9351b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22593766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aae4b2c164f286aeee70180f0b85a66a5a3652a07d87cc658851db5e53c9b59a`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 07 Oct 2022 04:21:33 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Thu, 30 Mar 2023 02:37:59 GMT
COPY dir:fcb1de0a76c41fc3dff8d6ca27f999d211e86842b0843ac2ebdecb15ff8e0492 in /usr/share/ 
# Thu, 30 Mar 2023 02:38:00 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Thu, 30 Mar 2023 02:38:01 GMT
EXPOSE 80
# Thu, 30 Mar 2023 02:38:01 GMT
VOLUME [/tmp]
# Thu, 30 Mar 2023 02:38:01 GMT
ENTRYPOINT ["/traefik"]
# Thu, 30 Mar 2023 02:38:01 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:39006e619508cd8a1ace2dcb57ecaa3a206fc01c9b72018e30b538ba58b0f45a`  
		Last Modified: Fri, 07 Oct 2022 04:22:39 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ed5475338aea0040268938cdb4cf5e6d08120622d034f2fe282ade7fb88f34`  
		Last Modified: Thu, 30 Mar 2023 02:39:32 GMT  
		Size: 308.3 KB (308275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62941aba458e9caf3e4a66617f7b97e463e427c1ee961fbc3b0a37b3dedaf385`  
		Last Modified: Thu, 30 Mar 2023 02:39:36 GMT  
		Size: 22.2 MB (22161951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0eba228e1865efa7bed0cd8ca41b7d6cf14dcab9f1852e3754b7815aeded5d20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21055086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79cd7b650b4ab04f4e437d8c394fb6f2190aea6b3e738817ce9f2462a9d93211`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 14 Mar 2023 01:31:59 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Thu, 30 Mar 2023 00:40:30 GMT
COPY dir:fcb1de0a76c41fc3dff8d6ca27f999d211e86842b0843ac2ebdecb15ff8e0492 in /usr/share/ 
# Thu, 30 Mar 2023 00:40:31 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Thu, 30 Mar 2023 00:40:32 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:40:32 GMT
VOLUME [/tmp]
# Thu, 30 Mar 2023 00:40:32 GMT
ENTRYPOINT ["/traefik"]
# Thu, 30 Mar 2023 00:40:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:68a2bb2e7a38ecc0a394b8fde6e116d903af0a9081c1816df304ab9a95b081da`  
		Last Modified: Tue, 14 Mar 2023 01:34:18 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae617ce90fe46cea74fe5b74b5c0b409ee3f81c32e2bb9f1aefe371e24ebccc1`  
		Last Modified: Thu, 30 Mar 2023 00:42:02 GMT  
		Size: 308.3 KB (308265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296e5dd1d0ad1bc244926e357696aac4774dcebeb52a2723b33bf9269b3df2db`  
		Last Modified: Thu, 30 Mar 2023 00:42:06 GMT  
		Size: 20.6 MB (20623281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:324f12be044568e2f6d8229c848734927a52950051372f956304692aa2ff1a58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20563152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b41da85c4671491cd2a55c06fe1efb206c993b03f2d5f02f5113268616bf0f04`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 27 Oct 2022 23:00:59 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Thu, 30 Mar 2023 03:27:00 GMT
COPY dir:fcb1de0a76c41fc3dff8d6ca27f999d211e86842b0843ac2ebdecb15ff8e0492 in /usr/share/ 
# Thu, 30 Mar 2023 03:27:01 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Thu, 30 Mar 2023 03:27:01 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:27:01 GMT
VOLUME [/tmp]
# Thu, 30 Mar 2023 03:27:01 GMT
ENTRYPOINT ["/traefik"]
# Thu, 30 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:384a668e636c3a58c260d7eacd140f07b0727673d5ba128334cbcedd184a99f2`  
		Last Modified: Thu, 27 Oct 2022 23:02:00 GMT  
		Size: 123.5 KB (123538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcae1c052addf1a94540e967bada340c12bef5e3c6fa1fd315bdc81f3e2db29b`  
		Last Modified: Thu, 30 Mar 2023 03:28:23 GMT  
		Size: 308.3 KB (308267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42d66bc2a6eaad18db8aeaaba24844b6f3fcb88954cbef25552a284d0c967de`  
		Last Modified: Thu, 30 Mar 2023 03:28:26 GMT  
		Size: 20.1 MB (20131347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-alpine`

```console
$ docker pull traefik@sha256:7fa25a5a54a44ddab4d6b5e40bf03175ae617b460c0ee4a744b859edfdf12c9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:323f96e7b93b93d1f3939c65b6c6ab4dd682087c4cc6842506e0526ba3b5ec4a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25652617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5752638b830b09f8b8d33d381e137e483de2476e8f9d7123a1c7caa0a3640575`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:37 GMT
ADD file:9663235f252e072c52b0f9e25845841e4321cce2caa7467a0d736c6003b05c00 in / 
# Wed, 29 Mar 2023 18:19:37 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 02:37:54 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 02:37:54 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 02:37:54 GMT
EXPOSE 80
# Thu, 30 Mar 2023 02:37:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 02:37:54 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 02:37:54 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f7dab3ab2d6ec29aa28769bec35331fb485b5837501b1e8556413d8b5a79c9c8`  
		Last Modified: Wed, 29 Mar 2023 18:20:25 GMT  
		Size: 2.8 MB (2829647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b336280e0077663b6ff48976dade0f4b39627828c80e6252ef3cbd195787a2`  
		Last Modified: Thu, 30 Mar 2023 02:39:15 GMT  
		Size: 660.5 KB (660537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9c0a6f6f71f1e51f885a6ef76ef507f598a8becb11334ab2eedda32ed2bf3d`  
		Last Modified: Thu, 30 Mar 2023 02:39:19 GMT  
		Size: 22.2 MB (22162065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfa1a444c49c4a20dc38ba06b91a7def26bd40e67624aaa412af8ae47e962cd`  
		Last Modified: Thu, 30 Mar 2023 02:39:15 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:7f9dabda3415134f3c6c55aa1c6d4a9714df3e6c1b17c09fa6829518be40304e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23928182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:989b6b4695cc561a8362ad5d755b293faf05ef51a2213c0f68940138fe65fd46`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:15 GMT
ADD file:1039802413c644346f599dac53a7c6dabd123027756231b9d8f64a1068c9779d in / 
# Wed, 29 Mar 2023 18:01:15 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:57 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 00:40:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 00:40:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 00:40:01 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:40:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 00:40:01 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 00:40:01 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ffeb76b9ee2f52d46487f4f9a7074ea62dea819a2dd53c9a2c6d703ca7b5aa06`  
		Last Modified: Wed, 29 Mar 2023 18:02:21 GMT  
		Size: 2.6 MB (2638259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b1182fcb4f775d878f0b8af17e60fdef00a0afb3a68f68731fdf08ca613566`  
		Last Modified: Thu, 30 Mar 2023 00:41:46 GMT  
		Size: 666.1 KB (666134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ace3e9b5f4c3d44312fca26e27d43459ab4671204cc813ae1a2d94bc295e24`  
		Last Modified: Thu, 30 Mar 2023 00:41:49 GMT  
		Size: 20.6 MB (20623422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fec87c1bbd8ed5033ef249c444c828c0d4a024613f7c067d6408df986bd229a`  
		Last Modified: Thu, 30 Mar 2023 00:41:46 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:604a02479b2cd6d49eefd5f24cc81497d3af5f7bc33c21d1cae3881779219515
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23519179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fe0b5ab962401db114bc8e05b69ff178950436ca17116fe2fd64b3189aa0acc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:25 GMT
ADD file:c3d52cc254959a9ff493e7347e6b1bc25c0ccfdcf9532dbf43173ddd182d0e4d in / 
# Wed, 29 Mar 2023 17:39:25 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:49 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 03:26:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 03:26:51 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 03:26:51 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:26:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 03:26:51 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 03:26:52 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:422ed46b1a92579f7c475c0c19fade6880a8d98f23a2b4ccfb77c265d4f72dfc`  
		Last Modified: Wed, 29 Mar 2023 17:40:13 GMT  
		Size: 2.7 MB (2725148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6752cbc5332b159f041b740aaa55aae27464ed4eccd5bef82a29db3a8910c02b`  
		Last Modified: Thu, 30 Mar 2023 03:28:09 GMT  
		Size: 662.3 KB (662304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77516a6a2e38caf662af65c73d4bed11e3775022a478ffb8c84004d4dcbc6f82`  
		Last Modified: Thu, 30 Mar 2023 03:28:11 GMT  
		Size: 20.1 MB (20131360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8cf26694e550c02564e364e7285e5830c82ec691f8de5269c861084468777b`  
		Last Modified: Thu, 30 Mar 2023 03:28:08 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f643d6e3857163a610f6ee48dcedefc4ae1c6957968b821a132c45dad295521d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:eb030d1415b37297490d0d042c132510d0592f8158bb80f98328bebe132c71c7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2036484756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd883fc0a81df58f398881ad9a26665e14af2ff944186704211ca53de351d281`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 08:48:48 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 16 Mar 2023 08:48:49 GMT
EXPOSE 80
# Thu, 16 Mar 2023 08:48:50 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Mar 2023 08:48:51 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c40e4a974e18ba73f3964c77bafb530b44a02b157bff67d57d80b50a37d306`  
		Last Modified: Thu, 16 Mar 2023 08:50:12 GMT  
		Size: 23.0 MB (22970100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b8a1819bca4f2eb81e780d11f83ab69e9c936aeaddbd31803a9949cf487145`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5590048d6ec03d383585a24a3e40df19cce710181b483bb92abd200c87c856`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbdbd264f1bd9f178ca6c87b2073841bac0e4226b3fed4145bbdb0c46e98ca1`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:saintmarcelin`

```console
$ docker pull traefik@sha256:90f12602b0cb4df586fe90d3aacfdcf34b2e72253bcd01167ec6d670b631d39e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:saintmarcelin` - linux; amd64

```console
$ docker pull traefik@sha256:e740be22cd324a87119d2091a70e8c89c7f8a0f83913caa7dbc098c40ed01b44
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40979650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31d787e98af349f3ec4332f4d1cebf0555523271d40666e6d462dccec7c88872`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:38 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Apr 2023 22:20:57 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.0-rc2/traefik_v2.10.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Apr 2023 22:20:57 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Apr 2023 22:20:57 GMT
EXPOSE 80
# Fri, 07 Apr 2023 22:20:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Apr 2023 22:20:57 GMT
CMD ["traefik"]
# Fri, 07 Apr 2023 22:20:57 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d055169f9c6f7e08b88a6ef90eba203750fcc51761ecb994e40aa2aaa640ff72`  
		Last Modified: Thu, 30 Mar 2023 02:38:35 GMT  
		Size: 622.2 KB (622239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4680b9aefc39947986fb5f7d0fbb6c51f79b9fee726231e6e22799985ada11e`  
		Last Modified: Fri, 07 Apr 2023 22:21:24 GMT  
		Size: 37.0 MB (36982480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c40271a2c0502a46ca8dca99a5196da7cac0b078453a70a90877bee34cb6a45c`  
		Last Modified: Fri, 07 Apr 2023 22:21:18 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; arm variant v6

```console
$ docker pull traefik@sha256:b45b8ce39f0f0a648e61c21b78a9a25f550969461997e9af661154f37e6c636f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37335481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:741d6b598348314376ea260c1fea9a9a81a56894b53da44daa8e972f4b6bf799`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:39 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 00:39:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.0-rc1/traefik_v2.10.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 00:39:53 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 00:39:53 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:39:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 00:39:53 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 00:39:53 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bd7901efecc8425b6d98584a9ee5d091a238a8936fb50b8aa4654afb90d05d`  
		Last Modified: Thu, 30 Mar 2023 00:41:05 GMT  
		Size: 624.4 KB (624425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc684a14f3623efaff9c3ff5a04d8dd15013918bff353a56fe64ba0ed9cc998b`  
		Last Modified: Thu, 30 Mar 2023 00:41:31 GMT  
		Size: 33.6 MB (33599887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d08a29db0e624938a5852b6f5752c900006cef7a5d8b305b400c6b9767a8e5`  
		Last Modified: Thu, 30 Mar 2023 00:41:25 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:4ac10aadbf80be52435784c32ad9fd4d80a95c949d12ff85e480ed0d0ce388ae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.6 MB (36598696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17449690bd237d6b44fdcfccf02d14b68f850e33f0476c25b6323f0f78539e30`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 03:26:45 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.0-rc1/traefik_v2.10.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 03:26:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 03:26:46 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:26:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 03:26:46 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 03:26:46 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4336eee5b1b811f9668d2251fb67e6099c4089ef7b26ade14aacd2f5f0982e06`  
		Last Modified: Thu, 30 Mar 2023 03:27:34 GMT  
		Size: 624.2 KB (624204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f80e6c463b9b292f88426c5afa82893107ee14f8f24ab7bbb5e1775e074ad7b0`  
		Last Modified: Thu, 30 Mar 2023 03:27:56 GMT  
		Size: 32.7 MB (32712271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68471cc27eba1f51573559a697edac9f1b8473bf301734e6d08d630fcb89288f`  
		Last Modified: Thu, 30 Mar 2023 03:27:52 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; s390x

```console
$ docker pull traefik@sha256:25628239cc46999c02e0e8468645f4d310276777bc9473fd83e740ef6d3138cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38416622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fd82d431bd0f17307f89ce4d5c99653fb6f91c9f51965591d424410e6d25f9e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:38:21 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Mar 2023 22:38:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.0-rc1/traefik_v2.10.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Mar 2023 22:38:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Mar 2023 22:38:39 GMT
EXPOSE 80
# Wed, 29 Mar 2023 22:38:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 22:38:40 GMT
CMD ["traefik"]
# Wed, 29 Mar 2023 22:38:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096a495bd82a55e97c5be084787578b5b5af0321a33c70ccf19bca0dc260a981`  
		Last Modified: Wed, 29 Mar 2023 22:39:11 GMT  
		Size: 622.6 KB (622584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6483277d1e50cb2a0b9fdcebf8901f64c898d7042e19bea5f36a5982a9c262`  
		Last Modified: Wed, 29 Mar 2023 22:39:32 GMT  
		Size: 34.6 MB (34618483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f079c1b0af8d690151aa9187d4308985a20f7ac72e4916f72e429e87a3dbf9`  
		Last Modified: Wed, 29 Mar 2023 22:39:26 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:saintmarcelin-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e06b8c9a11f534829f3f075965ea66db0848b8c65075ac79790ab13631922a8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:saintmarcelin-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:290c74bd221d9156e894120db45f83e6c3073414ae4726b33a6c5394aad11ced
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2051118218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12766268c3909b8aea4982e046e39d57a153a1a283de0210d852fd225fb75428`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 07 Apr 2023 22:17:15 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.0-rc2/traefik_v2.10.0-rc2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Fri, 07 Apr 2023 22:17:16 GMT
EXPOSE 80
# Fri, 07 Apr 2023 22:17:17 GMT
ENTRYPOINT ["/traefik"]
# Fri, 07 Apr 2023 22:17:17 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57437d77990e17f6f1c4de8c842c9be99cc65894850bdf5fda3ce6ad610bc94`  
		Last Modified: Fri, 07 Apr 2023 22:18:11 GMT  
		Size: 37.6 MB (37603585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9b44ad239fc25c916d9b6fd60d1ee079b9827218883933725f6c452eedcb20`  
		Last Modified: Fri, 07 Apr 2023 22:18:03 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb69fbbb0a60fb6bf98cbfdfc0c3fc66801acb7bcd8c847cc43aa78fa8128a3`  
		Last Modified: Fri, 07 Apr 2023 22:18:03 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d5bdf56292275f8e72e015f1c9d64eb2d9d4ee6ddde77defa0866df6a3bbe4`  
		Last Modified: Fri, 07 Apr 2023 22:18:03 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7`

```console
$ docker pull traefik@sha256:5d47b7bb25467dbc27ab2b260e496a7f9e1232511af369cdcc98daefba7979c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7` - linux; amd64

```console
$ docker pull traefik@sha256:d7bacaf9ca8d59b0e7c304920629d98bb98a545127ca4b10e16c8b252b9351b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22593766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aae4b2c164f286aeee70180f0b85a66a5a3652a07d87cc658851db5e53c9b59a`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 07 Oct 2022 04:21:33 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Thu, 30 Mar 2023 02:37:59 GMT
COPY dir:fcb1de0a76c41fc3dff8d6ca27f999d211e86842b0843ac2ebdecb15ff8e0492 in /usr/share/ 
# Thu, 30 Mar 2023 02:38:00 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Thu, 30 Mar 2023 02:38:01 GMT
EXPOSE 80
# Thu, 30 Mar 2023 02:38:01 GMT
VOLUME [/tmp]
# Thu, 30 Mar 2023 02:38:01 GMT
ENTRYPOINT ["/traefik"]
# Thu, 30 Mar 2023 02:38:01 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:39006e619508cd8a1ace2dcb57ecaa3a206fc01c9b72018e30b538ba58b0f45a`  
		Last Modified: Fri, 07 Oct 2022 04:22:39 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ed5475338aea0040268938cdb4cf5e6d08120622d034f2fe282ade7fb88f34`  
		Last Modified: Thu, 30 Mar 2023 02:39:32 GMT  
		Size: 308.3 KB (308275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62941aba458e9caf3e4a66617f7b97e463e427c1ee961fbc3b0a37b3dedaf385`  
		Last Modified: Thu, 30 Mar 2023 02:39:36 GMT  
		Size: 22.2 MB (22161951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0eba228e1865efa7bed0cd8ca41b7d6cf14dcab9f1852e3754b7815aeded5d20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21055086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79cd7b650b4ab04f4e437d8c394fb6f2190aea6b3e738817ce9f2462a9d93211`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 14 Mar 2023 01:31:59 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Thu, 30 Mar 2023 00:40:30 GMT
COPY dir:fcb1de0a76c41fc3dff8d6ca27f999d211e86842b0843ac2ebdecb15ff8e0492 in /usr/share/ 
# Thu, 30 Mar 2023 00:40:31 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Thu, 30 Mar 2023 00:40:32 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:40:32 GMT
VOLUME [/tmp]
# Thu, 30 Mar 2023 00:40:32 GMT
ENTRYPOINT ["/traefik"]
# Thu, 30 Mar 2023 00:40:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:68a2bb2e7a38ecc0a394b8fde6e116d903af0a9081c1816df304ab9a95b081da`  
		Last Modified: Tue, 14 Mar 2023 01:34:18 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae617ce90fe46cea74fe5b74b5c0b409ee3f81c32e2bb9f1aefe371e24ebccc1`  
		Last Modified: Thu, 30 Mar 2023 00:42:02 GMT  
		Size: 308.3 KB (308265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296e5dd1d0ad1bc244926e357696aac4774dcebeb52a2723b33bf9269b3df2db`  
		Last Modified: Thu, 30 Mar 2023 00:42:06 GMT  
		Size: 20.6 MB (20623281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:324f12be044568e2f6d8229c848734927a52950051372f956304692aa2ff1a58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20563152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b41da85c4671491cd2a55c06fe1efb206c993b03f2d5f02f5113268616bf0f04`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 27 Oct 2022 23:00:59 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Thu, 30 Mar 2023 03:27:00 GMT
COPY dir:fcb1de0a76c41fc3dff8d6ca27f999d211e86842b0843ac2ebdecb15ff8e0492 in /usr/share/ 
# Thu, 30 Mar 2023 03:27:01 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Thu, 30 Mar 2023 03:27:01 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:27:01 GMT
VOLUME [/tmp]
# Thu, 30 Mar 2023 03:27:01 GMT
ENTRYPOINT ["/traefik"]
# Thu, 30 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:384a668e636c3a58c260d7eacd140f07b0727673d5ba128334cbcedd184a99f2`  
		Last Modified: Thu, 27 Oct 2022 23:02:00 GMT  
		Size: 123.5 KB (123538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcae1c052addf1a94540e967bada340c12bef5e3c6fa1fd315bdc81f3e2db29b`  
		Last Modified: Thu, 30 Mar 2023 03:28:23 GMT  
		Size: 308.3 KB (308267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42d66bc2a6eaad18db8aeaaba24844b6f3fcb88954cbef25552a284d0c967de`  
		Last Modified: Thu, 30 Mar 2023 03:28:26 GMT  
		Size: 20.1 MB (20131347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-alpine`

```console
$ docker pull traefik@sha256:7fa25a5a54a44ddab4d6b5e40bf03175ae617b460c0ee4a744b859edfdf12c9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:323f96e7b93b93d1f3939c65b6c6ab4dd682087c4cc6842506e0526ba3b5ec4a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25652617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5752638b830b09f8b8d33d381e137e483de2476e8f9d7123a1c7caa0a3640575`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:37 GMT
ADD file:9663235f252e072c52b0f9e25845841e4321cce2caa7467a0d736c6003b05c00 in / 
# Wed, 29 Mar 2023 18:19:37 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 02:37:54 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 02:37:54 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 02:37:54 GMT
EXPOSE 80
# Thu, 30 Mar 2023 02:37:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 02:37:54 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 02:37:54 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f7dab3ab2d6ec29aa28769bec35331fb485b5837501b1e8556413d8b5a79c9c8`  
		Last Modified: Wed, 29 Mar 2023 18:20:25 GMT  
		Size: 2.8 MB (2829647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b336280e0077663b6ff48976dade0f4b39627828c80e6252ef3cbd195787a2`  
		Last Modified: Thu, 30 Mar 2023 02:39:15 GMT  
		Size: 660.5 KB (660537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9c0a6f6f71f1e51f885a6ef76ef507f598a8becb11334ab2eedda32ed2bf3d`  
		Last Modified: Thu, 30 Mar 2023 02:39:19 GMT  
		Size: 22.2 MB (22162065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfa1a444c49c4a20dc38ba06b91a7def26bd40e67624aaa412af8ae47e962cd`  
		Last Modified: Thu, 30 Mar 2023 02:39:15 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:7f9dabda3415134f3c6c55aa1c6d4a9714df3e6c1b17c09fa6829518be40304e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23928182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:989b6b4695cc561a8362ad5d755b293faf05ef51a2213c0f68940138fe65fd46`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:15 GMT
ADD file:1039802413c644346f599dac53a7c6dabd123027756231b9d8f64a1068c9779d in / 
# Wed, 29 Mar 2023 18:01:15 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:57 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 00:40:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 00:40:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 00:40:01 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:40:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 00:40:01 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 00:40:01 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ffeb76b9ee2f52d46487f4f9a7074ea62dea819a2dd53c9a2c6d703ca7b5aa06`  
		Last Modified: Wed, 29 Mar 2023 18:02:21 GMT  
		Size: 2.6 MB (2638259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b1182fcb4f775d878f0b8af17e60fdef00a0afb3a68f68731fdf08ca613566`  
		Last Modified: Thu, 30 Mar 2023 00:41:46 GMT  
		Size: 666.1 KB (666134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ace3e9b5f4c3d44312fca26e27d43459ab4671204cc813ae1a2d94bc295e24`  
		Last Modified: Thu, 30 Mar 2023 00:41:49 GMT  
		Size: 20.6 MB (20623422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fec87c1bbd8ed5033ef249c444c828c0d4a024613f7c067d6408df986bd229a`  
		Last Modified: Thu, 30 Mar 2023 00:41:46 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:604a02479b2cd6d49eefd5f24cc81497d3af5f7bc33c21d1cae3881779219515
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23519179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fe0b5ab962401db114bc8e05b69ff178950436ca17116fe2fd64b3189aa0acc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:25 GMT
ADD file:c3d52cc254959a9ff493e7347e6b1bc25c0ccfdcf9532dbf43173ddd182d0e4d in / 
# Wed, 29 Mar 2023 17:39:25 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:49 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 03:26:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 03:26:51 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 03:26:51 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:26:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 03:26:51 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 03:26:52 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:422ed46b1a92579f7c475c0c19fade6880a8d98f23a2b4ccfb77c265d4f72dfc`  
		Last Modified: Wed, 29 Mar 2023 17:40:13 GMT  
		Size: 2.7 MB (2725148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6752cbc5332b159f041b740aaa55aae27464ed4eccd5bef82a29db3a8910c02b`  
		Last Modified: Thu, 30 Mar 2023 03:28:09 GMT  
		Size: 662.3 KB (662304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77516a6a2e38caf662af65c73d4bed11e3775022a478ffb8c84004d4dcbc6f82`  
		Last Modified: Thu, 30 Mar 2023 03:28:11 GMT  
		Size: 20.1 MB (20131360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8cf26694e550c02564e364e7285e5830c82ec691f8de5269c861084468777b`  
		Last Modified: Thu, 30 Mar 2023 03:28:08 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f643d6e3857163a610f6ee48dcedefc4ae1c6957968b821a132c45dad295521d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:v1.7-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:eb030d1415b37297490d0d042c132510d0592f8158bb80f98328bebe132c71c7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2036484756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd883fc0a81df58f398881ad9a26665e14af2ff944186704211ca53de351d281`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 08:48:48 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 16 Mar 2023 08:48:49 GMT
EXPOSE 80
# Thu, 16 Mar 2023 08:48:50 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Mar 2023 08:48:51 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c40e4a974e18ba73f3964c77bafb530b44a02b157bff67d57d80b50a37d306`  
		Last Modified: Thu, 16 Mar 2023 08:50:12 GMT  
		Size: 23.0 MB (22970100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b8a1819bca4f2eb81e780d11f83ab69e9c936aeaddbd31803a9949cf487145`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5590048d6ec03d383585a24a3e40df19cce710181b483bb92abd200c87c856`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbdbd264f1bd9f178ca6c87b2073841bac0e4226b3fed4145bbdb0c46e98ca1`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.34`

```console
$ docker pull traefik@sha256:5d47b7bb25467dbc27ab2b260e496a7f9e1232511af369cdcc98daefba7979c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.34` - linux; amd64

```console
$ docker pull traefik@sha256:d7bacaf9ca8d59b0e7c304920629d98bb98a545127ca4b10e16c8b252b9351b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22593766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aae4b2c164f286aeee70180f0b85a66a5a3652a07d87cc658851db5e53c9b59a`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 07 Oct 2022 04:21:33 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Thu, 30 Mar 2023 02:37:59 GMT
COPY dir:fcb1de0a76c41fc3dff8d6ca27f999d211e86842b0843ac2ebdecb15ff8e0492 in /usr/share/ 
# Thu, 30 Mar 2023 02:38:00 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Thu, 30 Mar 2023 02:38:01 GMT
EXPOSE 80
# Thu, 30 Mar 2023 02:38:01 GMT
VOLUME [/tmp]
# Thu, 30 Mar 2023 02:38:01 GMT
ENTRYPOINT ["/traefik"]
# Thu, 30 Mar 2023 02:38:01 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:39006e619508cd8a1ace2dcb57ecaa3a206fc01c9b72018e30b538ba58b0f45a`  
		Last Modified: Fri, 07 Oct 2022 04:22:39 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ed5475338aea0040268938cdb4cf5e6d08120622d034f2fe282ade7fb88f34`  
		Last Modified: Thu, 30 Mar 2023 02:39:32 GMT  
		Size: 308.3 KB (308275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62941aba458e9caf3e4a66617f7b97e463e427c1ee961fbc3b0a37b3dedaf385`  
		Last Modified: Thu, 30 Mar 2023 02:39:36 GMT  
		Size: 22.2 MB (22161951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.34` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0eba228e1865efa7bed0cd8ca41b7d6cf14dcab9f1852e3754b7815aeded5d20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21055086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79cd7b650b4ab04f4e437d8c394fb6f2190aea6b3e738817ce9f2462a9d93211`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 14 Mar 2023 01:31:59 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Thu, 30 Mar 2023 00:40:30 GMT
COPY dir:fcb1de0a76c41fc3dff8d6ca27f999d211e86842b0843ac2ebdecb15ff8e0492 in /usr/share/ 
# Thu, 30 Mar 2023 00:40:31 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Thu, 30 Mar 2023 00:40:32 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:40:32 GMT
VOLUME [/tmp]
# Thu, 30 Mar 2023 00:40:32 GMT
ENTRYPOINT ["/traefik"]
# Thu, 30 Mar 2023 00:40:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:68a2bb2e7a38ecc0a394b8fde6e116d903af0a9081c1816df304ab9a95b081da`  
		Last Modified: Tue, 14 Mar 2023 01:34:18 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae617ce90fe46cea74fe5b74b5c0b409ee3f81c32e2bb9f1aefe371e24ebccc1`  
		Last Modified: Thu, 30 Mar 2023 00:42:02 GMT  
		Size: 308.3 KB (308265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296e5dd1d0ad1bc244926e357696aac4774dcebeb52a2723b33bf9269b3df2db`  
		Last Modified: Thu, 30 Mar 2023 00:42:06 GMT  
		Size: 20.6 MB (20623281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.34` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:324f12be044568e2f6d8229c848734927a52950051372f956304692aa2ff1a58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20563152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b41da85c4671491cd2a55c06fe1efb206c993b03f2d5f02f5113268616bf0f04`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 27 Oct 2022 23:00:59 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Thu, 30 Mar 2023 03:27:00 GMT
COPY dir:fcb1de0a76c41fc3dff8d6ca27f999d211e86842b0843ac2ebdecb15ff8e0492 in /usr/share/ 
# Thu, 30 Mar 2023 03:27:01 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Thu, 30 Mar 2023 03:27:01 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:27:01 GMT
VOLUME [/tmp]
# Thu, 30 Mar 2023 03:27:01 GMT
ENTRYPOINT ["/traefik"]
# Thu, 30 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:384a668e636c3a58c260d7eacd140f07b0727673d5ba128334cbcedd184a99f2`  
		Last Modified: Thu, 27 Oct 2022 23:02:00 GMT  
		Size: 123.5 KB (123538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcae1c052addf1a94540e967bada340c12bef5e3c6fa1fd315bdc81f3e2db29b`  
		Last Modified: Thu, 30 Mar 2023 03:28:23 GMT  
		Size: 308.3 KB (308267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42d66bc2a6eaad18db8aeaaba24844b6f3fcb88954cbef25552a284d0c967de`  
		Last Modified: Thu, 30 Mar 2023 03:28:26 GMT  
		Size: 20.1 MB (20131347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.34-alpine`

```console
$ docker pull traefik@sha256:7fa25a5a54a44ddab4d6b5e40bf03175ae617b460c0ee4a744b859edfdf12c9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.34-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:323f96e7b93b93d1f3939c65b6c6ab4dd682087c4cc6842506e0526ba3b5ec4a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25652617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5752638b830b09f8b8d33d381e137e483de2476e8f9d7123a1c7caa0a3640575`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:37 GMT
ADD file:9663235f252e072c52b0f9e25845841e4321cce2caa7467a0d736c6003b05c00 in / 
# Wed, 29 Mar 2023 18:19:37 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 02:37:54 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 02:37:54 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 02:37:54 GMT
EXPOSE 80
# Thu, 30 Mar 2023 02:37:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 02:37:54 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 02:37:54 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f7dab3ab2d6ec29aa28769bec35331fb485b5837501b1e8556413d8b5a79c9c8`  
		Last Modified: Wed, 29 Mar 2023 18:20:25 GMT  
		Size: 2.8 MB (2829647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b336280e0077663b6ff48976dade0f4b39627828c80e6252ef3cbd195787a2`  
		Last Modified: Thu, 30 Mar 2023 02:39:15 GMT  
		Size: 660.5 KB (660537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9c0a6f6f71f1e51f885a6ef76ef507f598a8becb11334ab2eedda32ed2bf3d`  
		Last Modified: Thu, 30 Mar 2023 02:39:19 GMT  
		Size: 22.2 MB (22162065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfa1a444c49c4a20dc38ba06b91a7def26bd40e67624aaa412af8ae47e962cd`  
		Last Modified: Thu, 30 Mar 2023 02:39:15 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.34-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:7f9dabda3415134f3c6c55aa1c6d4a9714df3e6c1b17c09fa6829518be40304e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23928182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:989b6b4695cc561a8362ad5d755b293faf05ef51a2213c0f68940138fe65fd46`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:15 GMT
ADD file:1039802413c644346f599dac53a7c6dabd123027756231b9d8f64a1068c9779d in / 
# Wed, 29 Mar 2023 18:01:15 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:57 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 00:40:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 00:40:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 00:40:01 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:40:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 00:40:01 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 00:40:01 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ffeb76b9ee2f52d46487f4f9a7074ea62dea819a2dd53c9a2c6d703ca7b5aa06`  
		Last Modified: Wed, 29 Mar 2023 18:02:21 GMT  
		Size: 2.6 MB (2638259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b1182fcb4f775d878f0b8af17e60fdef00a0afb3a68f68731fdf08ca613566`  
		Last Modified: Thu, 30 Mar 2023 00:41:46 GMT  
		Size: 666.1 KB (666134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ace3e9b5f4c3d44312fca26e27d43459ab4671204cc813ae1a2d94bc295e24`  
		Last Modified: Thu, 30 Mar 2023 00:41:49 GMT  
		Size: 20.6 MB (20623422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fec87c1bbd8ed5033ef249c444c828c0d4a024613f7c067d6408df986bd229a`  
		Last Modified: Thu, 30 Mar 2023 00:41:46 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.34-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:604a02479b2cd6d49eefd5f24cc81497d3af5f7bc33c21d1cae3881779219515
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23519179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fe0b5ab962401db114bc8e05b69ff178950436ca17116fe2fd64b3189aa0acc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:25 GMT
ADD file:c3d52cc254959a9ff493e7347e6b1bc25c0ccfdcf9532dbf43173ddd182d0e4d in / 
# Wed, 29 Mar 2023 17:39:25 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:49 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 03:26:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 03:26:51 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 03:26:51 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:26:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 03:26:51 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 03:26:52 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:422ed46b1a92579f7c475c0c19fade6880a8d98f23a2b4ccfb77c265d4f72dfc`  
		Last Modified: Wed, 29 Mar 2023 17:40:13 GMT  
		Size: 2.7 MB (2725148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6752cbc5332b159f041b740aaa55aae27464ed4eccd5bef82a29db3a8910c02b`  
		Last Modified: Thu, 30 Mar 2023 03:28:09 GMT  
		Size: 662.3 KB (662304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77516a6a2e38caf662af65c73d4bed11e3775022a478ffb8c84004d4dcbc6f82`  
		Last Modified: Thu, 30 Mar 2023 03:28:11 GMT  
		Size: 20.1 MB (20131360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8cf26694e550c02564e364e7285e5830c82ec691f8de5269c861084468777b`  
		Last Modified: Thu, 30 Mar 2023 03:28:08 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.34-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f643d6e3857163a610f6ee48dcedefc4ae1c6957968b821a132c45dad295521d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:v1.7.34-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:eb030d1415b37297490d0d042c132510d0592f8158bb80f98328bebe132c71c7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2036484756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd883fc0a81df58f398881ad9a26665e14af2ff944186704211ca53de351d281`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 08:48:48 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 16 Mar 2023 08:48:49 GMT
EXPOSE 80
# Thu, 16 Mar 2023 08:48:50 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Mar 2023 08:48:51 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c40e4a974e18ba73f3964c77bafb530b44a02b157bff67d57d80b50a37d306`  
		Last Modified: Thu, 16 Mar 2023 08:50:12 GMT  
		Size: 23.0 MB (22970100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b8a1819bca4f2eb81e780d11f83ab69e9c936aeaddbd31803a9949cf487145`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5590048d6ec03d383585a24a3e40df19cce710181b483bb92abd200c87c856`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbdbd264f1bd9f178ca6c87b2073841bac0e4226b3fed4145bbdb0c46e98ca1`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10`

```console
$ docker pull traefik@sha256:90f12602b0cb4df586fe90d3aacfdcf34b2e72253bcd01167ec6d670b631d39e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.10` - linux; amd64

```console
$ docker pull traefik@sha256:e740be22cd324a87119d2091a70e8c89c7f8a0f83913caa7dbc098c40ed01b44
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40979650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31d787e98af349f3ec4332f4d1cebf0555523271d40666e6d462dccec7c88872`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:38 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Apr 2023 22:20:57 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.0-rc2/traefik_v2.10.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Apr 2023 22:20:57 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Apr 2023 22:20:57 GMT
EXPOSE 80
# Fri, 07 Apr 2023 22:20:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Apr 2023 22:20:57 GMT
CMD ["traefik"]
# Fri, 07 Apr 2023 22:20:57 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d055169f9c6f7e08b88a6ef90eba203750fcc51761ecb994e40aa2aaa640ff72`  
		Last Modified: Thu, 30 Mar 2023 02:38:35 GMT  
		Size: 622.2 KB (622239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4680b9aefc39947986fb5f7d0fbb6c51f79b9fee726231e6e22799985ada11e`  
		Last Modified: Fri, 07 Apr 2023 22:21:24 GMT  
		Size: 37.0 MB (36982480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c40271a2c0502a46ca8dca99a5196da7cac0b078453a70a90877bee34cb6a45c`  
		Last Modified: Fri, 07 Apr 2023 22:21:18 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10` - linux; arm variant v6

```console
$ docker pull traefik@sha256:b45b8ce39f0f0a648e61c21b78a9a25f550969461997e9af661154f37e6c636f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37335481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:741d6b598348314376ea260c1fea9a9a81a56894b53da44daa8e972f4b6bf799`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:39 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 00:39:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.0-rc1/traefik_v2.10.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 00:39:53 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 00:39:53 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:39:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 00:39:53 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 00:39:53 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bd7901efecc8425b6d98584a9ee5d091a238a8936fb50b8aa4654afb90d05d`  
		Last Modified: Thu, 30 Mar 2023 00:41:05 GMT  
		Size: 624.4 KB (624425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc684a14f3623efaff9c3ff5a04d8dd15013918bff353a56fe64ba0ed9cc998b`  
		Last Modified: Thu, 30 Mar 2023 00:41:31 GMT  
		Size: 33.6 MB (33599887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d08a29db0e624938a5852b6f5752c900006cef7a5d8b305b400c6b9767a8e5`  
		Last Modified: Thu, 30 Mar 2023 00:41:25 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:4ac10aadbf80be52435784c32ad9fd4d80a95c949d12ff85e480ed0d0ce388ae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.6 MB (36598696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17449690bd237d6b44fdcfccf02d14b68f850e33f0476c25b6323f0f78539e30`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 03:26:45 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.0-rc1/traefik_v2.10.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 03:26:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 03:26:46 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:26:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 03:26:46 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 03:26:46 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4336eee5b1b811f9668d2251fb67e6099c4089ef7b26ade14aacd2f5f0982e06`  
		Last Modified: Thu, 30 Mar 2023 03:27:34 GMT  
		Size: 624.2 KB (624204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f80e6c463b9b292f88426c5afa82893107ee14f8f24ab7bbb5e1775e074ad7b0`  
		Last Modified: Thu, 30 Mar 2023 03:27:56 GMT  
		Size: 32.7 MB (32712271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68471cc27eba1f51573559a697edac9f1b8473bf301734e6d08d630fcb89288f`  
		Last Modified: Thu, 30 Mar 2023 03:27:52 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10` - linux; s390x

```console
$ docker pull traefik@sha256:25628239cc46999c02e0e8468645f4d310276777bc9473fd83e740ef6d3138cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38416622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fd82d431bd0f17307f89ce4d5c99653fb6f91c9f51965591d424410e6d25f9e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:38:21 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Mar 2023 22:38:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.0-rc1/traefik_v2.10.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Mar 2023 22:38:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Mar 2023 22:38:39 GMT
EXPOSE 80
# Wed, 29 Mar 2023 22:38:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 22:38:40 GMT
CMD ["traefik"]
# Wed, 29 Mar 2023 22:38:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096a495bd82a55e97c5be084787578b5b5af0321a33c70ccf19bca0dc260a981`  
		Last Modified: Wed, 29 Mar 2023 22:39:11 GMT  
		Size: 622.6 KB (622584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6483277d1e50cb2a0b9fdcebf8901f64c898d7042e19bea5f36a5982a9c262`  
		Last Modified: Wed, 29 Mar 2023 22:39:32 GMT  
		Size: 34.6 MB (34618483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f079c1b0af8d690151aa9187d4308985a20f7ac72e4916f72e429e87a3dbf9`  
		Last Modified: Wed, 29 Mar 2023 22:39:26 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e06b8c9a11f534829f3f075965ea66db0848b8c65075ac79790ab13631922a8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:v2.10-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:290c74bd221d9156e894120db45f83e6c3073414ae4726b33a6c5394aad11ced
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2051118218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12766268c3909b8aea4982e046e39d57a153a1a283de0210d852fd225fb75428`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 07 Apr 2023 22:17:15 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.0-rc2/traefik_v2.10.0-rc2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Fri, 07 Apr 2023 22:17:16 GMT
EXPOSE 80
# Fri, 07 Apr 2023 22:17:17 GMT
ENTRYPOINT ["/traefik"]
# Fri, 07 Apr 2023 22:17:17 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57437d77990e17f6f1c4de8c842c9be99cc65894850bdf5fda3ce6ad610bc94`  
		Last Modified: Fri, 07 Apr 2023 22:18:11 GMT  
		Size: 37.6 MB (37603585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9b44ad239fc25c916d9b6fd60d1ee079b9827218883933725f6c452eedcb20`  
		Last Modified: Fri, 07 Apr 2023 22:18:03 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb69fbbb0a60fb6bf98cbfdfc0c3fc66801acb7bcd8c847cc43aa78fa8128a3`  
		Last Modified: Fri, 07 Apr 2023 22:18:03 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d5bdf56292275f8e72e015f1c9d64eb2d9d4ee6ddde77defa0866df6a3bbe4`  
		Last Modified: Fri, 07 Apr 2023 22:18:03 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10.0-rc2`

```console
$ docker pull traefik@sha256:f8662c6403f1b3fa10d700967241a256428241dab83d2aafab8d8c0953a4ca51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `traefik:v2.10.0-rc2` - linux; amd64

```console
$ docker pull traefik@sha256:e740be22cd324a87119d2091a70e8c89c7f8a0f83913caa7dbc098c40ed01b44
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40979650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31d787e98af349f3ec4332f4d1cebf0555523271d40666e6d462dccec7c88872`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:38 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Apr 2023 22:20:57 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.0-rc2/traefik_v2.10.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Apr 2023 22:20:57 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Apr 2023 22:20:57 GMT
EXPOSE 80
# Fri, 07 Apr 2023 22:20:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Apr 2023 22:20:57 GMT
CMD ["traefik"]
# Fri, 07 Apr 2023 22:20:57 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d055169f9c6f7e08b88a6ef90eba203750fcc51761ecb994e40aa2aaa640ff72`  
		Last Modified: Thu, 30 Mar 2023 02:38:35 GMT  
		Size: 622.2 KB (622239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4680b9aefc39947986fb5f7d0fbb6c51f79b9fee726231e6e22799985ada11e`  
		Last Modified: Fri, 07 Apr 2023 22:21:24 GMT  
		Size: 37.0 MB (36982480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c40271a2c0502a46ca8dca99a5196da7cac0b078453a70a90877bee34cb6a45c`  
		Last Modified: Fri, 07 Apr 2023 22:21:18 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10.0-rc2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e06b8c9a11f534829f3f075965ea66db0848b8c65075ac79790ab13631922a8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:v2.10.0-rc2-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:290c74bd221d9156e894120db45f83e6c3073414ae4726b33a6c5394aad11ced
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2051118218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12766268c3909b8aea4982e046e39d57a153a1a283de0210d852fd225fb75428`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 07 Apr 2023 22:17:15 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.0-rc2/traefik_v2.10.0-rc2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Fri, 07 Apr 2023 22:17:16 GMT
EXPOSE 80
# Fri, 07 Apr 2023 22:17:17 GMT
ENTRYPOINT ["/traefik"]
# Fri, 07 Apr 2023 22:17:17 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57437d77990e17f6f1c4de8c842c9be99cc65894850bdf5fda3ce6ad610bc94`  
		Last Modified: Fri, 07 Apr 2023 22:18:11 GMT  
		Size: 37.6 MB (37603585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9b44ad239fc25c916d9b6fd60d1ee079b9827218883933725f6c452eedcb20`  
		Last Modified: Fri, 07 Apr 2023 22:18:03 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb69fbbb0a60fb6bf98cbfdfc0c3fc66801acb7bcd8c847cc43aa78fa8128a3`  
		Last Modified: Fri, 07 Apr 2023 22:18:03 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d5bdf56292275f8e72e015f1c9d64eb2d9d4ee6ddde77defa0866df6a3bbe4`  
		Last Modified: Fri, 07 Apr 2023 22:18:03 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.9`

```console
$ docker pull traefik@sha256:8d81a9df1435f9f3d36ac9398465ef2d5d61e671059974db753faaed14b627de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.9` - linux; amd64

```console
$ docker pull traefik@sha256:6dee6938b5ebfc511a82ef4e09c80268835a2f67393e5c06c3e4ef9a14d1817b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39613072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1e26b5f8193d713eb8f39d0ab0e3d513278f86e41644b07e189e1aef536b335`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:38 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Apr 2023 18:24:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Apr 2023 18:24:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Apr 2023 18:24:44 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:24:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:24:44 GMT
CMD ["traefik"]
# Thu, 06 Apr 2023 18:24:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d055169f9c6f7e08b88a6ef90eba203750fcc51761ecb994e40aa2aaa640ff72`  
		Last Modified: Thu, 30 Mar 2023 02:38:35 GMT  
		Size: 622.2 KB (622239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afaddc85d79e665b30c4ee7ce9fc12425532f4695c6888b052086589f12aa687`  
		Last Modified: Thu, 06 Apr 2023 18:25:11 GMT  
		Size: 35.6 MB (35615902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff733a62a1272d7fe4817f1b3a8faf56c8a7f0e3808baec593378d274c1d081`  
		Last Modified: Thu, 06 Apr 2023 18:25:06 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f76a8f0c2b54429df275eb7e842171230994dc28924cb17f65ca41a3c5cb94fc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37257635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c077549480f6828d39797ca3855e6299d0c1e7daf08d67cd62320c07515ff0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:39 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Apr 2023 18:49:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Apr 2023 18:49:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Apr 2023 18:49:31 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:49:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:49:31 GMT
CMD ["traefik"]
# Thu, 06 Apr 2023 18:49:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bd7901efecc8425b6d98584a9ee5d091a238a8936fb50b8aa4654afb90d05d`  
		Last Modified: Thu, 30 Mar 2023 00:41:05 GMT  
		Size: 624.4 KB (624425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:658599efc3390617789f600a87686c808ae0c26e3a0a310ca9ad50944f5061f2`  
		Last Modified: Thu, 06 Apr 2023 18:49:58 GMT  
		Size: 33.5 MB (33522040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39827a939bd6089039662bd6dc0237923c0b6b7d177fcf7f37bdcb9dcaf831ee`  
		Last Modified: Thu, 06 Apr 2023 18:49:52 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7b1ecf3dcf9d504f037e14d060c7bfcb87ebde442eaf3c1d89e0c2e2f180a987
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.5 MB (36503424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fa39db0cea458044cad085ee32cf6bb615ccff2f3f7bbbc5e57f9b36984afb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Apr 2023 18:51:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Apr 2023 18:51:04 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Apr 2023 18:51:04 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:51:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:51:04 GMT
CMD ["traefik"]
# Thu, 06 Apr 2023 18:51:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4336eee5b1b811f9668d2251fb67e6099c4089ef7b26ade14aacd2f5f0982e06`  
		Last Modified: Thu, 30 Mar 2023 03:27:34 GMT  
		Size: 624.2 KB (624204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9cadb05aa1b060d980fd3437917259c39ca7d9fb914fccd2d05ba2c3ac9d1e`  
		Last Modified: Thu, 06 Apr 2023 18:51:28 GMT  
		Size: 32.6 MB (32616998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1371d2d81d70ec646fa25de2ef0e1ecbf8a73448a75536cdae53906746ee2605`  
		Last Modified: Thu, 06 Apr 2023 18:51:24 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9` - linux; s390x

```console
$ docker pull traefik@sha256:40c157efc3aeb2a68be807c7bd9c56058b039f5dc04ea99a2d207f5694ba3498
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38337898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ed3cb8277e480dbe2a03868fd3de6e86d2381cb25b7d4cf62ca5209a4a8f36f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:38:21 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Apr 2023 18:46:14 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Apr 2023 18:46:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Apr 2023 18:46:16 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:46:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:46:16 GMT
CMD ["traefik"]
# Thu, 06 Apr 2023 18:46:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096a495bd82a55e97c5be084787578b5b5af0321a33c70ccf19bca0dc260a981`  
		Last Modified: Wed, 29 Mar 2023 22:39:11 GMT  
		Size: 622.6 KB (622584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff0e0742f027721acb6e403cfd9c33f5035562626412821cf440ee0a0d4bd6`  
		Last Modified: Thu, 06 Apr 2023 18:46:41 GMT  
		Size: 34.5 MB (34539759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566cf6a3c532656d496f8fab7a8822e11cef4dd8c1dab24cdf229bbf359101eb`  
		Last Modified: Thu, 06 Apr 2023 18:46:36 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.9-windowsservercore-1809`

```console
$ docker pull traefik@sha256:ec994d877f87622e6e0fe82b0ea8e3b3efabf1e0d8c57fe110f822b211243c08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:v2.9-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:38c71b3285dd02b9aa56ad826495f85e854606a04db526dcf7bf770ca9936a20
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2049781176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f645f991b33f438d120607abe7a2a158d8300068ceb916e0d7a6d2eaa095526e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Apr 2023 18:17:03 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 06 Apr 2023 18:17:04 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:17:05 GMT
ENTRYPOINT ["/traefik"]
# Thu, 06 Apr 2023 18:17:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b184b38bee4a888e16184a05c4770d36d87ad320077cbee08f12000fd700abed`  
		Last Modified: Thu, 06 Apr 2023 18:18:10 GMT  
		Size: 36.3 MB (36266505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32de5c550068bdd6a0e71f6aaae2c5ba100294dbb52006ca1247bc09cfb87e17`  
		Last Modified: Thu, 06 Apr 2023 18:18:00 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b65f112c430971f5c46a3133c30bd210125ddcf9493bca90d0553685871a5`  
		Last Modified: Thu, 06 Apr 2023 18:18:00 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8510431814f07a8c701f707dabf5daf9283df8769147fefe8634a06b3edf2a`  
		Last Modified: Thu, 06 Apr 2023 18:18:00 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.9.10`

```console
$ docker pull traefik@sha256:8d81a9df1435f9f3d36ac9398465ef2d5d61e671059974db753faaed14b627de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.9.10` - linux; amd64

```console
$ docker pull traefik@sha256:6dee6938b5ebfc511a82ef4e09c80268835a2f67393e5c06c3e4ef9a14d1817b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39613072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1e26b5f8193d713eb8f39d0ab0e3d513278f86e41644b07e189e1aef536b335`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:38 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Apr 2023 18:24:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Apr 2023 18:24:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Apr 2023 18:24:44 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:24:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:24:44 GMT
CMD ["traefik"]
# Thu, 06 Apr 2023 18:24:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d055169f9c6f7e08b88a6ef90eba203750fcc51761ecb994e40aa2aaa640ff72`  
		Last Modified: Thu, 30 Mar 2023 02:38:35 GMT  
		Size: 622.2 KB (622239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afaddc85d79e665b30c4ee7ce9fc12425532f4695c6888b052086589f12aa687`  
		Last Modified: Thu, 06 Apr 2023 18:25:11 GMT  
		Size: 35.6 MB (35615902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff733a62a1272d7fe4817f1b3a8faf56c8a7f0e3808baec593378d274c1d081`  
		Last Modified: Thu, 06 Apr 2023 18:25:06 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9.10` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f76a8f0c2b54429df275eb7e842171230994dc28924cb17f65ca41a3c5cb94fc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37257635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c077549480f6828d39797ca3855e6299d0c1e7daf08d67cd62320c07515ff0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:39 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Apr 2023 18:49:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Apr 2023 18:49:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Apr 2023 18:49:31 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:49:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:49:31 GMT
CMD ["traefik"]
# Thu, 06 Apr 2023 18:49:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bd7901efecc8425b6d98584a9ee5d091a238a8936fb50b8aa4654afb90d05d`  
		Last Modified: Thu, 30 Mar 2023 00:41:05 GMT  
		Size: 624.4 KB (624425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:658599efc3390617789f600a87686c808ae0c26e3a0a310ca9ad50944f5061f2`  
		Last Modified: Thu, 06 Apr 2023 18:49:58 GMT  
		Size: 33.5 MB (33522040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39827a939bd6089039662bd6dc0237923c0b6b7d177fcf7f37bdcb9dcaf831ee`  
		Last Modified: Thu, 06 Apr 2023 18:49:52 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9.10` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7b1ecf3dcf9d504f037e14d060c7bfcb87ebde442eaf3c1d89e0c2e2f180a987
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.5 MB (36503424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fa39db0cea458044cad085ee32cf6bb615ccff2f3f7bbbc5e57f9b36984afb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Apr 2023 18:51:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Apr 2023 18:51:04 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Apr 2023 18:51:04 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:51:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:51:04 GMT
CMD ["traefik"]
# Thu, 06 Apr 2023 18:51:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4336eee5b1b811f9668d2251fb67e6099c4089ef7b26ade14aacd2f5f0982e06`  
		Last Modified: Thu, 30 Mar 2023 03:27:34 GMT  
		Size: 624.2 KB (624204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9cadb05aa1b060d980fd3437917259c39ca7d9fb914fccd2d05ba2c3ac9d1e`  
		Last Modified: Thu, 06 Apr 2023 18:51:28 GMT  
		Size: 32.6 MB (32616998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1371d2d81d70ec646fa25de2ef0e1ecbf8a73448a75536cdae53906746ee2605`  
		Last Modified: Thu, 06 Apr 2023 18:51:24 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9.10` - linux; s390x

```console
$ docker pull traefik@sha256:40c157efc3aeb2a68be807c7bd9c56058b039f5dc04ea99a2d207f5694ba3498
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38337898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ed3cb8277e480dbe2a03868fd3de6e86d2381cb25b7d4cf62ca5209a4a8f36f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:38:21 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 06 Apr 2023 18:46:14 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 06 Apr 2023 18:46:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 06 Apr 2023 18:46:16 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:46:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Apr 2023 18:46:16 GMT
CMD ["traefik"]
# Thu, 06 Apr 2023 18:46:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096a495bd82a55e97c5be084787578b5b5af0321a33c70ccf19bca0dc260a981`  
		Last Modified: Wed, 29 Mar 2023 22:39:11 GMT  
		Size: 622.6 KB (622584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff0e0742f027721acb6e403cfd9c33f5035562626412821cf440ee0a0d4bd6`  
		Last Modified: Thu, 06 Apr 2023 18:46:41 GMT  
		Size: 34.5 MB (34539759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566cf6a3c532656d496f8fab7a8822e11cef4dd8c1dab24cdf229bbf359101eb`  
		Last Modified: Thu, 06 Apr 2023 18:46:36 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.9.10-windowsservercore-1809`

```console
$ docker pull traefik@sha256:ec994d877f87622e6e0fe82b0ea8e3b3efabf1e0d8c57fe110f822b211243c08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:v2.9.10-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:38c71b3285dd02b9aa56ad826495f85e854606a04db526dcf7bf770ca9936a20
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2049781176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f645f991b33f438d120607abe7a2a158d8300068ceb916e0d7a6d2eaa095526e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Apr 2023 18:17:03 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 06 Apr 2023 18:17:04 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:17:05 GMT
ENTRYPOINT ["/traefik"]
# Thu, 06 Apr 2023 18:17:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b184b38bee4a888e16184a05c4770d36d87ad320077cbee08f12000fd700abed`  
		Last Modified: Thu, 06 Apr 2023 18:18:10 GMT  
		Size: 36.3 MB (36266505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32de5c550068bdd6a0e71f6aaae2c5ba100294dbb52006ca1247bc09cfb87e17`  
		Last Modified: Thu, 06 Apr 2023 18:18:00 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b65f112c430971f5c46a3133c30bd210125ddcf9493bca90d0553685871a5`  
		Last Modified: Thu, 06 Apr 2023 18:18:00 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8510431814f07a8c701f707dabf5daf9283df8769147fefe8634a06b3edf2a`  
		Last Modified: Thu, 06 Apr 2023 18:18:00 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0`

```console
$ docker pull traefik@sha256:0d7e8693e44e52588366695db63512b6b7a92d34b2145c2c3c732fec27ee03e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v3.0` - linux; amd64

```console
$ docker pull traefik@sha256:a239deca1c7682fe9bb6a32e54364c7ff460205fa0e87c02bfeb66efb3f3a3d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40562953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42fc5a7c2d34a752fce6439cf3dc08ac747649d7712bc265c7dd7d1b38a2a45b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 02:37:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 02:37:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 02:37:35 GMT
EXPOSE 80
# Thu, 30 Mar 2023 02:37:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 02:37:35 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 02:37:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11624eb8d0cca298aa32848e39318bbc75ab1c404423d1d47c670fa60354e3`  
		Last Modified: Thu, 30 Mar 2023 02:38:16 GMT  
		Size: 661.1 KB (661099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9d40a9765a3ede8e4ec67030b20d484fedcea2ad98ee2b231ec3d86e6fd1b6`  
		Last Modified: Thu, 30 Mar 2023 02:38:21 GMT  
		Size: 37.1 MB (37074890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fca61e22e5a1dbbdeea08d3e394601c2c5492fc65d19af813ef66cc36a7d582`  
		Last Modified: Thu, 30 Mar 2023 02:38:15 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0` - linux; arm variant v6

```console
$ docker pull traefik@sha256:5da0026b1e1053a9bcef582853c749291cf651f2bc1e35a557d87080e78a74f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38289884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d444fca66ffd358a663e6075b1d97f53a52bd6d11aa27afa1aa0b8cf4179f67`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:13 GMT
ADD file:3fb55ad8134002858be264c3c2477d784e4a60f2f6501afa7cf3b10bfede51aa in / 
# Wed, 29 Mar 2023 18:01:13 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 00:39:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 00:39:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 00:39:31 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:39:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 00:39:31 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 00:39:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:872c99a87729fa48dce303fb615edbb1a5da837f627a0b3d28495a0400ca8335`  
		Last Modified: Wed, 29 Mar 2023 18:02:12 GMT  
		Size: 2.6 MB (2634030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb226453f567b759ad92b5db4fa1f391e1eb96232b14d006147344b993d24773`  
		Last Modified: Thu, 30 Mar 2023 00:40:46 GMT  
		Size: 666.2 KB (666166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f676a5305470c023669ddf7351410e0d65fa65bcfe24fc65a2e567699f7c00e6`  
		Last Modified: Thu, 30 Mar 2023 00:40:52 GMT  
		Size: 35.0 MB (34989322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb744443f625044ceb56795d0847c66fe1957350cdaa3a296ad67d692876d308`  
		Last Modified: Thu, 30 Mar 2023 00:40:46 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:529410986a68c6e7989a5a08afa53d087795a2f1406977d5d6b183bfdfab65dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37408212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e4bfdbd12bed1c2e46296bb16021a1eea4269055e03fdf9e30c035e5f9e8dc4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 03:26:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 03:26:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 03:26:35 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:26:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 03:26:35 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 03:26:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d019fab0470c352dfa2ff6c01be8f1d0344d43e9431a28656e78c5cabd03e67f`  
		Last Modified: Thu, 30 Mar 2023 03:27:17 GMT  
		Size: 662.3 KB (662323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82ed46bb3966bf021d56f3bfda66ada1ddde7199ee9d3446ebcbeffec692004`  
		Last Modified: Thu, 30 Mar 2023 03:27:20 GMT  
		Size: 34.0 MB (34023520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a93ddfbde23c1aa20ccac6b7cd3dcbda52d11c2b1627d41dc7fa169bd46430`  
		Last Modified: Thu, 30 Mar 2023 03:27:16 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0` - linux; s390x

```console
$ docker pull traefik@sha256:e8572896cf2369e9777be7e5ce1bce0b811642e09298039e0a9d51fa570172e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39131970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:194779f21f9e8eb09ec639ba646ce59761d5db6264648a5e162bf515e294517d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:07 GMT
ADD file:5cf392863cd9a0735de88f9e7dab93c9e74aca59ca05b792943cf3b621ea2c59 in / 
# Wed, 29 Mar 2023 17:42:07 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:38:08 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Mar 2023 22:38:14 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Mar 2023 22:38:15 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Mar 2023 22:38:16 GMT
EXPOSE 80
# Wed, 29 Mar 2023 22:38:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 22:38:16 GMT
CMD ["traefik"]
# Wed, 29 Mar 2023 22:38:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:1536575ac9c5f5fff4522c60d4610af0a52be584c36e652080c6c0ad169d4f27`  
		Last Modified: Wed, 29 Mar 2023 17:42:42 GMT  
		Size: 2.6 MB (2610636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246408072526d1b1e0fec7aaa14e46bd07b33c86c047b5d7cdce7778f992de28`  
		Last Modified: Wed, 29 Mar 2023 22:38:58 GMT  
		Size: 665.5 KB (665530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982fc64501c81b1c6a90bf3b79f669b6d16f9133509eb962541ae33f7f14c83c`  
		Last Modified: Wed, 29 Mar 2023 22:39:03 GMT  
		Size: 35.9 MB (35855437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b72fc0bf978c8423d98dc56a60760c0b3d12dbea0fd1524d98a88e3f173c6ab`  
		Last Modified: Wed, 29 Mar 2023 22:38:58 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0-windowsservercore-1809`

```console
$ docker pull traefik@sha256:2eb0d945da364a274f76288295b9120086404be2c7606fe340ac2ee6f1d64ed1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:v3.0-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:62e9db8356188c92dbce1706a8c2af3702993ee762b34d398fc7921eb03a3629
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2051205802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648f7c4938c24c605c3f3cbf0b16d4a5767ce075cd407fa9c6ab93e256035917`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 08:45:29 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 16 Mar 2023 08:45:30 GMT
EXPOSE 80
# Thu, 16 Mar 2023 08:45:31 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Mar 2023 08:45:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5eafb0300ea614e208e5052cfdd0941f2ad90a341c5b337ab489e223bb31e88`  
		Last Modified: Thu, 16 Mar 2023 08:49:24 GMT  
		Size: 37.7 MB (37691161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec0dc51e5d37193b3e6ebdd21f1bb94e44f593af5691b32af00720bb4548bbc`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28da668ed65b21bb734a5ba72dd5262a27de001c56a64bebf1db5e9244aaad4c`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6138998225adfde27a93f621c64ba53c628511ce9209f16661fd0c3619ff3e3`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0.0-beta2`

```console
$ docker pull traefik@sha256:0d7e8693e44e52588366695db63512b6b7a92d34b2145c2c3c732fec27ee03e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v3.0.0-beta2` - linux; amd64

```console
$ docker pull traefik@sha256:a239deca1c7682fe9bb6a32e54364c7ff460205fa0e87c02bfeb66efb3f3a3d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40562953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42fc5a7c2d34a752fce6439cf3dc08ac747649d7712bc265c7dd7d1b38a2a45b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 02:37:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 02:37:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 02:37:35 GMT
EXPOSE 80
# Thu, 30 Mar 2023 02:37:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 02:37:35 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 02:37:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11624eb8d0cca298aa32848e39318bbc75ab1c404423d1d47c670fa60354e3`  
		Last Modified: Thu, 30 Mar 2023 02:38:16 GMT  
		Size: 661.1 KB (661099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9d40a9765a3ede8e4ec67030b20d484fedcea2ad98ee2b231ec3d86e6fd1b6`  
		Last Modified: Thu, 30 Mar 2023 02:38:21 GMT  
		Size: 37.1 MB (37074890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fca61e22e5a1dbbdeea08d3e394601c2c5492fc65d19af813ef66cc36a7d582`  
		Last Modified: Thu, 30 Mar 2023 02:38:15 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0.0-beta2` - linux; arm variant v6

```console
$ docker pull traefik@sha256:5da0026b1e1053a9bcef582853c749291cf651f2bc1e35a557d87080e78a74f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38289884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d444fca66ffd358a663e6075b1d97f53a52bd6d11aa27afa1aa0b8cf4179f67`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:13 GMT
ADD file:3fb55ad8134002858be264c3c2477d784e4a60f2f6501afa7cf3b10bfede51aa in / 
# Wed, 29 Mar 2023 18:01:13 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 00:39:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 00:39:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 00:39:31 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:39:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 00:39:31 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 00:39:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:872c99a87729fa48dce303fb615edbb1a5da837f627a0b3d28495a0400ca8335`  
		Last Modified: Wed, 29 Mar 2023 18:02:12 GMT  
		Size: 2.6 MB (2634030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb226453f567b759ad92b5db4fa1f391e1eb96232b14d006147344b993d24773`  
		Last Modified: Thu, 30 Mar 2023 00:40:46 GMT  
		Size: 666.2 KB (666166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f676a5305470c023669ddf7351410e0d65fa65bcfe24fc65a2e567699f7c00e6`  
		Last Modified: Thu, 30 Mar 2023 00:40:52 GMT  
		Size: 35.0 MB (34989322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb744443f625044ceb56795d0847c66fe1957350cdaa3a296ad67d692876d308`  
		Last Modified: Thu, 30 Mar 2023 00:40:46 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0.0-beta2` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:529410986a68c6e7989a5a08afa53d087795a2f1406977d5d6b183bfdfab65dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37408212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e4bfdbd12bed1c2e46296bb16021a1eea4269055e03fdf9e30c035e5f9e8dc4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 03:26:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 03:26:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 03:26:35 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:26:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 03:26:35 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 03:26:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d019fab0470c352dfa2ff6c01be8f1d0344d43e9431a28656e78c5cabd03e67f`  
		Last Modified: Thu, 30 Mar 2023 03:27:17 GMT  
		Size: 662.3 KB (662323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82ed46bb3966bf021d56f3bfda66ada1ddde7199ee9d3446ebcbeffec692004`  
		Last Modified: Thu, 30 Mar 2023 03:27:20 GMT  
		Size: 34.0 MB (34023520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a93ddfbde23c1aa20ccac6b7cd3dcbda52d11c2b1627d41dc7fa169bd46430`  
		Last Modified: Thu, 30 Mar 2023 03:27:16 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0.0-beta2` - linux; s390x

```console
$ docker pull traefik@sha256:e8572896cf2369e9777be7e5ce1bce0b811642e09298039e0a9d51fa570172e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39131970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:194779f21f9e8eb09ec639ba646ce59761d5db6264648a5e162bf515e294517d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:07 GMT
ADD file:5cf392863cd9a0735de88f9e7dab93c9e74aca59ca05b792943cf3b621ea2c59 in / 
# Wed, 29 Mar 2023 17:42:07 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:38:08 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Mar 2023 22:38:14 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Mar 2023 22:38:15 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Mar 2023 22:38:16 GMT
EXPOSE 80
# Wed, 29 Mar 2023 22:38:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 22:38:16 GMT
CMD ["traefik"]
# Wed, 29 Mar 2023 22:38:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:1536575ac9c5f5fff4522c60d4610af0a52be584c36e652080c6c0ad169d4f27`  
		Last Modified: Wed, 29 Mar 2023 17:42:42 GMT  
		Size: 2.6 MB (2610636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246408072526d1b1e0fec7aaa14e46bd07b33c86c047b5d7cdce7778f992de28`  
		Last Modified: Wed, 29 Mar 2023 22:38:58 GMT  
		Size: 665.5 KB (665530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982fc64501c81b1c6a90bf3b79f669b6d16f9133509eb962541ae33f7f14c83c`  
		Last Modified: Wed, 29 Mar 2023 22:39:03 GMT  
		Size: 35.9 MB (35855437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b72fc0bf978c8423d98dc56a60760c0b3d12dbea0fd1524d98a88e3f173c6ab`  
		Last Modified: Wed, 29 Mar 2023 22:38:58 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0.0-beta2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:2eb0d945da364a274f76288295b9120086404be2c7606fe340ac2ee6f1d64ed1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:v3.0.0-beta2-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:62e9db8356188c92dbce1706a8c2af3702993ee762b34d398fc7921eb03a3629
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2051205802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648f7c4938c24c605c3f3cbf0b16d4a5767ce075cd407fa9c6ab93e256035917`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 08:45:29 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 16 Mar 2023 08:45:30 GMT
EXPOSE 80
# Thu, 16 Mar 2023 08:45:31 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Mar 2023 08:45:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5eafb0300ea614e208e5052cfdd0941f2ad90a341c5b337ab489e223bb31e88`  
		Last Modified: Thu, 16 Mar 2023 08:49:24 GMT  
		Size: 37.7 MB (37691161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec0dc51e5d37193b3e6ebdd21f1bb94e44f593af5691b32af00720bb4548bbc`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28da668ed65b21bb734a5ba72dd5262a27de001c56a64bebf1db5e9244aaad4c`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6138998225adfde27a93f621c64ba53c628511ce9209f16661fd0c3619ff3e3`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:ec994d877f87622e6e0fe82b0ea8e3b3efabf1e0d8c57fe110f822b211243c08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:38c71b3285dd02b9aa56ad826495f85e854606a04db526dcf7bf770ca9936a20
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2049781176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f645f991b33f438d120607abe7a2a158d8300068ceb916e0d7a6d2eaa095526e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Apr 2023 18:17:03 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 06 Apr 2023 18:17:04 GMT
EXPOSE 80
# Thu, 06 Apr 2023 18:17:05 GMT
ENTRYPOINT ["/traefik"]
# Thu, 06 Apr 2023 18:17:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b184b38bee4a888e16184a05c4770d36d87ad320077cbee08f12000fd700abed`  
		Last Modified: Thu, 06 Apr 2023 18:18:10 GMT  
		Size: 36.3 MB (36266505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32de5c550068bdd6a0e71f6aaae2c5ba100294dbb52006ca1247bc09cfb87e17`  
		Last Modified: Thu, 06 Apr 2023 18:18:00 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b65f112c430971f5c46a3133c30bd210125ddcf9493bca90d0553685871a5`  
		Last Modified: Thu, 06 Apr 2023 18:18:00 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8510431814f07a8c701f707dabf5daf9283df8769147fefe8634a06b3edf2a`  
		Last Modified: Thu, 06 Apr 2023 18:18:00 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
