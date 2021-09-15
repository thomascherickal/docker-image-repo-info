<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:1.7`](#traefik17)
-	[`traefik:1.7-alpine`](#traefik17-alpine)
-	[`traefik:1.7-windowsservercore-1809`](#traefik17-windowsservercore-1809)
-	[`traefik:1.7.30`](#traefik1730)
-	[`traefik:1.7.30-alpine`](#traefik1730-alpine)
-	[`traefik:1.7.30-windowsservercore-1809`](#traefik1730-windowsservercore-1809)
-	[`traefik:2.5`](#traefik25)
-	[`traefik:2.5-windowsservercore-1809`](#traefik25-windowsservercore-1809)
-	[`traefik:2.5.2`](#traefik252)
-	[`traefik:2.5.2-windowsservercore-1809`](#traefik252-windowsservercore-1809)
-	[`traefik:brie`](#traefikbrie)
-	[`traefik:brie-windowsservercore-1809`](#traefikbrie-windowsservercore-1809)
-	[`traefik:latest`](#traefiklatest)
-	[`traefik:maroilles`](#traefikmaroilles)
-	[`traefik:maroilles-alpine`](#traefikmaroilles-alpine)
-	[`traefik:maroilles-windowsservercore-1809`](#traefikmaroilles-windowsservercore-1809)
-	[`traefik:v1.7`](#traefikv17)
-	[`traefik:v1.7-alpine`](#traefikv17-alpine)
-	[`traefik:v1.7-windowsservercore-1809`](#traefikv17-windowsservercore-1809)
-	[`traefik:v1.7.30`](#traefikv1730)
-	[`traefik:v1.7.30-alpine`](#traefikv1730-alpine)
-	[`traefik:v1.7.30-windowsservercore-1809`](#traefikv1730-windowsservercore-1809)
-	[`traefik:v2.5`](#traefikv25)
-	[`traefik:v2.5-windowsservercore-1809`](#traefikv25-windowsservercore-1809)
-	[`traefik:v2.5.2`](#traefikv252)
-	[`traefik:v2.5.2-windowsservercore-1809`](#traefikv252-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:1.7`

```console
$ docker pull traefik@sha256:ca3883356d24f9fd6d36f0450d7f6f17a233317943517f6036c20ebf7c137781
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7` - linux; amd64

```console
$ docker pull traefik@sha256:353827cc14120a14b1eccbb2714039763d9cefc284213b53d82d14e110fadc39
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.1 MB (18124621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a2126389e0b0dbd13da033d79636b0f0626d73f1a6da0935ce6ce9eccae112a`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 09 Mar 2021 01:32:48 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Tue, 09 Mar 2021 01:32:49 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 08 Apr 2021 20:07:38 GMT
COPY file:bc0b1c0235bda22a75d2ef00a982989cdf1da3240f077584bca5c6b560a4c13a in / 
# Thu, 08 Apr 2021 20:07:38 GMT
EXPOSE 80
# Thu, 08 Apr 2021 20:07:39 GMT
VOLUME [/tmp]
# Thu, 08 Apr 2021 20:07:39 GMT
ENTRYPOINT ["/traefik"]
# Thu, 08 Apr 2021 20:07:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:53f50c15495c67f391a5750288681a589b19a39c4b78e7ebc0934606cc3d0bc3`  
		Last Modified: Tue, 09 Mar 2021 01:33:59 GMT  
		Size: 130.9 KB (130870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c044b3636c16c5ab8fc96a04f320c9f97ea23aaffec9adb2d8f20ebaef93f3`  
		Last Modified: Tue, 09 Mar 2021 01:33:59 GMT  
		Size: 308.8 KB (308823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb3d26b40720e4da5cbeb15193c698565e23551a24cc4abc4acd1b7de414279`  
		Last Modified: Thu, 08 Apr 2021 20:08:34 GMT  
		Size: 17.7 MB (17684928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:13bd9d65c0558740d1b8b6f8de06f314003be9b54eec4b8b67dad2cf58d037c3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16956525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f60cea7c66ee3601de1cf66168feceac0bc9ac1147103e54d63f742e570bb0ca`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 22 Jun 2021 21:21:29 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Tue, 22 Jun 2021 21:21:31 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Tue, 22 Jun 2021 21:21:34 GMT
COPY file:440b6b1ebd389a2397ffb187ded4c85dcf37b7284d94c693b0b603d51247c683 in / 
# Tue, 22 Jun 2021 21:21:35 GMT
EXPOSE 80
# Tue, 22 Jun 2021 21:21:35 GMT
VOLUME [/tmp]
# Tue, 22 Jun 2021 21:21:35 GMT
ENTRYPOINT ["/traefik"]
# Tue, 22 Jun 2021 21:21:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:00918d1fc688f95413059b21ca56a6453b74d2808448ca35ed04b737d4a22c74`  
		Last Modified: Tue, 22 Jun 2021 21:24:22 GMT  
		Size: 130.9 KB (130871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e7abe8d1c9d1c5c74050eb312423f911185ce6cc705d32631fad6a1b3a4450`  
		Last Modified: Tue, 22 Jun 2021 21:24:23 GMT  
		Size: 308.9 KB (308853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee57e616d21eeb2181fd86ab18cbdb3be5af9c65ddb68c3657ebba7e266a191`  
		Last Modified: Tue, 22 Jun 2021 21:24:33 GMT  
		Size: 16.5 MB (16516801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:f7fe0c0982ce55e8882f88193462be30b654f27dd1c5014243efd6fd85d563ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16533633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0c3dd29cfce4ed4d7084315b52be936e63726239cbae0f98cf0c36cfdd8707a`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Wed, 16 Jun 2021 11:17:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Wed, 16 Jun 2021 11:17:48 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Wed, 16 Jun 2021 11:17:48 GMT
COPY file:6fdd60dc35db1c19a5de5ed8b57f159a6e121ba0f1ddb3e48a6e185da99f8cca in / 
# Wed, 16 Jun 2021 11:17:49 GMT
EXPOSE 80
# Wed, 16 Jun 2021 11:17:49 GMT
VOLUME [/tmp]
# Wed, 16 Jun 2021 11:17:49 GMT
ENTRYPOINT ["/traefik"]
# Wed, 16 Jun 2021 11:17:49 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ba07573b64554f7a74d3d3b27c42e28f5209c9d82f79b2596a6b190ee5475c72`  
		Last Modified: Wed, 16 Jun 2021 11:19:25 GMT  
		Size: 130.9 KB (130872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8a5756798f3769843250c96f2b11eca4d4c83a91616dd5d97d17399022fc6e`  
		Last Modified: Wed, 16 Jun 2021 11:19:25 GMT  
		Size: 308.9 KB (308857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6af1647ff43bc2a163e816afb6eb2c410d240b736297469f44ec6db498f13fc`  
		Last Modified: Wed, 16 Jun 2021 11:19:28 GMT  
		Size: 16.1 MB (16093904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-alpine`

```console
$ docker pull traefik@sha256:b5f54c8cff7bb0a8a249cbb00d79197403d63e8d4f813e2e50ba87884114f955
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:81038c31f0c7151418b10af58c252fb5e4d76c11a3d0b7a22aa66d61c3aadadc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.2 MB (21176792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8d154c84159a4d96e8aedebfa3bce9d19fc139b450d3b4eee1bb46e4ab759a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:31 GMT
ADD file:9d14b11183983923090d9e6d15cc51ee210466296e913bfefbfd580b3de59c95 in / 
# Tue, 31 Aug 2021 23:18:31 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 06:15:05 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 01 Sep 2021 06:15:16 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 01 Sep 2021 06:15:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 01 Sep 2021 06:15:16 GMT
EXPOSE 80
# Wed, 01 Sep 2021 06:15:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Sep 2021 06:15:17 GMT
CMD ["traefik"]
# Wed, 01 Sep 2021 06:15:17 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6a428f9f83b0a29f1fdd2ccccca19a9bab805a925b8eddf432a5a3d3da04afbc`  
		Last Modified: Tue, 31 Aug 2021 23:19:15 GMT  
		Size: 2.8 MB (2817307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f794cbdc99470251c9539251dc8a5aba6a6f0d6b4fd07a519bf8d13a9d42bbec`  
		Last Modified: Wed, 01 Sep 2021 06:16:08 GMT  
		Size: 674.2 KB (674226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa68ae87a84c1bc651faa725d25b0c37abf9514b31398de8ec4113c983f7bd3c`  
		Last Modified: Wed, 01 Sep 2021 06:16:31 GMT  
		Size: 17.7 MB (17684891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d6a80456e69fce8cd53394e12769c6b2757b1a318d8abd6eb0b1aa982e6791`  
		Last Modified: Wed, 01 Sep 2021 06:16:28 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:293b013a4e5f743eff9d2002d2affd2f1c948a60e8298af651c591ab79aa23c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.8 MB (19817351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9cdda6ba44e4d81cacd510102508f96d75ef73b1177f41a7154ea2822f45398`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:57 GMT
ADD file:3e83d6b5df3a951968e475c7326baf5ef90a22f04163693db34f3b4fc5812434 in / 
# Tue, 31 Aug 2021 22:30:57 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 07:35:43 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 01 Sep 2021 07:36:13 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 01 Sep 2021 07:36:14 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 01 Sep 2021 07:36:14 GMT
EXPOSE 80
# Wed, 01 Sep 2021 07:36:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Sep 2021 07:36:15 GMT
CMD ["traefik"]
# Wed, 01 Sep 2021 07:36:15 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7fe987b00bcb1f14c5b65f89813475143c021e2f5c156705ac3525abe1b397a1`  
		Last Modified: Tue, 31 Aug 2021 22:32:38 GMT  
		Size: 2.6 MB (2623044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ba27e6c34ba3c95c27e5aeada45e16c63122f31ec4c676f827e54daf47caf1`  
		Last Modified: Wed, 01 Sep 2021 07:37:54 GMT  
		Size: 677.0 KB (677024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7656c78f5b42128229dc58a77d852c6a388c45cc8a4c25fcdeb15b3635aa24`  
		Last Modified: Wed, 01 Sep 2021 07:38:49 GMT  
		Size: 16.5 MB (16516915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e629e889c2474679b8c683c437e0f2c07f3eb6ff138f343123e94ba79b53f3bd`  
		Last Modified: Wed, 01 Sep 2021 07:38:38 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:86e637ce9b8977fd1ff0ec0051b5fae485669859e2ead6ea979dfa417bf551f9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.5 MB (19498314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4de5eb2d762e6c9497c99403310f87f4a28e3e9a6cb1fdde42caf8bd14a21eda`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:59 GMT
ADD file:da6c0ac7cb9f819998546d88fb489b746004eb2ad6da64a39210696ef0e66e54 in / 
# Wed, 01 Sep 2021 02:50:59 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 15:17:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 01 Sep 2021 15:18:09 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 01 Sep 2021 15:18:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 01 Sep 2021 15:18:09 GMT
EXPOSE 80
# Wed, 01 Sep 2021 15:18:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Sep 2021 15:18:10 GMT
CMD ["traefik"]
# Wed, 01 Sep 2021 15:18:10 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:07d756952c5cd45726cf9e8a292a3e05ca67eee5da176df7d632be8c5bb0ad04`  
		Last Modified: Wed, 01 Sep 2021 02:52:00 GMT  
		Size: 2.7 MB (2728407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b48c32784a3d41ea102d2f17f4d4e324c2ba601fb161674d9d4a00011aa73d1b`  
		Last Modified: Wed, 01 Sep 2021 15:19:10 GMT  
		Size: 675.5 KB (675540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1b0d042445ad5657836b1eac03f0ae037f0987de1e93443d6df927c4d4eeae`  
		Last Modified: Wed, 01 Sep 2021 15:19:44 GMT  
		Size: 16.1 MB (16093999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbcbd99d8138e0f5c6ce4e0ecc195d22221f020e36b06b095abdb44fb68a4efa`  
		Last Modified: Wed, 01 Sep 2021 15:19:41 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:1b0239abab3956d8d4196a010383178ee8aaef12f0b149639f2e3fa4ba4cb53d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `traefik:1.7-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull traefik@sha256:d1531e38dd2529216bc28c18053ed4f1bf45b41d1a7a6b8442022df1e468585c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2704996733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c03a2ee97d68f96240111c03d49cc4919ee386ac0379f32a4ef4d3cb22a91cc4`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 19:28:37 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 15 Sep 2021 19:28:38 GMT
EXPOSE 80
# Wed, 15 Sep 2021 19:28:39 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Sep 2021 19:28:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:e3704d6cbd09e058753b6a8d69ca830e6d27fe06bb0dfa835f5af467a730aa36`  
		Last Modified: Wed, 15 Sep 2021 19:29:52 GMT  
		Size: 18.3 MB (18293198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d3ef47b9f388a1fa894895dce20e457df357c460f0781eb3224b731e1c2fad`  
		Last Modified: Wed, 15 Sep 2021 19:29:48 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc66b759ec057c877e28b4bff777bd0d01802b2ae25dad9da11dc83b9ee4009`  
		Last Modified: Wed, 15 Sep 2021 19:29:48 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f3152ff49968644fbe2b5a199ab36a6e58ca1429b6e861613bf721541c6a50`  
		Last Modified: Wed, 15 Sep 2021 19:29:48 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.30`

```console
$ docker pull traefik@sha256:ca3883356d24f9fd6d36f0450d7f6f17a233317943517f6036c20ebf7c137781
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.30` - linux; amd64

```console
$ docker pull traefik@sha256:353827cc14120a14b1eccbb2714039763d9cefc284213b53d82d14e110fadc39
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.1 MB (18124621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a2126389e0b0dbd13da033d79636b0f0626d73f1a6da0935ce6ce9eccae112a`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 09 Mar 2021 01:32:48 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Tue, 09 Mar 2021 01:32:49 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 08 Apr 2021 20:07:38 GMT
COPY file:bc0b1c0235bda22a75d2ef00a982989cdf1da3240f077584bca5c6b560a4c13a in / 
# Thu, 08 Apr 2021 20:07:38 GMT
EXPOSE 80
# Thu, 08 Apr 2021 20:07:39 GMT
VOLUME [/tmp]
# Thu, 08 Apr 2021 20:07:39 GMT
ENTRYPOINT ["/traefik"]
# Thu, 08 Apr 2021 20:07:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:53f50c15495c67f391a5750288681a589b19a39c4b78e7ebc0934606cc3d0bc3`  
		Last Modified: Tue, 09 Mar 2021 01:33:59 GMT  
		Size: 130.9 KB (130870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c044b3636c16c5ab8fc96a04f320c9f97ea23aaffec9adb2d8f20ebaef93f3`  
		Last Modified: Tue, 09 Mar 2021 01:33:59 GMT  
		Size: 308.8 KB (308823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb3d26b40720e4da5cbeb15193c698565e23551a24cc4abc4acd1b7de414279`  
		Last Modified: Thu, 08 Apr 2021 20:08:34 GMT  
		Size: 17.7 MB (17684928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.30` - linux; arm variant v6

```console
$ docker pull traefik@sha256:13bd9d65c0558740d1b8b6f8de06f314003be9b54eec4b8b67dad2cf58d037c3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16956525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f60cea7c66ee3601de1cf66168feceac0bc9ac1147103e54d63f742e570bb0ca`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 22 Jun 2021 21:21:29 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Tue, 22 Jun 2021 21:21:31 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Tue, 22 Jun 2021 21:21:34 GMT
COPY file:440b6b1ebd389a2397ffb187ded4c85dcf37b7284d94c693b0b603d51247c683 in / 
# Tue, 22 Jun 2021 21:21:35 GMT
EXPOSE 80
# Tue, 22 Jun 2021 21:21:35 GMT
VOLUME [/tmp]
# Tue, 22 Jun 2021 21:21:35 GMT
ENTRYPOINT ["/traefik"]
# Tue, 22 Jun 2021 21:21:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:00918d1fc688f95413059b21ca56a6453b74d2808448ca35ed04b737d4a22c74`  
		Last Modified: Tue, 22 Jun 2021 21:24:22 GMT  
		Size: 130.9 KB (130871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e7abe8d1c9d1c5c74050eb312423f911185ce6cc705d32631fad6a1b3a4450`  
		Last Modified: Tue, 22 Jun 2021 21:24:23 GMT  
		Size: 308.9 KB (308853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee57e616d21eeb2181fd86ab18cbdb3be5af9c65ddb68c3657ebba7e266a191`  
		Last Modified: Tue, 22 Jun 2021 21:24:33 GMT  
		Size: 16.5 MB (16516801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.30` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:f7fe0c0982ce55e8882f88193462be30b654f27dd1c5014243efd6fd85d563ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16533633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0c3dd29cfce4ed4d7084315b52be936e63726239cbae0f98cf0c36cfdd8707a`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Wed, 16 Jun 2021 11:17:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Wed, 16 Jun 2021 11:17:48 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Wed, 16 Jun 2021 11:17:48 GMT
COPY file:6fdd60dc35db1c19a5de5ed8b57f159a6e121ba0f1ddb3e48a6e185da99f8cca in / 
# Wed, 16 Jun 2021 11:17:49 GMT
EXPOSE 80
# Wed, 16 Jun 2021 11:17:49 GMT
VOLUME [/tmp]
# Wed, 16 Jun 2021 11:17:49 GMT
ENTRYPOINT ["/traefik"]
# Wed, 16 Jun 2021 11:17:49 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ba07573b64554f7a74d3d3b27c42e28f5209c9d82f79b2596a6b190ee5475c72`  
		Last Modified: Wed, 16 Jun 2021 11:19:25 GMT  
		Size: 130.9 KB (130872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8a5756798f3769843250c96f2b11eca4d4c83a91616dd5d97d17399022fc6e`  
		Last Modified: Wed, 16 Jun 2021 11:19:25 GMT  
		Size: 308.9 KB (308857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6af1647ff43bc2a163e816afb6eb2c410d240b736297469f44ec6db498f13fc`  
		Last Modified: Wed, 16 Jun 2021 11:19:28 GMT  
		Size: 16.1 MB (16093904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.30-alpine`

```console
$ docker pull traefik@sha256:b5f54c8cff7bb0a8a249cbb00d79197403d63e8d4f813e2e50ba87884114f955
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.30-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:81038c31f0c7151418b10af58c252fb5e4d76c11a3d0b7a22aa66d61c3aadadc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.2 MB (21176792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8d154c84159a4d96e8aedebfa3bce9d19fc139b450d3b4eee1bb46e4ab759a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:31 GMT
ADD file:9d14b11183983923090d9e6d15cc51ee210466296e913bfefbfd580b3de59c95 in / 
# Tue, 31 Aug 2021 23:18:31 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 06:15:05 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 01 Sep 2021 06:15:16 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 01 Sep 2021 06:15:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 01 Sep 2021 06:15:16 GMT
EXPOSE 80
# Wed, 01 Sep 2021 06:15:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Sep 2021 06:15:17 GMT
CMD ["traefik"]
# Wed, 01 Sep 2021 06:15:17 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6a428f9f83b0a29f1fdd2ccccca19a9bab805a925b8eddf432a5a3d3da04afbc`  
		Last Modified: Tue, 31 Aug 2021 23:19:15 GMT  
		Size: 2.8 MB (2817307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f794cbdc99470251c9539251dc8a5aba6a6f0d6b4fd07a519bf8d13a9d42bbec`  
		Last Modified: Wed, 01 Sep 2021 06:16:08 GMT  
		Size: 674.2 KB (674226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa68ae87a84c1bc651faa725d25b0c37abf9514b31398de8ec4113c983f7bd3c`  
		Last Modified: Wed, 01 Sep 2021 06:16:31 GMT  
		Size: 17.7 MB (17684891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d6a80456e69fce8cd53394e12769c6b2757b1a318d8abd6eb0b1aa982e6791`  
		Last Modified: Wed, 01 Sep 2021 06:16:28 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.30-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:293b013a4e5f743eff9d2002d2affd2f1c948a60e8298af651c591ab79aa23c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.8 MB (19817351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9cdda6ba44e4d81cacd510102508f96d75ef73b1177f41a7154ea2822f45398`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:57 GMT
ADD file:3e83d6b5df3a951968e475c7326baf5ef90a22f04163693db34f3b4fc5812434 in / 
# Tue, 31 Aug 2021 22:30:57 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 07:35:43 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 01 Sep 2021 07:36:13 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 01 Sep 2021 07:36:14 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 01 Sep 2021 07:36:14 GMT
EXPOSE 80
# Wed, 01 Sep 2021 07:36:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Sep 2021 07:36:15 GMT
CMD ["traefik"]
# Wed, 01 Sep 2021 07:36:15 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7fe987b00bcb1f14c5b65f89813475143c021e2f5c156705ac3525abe1b397a1`  
		Last Modified: Tue, 31 Aug 2021 22:32:38 GMT  
		Size: 2.6 MB (2623044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ba27e6c34ba3c95c27e5aeada45e16c63122f31ec4c676f827e54daf47caf1`  
		Last Modified: Wed, 01 Sep 2021 07:37:54 GMT  
		Size: 677.0 KB (677024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7656c78f5b42128229dc58a77d852c6a388c45cc8a4c25fcdeb15b3635aa24`  
		Last Modified: Wed, 01 Sep 2021 07:38:49 GMT  
		Size: 16.5 MB (16516915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e629e889c2474679b8c683c437e0f2c07f3eb6ff138f343123e94ba79b53f3bd`  
		Last Modified: Wed, 01 Sep 2021 07:38:38 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.30-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:86e637ce9b8977fd1ff0ec0051b5fae485669859e2ead6ea979dfa417bf551f9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.5 MB (19498314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4de5eb2d762e6c9497c99403310f87f4a28e3e9a6cb1fdde42caf8bd14a21eda`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:59 GMT
ADD file:da6c0ac7cb9f819998546d88fb489b746004eb2ad6da64a39210696ef0e66e54 in / 
# Wed, 01 Sep 2021 02:50:59 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 15:17:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 01 Sep 2021 15:18:09 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 01 Sep 2021 15:18:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 01 Sep 2021 15:18:09 GMT
EXPOSE 80
# Wed, 01 Sep 2021 15:18:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Sep 2021 15:18:10 GMT
CMD ["traefik"]
# Wed, 01 Sep 2021 15:18:10 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:07d756952c5cd45726cf9e8a292a3e05ca67eee5da176df7d632be8c5bb0ad04`  
		Last Modified: Wed, 01 Sep 2021 02:52:00 GMT  
		Size: 2.7 MB (2728407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b48c32784a3d41ea102d2f17f4d4e324c2ba601fb161674d9d4a00011aa73d1b`  
		Last Modified: Wed, 01 Sep 2021 15:19:10 GMT  
		Size: 675.5 KB (675540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1b0d042445ad5657836b1eac03f0ae037f0987de1e93443d6df927c4d4eeae`  
		Last Modified: Wed, 01 Sep 2021 15:19:44 GMT  
		Size: 16.1 MB (16093999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbcbd99d8138e0f5c6ce4e0ecc195d22221f020e36b06b095abdb44fb68a4efa`  
		Last Modified: Wed, 01 Sep 2021 15:19:41 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.30-windowsservercore-1809`

```console
$ docker pull traefik@sha256:1b0239abab3956d8d4196a010383178ee8aaef12f0b149639f2e3fa4ba4cb53d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `traefik:1.7.30-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull traefik@sha256:d1531e38dd2529216bc28c18053ed4f1bf45b41d1a7a6b8442022df1e468585c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2704996733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c03a2ee97d68f96240111c03d49cc4919ee386ac0379f32a4ef4d3cb22a91cc4`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 19:28:37 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 15 Sep 2021 19:28:38 GMT
EXPOSE 80
# Wed, 15 Sep 2021 19:28:39 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Sep 2021 19:28:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:e3704d6cbd09e058753b6a8d69ca830e6d27fe06bb0dfa835f5af467a730aa36`  
		Last Modified: Wed, 15 Sep 2021 19:29:52 GMT  
		Size: 18.3 MB (18293198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d3ef47b9f388a1fa894895dce20e457df357c460f0781eb3224b731e1c2fad`  
		Last Modified: Wed, 15 Sep 2021 19:29:48 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc66b759ec057c877e28b4bff777bd0d01802b2ae25dad9da11dc83b9ee4009`  
		Last Modified: Wed, 15 Sep 2021 19:29:48 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f3152ff49968644fbe2b5a199ab36a6e58ca1429b6e861613bf721541c6a50`  
		Last Modified: Wed, 15 Sep 2021 19:29:48 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.5`

```console
$ docker pull traefik@sha256:b8802f19de00e344ae5f87d8dde9ff17360a10cf0d5e85949a065de89e69bbe3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.5` - linux; amd64

```console
$ docker pull traefik@sha256:68f43dcc76a589f56839c997a50428a50b296b52299c42637d3cc98101252a43
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (29040605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daa4d30f224b0690388615733d18d2c22bfe08b96cedde9fbebf588ef1a43160`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:28:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 02 Sep 2021 17:28:40 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.2/traefik_v2.5.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 02 Sep 2021 17:28:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 02 Sep 2021 17:28:41 GMT
EXPOSE 80
# Thu, 02 Sep 2021 17:28:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Sep 2021 17:28:41 GMT
CMD ["traefik"]
# Thu, 02 Sep 2021 17:28:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:a668d6573180decf676feb4d8a4a0228c209d5c1ee12dc67f82881a3fe3e6245`  
		Last Modified: Thu, 02 Sep 2021 17:29:16 GMT  
		Size: 25.6 MB (25569436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5147406fd5c8b1a00e8cbbddb8a2b6c3da434268d5bfbc8e0d98cbb70b2df7`  
		Last Modified: Thu, 02 Sep 2021 17:29:11 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.5` - linux; arm variant v6

```console
$ docker pull traefik@sha256:9c1172f6792773f08678c37f4de551c7a2a1d4d0c034e3412298586d18f88e19
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27284853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b9ce4b665be1ef5825b1937974c8cdefc7adaa100553a0e131bef7dd9e67085`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 18:16:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 02 Sep 2021 18:16:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.2/traefik_v2.5.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 02 Sep 2021 18:16:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 02 Sep 2021 18:16:10 GMT
EXPOSE 80
# Thu, 02 Sep 2021 18:16:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Sep 2021 18:16:10 GMT
CMD ["traefik"]
# Thu, 02 Sep 2021 18:16:11 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:99aa880db88f752c79e3dd82e0022a16a56928ec2d77eed2755cf821b41b9160`  
		Last Modified: Thu, 02 Sep 2021 18:18:15 GMT  
		Size: 24.0 MB (23995047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63372cda2fd2655b2566608d3b9695c4f8d874102341530d6f240d692b535256`  
		Last Modified: Thu, 02 Sep 2021 18:17:58 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.5` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:71b500c36ec3c881c73e28772d01a093a4ec6f44820aaf8a6b6f7d5faa6c206c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26697968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6fc50b9732b9564ef38927ead6989eca25b8520dc03fb71ce6229d884206f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:46:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 02 Sep 2021 17:46:59 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.2/traefik_v2.5.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 02 Sep 2021 17:46:59 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 02 Sep 2021 17:46:59 GMT
EXPOSE 80
# Thu, 02 Sep 2021 17:46:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Sep 2021 17:46:59 GMT
CMD ["traefik"]
# Thu, 02 Sep 2021 17:47:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:cd063daf3161b4aacc7decf9067ae7f44038f1975e9f27f228849742e9a86817`  
		Last Modified: Thu, 02 Sep 2021 17:47:59 GMT  
		Size: 23.3 MB (23326916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352613b664f9fb294d87cbf07347b5a13a2eea70c8e0a63fdba90e986cea9daa`  
		Last Modified: Thu, 02 Sep 2021 17:47:55 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.5-windowsservercore-1809`

```console
$ docker pull traefik@sha256:40f5c06205690b1ef13af267bbf9a33b78ce633fd00b672879d33eaa145d07bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `traefik:2.5-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull traefik@sha256:5b8d39092d5b4d34d7982cf52e64dda36010d56f9fcde4b8158114b9676e35d1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2712862774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf8044f7add003bfa95131b3c6df3f951261c6bcbf981f254d6fff903b6c1fc9`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 19:27:38 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.5.2/traefik_v2.5.2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 15 Sep 2021 19:27:39 GMT
EXPOSE 80
# Wed, 15 Sep 2021 19:27:40 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Sep 2021 19:27:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:c5602f67e70eed0e9ce04209a516843ea46b21e6c1de63843762859835c3a804`  
		Last Modified: Wed, 15 Sep 2021 19:29:31 GMT  
		Size: 26.2 MB (26159239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a0f05b90187b215602292d983f8ff2764bde51a6b0a32866a1c0c30137cd2d`  
		Last Modified: Wed, 15 Sep 2021 19:29:02 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa91e1e9dc00568b45849808e2a3e0fab0a0e7acd90b970dcc9d51f81209a32`  
		Last Modified: Wed, 15 Sep 2021 19:29:02 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49f804adb8a048fdcf5c18bbc72e802d05c1b335b68c82fc2bd467f09f47a47`  
		Last Modified: Wed, 15 Sep 2021 19:29:02 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.5.2`

```console
$ docker pull traefik@sha256:b8802f19de00e344ae5f87d8dde9ff17360a10cf0d5e85949a065de89e69bbe3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.5.2` - linux; amd64

```console
$ docker pull traefik@sha256:68f43dcc76a589f56839c997a50428a50b296b52299c42637d3cc98101252a43
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (29040605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daa4d30f224b0690388615733d18d2c22bfe08b96cedde9fbebf588ef1a43160`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:28:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 02 Sep 2021 17:28:40 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.2/traefik_v2.5.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 02 Sep 2021 17:28:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 02 Sep 2021 17:28:41 GMT
EXPOSE 80
# Thu, 02 Sep 2021 17:28:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Sep 2021 17:28:41 GMT
CMD ["traefik"]
# Thu, 02 Sep 2021 17:28:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:a668d6573180decf676feb4d8a4a0228c209d5c1ee12dc67f82881a3fe3e6245`  
		Last Modified: Thu, 02 Sep 2021 17:29:16 GMT  
		Size: 25.6 MB (25569436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5147406fd5c8b1a00e8cbbddb8a2b6c3da434268d5bfbc8e0d98cbb70b2df7`  
		Last Modified: Thu, 02 Sep 2021 17:29:11 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.5.2` - linux; arm variant v6

```console
$ docker pull traefik@sha256:9c1172f6792773f08678c37f4de551c7a2a1d4d0c034e3412298586d18f88e19
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27284853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b9ce4b665be1ef5825b1937974c8cdefc7adaa100553a0e131bef7dd9e67085`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 18:16:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 02 Sep 2021 18:16:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.2/traefik_v2.5.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 02 Sep 2021 18:16:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 02 Sep 2021 18:16:10 GMT
EXPOSE 80
# Thu, 02 Sep 2021 18:16:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Sep 2021 18:16:10 GMT
CMD ["traefik"]
# Thu, 02 Sep 2021 18:16:11 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:99aa880db88f752c79e3dd82e0022a16a56928ec2d77eed2755cf821b41b9160`  
		Last Modified: Thu, 02 Sep 2021 18:18:15 GMT  
		Size: 24.0 MB (23995047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63372cda2fd2655b2566608d3b9695c4f8d874102341530d6f240d692b535256`  
		Last Modified: Thu, 02 Sep 2021 18:17:58 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.5.2` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:71b500c36ec3c881c73e28772d01a093a4ec6f44820aaf8a6b6f7d5faa6c206c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26697968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6fc50b9732b9564ef38927ead6989eca25b8520dc03fb71ce6229d884206f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:46:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 02 Sep 2021 17:46:59 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.2/traefik_v2.5.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 02 Sep 2021 17:46:59 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 02 Sep 2021 17:46:59 GMT
EXPOSE 80
# Thu, 02 Sep 2021 17:46:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Sep 2021 17:46:59 GMT
CMD ["traefik"]
# Thu, 02 Sep 2021 17:47:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:cd063daf3161b4aacc7decf9067ae7f44038f1975e9f27f228849742e9a86817`  
		Last Modified: Thu, 02 Sep 2021 17:47:59 GMT  
		Size: 23.3 MB (23326916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352613b664f9fb294d87cbf07347b5a13a2eea70c8e0a63fdba90e986cea9daa`  
		Last Modified: Thu, 02 Sep 2021 17:47:55 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.5.2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:40f5c06205690b1ef13af267bbf9a33b78ce633fd00b672879d33eaa145d07bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `traefik:2.5.2-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull traefik@sha256:5b8d39092d5b4d34d7982cf52e64dda36010d56f9fcde4b8158114b9676e35d1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2712862774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf8044f7add003bfa95131b3c6df3f951261c6bcbf981f254d6fff903b6c1fc9`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 19:27:38 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.5.2/traefik_v2.5.2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 15 Sep 2021 19:27:39 GMT
EXPOSE 80
# Wed, 15 Sep 2021 19:27:40 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Sep 2021 19:27:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:c5602f67e70eed0e9ce04209a516843ea46b21e6c1de63843762859835c3a804`  
		Last Modified: Wed, 15 Sep 2021 19:29:31 GMT  
		Size: 26.2 MB (26159239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a0f05b90187b215602292d983f8ff2764bde51a6b0a32866a1c0c30137cd2d`  
		Last Modified: Wed, 15 Sep 2021 19:29:02 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa91e1e9dc00568b45849808e2a3e0fab0a0e7acd90b970dcc9d51f81209a32`  
		Last Modified: Wed, 15 Sep 2021 19:29:02 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49f804adb8a048fdcf5c18bbc72e802d05c1b335b68c82fc2bd467f09f47a47`  
		Last Modified: Wed, 15 Sep 2021 19:29:02 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:brie`

```console
$ docker pull traefik@sha256:b8802f19de00e344ae5f87d8dde9ff17360a10cf0d5e85949a065de89e69bbe3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:brie` - linux; amd64

```console
$ docker pull traefik@sha256:68f43dcc76a589f56839c997a50428a50b296b52299c42637d3cc98101252a43
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (29040605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daa4d30f224b0690388615733d18d2c22bfe08b96cedde9fbebf588ef1a43160`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:28:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 02 Sep 2021 17:28:40 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.2/traefik_v2.5.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 02 Sep 2021 17:28:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 02 Sep 2021 17:28:41 GMT
EXPOSE 80
# Thu, 02 Sep 2021 17:28:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Sep 2021 17:28:41 GMT
CMD ["traefik"]
# Thu, 02 Sep 2021 17:28:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:a668d6573180decf676feb4d8a4a0228c209d5c1ee12dc67f82881a3fe3e6245`  
		Last Modified: Thu, 02 Sep 2021 17:29:16 GMT  
		Size: 25.6 MB (25569436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5147406fd5c8b1a00e8cbbddb8a2b6c3da434268d5bfbc8e0d98cbb70b2df7`  
		Last Modified: Thu, 02 Sep 2021 17:29:11 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:brie` - linux; arm variant v6

```console
$ docker pull traefik@sha256:9c1172f6792773f08678c37f4de551c7a2a1d4d0c034e3412298586d18f88e19
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27284853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b9ce4b665be1ef5825b1937974c8cdefc7adaa100553a0e131bef7dd9e67085`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 18:16:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 02 Sep 2021 18:16:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.2/traefik_v2.5.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 02 Sep 2021 18:16:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 02 Sep 2021 18:16:10 GMT
EXPOSE 80
# Thu, 02 Sep 2021 18:16:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Sep 2021 18:16:10 GMT
CMD ["traefik"]
# Thu, 02 Sep 2021 18:16:11 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:99aa880db88f752c79e3dd82e0022a16a56928ec2d77eed2755cf821b41b9160`  
		Last Modified: Thu, 02 Sep 2021 18:18:15 GMT  
		Size: 24.0 MB (23995047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63372cda2fd2655b2566608d3b9695c4f8d874102341530d6f240d692b535256`  
		Last Modified: Thu, 02 Sep 2021 18:17:58 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:brie` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:71b500c36ec3c881c73e28772d01a093a4ec6f44820aaf8a6b6f7d5faa6c206c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26697968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6fc50b9732b9564ef38927ead6989eca25b8520dc03fb71ce6229d884206f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:46:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 02 Sep 2021 17:46:59 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.2/traefik_v2.5.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 02 Sep 2021 17:46:59 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 02 Sep 2021 17:46:59 GMT
EXPOSE 80
# Thu, 02 Sep 2021 17:46:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Sep 2021 17:46:59 GMT
CMD ["traefik"]
# Thu, 02 Sep 2021 17:47:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:cd063daf3161b4aacc7decf9067ae7f44038f1975e9f27f228849742e9a86817`  
		Last Modified: Thu, 02 Sep 2021 17:47:59 GMT  
		Size: 23.3 MB (23326916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352613b664f9fb294d87cbf07347b5a13a2eea70c8e0a63fdba90e986cea9daa`  
		Last Modified: Thu, 02 Sep 2021 17:47:55 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:brie-windowsservercore-1809`

```console
$ docker pull traefik@sha256:40f5c06205690b1ef13af267bbf9a33b78ce633fd00b672879d33eaa145d07bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `traefik:brie-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull traefik@sha256:5b8d39092d5b4d34d7982cf52e64dda36010d56f9fcde4b8158114b9676e35d1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2712862774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf8044f7add003bfa95131b3c6df3f951261c6bcbf981f254d6fff903b6c1fc9`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 19:27:38 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.5.2/traefik_v2.5.2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 15 Sep 2021 19:27:39 GMT
EXPOSE 80
# Wed, 15 Sep 2021 19:27:40 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Sep 2021 19:27:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:c5602f67e70eed0e9ce04209a516843ea46b21e6c1de63843762859835c3a804`  
		Last Modified: Wed, 15 Sep 2021 19:29:31 GMT  
		Size: 26.2 MB (26159239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a0f05b90187b215602292d983f8ff2764bde51a6b0a32866a1c0c30137cd2d`  
		Last Modified: Wed, 15 Sep 2021 19:29:02 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa91e1e9dc00568b45849808e2a3e0fab0a0e7acd90b970dcc9d51f81209a32`  
		Last Modified: Wed, 15 Sep 2021 19:29:02 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49f804adb8a048fdcf5c18bbc72e802d05c1b335b68c82fc2bd467f09f47a47`  
		Last Modified: Wed, 15 Sep 2021 19:29:02 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:b8802f19de00e344ae5f87d8dde9ff17360a10cf0d5e85949a065de89e69bbe3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:68f43dcc76a589f56839c997a50428a50b296b52299c42637d3cc98101252a43
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (29040605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daa4d30f224b0690388615733d18d2c22bfe08b96cedde9fbebf588ef1a43160`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:28:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 02 Sep 2021 17:28:40 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.2/traefik_v2.5.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 02 Sep 2021 17:28:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 02 Sep 2021 17:28:41 GMT
EXPOSE 80
# Thu, 02 Sep 2021 17:28:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Sep 2021 17:28:41 GMT
CMD ["traefik"]
# Thu, 02 Sep 2021 17:28:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:a668d6573180decf676feb4d8a4a0228c209d5c1ee12dc67f82881a3fe3e6245`  
		Last Modified: Thu, 02 Sep 2021 17:29:16 GMT  
		Size: 25.6 MB (25569436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5147406fd5c8b1a00e8cbbddb8a2b6c3da434268d5bfbc8e0d98cbb70b2df7`  
		Last Modified: Thu, 02 Sep 2021 17:29:11 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:9c1172f6792773f08678c37f4de551c7a2a1d4d0c034e3412298586d18f88e19
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27284853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b9ce4b665be1ef5825b1937974c8cdefc7adaa100553a0e131bef7dd9e67085`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 18:16:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 02 Sep 2021 18:16:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.2/traefik_v2.5.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 02 Sep 2021 18:16:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 02 Sep 2021 18:16:10 GMT
EXPOSE 80
# Thu, 02 Sep 2021 18:16:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Sep 2021 18:16:10 GMT
CMD ["traefik"]
# Thu, 02 Sep 2021 18:16:11 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:99aa880db88f752c79e3dd82e0022a16a56928ec2d77eed2755cf821b41b9160`  
		Last Modified: Thu, 02 Sep 2021 18:18:15 GMT  
		Size: 24.0 MB (23995047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63372cda2fd2655b2566608d3b9695c4f8d874102341530d6f240d692b535256`  
		Last Modified: Thu, 02 Sep 2021 18:17:58 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:71b500c36ec3c881c73e28772d01a093a4ec6f44820aaf8a6b6f7d5faa6c206c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26697968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6fc50b9732b9564ef38927ead6989eca25b8520dc03fb71ce6229d884206f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:46:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 02 Sep 2021 17:46:59 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.2/traefik_v2.5.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 02 Sep 2021 17:46:59 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 02 Sep 2021 17:46:59 GMT
EXPOSE 80
# Thu, 02 Sep 2021 17:46:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Sep 2021 17:46:59 GMT
CMD ["traefik"]
# Thu, 02 Sep 2021 17:47:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:cd063daf3161b4aacc7decf9067ae7f44038f1975e9f27f228849742e9a86817`  
		Last Modified: Thu, 02 Sep 2021 17:47:59 GMT  
		Size: 23.3 MB (23326916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352613b664f9fb294d87cbf07347b5a13a2eea70c8e0a63fdba90e986cea9daa`  
		Last Modified: Thu, 02 Sep 2021 17:47:55 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles`

```console
$ docker pull traefik@sha256:ca3883356d24f9fd6d36f0450d7f6f17a233317943517f6036c20ebf7c137781
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles` - linux; amd64

```console
$ docker pull traefik@sha256:353827cc14120a14b1eccbb2714039763d9cefc284213b53d82d14e110fadc39
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.1 MB (18124621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a2126389e0b0dbd13da033d79636b0f0626d73f1a6da0935ce6ce9eccae112a`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 09 Mar 2021 01:32:48 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Tue, 09 Mar 2021 01:32:49 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 08 Apr 2021 20:07:38 GMT
COPY file:bc0b1c0235bda22a75d2ef00a982989cdf1da3240f077584bca5c6b560a4c13a in / 
# Thu, 08 Apr 2021 20:07:38 GMT
EXPOSE 80
# Thu, 08 Apr 2021 20:07:39 GMT
VOLUME [/tmp]
# Thu, 08 Apr 2021 20:07:39 GMT
ENTRYPOINT ["/traefik"]
# Thu, 08 Apr 2021 20:07:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:53f50c15495c67f391a5750288681a589b19a39c4b78e7ebc0934606cc3d0bc3`  
		Last Modified: Tue, 09 Mar 2021 01:33:59 GMT  
		Size: 130.9 KB (130870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c044b3636c16c5ab8fc96a04f320c9f97ea23aaffec9adb2d8f20ebaef93f3`  
		Last Modified: Tue, 09 Mar 2021 01:33:59 GMT  
		Size: 308.8 KB (308823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb3d26b40720e4da5cbeb15193c698565e23551a24cc4abc4acd1b7de414279`  
		Last Modified: Thu, 08 Apr 2021 20:08:34 GMT  
		Size: 17.7 MB (17684928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm variant v6

```console
$ docker pull traefik@sha256:13bd9d65c0558740d1b8b6f8de06f314003be9b54eec4b8b67dad2cf58d037c3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16956525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f60cea7c66ee3601de1cf66168feceac0bc9ac1147103e54d63f742e570bb0ca`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 22 Jun 2021 21:21:29 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Tue, 22 Jun 2021 21:21:31 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Tue, 22 Jun 2021 21:21:34 GMT
COPY file:440b6b1ebd389a2397ffb187ded4c85dcf37b7284d94c693b0b603d51247c683 in / 
# Tue, 22 Jun 2021 21:21:35 GMT
EXPOSE 80
# Tue, 22 Jun 2021 21:21:35 GMT
VOLUME [/tmp]
# Tue, 22 Jun 2021 21:21:35 GMT
ENTRYPOINT ["/traefik"]
# Tue, 22 Jun 2021 21:21:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:00918d1fc688f95413059b21ca56a6453b74d2808448ca35ed04b737d4a22c74`  
		Last Modified: Tue, 22 Jun 2021 21:24:22 GMT  
		Size: 130.9 KB (130871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e7abe8d1c9d1c5c74050eb312423f911185ce6cc705d32631fad6a1b3a4450`  
		Last Modified: Tue, 22 Jun 2021 21:24:23 GMT  
		Size: 308.9 KB (308853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee57e616d21eeb2181fd86ab18cbdb3be5af9c65ddb68c3657ebba7e266a191`  
		Last Modified: Tue, 22 Jun 2021 21:24:33 GMT  
		Size: 16.5 MB (16516801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:f7fe0c0982ce55e8882f88193462be30b654f27dd1c5014243efd6fd85d563ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16533633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0c3dd29cfce4ed4d7084315b52be936e63726239cbae0f98cf0c36cfdd8707a`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Wed, 16 Jun 2021 11:17:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Wed, 16 Jun 2021 11:17:48 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Wed, 16 Jun 2021 11:17:48 GMT
COPY file:6fdd60dc35db1c19a5de5ed8b57f159a6e121ba0f1ddb3e48a6e185da99f8cca in / 
# Wed, 16 Jun 2021 11:17:49 GMT
EXPOSE 80
# Wed, 16 Jun 2021 11:17:49 GMT
VOLUME [/tmp]
# Wed, 16 Jun 2021 11:17:49 GMT
ENTRYPOINT ["/traefik"]
# Wed, 16 Jun 2021 11:17:49 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ba07573b64554f7a74d3d3b27c42e28f5209c9d82f79b2596a6b190ee5475c72`  
		Last Modified: Wed, 16 Jun 2021 11:19:25 GMT  
		Size: 130.9 KB (130872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8a5756798f3769843250c96f2b11eca4d4c83a91616dd5d97d17399022fc6e`  
		Last Modified: Wed, 16 Jun 2021 11:19:25 GMT  
		Size: 308.9 KB (308857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6af1647ff43bc2a163e816afb6eb2c410d240b736297469f44ec6db498f13fc`  
		Last Modified: Wed, 16 Jun 2021 11:19:28 GMT  
		Size: 16.1 MB (16093904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-alpine`

```console
$ docker pull traefik@sha256:b5f54c8cff7bb0a8a249cbb00d79197403d63e8d4f813e2e50ba87884114f955
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:81038c31f0c7151418b10af58c252fb5e4d76c11a3d0b7a22aa66d61c3aadadc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.2 MB (21176792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8d154c84159a4d96e8aedebfa3bce9d19fc139b450d3b4eee1bb46e4ab759a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:31 GMT
ADD file:9d14b11183983923090d9e6d15cc51ee210466296e913bfefbfd580b3de59c95 in / 
# Tue, 31 Aug 2021 23:18:31 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 06:15:05 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 01 Sep 2021 06:15:16 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 01 Sep 2021 06:15:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 01 Sep 2021 06:15:16 GMT
EXPOSE 80
# Wed, 01 Sep 2021 06:15:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Sep 2021 06:15:17 GMT
CMD ["traefik"]
# Wed, 01 Sep 2021 06:15:17 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6a428f9f83b0a29f1fdd2ccccca19a9bab805a925b8eddf432a5a3d3da04afbc`  
		Last Modified: Tue, 31 Aug 2021 23:19:15 GMT  
		Size: 2.8 MB (2817307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f794cbdc99470251c9539251dc8a5aba6a6f0d6b4fd07a519bf8d13a9d42bbec`  
		Last Modified: Wed, 01 Sep 2021 06:16:08 GMT  
		Size: 674.2 KB (674226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa68ae87a84c1bc651faa725d25b0c37abf9514b31398de8ec4113c983f7bd3c`  
		Last Modified: Wed, 01 Sep 2021 06:16:31 GMT  
		Size: 17.7 MB (17684891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d6a80456e69fce8cd53394e12769c6b2757b1a318d8abd6eb0b1aa982e6791`  
		Last Modified: Wed, 01 Sep 2021 06:16:28 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:293b013a4e5f743eff9d2002d2affd2f1c948a60e8298af651c591ab79aa23c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.8 MB (19817351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9cdda6ba44e4d81cacd510102508f96d75ef73b1177f41a7154ea2822f45398`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:57 GMT
ADD file:3e83d6b5df3a951968e475c7326baf5ef90a22f04163693db34f3b4fc5812434 in / 
# Tue, 31 Aug 2021 22:30:57 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 07:35:43 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 01 Sep 2021 07:36:13 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 01 Sep 2021 07:36:14 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 01 Sep 2021 07:36:14 GMT
EXPOSE 80
# Wed, 01 Sep 2021 07:36:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Sep 2021 07:36:15 GMT
CMD ["traefik"]
# Wed, 01 Sep 2021 07:36:15 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7fe987b00bcb1f14c5b65f89813475143c021e2f5c156705ac3525abe1b397a1`  
		Last Modified: Tue, 31 Aug 2021 22:32:38 GMT  
		Size: 2.6 MB (2623044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ba27e6c34ba3c95c27e5aeada45e16c63122f31ec4c676f827e54daf47caf1`  
		Last Modified: Wed, 01 Sep 2021 07:37:54 GMT  
		Size: 677.0 KB (677024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7656c78f5b42128229dc58a77d852c6a388c45cc8a4c25fcdeb15b3635aa24`  
		Last Modified: Wed, 01 Sep 2021 07:38:49 GMT  
		Size: 16.5 MB (16516915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e629e889c2474679b8c683c437e0f2c07f3eb6ff138f343123e94ba79b53f3bd`  
		Last Modified: Wed, 01 Sep 2021 07:38:38 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:86e637ce9b8977fd1ff0ec0051b5fae485669859e2ead6ea979dfa417bf551f9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.5 MB (19498314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4de5eb2d762e6c9497c99403310f87f4a28e3e9a6cb1fdde42caf8bd14a21eda`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:59 GMT
ADD file:da6c0ac7cb9f819998546d88fb489b746004eb2ad6da64a39210696ef0e66e54 in / 
# Wed, 01 Sep 2021 02:50:59 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 15:17:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 01 Sep 2021 15:18:09 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 01 Sep 2021 15:18:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 01 Sep 2021 15:18:09 GMT
EXPOSE 80
# Wed, 01 Sep 2021 15:18:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Sep 2021 15:18:10 GMT
CMD ["traefik"]
# Wed, 01 Sep 2021 15:18:10 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:07d756952c5cd45726cf9e8a292a3e05ca67eee5da176df7d632be8c5bb0ad04`  
		Last Modified: Wed, 01 Sep 2021 02:52:00 GMT  
		Size: 2.7 MB (2728407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b48c32784a3d41ea102d2f17f4d4e324c2ba601fb161674d9d4a00011aa73d1b`  
		Last Modified: Wed, 01 Sep 2021 15:19:10 GMT  
		Size: 675.5 KB (675540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1b0d042445ad5657836b1eac03f0ae037f0987de1e93443d6df927c4d4eeae`  
		Last Modified: Wed, 01 Sep 2021 15:19:44 GMT  
		Size: 16.1 MB (16093999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbcbd99d8138e0f5c6ce4e0ecc195d22221f020e36b06b095abdb44fb68a4efa`  
		Last Modified: Wed, 01 Sep 2021 15:19:41 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-windowsservercore-1809`

```console
$ docker pull traefik@sha256:1b0239abab3956d8d4196a010383178ee8aaef12f0b149639f2e3fa4ba4cb53d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull traefik@sha256:d1531e38dd2529216bc28c18053ed4f1bf45b41d1a7a6b8442022df1e468585c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2704996733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c03a2ee97d68f96240111c03d49cc4919ee386ac0379f32a4ef4d3cb22a91cc4`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 19:28:37 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 15 Sep 2021 19:28:38 GMT
EXPOSE 80
# Wed, 15 Sep 2021 19:28:39 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Sep 2021 19:28:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:e3704d6cbd09e058753b6a8d69ca830e6d27fe06bb0dfa835f5af467a730aa36`  
		Last Modified: Wed, 15 Sep 2021 19:29:52 GMT  
		Size: 18.3 MB (18293198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d3ef47b9f388a1fa894895dce20e457df357c460f0781eb3224b731e1c2fad`  
		Last Modified: Wed, 15 Sep 2021 19:29:48 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc66b759ec057c877e28b4bff777bd0d01802b2ae25dad9da11dc83b9ee4009`  
		Last Modified: Wed, 15 Sep 2021 19:29:48 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f3152ff49968644fbe2b5a199ab36a6e58ca1429b6e861613bf721541c6a50`  
		Last Modified: Wed, 15 Sep 2021 19:29:48 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7`

```console
$ docker pull traefik@sha256:ca3883356d24f9fd6d36f0450d7f6f17a233317943517f6036c20ebf7c137781
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7` - linux; amd64

```console
$ docker pull traefik@sha256:353827cc14120a14b1eccbb2714039763d9cefc284213b53d82d14e110fadc39
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.1 MB (18124621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a2126389e0b0dbd13da033d79636b0f0626d73f1a6da0935ce6ce9eccae112a`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 09 Mar 2021 01:32:48 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Tue, 09 Mar 2021 01:32:49 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 08 Apr 2021 20:07:38 GMT
COPY file:bc0b1c0235bda22a75d2ef00a982989cdf1da3240f077584bca5c6b560a4c13a in / 
# Thu, 08 Apr 2021 20:07:38 GMT
EXPOSE 80
# Thu, 08 Apr 2021 20:07:39 GMT
VOLUME [/tmp]
# Thu, 08 Apr 2021 20:07:39 GMT
ENTRYPOINT ["/traefik"]
# Thu, 08 Apr 2021 20:07:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:53f50c15495c67f391a5750288681a589b19a39c4b78e7ebc0934606cc3d0bc3`  
		Last Modified: Tue, 09 Mar 2021 01:33:59 GMT  
		Size: 130.9 KB (130870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c044b3636c16c5ab8fc96a04f320c9f97ea23aaffec9adb2d8f20ebaef93f3`  
		Last Modified: Tue, 09 Mar 2021 01:33:59 GMT  
		Size: 308.8 KB (308823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb3d26b40720e4da5cbeb15193c698565e23551a24cc4abc4acd1b7de414279`  
		Last Modified: Thu, 08 Apr 2021 20:08:34 GMT  
		Size: 17.7 MB (17684928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:13bd9d65c0558740d1b8b6f8de06f314003be9b54eec4b8b67dad2cf58d037c3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16956525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f60cea7c66ee3601de1cf66168feceac0bc9ac1147103e54d63f742e570bb0ca`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 22 Jun 2021 21:21:29 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Tue, 22 Jun 2021 21:21:31 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Tue, 22 Jun 2021 21:21:34 GMT
COPY file:440b6b1ebd389a2397ffb187ded4c85dcf37b7284d94c693b0b603d51247c683 in / 
# Tue, 22 Jun 2021 21:21:35 GMT
EXPOSE 80
# Tue, 22 Jun 2021 21:21:35 GMT
VOLUME [/tmp]
# Tue, 22 Jun 2021 21:21:35 GMT
ENTRYPOINT ["/traefik"]
# Tue, 22 Jun 2021 21:21:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:00918d1fc688f95413059b21ca56a6453b74d2808448ca35ed04b737d4a22c74`  
		Last Modified: Tue, 22 Jun 2021 21:24:22 GMT  
		Size: 130.9 KB (130871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e7abe8d1c9d1c5c74050eb312423f911185ce6cc705d32631fad6a1b3a4450`  
		Last Modified: Tue, 22 Jun 2021 21:24:23 GMT  
		Size: 308.9 KB (308853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee57e616d21eeb2181fd86ab18cbdb3be5af9c65ddb68c3657ebba7e266a191`  
		Last Modified: Tue, 22 Jun 2021 21:24:33 GMT  
		Size: 16.5 MB (16516801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:f7fe0c0982ce55e8882f88193462be30b654f27dd1c5014243efd6fd85d563ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16533633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0c3dd29cfce4ed4d7084315b52be936e63726239cbae0f98cf0c36cfdd8707a`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Wed, 16 Jun 2021 11:17:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Wed, 16 Jun 2021 11:17:48 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Wed, 16 Jun 2021 11:17:48 GMT
COPY file:6fdd60dc35db1c19a5de5ed8b57f159a6e121ba0f1ddb3e48a6e185da99f8cca in / 
# Wed, 16 Jun 2021 11:17:49 GMT
EXPOSE 80
# Wed, 16 Jun 2021 11:17:49 GMT
VOLUME [/tmp]
# Wed, 16 Jun 2021 11:17:49 GMT
ENTRYPOINT ["/traefik"]
# Wed, 16 Jun 2021 11:17:49 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ba07573b64554f7a74d3d3b27c42e28f5209c9d82f79b2596a6b190ee5475c72`  
		Last Modified: Wed, 16 Jun 2021 11:19:25 GMT  
		Size: 130.9 KB (130872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8a5756798f3769843250c96f2b11eca4d4c83a91616dd5d97d17399022fc6e`  
		Last Modified: Wed, 16 Jun 2021 11:19:25 GMT  
		Size: 308.9 KB (308857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6af1647ff43bc2a163e816afb6eb2c410d240b736297469f44ec6db498f13fc`  
		Last Modified: Wed, 16 Jun 2021 11:19:28 GMT  
		Size: 16.1 MB (16093904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-alpine`

```console
$ docker pull traefik@sha256:b5f54c8cff7bb0a8a249cbb00d79197403d63e8d4f813e2e50ba87884114f955
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:81038c31f0c7151418b10af58c252fb5e4d76c11a3d0b7a22aa66d61c3aadadc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.2 MB (21176792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8d154c84159a4d96e8aedebfa3bce9d19fc139b450d3b4eee1bb46e4ab759a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:31 GMT
ADD file:9d14b11183983923090d9e6d15cc51ee210466296e913bfefbfd580b3de59c95 in / 
# Tue, 31 Aug 2021 23:18:31 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 06:15:05 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 01 Sep 2021 06:15:16 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 01 Sep 2021 06:15:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 01 Sep 2021 06:15:16 GMT
EXPOSE 80
# Wed, 01 Sep 2021 06:15:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Sep 2021 06:15:17 GMT
CMD ["traefik"]
# Wed, 01 Sep 2021 06:15:17 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6a428f9f83b0a29f1fdd2ccccca19a9bab805a925b8eddf432a5a3d3da04afbc`  
		Last Modified: Tue, 31 Aug 2021 23:19:15 GMT  
		Size: 2.8 MB (2817307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f794cbdc99470251c9539251dc8a5aba6a6f0d6b4fd07a519bf8d13a9d42bbec`  
		Last Modified: Wed, 01 Sep 2021 06:16:08 GMT  
		Size: 674.2 KB (674226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa68ae87a84c1bc651faa725d25b0c37abf9514b31398de8ec4113c983f7bd3c`  
		Last Modified: Wed, 01 Sep 2021 06:16:31 GMT  
		Size: 17.7 MB (17684891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d6a80456e69fce8cd53394e12769c6b2757b1a318d8abd6eb0b1aa982e6791`  
		Last Modified: Wed, 01 Sep 2021 06:16:28 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:293b013a4e5f743eff9d2002d2affd2f1c948a60e8298af651c591ab79aa23c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.8 MB (19817351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9cdda6ba44e4d81cacd510102508f96d75ef73b1177f41a7154ea2822f45398`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:57 GMT
ADD file:3e83d6b5df3a951968e475c7326baf5ef90a22f04163693db34f3b4fc5812434 in / 
# Tue, 31 Aug 2021 22:30:57 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 07:35:43 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 01 Sep 2021 07:36:13 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 01 Sep 2021 07:36:14 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 01 Sep 2021 07:36:14 GMT
EXPOSE 80
# Wed, 01 Sep 2021 07:36:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Sep 2021 07:36:15 GMT
CMD ["traefik"]
# Wed, 01 Sep 2021 07:36:15 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7fe987b00bcb1f14c5b65f89813475143c021e2f5c156705ac3525abe1b397a1`  
		Last Modified: Tue, 31 Aug 2021 22:32:38 GMT  
		Size: 2.6 MB (2623044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ba27e6c34ba3c95c27e5aeada45e16c63122f31ec4c676f827e54daf47caf1`  
		Last Modified: Wed, 01 Sep 2021 07:37:54 GMT  
		Size: 677.0 KB (677024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7656c78f5b42128229dc58a77d852c6a388c45cc8a4c25fcdeb15b3635aa24`  
		Last Modified: Wed, 01 Sep 2021 07:38:49 GMT  
		Size: 16.5 MB (16516915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e629e889c2474679b8c683c437e0f2c07f3eb6ff138f343123e94ba79b53f3bd`  
		Last Modified: Wed, 01 Sep 2021 07:38:38 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:86e637ce9b8977fd1ff0ec0051b5fae485669859e2ead6ea979dfa417bf551f9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.5 MB (19498314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4de5eb2d762e6c9497c99403310f87f4a28e3e9a6cb1fdde42caf8bd14a21eda`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:59 GMT
ADD file:da6c0ac7cb9f819998546d88fb489b746004eb2ad6da64a39210696ef0e66e54 in / 
# Wed, 01 Sep 2021 02:50:59 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 15:17:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 01 Sep 2021 15:18:09 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 01 Sep 2021 15:18:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 01 Sep 2021 15:18:09 GMT
EXPOSE 80
# Wed, 01 Sep 2021 15:18:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Sep 2021 15:18:10 GMT
CMD ["traefik"]
# Wed, 01 Sep 2021 15:18:10 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:07d756952c5cd45726cf9e8a292a3e05ca67eee5da176df7d632be8c5bb0ad04`  
		Last Modified: Wed, 01 Sep 2021 02:52:00 GMT  
		Size: 2.7 MB (2728407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b48c32784a3d41ea102d2f17f4d4e324c2ba601fb161674d9d4a00011aa73d1b`  
		Last Modified: Wed, 01 Sep 2021 15:19:10 GMT  
		Size: 675.5 KB (675540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1b0d042445ad5657836b1eac03f0ae037f0987de1e93443d6df927c4d4eeae`  
		Last Modified: Wed, 01 Sep 2021 15:19:44 GMT  
		Size: 16.1 MB (16093999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbcbd99d8138e0f5c6ce4e0ecc195d22221f020e36b06b095abdb44fb68a4efa`  
		Last Modified: Wed, 01 Sep 2021 15:19:41 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:1b0239abab3956d8d4196a010383178ee8aaef12f0b149639f2e3fa4ba4cb53d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `traefik:v1.7-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull traefik@sha256:d1531e38dd2529216bc28c18053ed4f1bf45b41d1a7a6b8442022df1e468585c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2704996733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c03a2ee97d68f96240111c03d49cc4919ee386ac0379f32a4ef4d3cb22a91cc4`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 19:28:37 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 15 Sep 2021 19:28:38 GMT
EXPOSE 80
# Wed, 15 Sep 2021 19:28:39 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Sep 2021 19:28:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:e3704d6cbd09e058753b6a8d69ca830e6d27fe06bb0dfa835f5af467a730aa36`  
		Last Modified: Wed, 15 Sep 2021 19:29:52 GMT  
		Size: 18.3 MB (18293198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d3ef47b9f388a1fa894895dce20e457df357c460f0781eb3224b731e1c2fad`  
		Last Modified: Wed, 15 Sep 2021 19:29:48 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc66b759ec057c877e28b4bff777bd0d01802b2ae25dad9da11dc83b9ee4009`  
		Last Modified: Wed, 15 Sep 2021 19:29:48 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f3152ff49968644fbe2b5a199ab36a6e58ca1429b6e861613bf721541c6a50`  
		Last Modified: Wed, 15 Sep 2021 19:29:48 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.30`

```console
$ docker pull traefik@sha256:ca3883356d24f9fd6d36f0450d7f6f17a233317943517f6036c20ebf7c137781
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.30` - linux; amd64

```console
$ docker pull traefik@sha256:353827cc14120a14b1eccbb2714039763d9cefc284213b53d82d14e110fadc39
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.1 MB (18124621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a2126389e0b0dbd13da033d79636b0f0626d73f1a6da0935ce6ce9eccae112a`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 09 Mar 2021 01:32:48 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Tue, 09 Mar 2021 01:32:49 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 08 Apr 2021 20:07:38 GMT
COPY file:bc0b1c0235bda22a75d2ef00a982989cdf1da3240f077584bca5c6b560a4c13a in / 
# Thu, 08 Apr 2021 20:07:38 GMT
EXPOSE 80
# Thu, 08 Apr 2021 20:07:39 GMT
VOLUME [/tmp]
# Thu, 08 Apr 2021 20:07:39 GMT
ENTRYPOINT ["/traefik"]
# Thu, 08 Apr 2021 20:07:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:53f50c15495c67f391a5750288681a589b19a39c4b78e7ebc0934606cc3d0bc3`  
		Last Modified: Tue, 09 Mar 2021 01:33:59 GMT  
		Size: 130.9 KB (130870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c044b3636c16c5ab8fc96a04f320c9f97ea23aaffec9adb2d8f20ebaef93f3`  
		Last Modified: Tue, 09 Mar 2021 01:33:59 GMT  
		Size: 308.8 KB (308823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb3d26b40720e4da5cbeb15193c698565e23551a24cc4abc4acd1b7de414279`  
		Last Modified: Thu, 08 Apr 2021 20:08:34 GMT  
		Size: 17.7 MB (17684928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.30` - linux; arm variant v6

```console
$ docker pull traefik@sha256:13bd9d65c0558740d1b8b6f8de06f314003be9b54eec4b8b67dad2cf58d037c3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16956525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f60cea7c66ee3601de1cf66168feceac0bc9ac1147103e54d63f742e570bb0ca`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 22 Jun 2021 21:21:29 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Tue, 22 Jun 2021 21:21:31 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Tue, 22 Jun 2021 21:21:34 GMT
COPY file:440b6b1ebd389a2397ffb187ded4c85dcf37b7284d94c693b0b603d51247c683 in / 
# Tue, 22 Jun 2021 21:21:35 GMT
EXPOSE 80
# Tue, 22 Jun 2021 21:21:35 GMT
VOLUME [/tmp]
# Tue, 22 Jun 2021 21:21:35 GMT
ENTRYPOINT ["/traefik"]
# Tue, 22 Jun 2021 21:21:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:00918d1fc688f95413059b21ca56a6453b74d2808448ca35ed04b737d4a22c74`  
		Last Modified: Tue, 22 Jun 2021 21:24:22 GMT  
		Size: 130.9 KB (130871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e7abe8d1c9d1c5c74050eb312423f911185ce6cc705d32631fad6a1b3a4450`  
		Last Modified: Tue, 22 Jun 2021 21:24:23 GMT  
		Size: 308.9 KB (308853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee57e616d21eeb2181fd86ab18cbdb3be5af9c65ddb68c3657ebba7e266a191`  
		Last Modified: Tue, 22 Jun 2021 21:24:33 GMT  
		Size: 16.5 MB (16516801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.30` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:f7fe0c0982ce55e8882f88193462be30b654f27dd1c5014243efd6fd85d563ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16533633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0c3dd29cfce4ed4d7084315b52be936e63726239cbae0f98cf0c36cfdd8707a`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Wed, 16 Jun 2021 11:17:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Wed, 16 Jun 2021 11:17:48 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Wed, 16 Jun 2021 11:17:48 GMT
COPY file:6fdd60dc35db1c19a5de5ed8b57f159a6e121ba0f1ddb3e48a6e185da99f8cca in / 
# Wed, 16 Jun 2021 11:17:49 GMT
EXPOSE 80
# Wed, 16 Jun 2021 11:17:49 GMT
VOLUME [/tmp]
# Wed, 16 Jun 2021 11:17:49 GMT
ENTRYPOINT ["/traefik"]
# Wed, 16 Jun 2021 11:17:49 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ba07573b64554f7a74d3d3b27c42e28f5209c9d82f79b2596a6b190ee5475c72`  
		Last Modified: Wed, 16 Jun 2021 11:19:25 GMT  
		Size: 130.9 KB (130872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8a5756798f3769843250c96f2b11eca4d4c83a91616dd5d97d17399022fc6e`  
		Last Modified: Wed, 16 Jun 2021 11:19:25 GMT  
		Size: 308.9 KB (308857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6af1647ff43bc2a163e816afb6eb2c410d240b736297469f44ec6db498f13fc`  
		Last Modified: Wed, 16 Jun 2021 11:19:28 GMT  
		Size: 16.1 MB (16093904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.30-alpine`

```console
$ docker pull traefik@sha256:b5f54c8cff7bb0a8a249cbb00d79197403d63e8d4f813e2e50ba87884114f955
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.30-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:81038c31f0c7151418b10af58c252fb5e4d76c11a3d0b7a22aa66d61c3aadadc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.2 MB (21176792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8d154c84159a4d96e8aedebfa3bce9d19fc139b450d3b4eee1bb46e4ab759a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:31 GMT
ADD file:9d14b11183983923090d9e6d15cc51ee210466296e913bfefbfd580b3de59c95 in / 
# Tue, 31 Aug 2021 23:18:31 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 06:15:05 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 01 Sep 2021 06:15:16 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 01 Sep 2021 06:15:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 01 Sep 2021 06:15:16 GMT
EXPOSE 80
# Wed, 01 Sep 2021 06:15:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Sep 2021 06:15:17 GMT
CMD ["traefik"]
# Wed, 01 Sep 2021 06:15:17 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6a428f9f83b0a29f1fdd2ccccca19a9bab805a925b8eddf432a5a3d3da04afbc`  
		Last Modified: Tue, 31 Aug 2021 23:19:15 GMT  
		Size: 2.8 MB (2817307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f794cbdc99470251c9539251dc8a5aba6a6f0d6b4fd07a519bf8d13a9d42bbec`  
		Last Modified: Wed, 01 Sep 2021 06:16:08 GMT  
		Size: 674.2 KB (674226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa68ae87a84c1bc651faa725d25b0c37abf9514b31398de8ec4113c983f7bd3c`  
		Last Modified: Wed, 01 Sep 2021 06:16:31 GMT  
		Size: 17.7 MB (17684891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d6a80456e69fce8cd53394e12769c6b2757b1a318d8abd6eb0b1aa982e6791`  
		Last Modified: Wed, 01 Sep 2021 06:16:28 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.30-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:293b013a4e5f743eff9d2002d2affd2f1c948a60e8298af651c591ab79aa23c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.8 MB (19817351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9cdda6ba44e4d81cacd510102508f96d75ef73b1177f41a7154ea2822f45398`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:57 GMT
ADD file:3e83d6b5df3a951968e475c7326baf5ef90a22f04163693db34f3b4fc5812434 in / 
# Tue, 31 Aug 2021 22:30:57 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 07:35:43 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 01 Sep 2021 07:36:13 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 01 Sep 2021 07:36:14 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 01 Sep 2021 07:36:14 GMT
EXPOSE 80
# Wed, 01 Sep 2021 07:36:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Sep 2021 07:36:15 GMT
CMD ["traefik"]
# Wed, 01 Sep 2021 07:36:15 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7fe987b00bcb1f14c5b65f89813475143c021e2f5c156705ac3525abe1b397a1`  
		Last Modified: Tue, 31 Aug 2021 22:32:38 GMT  
		Size: 2.6 MB (2623044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ba27e6c34ba3c95c27e5aeada45e16c63122f31ec4c676f827e54daf47caf1`  
		Last Modified: Wed, 01 Sep 2021 07:37:54 GMT  
		Size: 677.0 KB (677024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7656c78f5b42128229dc58a77d852c6a388c45cc8a4c25fcdeb15b3635aa24`  
		Last Modified: Wed, 01 Sep 2021 07:38:49 GMT  
		Size: 16.5 MB (16516915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e629e889c2474679b8c683c437e0f2c07f3eb6ff138f343123e94ba79b53f3bd`  
		Last Modified: Wed, 01 Sep 2021 07:38:38 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.30-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:86e637ce9b8977fd1ff0ec0051b5fae485669859e2ead6ea979dfa417bf551f9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.5 MB (19498314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4de5eb2d762e6c9497c99403310f87f4a28e3e9a6cb1fdde42caf8bd14a21eda`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:59 GMT
ADD file:da6c0ac7cb9f819998546d88fb489b746004eb2ad6da64a39210696ef0e66e54 in / 
# Wed, 01 Sep 2021 02:50:59 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 15:17:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 01 Sep 2021 15:18:09 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 01 Sep 2021 15:18:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 01 Sep 2021 15:18:09 GMT
EXPOSE 80
# Wed, 01 Sep 2021 15:18:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Sep 2021 15:18:10 GMT
CMD ["traefik"]
# Wed, 01 Sep 2021 15:18:10 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:07d756952c5cd45726cf9e8a292a3e05ca67eee5da176df7d632be8c5bb0ad04`  
		Last Modified: Wed, 01 Sep 2021 02:52:00 GMT  
		Size: 2.7 MB (2728407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b48c32784a3d41ea102d2f17f4d4e324c2ba601fb161674d9d4a00011aa73d1b`  
		Last Modified: Wed, 01 Sep 2021 15:19:10 GMT  
		Size: 675.5 KB (675540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1b0d042445ad5657836b1eac03f0ae037f0987de1e93443d6df927c4d4eeae`  
		Last Modified: Wed, 01 Sep 2021 15:19:44 GMT  
		Size: 16.1 MB (16093999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbcbd99d8138e0f5c6ce4e0ecc195d22221f020e36b06b095abdb44fb68a4efa`  
		Last Modified: Wed, 01 Sep 2021 15:19:41 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.30-windowsservercore-1809`

```console
$ docker pull traefik@sha256:1b0239abab3956d8d4196a010383178ee8aaef12f0b149639f2e3fa4ba4cb53d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `traefik:v1.7.30-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull traefik@sha256:d1531e38dd2529216bc28c18053ed4f1bf45b41d1a7a6b8442022df1e468585c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2704996733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c03a2ee97d68f96240111c03d49cc4919ee386ac0379f32a4ef4d3cb22a91cc4`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 19:28:37 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 15 Sep 2021 19:28:38 GMT
EXPOSE 80
# Wed, 15 Sep 2021 19:28:39 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Sep 2021 19:28:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:e3704d6cbd09e058753b6a8d69ca830e6d27fe06bb0dfa835f5af467a730aa36`  
		Last Modified: Wed, 15 Sep 2021 19:29:52 GMT  
		Size: 18.3 MB (18293198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d3ef47b9f388a1fa894895dce20e457df357c460f0781eb3224b731e1c2fad`  
		Last Modified: Wed, 15 Sep 2021 19:29:48 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc66b759ec057c877e28b4bff777bd0d01802b2ae25dad9da11dc83b9ee4009`  
		Last Modified: Wed, 15 Sep 2021 19:29:48 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f3152ff49968644fbe2b5a199ab36a6e58ca1429b6e861613bf721541c6a50`  
		Last Modified: Wed, 15 Sep 2021 19:29:48 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.5`

```console
$ docker pull traefik@sha256:b8802f19de00e344ae5f87d8dde9ff17360a10cf0d5e85949a065de89e69bbe3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.5` - linux; amd64

```console
$ docker pull traefik@sha256:68f43dcc76a589f56839c997a50428a50b296b52299c42637d3cc98101252a43
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (29040605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daa4d30f224b0690388615733d18d2c22bfe08b96cedde9fbebf588ef1a43160`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:28:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 02 Sep 2021 17:28:40 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.2/traefik_v2.5.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 02 Sep 2021 17:28:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 02 Sep 2021 17:28:41 GMT
EXPOSE 80
# Thu, 02 Sep 2021 17:28:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Sep 2021 17:28:41 GMT
CMD ["traefik"]
# Thu, 02 Sep 2021 17:28:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:a668d6573180decf676feb4d8a4a0228c209d5c1ee12dc67f82881a3fe3e6245`  
		Last Modified: Thu, 02 Sep 2021 17:29:16 GMT  
		Size: 25.6 MB (25569436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5147406fd5c8b1a00e8cbbddb8a2b6c3da434268d5bfbc8e0d98cbb70b2df7`  
		Last Modified: Thu, 02 Sep 2021 17:29:11 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.5` - linux; arm variant v6

```console
$ docker pull traefik@sha256:9c1172f6792773f08678c37f4de551c7a2a1d4d0c034e3412298586d18f88e19
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27284853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b9ce4b665be1ef5825b1937974c8cdefc7adaa100553a0e131bef7dd9e67085`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 18:16:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 02 Sep 2021 18:16:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.2/traefik_v2.5.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 02 Sep 2021 18:16:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 02 Sep 2021 18:16:10 GMT
EXPOSE 80
# Thu, 02 Sep 2021 18:16:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Sep 2021 18:16:10 GMT
CMD ["traefik"]
# Thu, 02 Sep 2021 18:16:11 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:99aa880db88f752c79e3dd82e0022a16a56928ec2d77eed2755cf821b41b9160`  
		Last Modified: Thu, 02 Sep 2021 18:18:15 GMT  
		Size: 24.0 MB (23995047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63372cda2fd2655b2566608d3b9695c4f8d874102341530d6f240d692b535256`  
		Last Modified: Thu, 02 Sep 2021 18:17:58 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.5` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:71b500c36ec3c881c73e28772d01a093a4ec6f44820aaf8a6b6f7d5faa6c206c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26697968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6fc50b9732b9564ef38927ead6989eca25b8520dc03fb71ce6229d884206f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:46:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 02 Sep 2021 17:46:59 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.2/traefik_v2.5.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 02 Sep 2021 17:46:59 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 02 Sep 2021 17:46:59 GMT
EXPOSE 80
# Thu, 02 Sep 2021 17:46:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Sep 2021 17:46:59 GMT
CMD ["traefik"]
# Thu, 02 Sep 2021 17:47:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:cd063daf3161b4aacc7decf9067ae7f44038f1975e9f27f228849742e9a86817`  
		Last Modified: Thu, 02 Sep 2021 17:47:59 GMT  
		Size: 23.3 MB (23326916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352613b664f9fb294d87cbf07347b5a13a2eea70c8e0a63fdba90e986cea9daa`  
		Last Modified: Thu, 02 Sep 2021 17:47:55 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.5-windowsservercore-1809`

```console
$ docker pull traefik@sha256:40f5c06205690b1ef13af267bbf9a33b78ce633fd00b672879d33eaa145d07bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `traefik:v2.5-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull traefik@sha256:5b8d39092d5b4d34d7982cf52e64dda36010d56f9fcde4b8158114b9676e35d1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2712862774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf8044f7add003bfa95131b3c6df3f951261c6bcbf981f254d6fff903b6c1fc9`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 19:27:38 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.5.2/traefik_v2.5.2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 15 Sep 2021 19:27:39 GMT
EXPOSE 80
# Wed, 15 Sep 2021 19:27:40 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Sep 2021 19:27:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:c5602f67e70eed0e9ce04209a516843ea46b21e6c1de63843762859835c3a804`  
		Last Modified: Wed, 15 Sep 2021 19:29:31 GMT  
		Size: 26.2 MB (26159239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a0f05b90187b215602292d983f8ff2764bde51a6b0a32866a1c0c30137cd2d`  
		Last Modified: Wed, 15 Sep 2021 19:29:02 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa91e1e9dc00568b45849808e2a3e0fab0a0e7acd90b970dcc9d51f81209a32`  
		Last Modified: Wed, 15 Sep 2021 19:29:02 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49f804adb8a048fdcf5c18bbc72e802d05c1b335b68c82fc2bd467f09f47a47`  
		Last Modified: Wed, 15 Sep 2021 19:29:02 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.5.2`

```console
$ docker pull traefik@sha256:b8802f19de00e344ae5f87d8dde9ff17360a10cf0d5e85949a065de89e69bbe3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.5.2` - linux; amd64

```console
$ docker pull traefik@sha256:68f43dcc76a589f56839c997a50428a50b296b52299c42637d3cc98101252a43
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (29040605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daa4d30f224b0690388615733d18d2c22bfe08b96cedde9fbebf588ef1a43160`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:28:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 02 Sep 2021 17:28:40 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.2/traefik_v2.5.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 02 Sep 2021 17:28:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 02 Sep 2021 17:28:41 GMT
EXPOSE 80
# Thu, 02 Sep 2021 17:28:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Sep 2021 17:28:41 GMT
CMD ["traefik"]
# Thu, 02 Sep 2021 17:28:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:a668d6573180decf676feb4d8a4a0228c209d5c1ee12dc67f82881a3fe3e6245`  
		Last Modified: Thu, 02 Sep 2021 17:29:16 GMT  
		Size: 25.6 MB (25569436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5147406fd5c8b1a00e8cbbddb8a2b6c3da434268d5bfbc8e0d98cbb70b2df7`  
		Last Modified: Thu, 02 Sep 2021 17:29:11 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.5.2` - linux; arm variant v6

```console
$ docker pull traefik@sha256:9c1172f6792773f08678c37f4de551c7a2a1d4d0c034e3412298586d18f88e19
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27284853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b9ce4b665be1ef5825b1937974c8cdefc7adaa100553a0e131bef7dd9e67085`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 18:16:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 02 Sep 2021 18:16:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.2/traefik_v2.5.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 02 Sep 2021 18:16:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 02 Sep 2021 18:16:10 GMT
EXPOSE 80
# Thu, 02 Sep 2021 18:16:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Sep 2021 18:16:10 GMT
CMD ["traefik"]
# Thu, 02 Sep 2021 18:16:11 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:99aa880db88f752c79e3dd82e0022a16a56928ec2d77eed2755cf821b41b9160`  
		Last Modified: Thu, 02 Sep 2021 18:18:15 GMT  
		Size: 24.0 MB (23995047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63372cda2fd2655b2566608d3b9695c4f8d874102341530d6f240d692b535256`  
		Last Modified: Thu, 02 Sep 2021 18:17:58 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.5.2` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:71b500c36ec3c881c73e28772d01a093a4ec6f44820aaf8a6b6f7d5faa6c206c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26697968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6fc50b9732b9564ef38927ead6989eca25b8520dc03fb71ce6229d884206f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:46:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 02 Sep 2021 17:46:59 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.2/traefik_v2.5.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 02 Sep 2021 17:46:59 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 02 Sep 2021 17:46:59 GMT
EXPOSE 80
# Thu, 02 Sep 2021 17:46:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Sep 2021 17:46:59 GMT
CMD ["traefik"]
# Thu, 02 Sep 2021 17:47:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:cd063daf3161b4aacc7decf9067ae7f44038f1975e9f27f228849742e9a86817`  
		Last Modified: Thu, 02 Sep 2021 17:47:59 GMT  
		Size: 23.3 MB (23326916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352613b664f9fb294d87cbf07347b5a13a2eea70c8e0a63fdba90e986cea9daa`  
		Last Modified: Thu, 02 Sep 2021 17:47:55 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.5.2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:40f5c06205690b1ef13af267bbf9a33b78ce633fd00b672879d33eaa145d07bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `traefik:v2.5.2-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull traefik@sha256:5b8d39092d5b4d34d7982cf52e64dda36010d56f9fcde4b8158114b9676e35d1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2712862774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf8044f7add003bfa95131b3c6df3f951261c6bcbf981f254d6fff903b6c1fc9`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 19:27:38 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.5.2/traefik_v2.5.2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 15 Sep 2021 19:27:39 GMT
EXPOSE 80
# Wed, 15 Sep 2021 19:27:40 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Sep 2021 19:27:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:c5602f67e70eed0e9ce04209a516843ea46b21e6c1de63843762859835c3a804`  
		Last Modified: Wed, 15 Sep 2021 19:29:31 GMT  
		Size: 26.2 MB (26159239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a0f05b90187b215602292d983f8ff2764bde51a6b0a32866a1c0c30137cd2d`  
		Last Modified: Wed, 15 Sep 2021 19:29:02 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa91e1e9dc00568b45849808e2a3e0fab0a0e7acd90b970dcc9d51f81209a32`  
		Last Modified: Wed, 15 Sep 2021 19:29:02 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49f804adb8a048fdcf5c18bbc72e802d05c1b335b68c82fc2bd467f09f47a47`  
		Last Modified: Wed, 15 Sep 2021 19:29:02 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:40f5c06205690b1ef13af267bbf9a33b78ce633fd00b672879d33eaa145d07bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull traefik@sha256:5b8d39092d5b4d34d7982cf52e64dda36010d56f9fcde4b8158114b9676e35d1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2712862774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf8044f7add003bfa95131b3c6df3f951261c6bcbf981f254d6fff903b6c1fc9`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 19:27:38 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.5.2/traefik_v2.5.2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 15 Sep 2021 19:27:39 GMT
EXPOSE 80
# Wed, 15 Sep 2021 19:27:40 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Sep 2021 19:27:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:c5602f67e70eed0e9ce04209a516843ea46b21e6c1de63843762859835c3a804`  
		Last Modified: Wed, 15 Sep 2021 19:29:31 GMT  
		Size: 26.2 MB (26159239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a0f05b90187b215602292d983f8ff2764bde51a6b0a32866a1c0c30137cd2d`  
		Last Modified: Wed, 15 Sep 2021 19:29:02 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa91e1e9dc00568b45849808e2a3e0fab0a0e7acd90b970dcc9d51f81209a32`  
		Last Modified: Wed, 15 Sep 2021 19:29:02 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49f804adb8a048fdcf5c18bbc72e802d05c1b335b68c82fc2bd467f09f47a47`  
		Last Modified: Wed, 15 Sep 2021 19:29:02 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
