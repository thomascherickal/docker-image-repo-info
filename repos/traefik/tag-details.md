<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:1.7`](#traefik17)
-	[`traefik:1.7-alpine`](#traefik17-alpine)
-	[`traefik:1.7-windowsservercore-1809`](#traefik17-windowsservercore-1809)
-	[`traefik:1.7.29`](#traefik1729)
-	[`traefik:1.7.29-alpine`](#traefik1729-alpine)
-	[`traefik:1.7.29-windowsservercore-1809`](#traefik1729-windowsservercore-1809)
-	[`traefik:2.4`](#traefik24)
-	[`traefik:2.4-windowsservercore-1809`](#traefik24-windowsservercore-1809)
-	[`traefik:2.4.8`](#traefik248)
-	[`traefik:2.4.8-windowsservercore-1809`](#traefik248-windowsservercore-1809)
-	[`traefik:latest`](#traefiklatest)
-	[`traefik:livarot`](#traefiklivarot)
-	[`traefik:livarot-windowsservercore-1809`](#traefiklivarot-windowsservercore-1809)
-	[`traefik:maroilles`](#traefikmaroilles)
-	[`traefik:maroilles-alpine`](#traefikmaroilles-alpine)
-	[`traefik:maroilles-windowsservercore-1809`](#traefikmaroilles-windowsservercore-1809)
-	[`traefik:v1.7`](#traefikv17)
-	[`traefik:v1.7-alpine`](#traefikv17-alpine)
-	[`traefik:v1.7-windowsservercore-1809`](#traefikv17-windowsservercore-1809)
-	[`traefik:v1.7.29`](#traefikv1729)
-	[`traefik:v1.7.29-alpine`](#traefikv1729-alpine)
-	[`traefik:v1.7.29-windowsservercore-1809`](#traefikv1729-windowsservercore-1809)
-	[`traefik:v2.4`](#traefikv24)
-	[`traefik:v2.4-windowsservercore-1809`](#traefikv24-windowsservercore-1809)
-	[`traefik:v2.4.8`](#traefikv248)
-	[`traefik:v2.4.8-windowsservercore-1809`](#traefikv248-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:1.7`

```console
$ docker pull traefik@sha256:104e0d832ae7a26f56d8f22c92df8a94cb4fbbbb2a6a4f50a710434c40145847
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7` - linux; amd64

```console
$ docker pull traefik@sha256:e00ee616a3b242471dfd37fc4a47224500fb650d8472e80585bbce4af3758ff3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.1 MB (18137157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:906db490f80d11b8292995bafb68f446c473a489529213f82847242ae262b9d0`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 09 Mar 2021 01:32:48 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Tue, 09 Mar 2021 01:32:49 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Mon, 29 Mar 2021 20:21:39 GMT
COPY file:7412e1ec4df789a7c412d984053a91d6cbcfa5e717664daefd86f56d52133131 in / 
# Mon, 29 Mar 2021 20:21:39 GMT
EXPOSE 80
# Mon, 29 Mar 2021 20:21:39 GMT
VOLUME [/tmp]
# Mon, 29 Mar 2021 20:21:40 GMT
ENTRYPOINT ["/traefik"]
# Mon, 29 Mar 2021 20:21:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:94cd79ea7d84d34c942e13e7ef49f4d9b4d37a2c59fef618dc5ca44a93b5f66a`  
		Last Modified: Mon, 29 Mar 2021 20:22:35 GMT  
		Size: 17.7 MB (17697464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:ef4135732d30c6209b85cf47d6ce104df48f6c9139fde1f2f3eb5925704fa62a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16957254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f28c73e8f22c4d8b96ece80d2d6e3b65ae6246aa2ae4f356615714c2a7e79768`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:26:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Wed, 24 Feb 2021 23:34:19 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Mon, 29 Mar 2021 20:07:01 GMT
COPY file:021b5194c9f396ca24aaadd4ab3f8978febba7dff422827e0a613bb38224e5a2 in / 
# Mon, 29 Mar 2021 20:07:03 GMT
EXPOSE 80
# Mon, 29 Mar 2021 20:07:03 GMT
VOLUME [/tmp]
# Mon, 29 Mar 2021 20:07:04 GMT
ENTRYPOINT ["/traefik"]
# Mon, 29 Mar 2021 20:07:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:7e0c903ccfa53274059f2a4921657f10271ac6374b3f7f9094c4f026cc5a5b22`  
		Last Modified: Mon, 29 Mar 2021 20:07:50 GMT  
		Size: 16.5 MB (16517526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:58672e0711556e25704de4035eac1dd218ce82998a83986d912d4bff36aab0c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16538128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:526c897fe43b070574d98f9135897eaa2106fc575b3cec56dc9f9b213cfe72e2`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:27:56 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 25 Feb 2021 04:23:55 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Mon, 29 Mar 2021 19:52:36 GMT
COPY file:74c43ad3c5d71b75ac8726ad0ece7d7b6df15ddafbb3a2788809aba508d44be4 in / 
# Mon, 29 Mar 2021 19:52:37 GMT
EXPOSE 80
# Mon, 29 Mar 2021 19:52:38 GMT
VOLUME [/tmp]
# Mon, 29 Mar 2021 19:52:39 GMT
ENTRYPOINT ["/traefik"]
# Mon, 29 Mar 2021 19:52:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:de9c77266db7cadaf81c6da0e1965473c18b40e57e28336f2a8741e83f19d269`  
		Last Modified: Mon, 29 Mar 2021 19:53:22 GMT  
		Size: 16.1 MB (16098424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-alpine`

```console
$ docker pull traefik@sha256:5b2f8b55f214739049c50d852f607e5c6fd88db97a2c421b8bacd21c7d580197
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:8f3f2a0d4f3328c773a6e318f97f2737b8b01d878e1c6c28aae2c619bab6e715
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.2 MB (21187519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4b8d97846317066736c27e97b1037c0852ca8ffb67dc7194369a5629455a9a8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:19 GMT
ADD file:c744c1dc3da4145771e66d90e2e97a4f7fb702e5e07cf4e766ee0792cf161d92 in / 
# Wed, 31 Mar 2021 20:10:19 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:29:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 17:29:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.29/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 17:29:28 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 17:29:28 GMT
EXPOSE 80
# Thu, 01 Apr 2021 17:29:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 17:29:28 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 17:29:28 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9b794450f7b6db7c944ba1f4161edb68cb535052fe7db8ac06e613516c4a658d`  
		Last Modified: Wed, 31 Mar 2021 20:11:14 GMT  
		Size: 2.8 MB (2815346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c8802178dbdb14a188b12c88bfc76fb3c53283d93692a8f0e361bb1a3252d22`  
		Last Modified: Thu, 01 Apr 2021 17:29:57 GMT  
		Size: 674.2 KB (674206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6018d46b9ec53062f07d28e96d77f33343b177110d3d858548045fe10632aa54`  
		Last Modified: Thu, 01 Apr 2021 17:30:28 GMT  
		Size: 17.7 MB (17697599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b85e62c76fe27cb456ba2e73677bcc61a252d22da2283e8b116c49c13e6c17`  
		Last Modified: Thu, 01 Apr 2021 17:30:25 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f979f91b731033e20c3a939a8cf4421cef79843d72baf7f38ac1d05fdd2acc37
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.8 MB (19815995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d03cd3ce2303375e1d78220cb677c06b645760b71285ee468a5d297eedce7963`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:20 GMT
ADD file:15a1f9d3700deb648f0b3701afebc97ff28eb30d1b55e18dc9c696a9dd5c8e36 in / 
# Wed, 31 Mar 2021 17:19:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:52:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 03:53:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.29/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 03:53:06 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 03:53:07 GMT
EXPOSE 80
# Thu, 01 Apr 2021 03:53:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 03:53:09 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 03:53:10 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ac95243af174972febc49043f62f7b952a0c610e59b55ac4133f442e399e8729`  
		Last Modified: Wed, 31 Mar 2021 17:20:17 GMT  
		Size: 2.6 MB (2621248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25173f2bf7681888ff03bae0a793dcd2a8124175d360f999d21081483f90f181`  
		Last Modified: Thu, 01 Apr 2021 03:54:34 GMT  
		Size: 677.0 KB (677016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742427c956b4efd61ff21935a676a11fdd90f92afb76982a28be9f89e8adae33`  
		Last Modified: Thu, 01 Apr 2021 03:54:59 GMT  
		Size: 16.5 MB (16517363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b0d542a2b35d39348ec0f66b5b6f569020a95387fb7ee91fa9b627a363c171`  
		Last Modified: Thu, 01 Apr 2021 03:54:53 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:8f65a24b005efbe080078a819063b42dce92fa6e67e3ac4cc510ae2e02ad4004
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.5 MB (19500215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f91b2537ad19012ff83bee5b54a15a1d505afbb10d4170ffac365f414e362bc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:02 GMT
ADD file:174ba1b913c5cf549fcdfc259e8e3aa8f49cea660865fd54b8aacb430602a783 in / 
# Wed, 31 Mar 2021 17:22:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:15:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 16:15:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.29/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 16:15:40 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 16:15:42 GMT
EXPOSE 80
# Thu, 01 Apr 2021 16:15:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 16:15:44 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 16:15:45 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a3cf95b55367cb73f51318ee9c854def347373482336709ca1882a5d4c20b7c7`  
		Last Modified: Wed, 31 Mar 2021 17:23:00 GMT  
		Size: 2.7 MB (2725871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c5532ded8a461bb2539065ec0daf26ce2ecfed811ad86719ad11c964ab658`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 675.5 KB (675530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77a352edb1d69d5ba0f49daf5aeaeae71629ebbbded0ebf1e9fd64d0530136c`  
		Last Modified: Thu, 01 Apr 2021 16:18:23 GMT  
		Size: 16.1 MB (16098446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630d8f1d2a4cb7186cfdd5067d1f7497927474b2990138559aecc0df5c0f942a`  
		Last Modified: Thu, 01 Apr 2021 16:18:19 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:6eecb378641177fca09f19127265ab91271448ef60a5268ee68987276ccfe8c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `traefik:1.7-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull traefik@sha256:cf4582a473eb76ed41b990dfa297cc4d3bbd7f591095247d8d8594c00fbb78d4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2488937386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0972d358793f50271670241e2fe9aec32fe3650e7d8910e0b096f62563a41e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 29 Mar 2021 20:16:24 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.29/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Mon, 29 Mar 2021 20:16:26 GMT
EXPOSE 80
# Mon, 29 Mar 2021 20:16:27 GMT
ENTRYPOINT ["/traefik"]
# Mon, 29 Mar 2021 20:16:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530c2cf8b93172ab27963511ee3d2f36f94cc25e63ec870d1d91d56e05dd9722`  
		Last Modified: Mon, 29 Mar 2021 20:17:16 GMT  
		Size: 27.4 MB (27397196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be393dbe8be8c7a56d7d6fe4c431c56dd54a387bb81f572283ee86e3015dcb51`  
		Last Modified: Mon, 29 Mar 2021 20:17:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4d019fc76e3913da39f4402716b57bfa0395c64227907a2eb2b81878148ff7`  
		Last Modified: Mon, 29 Mar 2021 20:17:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d834588bef160f62373a77ce715af11b673c3e1673def36b2dcc290eb522870a`  
		Last Modified: Mon, 29 Mar 2021 20:17:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.29`

```console
$ docker pull traefik@sha256:104e0d832ae7a26f56d8f22c92df8a94cb4fbbbb2a6a4f50a710434c40145847
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.29` - linux; amd64

```console
$ docker pull traefik@sha256:e00ee616a3b242471dfd37fc4a47224500fb650d8472e80585bbce4af3758ff3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.1 MB (18137157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:906db490f80d11b8292995bafb68f446c473a489529213f82847242ae262b9d0`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 09 Mar 2021 01:32:48 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Tue, 09 Mar 2021 01:32:49 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Mon, 29 Mar 2021 20:21:39 GMT
COPY file:7412e1ec4df789a7c412d984053a91d6cbcfa5e717664daefd86f56d52133131 in / 
# Mon, 29 Mar 2021 20:21:39 GMT
EXPOSE 80
# Mon, 29 Mar 2021 20:21:39 GMT
VOLUME [/tmp]
# Mon, 29 Mar 2021 20:21:40 GMT
ENTRYPOINT ["/traefik"]
# Mon, 29 Mar 2021 20:21:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:94cd79ea7d84d34c942e13e7ef49f4d9b4d37a2c59fef618dc5ca44a93b5f66a`  
		Last Modified: Mon, 29 Mar 2021 20:22:35 GMT  
		Size: 17.7 MB (17697464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.29` - linux; arm variant v6

```console
$ docker pull traefik@sha256:ef4135732d30c6209b85cf47d6ce104df48f6c9139fde1f2f3eb5925704fa62a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16957254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f28c73e8f22c4d8b96ece80d2d6e3b65ae6246aa2ae4f356615714c2a7e79768`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:26:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Wed, 24 Feb 2021 23:34:19 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Mon, 29 Mar 2021 20:07:01 GMT
COPY file:021b5194c9f396ca24aaadd4ab3f8978febba7dff422827e0a613bb38224e5a2 in / 
# Mon, 29 Mar 2021 20:07:03 GMT
EXPOSE 80
# Mon, 29 Mar 2021 20:07:03 GMT
VOLUME [/tmp]
# Mon, 29 Mar 2021 20:07:04 GMT
ENTRYPOINT ["/traefik"]
# Mon, 29 Mar 2021 20:07:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:7e0c903ccfa53274059f2a4921657f10271ac6374b3f7f9094c4f026cc5a5b22`  
		Last Modified: Mon, 29 Mar 2021 20:07:50 GMT  
		Size: 16.5 MB (16517526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.29` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:58672e0711556e25704de4035eac1dd218ce82998a83986d912d4bff36aab0c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16538128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:526c897fe43b070574d98f9135897eaa2106fc575b3cec56dc9f9b213cfe72e2`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:27:56 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 25 Feb 2021 04:23:55 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Mon, 29 Mar 2021 19:52:36 GMT
COPY file:74c43ad3c5d71b75ac8726ad0ece7d7b6df15ddafbb3a2788809aba508d44be4 in / 
# Mon, 29 Mar 2021 19:52:37 GMT
EXPOSE 80
# Mon, 29 Mar 2021 19:52:38 GMT
VOLUME [/tmp]
# Mon, 29 Mar 2021 19:52:39 GMT
ENTRYPOINT ["/traefik"]
# Mon, 29 Mar 2021 19:52:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:de9c77266db7cadaf81c6da0e1965473c18b40e57e28336f2a8741e83f19d269`  
		Last Modified: Mon, 29 Mar 2021 19:53:22 GMT  
		Size: 16.1 MB (16098424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.29-alpine`

```console
$ docker pull traefik@sha256:5b2f8b55f214739049c50d852f607e5c6fd88db97a2c421b8bacd21c7d580197
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.29-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:8f3f2a0d4f3328c773a6e318f97f2737b8b01d878e1c6c28aae2c619bab6e715
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.2 MB (21187519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4b8d97846317066736c27e97b1037c0852ca8ffb67dc7194369a5629455a9a8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:19 GMT
ADD file:c744c1dc3da4145771e66d90e2e97a4f7fb702e5e07cf4e766ee0792cf161d92 in / 
# Wed, 31 Mar 2021 20:10:19 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:29:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 17:29:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.29/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 17:29:28 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 17:29:28 GMT
EXPOSE 80
# Thu, 01 Apr 2021 17:29:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 17:29:28 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 17:29:28 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9b794450f7b6db7c944ba1f4161edb68cb535052fe7db8ac06e613516c4a658d`  
		Last Modified: Wed, 31 Mar 2021 20:11:14 GMT  
		Size: 2.8 MB (2815346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c8802178dbdb14a188b12c88bfc76fb3c53283d93692a8f0e361bb1a3252d22`  
		Last Modified: Thu, 01 Apr 2021 17:29:57 GMT  
		Size: 674.2 KB (674206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6018d46b9ec53062f07d28e96d77f33343b177110d3d858548045fe10632aa54`  
		Last Modified: Thu, 01 Apr 2021 17:30:28 GMT  
		Size: 17.7 MB (17697599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b85e62c76fe27cb456ba2e73677bcc61a252d22da2283e8b116c49c13e6c17`  
		Last Modified: Thu, 01 Apr 2021 17:30:25 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.29-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f979f91b731033e20c3a939a8cf4421cef79843d72baf7f38ac1d05fdd2acc37
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.8 MB (19815995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d03cd3ce2303375e1d78220cb677c06b645760b71285ee468a5d297eedce7963`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:20 GMT
ADD file:15a1f9d3700deb648f0b3701afebc97ff28eb30d1b55e18dc9c696a9dd5c8e36 in / 
# Wed, 31 Mar 2021 17:19:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:52:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 03:53:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.29/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 03:53:06 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 03:53:07 GMT
EXPOSE 80
# Thu, 01 Apr 2021 03:53:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 03:53:09 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 03:53:10 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ac95243af174972febc49043f62f7b952a0c610e59b55ac4133f442e399e8729`  
		Last Modified: Wed, 31 Mar 2021 17:20:17 GMT  
		Size: 2.6 MB (2621248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25173f2bf7681888ff03bae0a793dcd2a8124175d360f999d21081483f90f181`  
		Last Modified: Thu, 01 Apr 2021 03:54:34 GMT  
		Size: 677.0 KB (677016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742427c956b4efd61ff21935a676a11fdd90f92afb76982a28be9f89e8adae33`  
		Last Modified: Thu, 01 Apr 2021 03:54:59 GMT  
		Size: 16.5 MB (16517363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b0d542a2b35d39348ec0f66b5b6f569020a95387fb7ee91fa9b627a363c171`  
		Last Modified: Thu, 01 Apr 2021 03:54:53 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.29-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:8f65a24b005efbe080078a819063b42dce92fa6e67e3ac4cc510ae2e02ad4004
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.5 MB (19500215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f91b2537ad19012ff83bee5b54a15a1d505afbb10d4170ffac365f414e362bc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:02 GMT
ADD file:174ba1b913c5cf549fcdfc259e8e3aa8f49cea660865fd54b8aacb430602a783 in / 
# Wed, 31 Mar 2021 17:22:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:15:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 16:15:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.29/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 16:15:40 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 16:15:42 GMT
EXPOSE 80
# Thu, 01 Apr 2021 16:15:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 16:15:44 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 16:15:45 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a3cf95b55367cb73f51318ee9c854def347373482336709ca1882a5d4c20b7c7`  
		Last Modified: Wed, 31 Mar 2021 17:23:00 GMT  
		Size: 2.7 MB (2725871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c5532ded8a461bb2539065ec0daf26ce2ecfed811ad86719ad11c964ab658`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 675.5 KB (675530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77a352edb1d69d5ba0f49daf5aeaeae71629ebbbded0ebf1e9fd64d0530136c`  
		Last Modified: Thu, 01 Apr 2021 16:18:23 GMT  
		Size: 16.1 MB (16098446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630d8f1d2a4cb7186cfdd5067d1f7497927474b2990138559aecc0df5c0f942a`  
		Last Modified: Thu, 01 Apr 2021 16:18:19 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.29-windowsservercore-1809`

```console
$ docker pull traefik@sha256:6eecb378641177fca09f19127265ab91271448ef60a5268ee68987276ccfe8c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `traefik:1.7.29-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull traefik@sha256:cf4582a473eb76ed41b990dfa297cc4d3bbd7f591095247d8d8594c00fbb78d4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2488937386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0972d358793f50271670241e2fe9aec32fe3650e7d8910e0b096f62563a41e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 29 Mar 2021 20:16:24 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.29/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Mon, 29 Mar 2021 20:16:26 GMT
EXPOSE 80
# Mon, 29 Mar 2021 20:16:27 GMT
ENTRYPOINT ["/traefik"]
# Mon, 29 Mar 2021 20:16:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530c2cf8b93172ab27963511ee3d2f36f94cc25e63ec870d1d91d56e05dd9722`  
		Last Modified: Mon, 29 Mar 2021 20:17:16 GMT  
		Size: 27.4 MB (27397196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be393dbe8be8c7a56d7d6fe4c431c56dd54a387bb81f572283ee86e3015dcb51`  
		Last Modified: Mon, 29 Mar 2021 20:17:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4d019fc76e3913da39f4402716b57bfa0395c64227907a2eb2b81878148ff7`  
		Last Modified: Mon, 29 Mar 2021 20:17:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d834588bef160f62373a77ce715af11b673c3e1673def36b2dcc290eb522870a`  
		Last Modified: Mon, 29 Mar 2021 20:17:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.4`

```console
$ docker pull traefik@sha256:d7d63b0d442f9954fbcb09e6fcc1a9c6251873469ee19f8aeaa13f0c776b3de6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.4` - linux; amd64

```console
$ docker pull traefik@sha256:51f066bfd65b83782047df91948efb5dad5f7cba31a057b0aee90a741896e710
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27827436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31431ad170701ff91cf26d1b06d8b5848a671e5fd3bab56276adf01727bc9831`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:19 GMT
ADD file:c744c1dc3da4145771e66d90e2e97a4f7fb702e5e07cf4e766ee0792cf161d92 in / 
# Wed, 31 Mar 2021 20:10:19 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:29:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 17:29:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 17:29:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 17:29:20 GMT
EXPOSE 80
# Thu, 01 Apr 2021 17:29:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 17:29:21 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 17:29:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9b794450f7b6db7c944ba1f4161edb68cb535052fe7db8ac06e613516c4a658d`  
		Last Modified: Wed, 31 Mar 2021 20:11:14 GMT  
		Size: 2.8 MB (2815346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c8802178dbdb14a188b12c88bfc76fb3c53283d93692a8f0e361bb1a3252d22`  
		Last Modified: Thu, 01 Apr 2021 17:29:57 GMT  
		Size: 674.2 KB (674206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365a033b4de2d1b88bb65502713fd041850bb27f0aab73939280b4fc2bec7ecf`  
		Last Modified: Thu, 01 Apr 2021 17:30:02 GMT  
		Size: 24.3 MB (24337516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a316ffd61dd62a5a271a399314e5f36d68b7ddb77e6600bc19fa0912593a0645`  
		Last Modified: Thu, 01 Apr 2021 17:29:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:445ec88018c03307101e734adfd8425f4da87e9ffd5d83b1e5fb512d280df5df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26025735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a68d5d0d7cdf26c5ef8132873c04d3e8cc92b65cd6ad0af323361a5c222c57f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:20 GMT
ADD file:15a1f9d3700deb648f0b3701afebc97ff28eb30d1b55e18dc9c696a9dd5c8e36 in / 
# Wed, 31 Mar 2021 17:19:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:52:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 03:52:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 03:52:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 03:52:45 GMT
EXPOSE 80
# Thu, 01 Apr 2021 03:52:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 03:52:48 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 03:52:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ac95243af174972febc49043f62f7b952a0c610e59b55ac4133f442e399e8729`  
		Last Modified: Wed, 31 Mar 2021 17:20:17 GMT  
		Size: 2.6 MB (2621248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25173f2bf7681888ff03bae0a793dcd2a8124175d360f999d21081483f90f181`  
		Last Modified: Thu, 01 Apr 2021 03:54:34 GMT  
		Size: 677.0 KB (677016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9546526ac0315b3d34e7f88f707fb5355cffd936afb2e80198eff85c6524a05`  
		Last Modified: Thu, 01 Apr 2021 03:54:41 GMT  
		Size: 22.7 MB (22727103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddd0b0952f4a6439010368b09c4bee68dd82bad0c47ff2a4a3a0b8ce6a2c498`  
		Last Modified: Thu, 01 Apr 2021 03:54:33 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.4` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:edd78c8c05d3050cbd62e00de1575597f2a1c628fd5faefecb0d8b20c35d7ba9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25475489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19eb3704549293128f6d623b5a417a6cf34b01a797b4e0bf36dee8ef8f255e71`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:02 GMT
ADD file:174ba1b913c5cf549fcdfc259e8e3aa8f49cea660865fd54b8aacb430602a783 in / 
# Wed, 31 Mar 2021 17:22:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:15:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 16:15:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 16:15:22 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 16:15:23 GMT
EXPOSE 80
# Thu, 01 Apr 2021 16:15:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 16:15:24 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 16:15:25 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a3cf95b55367cb73f51318ee9c854def347373482336709ca1882a5d4c20b7c7`  
		Last Modified: Wed, 31 Mar 2021 17:23:00 GMT  
		Size: 2.7 MB (2725871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c5532ded8a461bb2539065ec0daf26ce2ecfed811ad86719ad11c964ab658`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 675.5 KB (675530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664cdd830c93e0170df8d4ed17b45f260ee577dcfb6db4d48f6e009b108ff81d`  
		Last Modified: Thu, 01 Apr 2021 16:18:03 GMT  
		Size: 22.1 MB (22073720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bdc2d37fb1c66af3a73e5fff4790dcfa4572a7fd25779591f80bd086c718df`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:37b2b7f435939b597589efb591686eca5a0e6ae850d1c80ec0cb3f996c05d24f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `traefik:2.4-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull traefik@sha256:9345ce86759b6cc6053762a836111a43408fa15fc5571fba77ea93b43deefa00
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2495650153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f005e85992474d2eb3b06c7502a58d38c633edde288a548518128cd3e938f79c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 24 Mar 2021 01:16:17 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 24 Mar 2021 01:16:19 GMT
EXPOSE 80
# Wed, 24 Mar 2021 01:16:20 GMT
ENTRYPOINT ["/traefik"]
# Wed, 24 Mar 2021 01:16:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138871c226c89b2e75588935069c544f0c8ce5f68930fab95af0e4ca5a825d73`  
		Last Modified: Wed, 24 Mar 2021 01:17:09 GMT  
		Size: 34.1 MB (34109955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8574b4de7673b299ad666f81cd495bcfac5bf87fb33d4ef2781bdfcef30267`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb49e94abf40397ca09c966a1b4beb9579a20cb39ca8c9e17299ff206eb038e`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2d3f9210f45b7cb7f4c1ea77897d4576fcff778e51504d060afb3b28f4ae94`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.4.8`

```console
$ docker pull traefik@sha256:d7d63b0d442f9954fbcb09e6fcc1a9c6251873469ee19f8aeaa13f0c776b3de6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.4.8` - linux; amd64

```console
$ docker pull traefik@sha256:51f066bfd65b83782047df91948efb5dad5f7cba31a057b0aee90a741896e710
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27827436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31431ad170701ff91cf26d1b06d8b5848a671e5fd3bab56276adf01727bc9831`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:19 GMT
ADD file:c744c1dc3da4145771e66d90e2e97a4f7fb702e5e07cf4e766ee0792cf161d92 in / 
# Wed, 31 Mar 2021 20:10:19 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:29:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 17:29:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 17:29:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 17:29:20 GMT
EXPOSE 80
# Thu, 01 Apr 2021 17:29:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 17:29:21 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 17:29:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9b794450f7b6db7c944ba1f4161edb68cb535052fe7db8ac06e613516c4a658d`  
		Last Modified: Wed, 31 Mar 2021 20:11:14 GMT  
		Size: 2.8 MB (2815346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c8802178dbdb14a188b12c88bfc76fb3c53283d93692a8f0e361bb1a3252d22`  
		Last Modified: Thu, 01 Apr 2021 17:29:57 GMT  
		Size: 674.2 KB (674206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365a033b4de2d1b88bb65502713fd041850bb27f0aab73939280b4fc2bec7ecf`  
		Last Modified: Thu, 01 Apr 2021 17:30:02 GMT  
		Size: 24.3 MB (24337516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a316ffd61dd62a5a271a399314e5f36d68b7ddb77e6600bc19fa0912593a0645`  
		Last Modified: Thu, 01 Apr 2021 17:29:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.4.8` - linux; arm variant v6

```console
$ docker pull traefik@sha256:445ec88018c03307101e734adfd8425f4da87e9ffd5d83b1e5fb512d280df5df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26025735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a68d5d0d7cdf26c5ef8132873c04d3e8cc92b65cd6ad0af323361a5c222c57f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:20 GMT
ADD file:15a1f9d3700deb648f0b3701afebc97ff28eb30d1b55e18dc9c696a9dd5c8e36 in / 
# Wed, 31 Mar 2021 17:19:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:52:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 03:52:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 03:52:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 03:52:45 GMT
EXPOSE 80
# Thu, 01 Apr 2021 03:52:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 03:52:48 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 03:52:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ac95243af174972febc49043f62f7b952a0c610e59b55ac4133f442e399e8729`  
		Last Modified: Wed, 31 Mar 2021 17:20:17 GMT  
		Size: 2.6 MB (2621248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25173f2bf7681888ff03bae0a793dcd2a8124175d360f999d21081483f90f181`  
		Last Modified: Thu, 01 Apr 2021 03:54:34 GMT  
		Size: 677.0 KB (677016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9546526ac0315b3d34e7f88f707fb5355cffd936afb2e80198eff85c6524a05`  
		Last Modified: Thu, 01 Apr 2021 03:54:41 GMT  
		Size: 22.7 MB (22727103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddd0b0952f4a6439010368b09c4bee68dd82bad0c47ff2a4a3a0b8ce6a2c498`  
		Last Modified: Thu, 01 Apr 2021 03:54:33 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.4.8` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:edd78c8c05d3050cbd62e00de1575597f2a1c628fd5faefecb0d8b20c35d7ba9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25475489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19eb3704549293128f6d623b5a417a6cf34b01a797b4e0bf36dee8ef8f255e71`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:02 GMT
ADD file:174ba1b913c5cf549fcdfc259e8e3aa8f49cea660865fd54b8aacb430602a783 in / 
# Wed, 31 Mar 2021 17:22:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:15:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 16:15:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 16:15:22 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 16:15:23 GMT
EXPOSE 80
# Thu, 01 Apr 2021 16:15:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 16:15:24 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 16:15:25 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a3cf95b55367cb73f51318ee9c854def347373482336709ca1882a5d4c20b7c7`  
		Last Modified: Wed, 31 Mar 2021 17:23:00 GMT  
		Size: 2.7 MB (2725871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c5532ded8a461bb2539065ec0daf26ce2ecfed811ad86719ad11c964ab658`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 675.5 KB (675530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664cdd830c93e0170df8d4ed17b45f260ee577dcfb6db4d48f6e009b108ff81d`  
		Last Modified: Thu, 01 Apr 2021 16:18:03 GMT  
		Size: 22.1 MB (22073720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bdc2d37fb1c66af3a73e5fff4790dcfa4572a7fd25779591f80bd086c718df`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.4.8-windowsservercore-1809`

```console
$ docker pull traefik@sha256:37b2b7f435939b597589efb591686eca5a0e6ae850d1c80ec0cb3f996c05d24f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `traefik:2.4.8-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull traefik@sha256:9345ce86759b6cc6053762a836111a43408fa15fc5571fba77ea93b43deefa00
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2495650153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f005e85992474d2eb3b06c7502a58d38c633edde288a548518128cd3e938f79c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 24 Mar 2021 01:16:17 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 24 Mar 2021 01:16:19 GMT
EXPOSE 80
# Wed, 24 Mar 2021 01:16:20 GMT
ENTRYPOINT ["/traefik"]
# Wed, 24 Mar 2021 01:16:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138871c226c89b2e75588935069c544f0c8ce5f68930fab95af0e4ca5a825d73`  
		Last Modified: Wed, 24 Mar 2021 01:17:09 GMT  
		Size: 34.1 MB (34109955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8574b4de7673b299ad666f81cd495bcfac5bf87fb33d4ef2781bdfcef30267`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb49e94abf40397ca09c966a1b4beb9579a20cb39ca8c9e17299ff206eb038e`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2d3f9210f45b7cb7f4c1ea77897d4576fcff778e51504d060afb3b28f4ae94`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:d7d63b0d442f9954fbcb09e6fcc1a9c6251873469ee19f8aeaa13f0c776b3de6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:51f066bfd65b83782047df91948efb5dad5f7cba31a057b0aee90a741896e710
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27827436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31431ad170701ff91cf26d1b06d8b5848a671e5fd3bab56276adf01727bc9831`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:19 GMT
ADD file:c744c1dc3da4145771e66d90e2e97a4f7fb702e5e07cf4e766ee0792cf161d92 in / 
# Wed, 31 Mar 2021 20:10:19 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:29:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 17:29:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 17:29:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 17:29:20 GMT
EXPOSE 80
# Thu, 01 Apr 2021 17:29:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 17:29:21 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 17:29:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9b794450f7b6db7c944ba1f4161edb68cb535052fe7db8ac06e613516c4a658d`  
		Last Modified: Wed, 31 Mar 2021 20:11:14 GMT  
		Size: 2.8 MB (2815346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c8802178dbdb14a188b12c88bfc76fb3c53283d93692a8f0e361bb1a3252d22`  
		Last Modified: Thu, 01 Apr 2021 17:29:57 GMT  
		Size: 674.2 KB (674206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365a033b4de2d1b88bb65502713fd041850bb27f0aab73939280b4fc2bec7ecf`  
		Last Modified: Thu, 01 Apr 2021 17:30:02 GMT  
		Size: 24.3 MB (24337516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a316ffd61dd62a5a271a399314e5f36d68b7ddb77e6600bc19fa0912593a0645`  
		Last Modified: Thu, 01 Apr 2021 17:29:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:445ec88018c03307101e734adfd8425f4da87e9ffd5d83b1e5fb512d280df5df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26025735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a68d5d0d7cdf26c5ef8132873c04d3e8cc92b65cd6ad0af323361a5c222c57f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:20 GMT
ADD file:15a1f9d3700deb648f0b3701afebc97ff28eb30d1b55e18dc9c696a9dd5c8e36 in / 
# Wed, 31 Mar 2021 17:19:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:52:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 03:52:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 03:52:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 03:52:45 GMT
EXPOSE 80
# Thu, 01 Apr 2021 03:52:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 03:52:48 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 03:52:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ac95243af174972febc49043f62f7b952a0c610e59b55ac4133f442e399e8729`  
		Last Modified: Wed, 31 Mar 2021 17:20:17 GMT  
		Size: 2.6 MB (2621248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25173f2bf7681888ff03bae0a793dcd2a8124175d360f999d21081483f90f181`  
		Last Modified: Thu, 01 Apr 2021 03:54:34 GMT  
		Size: 677.0 KB (677016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9546526ac0315b3d34e7f88f707fb5355cffd936afb2e80198eff85c6524a05`  
		Last Modified: Thu, 01 Apr 2021 03:54:41 GMT  
		Size: 22.7 MB (22727103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddd0b0952f4a6439010368b09c4bee68dd82bad0c47ff2a4a3a0b8ce6a2c498`  
		Last Modified: Thu, 01 Apr 2021 03:54:33 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:edd78c8c05d3050cbd62e00de1575597f2a1c628fd5faefecb0d8b20c35d7ba9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25475489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19eb3704549293128f6d623b5a417a6cf34b01a797b4e0bf36dee8ef8f255e71`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:02 GMT
ADD file:174ba1b913c5cf549fcdfc259e8e3aa8f49cea660865fd54b8aacb430602a783 in / 
# Wed, 31 Mar 2021 17:22:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:15:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 16:15:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 16:15:22 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 16:15:23 GMT
EXPOSE 80
# Thu, 01 Apr 2021 16:15:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 16:15:24 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 16:15:25 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a3cf95b55367cb73f51318ee9c854def347373482336709ca1882a5d4c20b7c7`  
		Last Modified: Wed, 31 Mar 2021 17:23:00 GMT  
		Size: 2.7 MB (2725871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c5532ded8a461bb2539065ec0daf26ce2ecfed811ad86719ad11c964ab658`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 675.5 KB (675530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664cdd830c93e0170df8d4ed17b45f260ee577dcfb6db4d48f6e009b108ff81d`  
		Last Modified: Thu, 01 Apr 2021 16:18:03 GMT  
		Size: 22.1 MB (22073720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bdc2d37fb1c66af3a73e5fff4790dcfa4572a7fd25779591f80bd086c718df`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:livarot`

```console
$ docker pull traefik@sha256:d7d63b0d442f9954fbcb09e6fcc1a9c6251873469ee19f8aeaa13f0c776b3de6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:livarot` - linux; amd64

```console
$ docker pull traefik@sha256:51f066bfd65b83782047df91948efb5dad5f7cba31a057b0aee90a741896e710
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27827436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31431ad170701ff91cf26d1b06d8b5848a671e5fd3bab56276adf01727bc9831`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:19 GMT
ADD file:c744c1dc3da4145771e66d90e2e97a4f7fb702e5e07cf4e766ee0792cf161d92 in / 
# Wed, 31 Mar 2021 20:10:19 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:29:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 17:29:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 17:29:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 17:29:20 GMT
EXPOSE 80
# Thu, 01 Apr 2021 17:29:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 17:29:21 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 17:29:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9b794450f7b6db7c944ba1f4161edb68cb535052fe7db8ac06e613516c4a658d`  
		Last Modified: Wed, 31 Mar 2021 20:11:14 GMT  
		Size: 2.8 MB (2815346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c8802178dbdb14a188b12c88bfc76fb3c53283d93692a8f0e361bb1a3252d22`  
		Last Modified: Thu, 01 Apr 2021 17:29:57 GMT  
		Size: 674.2 KB (674206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365a033b4de2d1b88bb65502713fd041850bb27f0aab73939280b4fc2bec7ecf`  
		Last Modified: Thu, 01 Apr 2021 17:30:02 GMT  
		Size: 24.3 MB (24337516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a316ffd61dd62a5a271a399314e5f36d68b7ddb77e6600bc19fa0912593a0645`  
		Last Modified: Thu, 01 Apr 2021 17:29:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:livarot` - linux; arm variant v6

```console
$ docker pull traefik@sha256:445ec88018c03307101e734adfd8425f4da87e9ffd5d83b1e5fb512d280df5df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26025735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a68d5d0d7cdf26c5ef8132873c04d3e8cc92b65cd6ad0af323361a5c222c57f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:20 GMT
ADD file:15a1f9d3700deb648f0b3701afebc97ff28eb30d1b55e18dc9c696a9dd5c8e36 in / 
# Wed, 31 Mar 2021 17:19:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:52:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 03:52:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 03:52:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 03:52:45 GMT
EXPOSE 80
# Thu, 01 Apr 2021 03:52:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 03:52:48 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 03:52:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ac95243af174972febc49043f62f7b952a0c610e59b55ac4133f442e399e8729`  
		Last Modified: Wed, 31 Mar 2021 17:20:17 GMT  
		Size: 2.6 MB (2621248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25173f2bf7681888ff03bae0a793dcd2a8124175d360f999d21081483f90f181`  
		Last Modified: Thu, 01 Apr 2021 03:54:34 GMT  
		Size: 677.0 KB (677016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9546526ac0315b3d34e7f88f707fb5355cffd936afb2e80198eff85c6524a05`  
		Last Modified: Thu, 01 Apr 2021 03:54:41 GMT  
		Size: 22.7 MB (22727103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddd0b0952f4a6439010368b09c4bee68dd82bad0c47ff2a4a3a0b8ce6a2c498`  
		Last Modified: Thu, 01 Apr 2021 03:54:33 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:livarot` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:edd78c8c05d3050cbd62e00de1575597f2a1c628fd5faefecb0d8b20c35d7ba9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25475489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19eb3704549293128f6d623b5a417a6cf34b01a797b4e0bf36dee8ef8f255e71`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:02 GMT
ADD file:174ba1b913c5cf549fcdfc259e8e3aa8f49cea660865fd54b8aacb430602a783 in / 
# Wed, 31 Mar 2021 17:22:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:15:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 16:15:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 16:15:22 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 16:15:23 GMT
EXPOSE 80
# Thu, 01 Apr 2021 16:15:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 16:15:24 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 16:15:25 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a3cf95b55367cb73f51318ee9c854def347373482336709ca1882a5d4c20b7c7`  
		Last Modified: Wed, 31 Mar 2021 17:23:00 GMT  
		Size: 2.7 MB (2725871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c5532ded8a461bb2539065ec0daf26ce2ecfed811ad86719ad11c964ab658`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 675.5 KB (675530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664cdd830c93e0170df8d4ed17b45f260ee577dcfb6db4d48f6e009b108ff81d`  
		Last Modified: Thu, 01 Apr 2021 16:18:03 GMT  
		Size: 22.1 MB (22073720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bdc2d37fb1c66af3a73e5fff4790dcfa4572a7fd25779591f80bd086c718df`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:livarot-windowsservercore-1809`

```console
$ docker pull traefik@sha256:37b2b7f435939b597589efb591686eca5a0e6ae850d1c80ec0cb3f996c05d24f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `traefik:livarot-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull traefik@sha256:9345ce86759b6cc6053762a836111a43408fa15fc5571fba77ea93b43deefa00
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2495650153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f005e85992474d2eb3b06c7502a58d38c633edde288a548518128cd3e938f79c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 24 Mar 2021 01:16:17 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 24 Mar 2021 01:16:19 GMT
EXPOSE 80
# Wed, 24 Mar 2021 01:16:20 GMT
ENTRYPOINT ["/traefik"]
# Wed, 24 Mar 2021 01:16:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138871c226c89b2e75588935069c544f0c8ce5f68930fab95af0e4ca5a825d73`  
		Last Modified: Wed, 24 Mar 2021 01:17:09 GMT  
		Size: 34.1 MB (34109955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8574b4de7673b299ad666f81cd495bcfac5bf87fb33d4ef2781bdfcef30267`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb49e94abf40397ca09c966a1b4beb9579a20cb39ca8c9e17299ff206eb038e`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2d3f9210f45b7cb7f4c1ea77897d4576fcff778e51504d060afb3b28f4ae94`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles`

```console
$ docker pull traefik@sha256:104e0d832ae7a26f56d8f22c92df8a94cb4fbbbb2a6a4f50a710434c40145847
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles` - linux; amd64

```console
$ docker pull traefik@sha256:e00ee616a3b242471dfd37fc4a47224500fb650d8472e80585bbce4af3758ff3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.1 MB (18137157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:906db490f80d11b8292995bafb68f446c473a489529213f82847242ae262b9d0`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 09 Mar 2021 01:32:48 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Tue, 09 Mar 2021 01:32:49 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Mon, 29 Mar 2021 20:21:39 GMT
COPY file:7412e1ec4df789a7c412d984053a91d6cbcfa5e717664daefd86f56d52133131 in / 
# Mon, 29 Mar 2021 20:21:39 GMT
EXPOSE 80
# Mon, 29 Mar 2021 20:21:39 GMT
VOLUME [/tmp]
# Mon, 29 Mar 2021 20:21:40 GMT
ENTRYPOINT ["/traefik"]
# Mon, 29 Mar 2021 20:21:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:94cd79ea7d84d34c942e13e7ef49f4d9b4d37a2c59fef618dc5ca44a93b5f66a`  
		Last Modified: Mon, 29 Mar 2021 20:22:35 GMT  
		Size: 17.7 MB (17697464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm variant v6

```console
$ docker pull traefik@sha256:ef4135732d30c6209b85cf47d6ce104df48f6c9139fde1f2f3eb5925704fa62a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16957254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f28c73e8f22c4d8b96ece80d2d6e3b65ae6246aa2ae4f356615714c2a7e79768`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:26:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Wed, 24 Feb 2021 23:34:19 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Mon, 29 Mar 2021 20:07:01 GMT
COPY file:021b5194c9f396ca24aaadd4ab3f8978febba7dff422827e0a613bb38224e5a2 in / 
# Mon, 29 Mar 2021 20:07:03 GMT
EXPOSE 80
# Mon, 29 Mar 2021 20:07:03 GMT
VOLUME [/tmp]
# Mon, 29 Mar 2021 20:07:04 GMT
ENTRYPOINT ["/traefik"]
# Mon, 29 Mar 2021 20:07:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:7e0c903ccfa53274059f2a4921657f10271ac6374b3f7f9094c4f026cc5a5b22`  
		Last Modified: Mon, 29 Mar 2021 20:07:50 GMT  
		Size: 16.5 MB (16517526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:58672e0711556e25704de4035eac1dd218ce82998a83986d912d4bff36aab0c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16538128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:526c897fe43b070574d98f9135897eaa2106fc575b3cec56dc9f9b213cfe72e2`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:27:56 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 25 Feb 2021 04:23:55 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Mon, 29 Mar 2021 19:52:36 GMT
COPY file:74c43ad3c5d71b75ac8726ad0ece7d7b6df15ddafbb3a2788809aba508d44be4 in / 
# Mon, 29 Mar 2021 19:52:37 GMT
EXPOSE 80
# Mon, 29 Mar 2021 19:52:38 GMT
VOLUME [/tmp]
# Mon, 29 Mar 2021 19:52:39 GMT
ENTRYPOINT ["/traefik"]
# Mon, 29 Mar 2021 19:52:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:de9c77266db7cadaf81c6da0e1965473c18b40e57e28336f2a8741e83f19d269`  
		Last Modified: Mon, 29 Mar 2021 19:53:22 GMT  
		Size: 16.1 MB (16098424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-alpine`

```console
$ docker pull traefik@sha256:5b2f8b55f214739049c50d852f607e5c6fd88db97a2c421b8bacd21c7d580197
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:8f3f2a0d4f3328c773a6e318f97f2737b8b01d878e1c6c28aae2c619bab6e715
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.2 MB (21187519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4b8d97846317066736c27e97b1037c0852ca8ffb67dc7194369a5629455a9a8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:19 GMT
ADD file:c744c1dc3da4145771e66d90e2e97a4f7fb702e5e07cf4e766ee0792cf161d92 in / 
# Wed, 31 Mar 2021 20:10:19 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:29:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 17:29:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.29/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 17:29:28 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 17:29:28 GMT
EXPOSE 80
# Thu, 01 Apr 2021 17:29:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 17:29:28 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 17:29:28 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9b794450f7b6db7c944ba1f4161edb68cb535052fe7db8ac06e613516c4a658d`  
		Last Modified: Wed, 31 Mar 2021 20:11:14 GMT  
		Size: 2.8 MB (2815346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c8802178dbdb14a188b12c88bfc76fb3c53283d93692a8f0e361bb1a3252d22`  
		Last Modified: Thu, 01 Apr 2021 17:29:57 GMT  
		Size: 674.2 KB (674206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6018d46b9ec53062f07d28e96d77f33343b177110d3d858548045fe10632aa54`  
		Last Modified: Thu, 01 Apr 2021 17:30:28 GMT  
		Size: 17.7 MB (17697599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b85e62c76fe27cb456ba2e73677bcc61a252d22da2283e8b116c49c13e6c17`  
		Last Modified: Thu, 01 Apr 2021 17:30:25 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f979f91b731033e20c3a939a8cf4421cef79843d72baf7f38ac1d05fdd2acc37
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.8 MB (19815995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d03cd3ce2303375e1d78220cb677c06b645760b71285ee468a5d297eedce7963`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:20 GMT
ADD file:15a1f9d3700deb648f0b3701afebc97ff28eb30d1b55e18dc9c696a9dd5c8e36 in / 
# Wed, 31 Mar 2021 17:19:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:52:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 03:53:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.29/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 03:53:06 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 03:53:07 GMT
EXPOSE 80
# Thu, 01 Apr 2021 03:53:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 03:53:09 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 03:53:10 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ac95243af174972febc49043f62f7b952a0c610e59b55ac4133f442e399e8729`  
		Last Modified: Wed, 31 Mar 2021 17:20:17 GMT  
		Size: 2.6 MB (2621248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25173f2bf7681888ff03bae0a793dcd2a8124175d360f999d21081483f90f181`  
		Last Modified: Thu, 01 Apr 2021 03:54:34 GMT  
		Size: 677.0 KB (677016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742427c956b4efd61ff21935a676a11fdd90f92afb76982a28be9f89e8adae33`  
		Last Modified: Thu, 01 Apr 2021 03:54:59 GMT  
		Size: 16.5 MB (16517363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b0d542a2b35d39348ec0f66b5b6f569020a95387fb7ee91fa9b627a363c171`  
		Last Modified: Thu, 01 Apr 2021 03:54:53 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:8f65a24b005efbe080078a819063b42dce92fa6e67e3ac4cc510ae2e02ad4004
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.5 MB (19500215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f91b2537ad19012ff83bee5b54a15a1d505afbb10d4170ffac365f414e362bc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:02 GMT
ADD file:174ba1b913c5cf549fcdfc259e8e3aa8f49cea660865fd54b8aacb430602a783 in / 
# Wed, 31 Mar 2021 17:22:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:15:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 16:15:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.29/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 16:15:40 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 16:15:42 GMT
EXPOSE 80
# Thu, 01 Apr 2021 16:15:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 16:15:44 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 16:15:45 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a3cf95b55367cb73f51318ee9c854def347373482336709ca1882a5d4c20b7c7`  
		Last Modified: Wed, 31 Mar 2021 17:23:00 GMT  
		Size: 2.7 MB (2725871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c5532ded8a461bb2539065ec0daf26ce2ecfed811ad86719ad11c964ab658`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 675.5 KB (675530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77a352edb1d69d5ba0f49daf5aeaeae71629ebbbded0ebf1e9fd64d0530136c`  
		Last Modified: Thu, 01 Apr 2021 16:18:23 GMT  
		Size: 16.1 MB (16098446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630d8f1d2a4cb7186cfdd5067d1f7497927474b2990138559aecc0df5c0f942a`  
		Last Modified: Thu, 01 Apr 2021 16:18:19 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-windowsservercore-1809`

```console
$ docker pull traefik@sha256:6eecb378641177fca09f19127265ab91271448ef60a5268ee68987276ccfe8c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull traefik@sha256:cf4582a473eb76ed41b990dfa297cc4d3bbd7f591095247d8d8594c00fbb78d4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2488937386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0972d358793f50271670241e2fe9aec32fe3650e7d8910e0b096f62563a41e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 29 Mar 2021 20:16:24 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.29/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Mon, 29 Mar 2021 20:16:26 GMT
EXPOSE 80
# Mon, 29 Mar 2021 20:16:27 GMT
ENTRYPOINT ["/traefik"]
# Mon, 29 Mar 2021 20:16:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530c2cf8b93172ab27963511ee3d2f36f94cc25e63ec870d1d91d56e05dd9722`  
		Last Modified: Mon, 29 Mar 2021 20:17:16 GMT  
		Size: 27.4 MB (27397196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be393dbe8be8c7a56d7d6fe4c431c56dd54a387bb81f572283ee86e3015dcb51`  
		Last Modified: Mon, 29 Mar 2021 20:17:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4d019fc76e3913da39f4402716b57bfa0395c64227907a2eb2b81878148ff7`  
		Last Modified: Mon, 29 Mar 2021 20:17:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d834588bef160f62373a77ce715af11b673c3e1673def36b2dcc290eb522870a`  
		Last Modified: Mon, 29 Mar 2021 20:17:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7`

```console
$ docker pull traefik@sha256:104e0d832ae7a26f56d8f22c92df8a94cb4fbbbb2a6a4f50a710434c40145847
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7` - linux; amd64

```console
$ docker pull traefik@sha256:e00ee616a3b242471dfd37fc4a47224500fb650d8472e80585bbce4af3758ff3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.1 MB (18137157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:906db490f80d11b8292995bafb68f446c473a489529213f82847242ae262b9d0`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 09 Mar 2021 01:32:48 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Tue, 09 Mar 2021 01:32:49 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Mon, 29 Mar 2021 20:21:39 GMT
COPY file:7412e1ec4df789a7c412d984053a91d6cbcfa5e717664daefd86f56d52133131 in / 
# Mon, 29 Mar 2021 20:21:39 GMT
EXPOSE 80
# Mon, 29 Mar 2021 20:21:39 GMT
VOLUME [/tmp]
# Mon, 29 Mar 2021 20:21:40 GMT
ENTRYPOINT ["/traefik"]
# Mon, 29 Mar 2021 20:21:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:94cd79ea7d84d34c942e13e7ef49f4d9b4d37a2c59fef618dc5ca44a93b5f66a`  
		Last Modified: Mon, 29 Mar 2021 20:22:35 GMT  
		Size: 17.7 MB (17697464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:ef4135732d30c6209b85cf47d6ce104df48f6c9139fde1f2f3eb5925704fa62a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16957254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f28c73e8f22c4d8b96ece80d2d6e3b65ae6246aa2ae4f356615714c2a7e79768`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:26:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Wed, 24 Feb 2021 23:34:19 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Mon, 29 Mar 2021 20:07:01 GMT
COPY file:021b5194c9f396ca24aaadd4ab3f8978febba7dff422827e0a613bb38224e5a2 in / 
# Mon, 29 Mar 2021 20:07:03 GMT
EXPOSE 80
# Mon, 29 Mar 2021 20:07:03 GMT
VOLUME [/tmp]
# Mon, 29 Mar 2021 20:07:04 GMT
ENTRYPOINT ["/traefik"]
# Mon, 29 Mar 2021 20:07:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:7e0c903ccfa53274059f2a4921657f10271ac6374b3f7f9094c4f026cc5a5b22`  
		Last Modified: Mon, 29 Mar 2021 20:07:50 GMT  
		Size: 16.5 MB (16517526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:58672e0711556e25704de4035eac1dd218ce82998a83986d912d4bff36aab0c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16538128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:526c897fe43b070574d98f9135897eaa2106fc575b3cec56dc9f9b213cfe72e2`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:27:56 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 25 Feb 2021 04:23:55 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Mon, 29 Mar 2021 19:52:36 GMT
COPY file:74c43ad3c5d71b75ac8726ad0ece7d7b6df15ddafbb3a2788809aba508d44be4 in / 
# Mon, 29 Mar 2021 19:52:37 GMT
EXPOSE 80
# Mon, 29 Mar 2021 19:52:38 GMT
VOLUME [/tmp]
# Mon, 29 Mar 2021 19:52:39 GMT
ENTRYPOINT ["/traefik"]
# Mon, 29 Mar 2021 19:52:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:de9c77266db7cadaf81c6da0e1965473c18b40e57e28336f2a8741e83f19d269`  
		Last Modified: Mon, 29 Mar 2021 19:53:22 GMT  
		Size: 16.1 MB (16098424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-alpine`

```console
$ docker pull traefik@sha256:5b2f8b55f214739049c50d852f607e5c6fd88db97a2c421b8bacd21c7d580197
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:8f3f2a0d4f3328c773a6e318f97f2737b8b01d878e1c6c28aae2c619bab6e715
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.2 MB (21187519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4b8d97846317066736c27e97b1037c0852ca8ffb67dc7194369a5629455a9a8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:19 GMT
ADD file:c744c1dc3da4145771e66d90e2e97a4f7fb702e5e07cf4e766ee0792cf161d92 in / 
# Wed, 31 Mar 2021 20:10:19 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:29:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 17:29:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.29/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 17:29:28 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 17:29:28 GMT
EXPOSE 80
# Thu, 01 Apr 2021 17:29:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 17:29:28 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 17:29:28 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9b794450f7b6db7c944ba1f4161edb68cb535052fe7db8ac06e613516c4a658d`  
		Last Modified: Wed, 31 Mar 2021 20:11:14 GMT  
		Size: 2.8 MB (2815346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c8802178dbdb14a188b12c88bfc76fb3c53283d93692a8f0e361bb1a3252d22`  
		Last Modified: Thu, 01 Apr 2021 17:29:57 GMT  
		Size: 674.2 KB (674206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6018d46b9ec53062f07d28e96d77f33343b177110d3d858548045fe10632aa54`  
		Last Modified: Thu, 01 Apr 2021 17:30:28 GMT  
		Size: 17.7 MB (17697599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b85e62c76fe27cb456ba2e73677bcc61a252d22da2283e8b116c49c13e6c17`  
		Last Modified: Thu, 01 Apr 2021 17:30:25 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f979f91b731033e20c3a939a8cf4421cef79843d72baf7f38ac1d05fdd2acc37
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.8 MB (19815995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d03cd3ce2303375e1d78220cb677c06b645760b71285ee468a5d297eedce7963`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:20 GMT
ADD file:15a1f9d3700deb648f0b3701afebc97ff28eb30d1b55e18dc9c696a9dd5c8e36 in / 
# Wed, 31 Mar 2021 17:19:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:52:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 03:53:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.29/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 03:53:06 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 03:53:07 GMT
EXPOSE 80
# Thu, 01 Apr 2021 03:53:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 03:53:09 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 03:53:10 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ac95243af174972febc49043f62f7b952a0c610e59b55ac4133f442e399e8729`  
		Last Modified: Wed, 31 Mar 2021 17:20:17 GMT  
		Size: 2.6 MB (2621248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25173f2bf7681888ff03bae0a793dcd2a8124175d360f999d21081483f90f181`  
		Last Modified: Thu, 01 Apr 2021 03:54:34 GMT  
		Size: 677.0 KB (677016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742427c956b4efd61ff21935a676a11fdd90f92afb76982a28be9f89e8adae33`  
		Last Modified: Thu, 01 Apr 2021 03:54:59 GMT  
		Size: 16.5 MB (16517363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b0d542a2b35d39348ec0f66b5b6f569020a95387fb7ee91fa9b627a363c171`  
		Last Modified: Thu, 01 Apr 2021 03:54:53 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:8f65a24b005efbe080078a819063b42dce92fa6e67e3ac4cc510ae2e02ad4004
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.5 MB (19500215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f91b2537ad19012ff83bee5b54a15a1d505afbb10d4170ffac365f414e362bc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:02 GMT
ADD file:174ba1b913c5cf549fcdfc259e8e3aa8f49cea660865fd54b8aacb430602a783 in / 
# Wed, 31 Mar 2021 17:22:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:15:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 16:15:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.29/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 16:15:40 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 16:15:42 GMT
EXPOSE 80
# Thu, 01 Apr 2021 16:15:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 16:15:44 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 16:15:45 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a3cf95b55367cb73f51318ee9c854def347373482336709ca1882a5d4c20b7c7`  
		Last Modified: Wed, 31 Mar 2021 17:23:00 GMT  
		Size: 2.7 MB (2725871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c5532ded8a461bb2539065ec0daf26ce2ecfed811ad86719ad11c964ab658`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 675.5 KB (675530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77a352edb1d69d5ba0f49daf5aeaeae71629ebbbded0ebf1e9fd64d0530136c`  
		Last Modified: Thu, 01 Apr 2021 16:18:23 GMT  
		Size: 16.1 MB (16098446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630d8f1d2a4cb7186cfdd5067d1f7497927474b2990138559aecc0df5c0f942a`  
		Last Modified: Thu, 01 Apr 2021 16:18:19 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:6eecb378641177fca09f19127265ab91271448ef60a5268ee68987276ccfe8c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `traefik:v1.7-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull traefik@sha256:cf4582a473eb76ed41b990dfa297cc4d3bbd7f591095247d8d8594c00fbb78d4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2488937386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0972d358793f50271670241e2fe9aec32fe3650e7d8910e0b096f62563a41e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 29 Mar 2021 20:16:24 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.29/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Mon, 29 Mar 2021 20:16:26 GMT
EXPOSE 80
# Mon, 29 Mar 2021 20:16:27 GMT
ENTRYPOINT ["/traefik"]
# Mon, 29 Mar 2021 20:16:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530c2cf8b93172ab27963511ee3d2f36f94cc25e63ec870d1d91d56e05dd9722`  
		Last Modified: Mon, 29 Mar 2021 20:17:16 GMT  
		Size: 27.4 MB (27397196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be393dbe8be8c7a56d7d6fe4c431c56dd54a387bb81f572283ee86e3015dcb51`  
		Last Modified: Mon, 29 Mar 2021 20:17:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4d019fc76e3913da39f4402716b57bfa0395c64227907a2eb2b81878148ff7`  
		Last Modified: Mon, 29 Mar 2021 20:17:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d834588bef160f62373a77ce715af11b673c3e1673def36b2dcc290eb522870a`  
		Last Modified: Mon, 29 Mar 2021 20:17:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.29`

```console
$ docker pull traefik@sha256:104e0d832ae7a26f56d8f22c92df8a94cb4fbbbb2a6a4f50a710434c40145847
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.29` - linux; amd64

```console
$ docker pull traefik@sha256:e00ee616a3b242471dfd37fc4a47224500fb650d8472e80585bbce4af3758ff3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.1 MB (18137157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:906db490f80d11b8292995bafb68f446c473a489529213f82847242ae262b9d0`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 09 Mar 2021 01:32:48 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Tue, 09 Mar 2021 01:32:49 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Mon, 29 Mar 2021 20:21:39 GMT
COPY file:7412e1ec4df789a7c412d984053a91d6cbcfa5e717664daefd86f56d52133131 in / 
# Mon, 29 Mar 2021 20:21:39 GMT
EXPOSE 80
# Mon, 29 Mar 2021 20:21:39 GMT
VOLUME [/tmp]
# Mon, 29 Mar 2021 20:21:40 GMT
ENTRYPOINT ["/traefik"]
# Mon, 29 Mar 2021 20:21:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:94cd79ea7d84d34c942e13e7ef49f4d9b4d37a2c59fef618dc5ca44a93b5f66a`  
		Last Modified: Mon, 29 Mar 2021 20:22:35 GMT  
		Size: 17.7 MB (17697464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.29` - linux; arm variant v6

```console
$ docker pull traefik@sha256:ef4135732d30c6209b85cf47d6ce104df48f6c9139fde1f2f3eb5925704fa62a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16957254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f28c73e8f22c4d8b96ece80d2d6e3b65ae6246aa2ae4f356615714c2a7e79768`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:26:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Wed, 24 Feb 2021 23:34:19 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Mon, 29 Mar 2021 20:07:01 GMT
COPY file:021b5194c9f396ca24aaadd4ab3f8978febba7dff422827e0a613bb38224e5a2 in / 
# Mon, 29 Mar 2021 20:07:03 GMT
EXPOSE 80
# Mon, 29 Mar 2021 20:07:03 GMT
VOLUME [/tmp]
# Mon, 29 Mar 2021 20:07:04 GMT
ENTRYPOINT ["/traefik"]
# Mon, 29 Mar 2021 20:07:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:7e0c903ccfa53274059f2a4921657f10271ac6374b3f7f9094c4f026cc5a5b22`  
		Last Modified: Mon, 29 Mar 2021 20:07:50 GMT  
		Size: 16.5 MB (16517526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.29` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:58672e0711556e25704de4035eac1dd218ce82998a83986d912d4bff36aab0c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16538128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:526c897fe43b070574d98f9135897eaa2106fc575b3cec56dc9f9b213cfe72e2`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:27:56 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 25 Feb 2021 04:23:55 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Mon, 29 Mar 2021 19:52:36 GMT
COPY file:74c43ad3c5d71b75ac8726ad0ece7d7b6df15ddafbb3a2788809aba508d44be4 in / 
# Mon, 29 Mar 2021 19:52:37 GMT
EXPOSE 80
# Mon, 29 Mar 2021 19:52:38 GMT
VOLUME [/tmp]
# Mon, 29 Mar 2021 19:52:39 GMT
ENTRYPOINT ["/traefik"]
# Mon, 29 Mar 2021 19:52:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:de9c77266db7cadaf81c6da0e1965473c18b40e57e28336f2a8741e83f19d269`  
		Last Modified: Mon, 29 Mar 2021 19:53:22 GMT  
		Size: 16.1 MB (16098424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.29-alpine`

```console
$ docker pull traefik@sha256:5b2f8b55f214739049c50d852f607e5c6fd88db97a2c421b8bacd21c7d580197
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.29-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:8f3f2a0d4f3328c773a6e318f97f2737b8b01d878e1c6c28aae2c619bab6e715
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.2 MB (21187519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4b8d97846317066736c27e97b1037c0852ca8ffb67dc7194369a5629455a9a8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:19 GMT
ADD file:c744c1dc3da4145771e66d90e2e97a4f7fb702e5e07cf4e766ee0792cf161d92 in / 
# Wed, 31 Mar 2021 20:10:19 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:29:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 17:29:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.29/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 17:29:28 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 17:29:28 GMT
EXPOSE 80
# Thu, 01 Apr 2021 17:29:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 17:29:28 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 17:29:28 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9b794450f7b6db7c944ba1f4161edb68cb535052fe7db8ac06e613516c4a658d`  
		Last Modified: Wed, 31 Mar 2021 20:11:14 GMT  
		Size: 2.8 MB (2815346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c8802178dbdb14a188b12c88bfc76fb3c53283d93692a8f0e361bb1a3252d22`  
		Last Modified: Thu, 01 Apr 2021 17:29:57 GMT  
		Size: 674.2 KB (674206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6018d46b9ec53062f07d28e96d77f33343b177110d3d858548045fe10632aa54`  
		Last Modified: Thu, 01 Apr 2021 17:30:28 GMT  
		Size: 17.7 MB (17697599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b85e62c76fe27cb456ba2e73677bcc61a252d22da2283e8b116c49c13e6c17`  
		Last Modified: Thu, 01 Apr 2021 17:30:25 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.29-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f979f91b731033e20c3a939a8cf4421cef79843d72baf7f38ac1d05fdd2acc37
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.8 MB (19815995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d03cd3ce2303375e1d78220cb677c06b645760b71285ee468a5d297eedce7963`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:20 GMT
ADD file:15a1f9d3700deb648f0b3701afebc97ff28eb30d1b55e18dc9c696a9dd5c8e36 in / 
# Wed, 31 Mar 2021 17:19:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:52:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 03:53:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.29/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 03:53:06 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 03:53:07 GMT
EXPOSE 80
# Thu, 01 Apr 2021 03:53:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 03:53:09 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 03:53:10 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ac95243af174972febc49043f62f7b952a0c610e59b55ac4133f442e399e8729`  
		Last Modified: Wed, 31 Mar 2021 17:20:17 GMT  
		Size: 2.6 MB (2621248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25173f2bf7681888ff03bae0a793dcd2a8124175d360f999d21081483f90f181`  
		Last Modified: Thu, 01 Apr 2021 03:54:34 GMT  
		Size: 677.0 KB (677016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742427c956b4efd61ff21935a676a11fdd90f92afb76982a28be9f89e8adae33`  
		Last Modified: Thu, 01 Apr 2021 03:54:59 GMT  
		Size: 16.5 MB (16517363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b0d542a2b35d39348ec0f66b5b6f569020a95387fb7ee91fa9b627a363c171`  
		Last Modified: Thu, 01 Apr 2021 03:54:53 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.29-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:8f65a24b005efbe080078a819063b42dce92fa6e67e3ac4cc510ae2e02ad4004
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.5 MB (19500215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f91b2537ad19012ff83bee5b54a15a1d505afbb10d4170ffac365f414e362bc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:02 GMT
ADD file:174ba1b913c5cf549fcdfc259e8e3aa8f49cea660865fd54b8aacb430602a783 in / 
# Wed, 31 Mar 2021 17:22:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:15:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 16:15:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.29/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 16:15:40 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 16:15:42 GMT
EXPOSE 80
# Thu, 01 Apr 2021 16:15:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 16:15:44 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 16:15:45 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a3cf95b55367cb73f51318ee9c854def347373482336709ca1882a5d4c20b7c7`  
		Last Modified: Wed, 31 Mar 2021 17:23:00 GMT  
		Size: 2.7 MB (2725871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c5532ded8a461bb2539065ec0daf26ce2ecfed811ad86719ad11c964ab658`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 675.5 KB (675530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77a352edb1d69d5ba0f49daf5aeaeae71629ebbbded0ebf1e9fd64d0530136c`  
		Last Modified: Thu, 01 Apr 2021 16:18:23 GMT  
		Size: 16.1 MB (16098446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630d8f1d2a4cb7186cfdd5067d1f7497927474b2990138559aecc0df5c0f942a`  
		Last Modified: Thu, 01 Apr 2021 16:18:19 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.29-windowsservercore-1809`

```console
$ docker pull traefik@sha256:6eecb378641177fca09f19127265ab91271448ef60a5268ee68987276ccfe8c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `traefik:v1.7.29-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull traefik@sha256:cf4582a473eb76ed41b990dfa297cc4d3bbd7f591095247d8d8594c00fbb78d4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2488937386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0972d358793f50271670241e2fe9aec32fe3650e7d8910e0b096f62563a41e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 29 Mar 2021 20:16:24 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.29/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Mon, 29 Mar 2021 20:16:26 GMT
EXPOSE 80
# Mon, 29 Mar 2021 20:16:27 GMT
ENTRYPOINT ["/traefik"]
# Mon, 29 Mar 2021 20:16:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.29 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530c2cf8b93172ab27963511ee3d2f36f94cc25e63ec870d1d91d56e05dd9722`  
		Last Modified: Mon, 29 Mar 2021 20:17:16 GMT  
		Size: 27.4 MB (27397196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be393dbe8be8c7a56d7d6fe4c431c56dd54a387bb81f572283ee86e3015dcb51`  
		Last Modified: Mon, 29 Mar 2021 20:17:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4d019fc76e3913da39f4402716b57bfa0395c64227907a2eb2b81878148ff7`  
		Last Modified: Mon, 29 Mar 2021 20:17:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d834588bef160f62373a77ce715af11b673c3e1673def36b2dcc290eb522870a`  
		Last Modified: Mon, 29 Mar 2021 20:17:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.4`

```console
$ docker pull traefik@sha256:d7d63b0d442f9954fbcb09e6fcc1a9c6251873469ee19f8aeaa13f0c776b3de6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.4` - linux; amd64

```console
$ docker pull traefik@sha256:51f066bfd65b83782047df91948efb5dad5f7cba31a057b0aee90a741896e710
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27827436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31431ad170701ff91cf26d1b06d8b5848a671e5fd3bab56276adf01727bc9831`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:19 GMT
ADD file:c744c1dc3da4145771e66d90e2e97a4f7fb702e5e07cf4e766ee0792cf161d92 in / 
# Wed, 31 Mar 2021 20:10:19 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:29:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 17:29:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 17:29:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 17:29:20 GMT
EXPOSE 80
# Thu, 01 Apr 2021 17:29:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 17:29:21 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 17:29:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9b794450f7b6db7c944ba1f4161edb68cb535052fe7db8ac06e613516c4a658d`  
		Last Modified: Wed, 31 Mar 2021 20:11:14 GMT  
		Size: 2.8 MB (2815346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c8802178dbdb14a188b12c88bfc76fb3c53283d93692a8f0e361bb1a3252d22`  
		Last Modified: Thu, 01 Apr 2021 17:29:57 GMT  
		Size: 674.2 KB (674206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365a033b4de2d1b88bb65502713fd041850bb27f0aab73939280b4fc2bec7ecf`  
		Last Modified: Thu, 01 Apr 2021 17:30:02 GMT  
		Size: 24.3 MB (24337516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a316ffd61dd62a5a271a399314e5f36d68b7ddb77e6600bc19fa0912593a0645`  
		Last Modified: Thu, 01 Apr 2021 17:29:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:445ec88018c03307101e734adfd8425f4da87e9ffd5d83b1e5fb512d280df5df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26025735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a68d5d0d7cdf26c5ef8132873c04d3e8cc92b65cd6ad0af323361a5c222c57f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:20 GMT
ADD file:15a1f9d3700deb648f0b3701afebc97ff28eb30d1b55e18dc9c696a9dd5c8e36 in / 
# Wed, 31 Mar 2021 17:19:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:52:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 03:52:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 03:52:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 03:52:45 GMT
EXPOSE 80
# Thu, 01 Apr 2021 03:52:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 03:52:48 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 03:52:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ac95243af174972febc49043f62f7b952a0c610e59b55ac4133f442e399e8729`  
		Last Modified: Wed, 31 Mar 2021 17:20:17 GMT  
		Size: 2.6 MB (2621248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25173f2bf7681888ff03bae0a793dcd2a8124175d360f999d21081483f90f181`  
		Last Modified: Thu, 01 Apr 2021 03:54:34 GMT  
		Size: 677.0 KB (677016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9546526ac0315b3d34e7f88f707fb5355cffd936afb2e80198eff85c6524a05`  
		Last Modified: Thu, 01 Apr 2021 03:54:41 GMT  
		Size: 22.7 MB (22727103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddd0b0952f4a6439010368b09c4bee68dd82bad0c47ff2a4a3a0b8ce6a2c498`  
		Last Modified: Thu, 01 Apr 2021 03:54:33 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.4` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:edd78c8c05d3050cbd62e00de1575597f2a1c628fd5faefecb0d8b20c35d7ba9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25475489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19eb3704549293128f6d623b5a417a6cf34b01a797b4e0bf36dee8ef8f255e71`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:02 GMT
ADD file:174ba1b913c5cf549fcdfc259e8e3aa8f49cea660865fd54b8aacb430602a783 in / 
# Wed, 31 Mar 2021 17:22:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:15:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 16:15:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 16:15:22 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 16:15:23 GMT
EXPOSE 80
# Thu, 01 Apr 2021 16:15:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 16:15:24 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 16:15:25 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a3cf95b55367cb73f51318ee9c854def347373482336709ca1882a5d4c20b7c7`  
		Last Modified: Wed, 31 Mar 2021 17:23:00 GMT  
		Size: 2.7 MB (2725871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c5532ded8a461bb2539065ec0daf26ce2ecfed811ad86719ad11c964ab658`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 675.5 KB (675530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664cdd830c93e0170df8d4ed17b45f260ee577dcfb6db4d48f6e009b108ff81d`  
		Last Modified: Thu, 01 Apr 2021 16:18:03 GMT  
		Size: 22.1 MB (22073720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bdc2d37fb1c66af3a73e5fff4790dcfa4572a7fd25779591f80bd086c718df`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:37b2b7f435939b597589efb591686eca5a0e6ae850d1c80ec0cb3f996c05d24f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `traefik:v2.4-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull traefik@sha256:9345ce86759b6cc6053762a836111a43408fa15fc5571fba77ea93b43deefa00
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2495650153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f005e85992474d2eb3b06c7502a58d38c633edde288a548518128cd3e938f79c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 24 Mar 2021 01:16:17 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 24 Mar 2021 01:16:19 GMT
EXPOSE 80
# Wed, 24 Mar 2021 01:16:20 GMT
ENTRYPOINT ["/traefik"]
# Wed, 24 Mar 2021 01:16:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138871c226c89b2e75588935069c544f0c8ce5f68930fab95af0e4ca5a825d73`  
		Last Modified: Wed, 24 Mar 2021 01:17:09 GMT  
		Size: 34.1 MB (34109955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8574b4de7673b299ad666f81cd495bcfac5bf87fb33d4ef2781bdfcef30267`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb49e94abf40397ca09c966a1b4beb9579a20cb39ca8c9e17299ff206eb038e`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2d3f9210f45b7cb7f4c1ea77897d4576fcff778e51504d060afb3b28f4ae94`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.4.8`

```console
$ docker pull traefik@sha256:d7d63b0d442f9954fbcb09e6fcc1a9c6251873469ee19f8aeaa13f0c776b3de6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.4.8` - linux; amd64

```console
$ docker pull traefik@sha256:51f066bfd65b83782047df91948efb5dad5f7cba31a057b0aee90a741896e710
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27827436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31431ad170701ff91cf26d1b06d8b5848a671e5fd3bab56276adf01727bc9831`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:19 GMT
ADD file:c744c1dc3da4145771e66d90e2e97a4f7fb702e5e07cf4e766ee0792cf161d92 in / 
# Wed, 31 Mar 2021 20:10:19 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:29:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 17:29:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 17:29:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 17:29:20 GMT
EXPOSE 80
# Thu, 01 Apr 2021 17:29:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 17:29:21 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 17:29:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9b794450f7b6db7c944ba1f4161edb68cb535052fe7db8ac06e613516c4a658d`  
		Last Modified: Wed, 31 Mar 2021 20:11:14 GMT  
		Size: 2.8 MB (2815346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c8802178dbdb14a188b12c88bfc76fb3c53283d93692a8f0e361bb1a3252d22`  
		Last Modified: Thu, 01 Apr 2021 17:29:57 GMT  
		Size: 674.2 KB (674206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365a033b4de2d1b88bb65502713fd041850bb27f0aab73939280b4fc2bec7ecf`  
		Last Modified: Thu, 01 Apr 2021 17:30:02 GMT  
		Size: 24.3 MB (24337516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a316ffd61dd62a5a271a399314e5f36d68b7ddb77e6600bc19fa0912593a0645`  
		Last Modified: Thu, 01 Apr 2021 17:29:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.4.8` - linux; arm variant v6

```console
$ docker pull traefik@sha256:445ec88018c03307101e734adfd8425f4da87e9ffd5d83b1e5fb512d280df5df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26025735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a68d5d0d7cdf26c5ef8132873c04d3e8cc92b65cd6ad0af323361a5c222c57f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:20 GMT
ADD file:15a1f9d3700deb648f0b3701afebc97ff28eb30d1b55e18dc9c696a9dd5c8e36 in / 
# Wed, 31 Mar 2021 17:19:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:52:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 03:52:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 03:52:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 03:52:45 GMT
EXPOSE 80
# Thu, 01 Apr 2021 03:52:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 03:52:48 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 03:52:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ac95243af174972febc49043f62f7b952a0c610e59b55ac4133f442e399e8729`  
		Last Modified: Wed, 31 Mar 2021 17:20:17 GMT  
		Size: 2.6 MB (2621248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25173f2bf7681888ff03bae0a793dcd2a8124175d360f999d21081483f90f181`  
		Last Modified: Thu, 01 Apr 2021 03:54:34 GMT  
		Size: 677.0 KB (677016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9546526ac0315b3d34e7f88f707fb5355cffd936afb2e80198eff85c6524a05`  
		Last Modified: Thu, 01 Apr 2021 03:54:41 GMT  
		Size: 22.7 MB (22727103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddd0b0952f4a6439010368b09c4bee68dd82bad0c47ff2a4a3a0b8ce6a2c498`  
		Last Modified: Thu, 01 Apr 2021 03:54:33 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.4.8` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:edd78c8c05d3050cbd62e00de1575597f2a1c628fd5faefecb0d8b20c35d7ba9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25475489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19eb3704549293128f6d623b5a417a6cf34b01a797b4e0bf36dee8ef8f255e71`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:02 GMT
ADD file:174ba1b913c5cf549fcdfc259e8e3aa8f49cea660865fd54b8aacb430602a783 in / 
# Wed, 31 Mar 2021 17:22:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:15:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 16:15:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 16:15:22 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 16:15:23 GMT
EXPOSE 80
# Thu, 01 Apr 2021 16:15:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 16:15:24 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 16:15:25 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a3cf95b55367cb73f51318ee9c854def347373482336709ca1882a5d4c20b7c7`  
		Last Modified: Wed, 31 Mar 2021 17:23:00 GMT  
		Size: 2.7 MB (2725871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c5532ded8a461bb2539065ec0daf26ce2ecfed811ad86719ad11c964ab658`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 675.5 KB (675530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664cdd830c93e0170df8d4ed17b45f260ee577dcfb6db4d48f6e009b108ff81d`  
		Last Modified: Thu, 01 Apr 2021 16:18:03 GMT  
		Size: 22.1 MB (22073720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bdc2d37fb1c66af3a73e5fff4790dcfa4572a7fd25779591f80bd086c718df`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.4.8-windowsservercore-1809`

```console
$ docker pull traefik@sha256:37b2b7f435939b597589efb591686eca5a0e6ae850d1c80ec0cb3f996c05d24f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `traefik:v2.4.8-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull traefik@sha256:9345ce86759b6cc6053762a836111a43408fa15fc5571fba77ea93b43deefa00
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2495650153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f005e85992474d2eb3b06c7502a58d38c633edde288a548518128cd3e938f79c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 24 Mar 2021 01:16:17 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 24 Mar 2021 01:16:19 GMT
EXPOSE 80
# Wed, 24 Mar 2021 01:16:20 GMT
ENTRYPOINT ["/traefik"]
# Wed, 24 Mar 2021 01:16:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138871c226c89b2e75588935069c544f0c8ce5f68930fab95af0e4ca5a825d73`  
		Last Modified: Wed, 24 Mar 2021 01:17:09 GMT  
		Size: 34.1 MB (34109955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8574b4de7673b299ad666f81cd495bcfac5bf87fb33d4ef2781bdfcef30267`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb49e94abf40397ca09c966a1b4beb9579a20cb39ca8c9e17299ff206eb038e`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2d3f9210f45b7cb7f4c1ea77897d4576fcff778e51504d060afb3b28f4ae94`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:37b2b7f435939b597589efb591686eca5a0e6ae850d1c80ec0cb3f996c05d24f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull traefik@sha256:9345ce86759b6cc6053762a836111a43408fa15fc5571fba77ea93b43deefa00
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2495650153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f005e85992474d2eb3b06c7502a58d38c633edde288a548518128cd3e938f79c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 24 Mar 2021 01:16:17 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 24 Mar 2021 01:16:19 GMT
EXPOSE 80
# Wed, 24 Mar 2021 01:16:20 GMT
ENTRYPOINT ["/traefik"]
# Wed, 24 Mar 2021 01:16:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138871c226c89b2e75588935069c544f0c8ce5f68930fab95af0e4ca5a825d73`  
		Last Modified: Wed, 24 Mar 2021 01:17:09 GMT  
		Size: 34.1 MB (34109955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8574b4de7673b299ad666f81cd495bcfac5bf87fb33d4ef2781bdfcef30267`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb49e94abf40397ca09c966a1b4beb9579a20cb39ca8c9e17299ff206eb038e`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2d3f9210f45b7cb7f4c1ea77897d4576fcff778e51504d060afb3b28f4ae94`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
