<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:1.7`](#traefik17)
-	[`traefik:1.7.25`](#traefik1725)
-	[`traefik:1.7.25-alpine`](#traefik1725-alpine)
-	[`traefik:1.7.25-windowsservercore-1809`](#traefik1725-windowsservercore-1809)
-	[`traefik:1.7-alpine`](#traefik17-alpine)
-	[`traefik:1.7-windowsservercore-1809`](#traefik17-windowsservercore-1809)
-	[`traefik:2.2`](#traefik22)
-	[`traefik:2.2.7`](#traefik227)
-	[`traefik:2.2.7-windowsservercore-1809`](#traefik227-windowsservercore-1809)
-	[`traefik:2.2-windowsservercore-1809`](#traefik22-windowsservercore-1809)
-	[`traefik:2.3`](#traefik23)
-	[`traefik:2.3.0-rc2`](#traefik230-rc2)
-	[`traefik:2.3.0-rc2-windowsservercore-1809`](#traefik230-rc2-windowsservercore-1809)
-	[`traefik:2.3-windowsservercore-1809`](#traefik23-windowsservercore-1809)
-	[`traefik:chevrotin`](#traefikchevrotin)
-	[`traefik:chevrotin-windowsservercore-1809`](#traefikchevrotin-windowsservercore-1809)
-	[`traefik:latest`](#traefiklatest)
-	[`traefik:maroilles`](#traefikmaroilles)
-	[`traefik:maroilles-alpine`](#traefikmaroilles-alpine)
-	[`traefik:maroilles-windowsservercore-1809`](#traefikmaroilles-windowsservercore-1809)
-	[`traefik:picodon`](#traefikpicodon)
-	[`traefik:picodon-windowsservercore-1809`](#traefikpicodon-windowsservercore-1809)
-	[`traefik:v1.7`](#traefikv17)
-	[`traefik:v1.7.25`](#traefikv1725)
-	[`traefik:v1.7.25-alpine`](#traefikv1725-alpine)
-	[`traefik:v1.7.25-windowsservercore-1809`](#traefikv1725-windowsservercore-1809)
-	[`traefik:v1.7-alpine`](#traefikv17-alpine)
-	[`traefik:v1.7-windowsservercore-1809`](#traefikv17-windowsservercore-1809)
-	[`traefik:v2.2`](#traefikv22)
-	[`traefik:v2.2.7`](#traefikv227)
-	[`traefik:v2.2.7-windowsservercore-1809`](#traefikv227-windowsservercore-1809)
-	[`traefik:v2.2-windowsservercore-1809`](#traefikv22-windowsservercore-1809)
-	[`traefik:v2.3`](#traefikv23)
-	[`traefik:v2.3.0-rc2`](#traefikv230-rc2)
-	[`traefik:v2.3.0-rc2-windowsservercore-1809`](#traefikv230-rc2-windowsservercore-1809)
-	[`traefik:v2.3-windowsservercore-1809`](#traefikv23-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:1.7`

```console
$ docker pull traefik@sha256:1fa3e9ee4509211196b926eb90d07ffbdf72d730ff3d8c428ac94f3b1c784783
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7` - linux; amd64

```console
$ docker pull traefik@sha256:6eac900151c64c8465ef0e38b27d4ae9d877616230162279727337b47ff5dc08
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21584351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca551e784d546c33bab389a7b90aca0c74fa026194a34cbd4a6805a32fde606f`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 02:50:22 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 02:50:24 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 15 Jul 2020 23:54:07 GMT
COPY file:dbebc61aa00cc3bd336b1fe611a0e32e7ad8b4b311e43c336de691d7c04a47af in / 
# Wed, 15 Jul 2020 23:54:08 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:54:08 GMT
VOLUME [/tmp]
# Wed, 15 Jul 2020 23:54:08 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jul 2020 23:54:08 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e40d0b92fe2d2ef50c6f43f32c33dc117ab26d69a29d74ae15725a379dbde0c2`  
		Last Modified: Fri, 21 Feb 2020 02:51:04 GMT  
		Size: 131.7 KB (131682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c068c5049677b6879089396aa0d2d162ac9697e25bacf333c0596a248bae8a5`  
		Last Modified: Fri, 21 Feb 2020 02:51:04 GMT  
		Size: 327.4 KB (327376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2668a1328cae473e5092f00bde31aa8d95bd00773bd3dbb5bf938539066ec41e`  
		Last Modified: Wed, 15 Jul 2020 23:54:48 GMT  
		Size: 21.1 MB (21125293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:201b3f9b283f6bc734fe33ab3c1c7c428d5878ccf4836be1892f1aea6bd63a9d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20231475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47cc1d1e27878e29edf1fc95fa792416065312621456b2f166e71de4782cae1e`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 03:46:16 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 03:46:17 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 15 Jul 2020 23:07:11 GMT
COPY file:185bd7cda9d632ce86c62da94a8061efac1291f616a72972fcda00ba82e29c4d in / 
# Wed, 15 Jul 2020 23:07:12 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:07:14 GMT
VOLUME [/tmp]
# Wed, 15 Jul 2020 23:07:15 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jul 2020 23:07:16 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:3ea78b0360c0223e83ecbb7336ab0de873d099e2aa889216bc3622c7dc315adc`  
		Last Modified: Tue, 24 Mar 2020 03:47:54 GMT  
		Size: 131.7 KB (131681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd374e140760994a9274b43e4cbf314b61a77acb227eca705d35780bb33a6a07`  
		Last Modified: Tue, 24 Mar 2020 03:47:55 GMT  
		Size: 327.4 KB (327405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5eb8f091d88a8df352ff16fe91d7b9d4a458c1fbb7e28ce7a282293681e2c91`  
		Last Modified: Wed, 15 Jul 2020 23:08:16 GMT  
		Size: 19.8 MB (19772389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:c98ea0955bb58f169837a6a29663ccec288bc496290aa06d19a63b1922ea44fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.0 MB (19952902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c7f0e9591004fb0d9f0ec32c8b5e3294790b993e054cb774f1b08055583fcde`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 05:55:25 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 05:55:26 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 15 Jul 2020 23:30:24 GMT
COPY file:2004fb63ffb43df9c881281b0e9250dcd15332dde58681121ec9738221528602 in / 
# Wed, 15 Jul 2020 23:30:25 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:30:26 GMT
VOLUME [/tmp]
# Wed, 15 Jul 2020 23:30:27 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jul 2020 23:30:28 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:58ceb9a2a8ba9dd83eef0c2cf887c175911b301df486d142f7d09293605add22`  
		Last Modified: Tue, 24 Mar 2020 05:56:42 GMT  
		Size: 131.7 KB (131676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b9edf48787b0368bb1af04734041d3b374acefa70417bdf0090919056c874d`  
		Last Modified: Tue, 24 Mar 2020 05:56:42 GMT  
		Size: 327.4 KB (327402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100a118a37516ea44966052eb5d2b1de534be63dd7da7443bf69a60c4cf3731d`  
		Last Modified: Wed, 15 Jul 2020 23:31:38 GMT  
		Size: 19.5 MB (19493824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.25`

```console
$ docker pull traefik@sha256:1fa3e9ee4509211196b926eb90d07ffbdf72d730ff3d8c428ac94f3b1c784783
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.25` - linux; amd64

```console
$ docker pull traefik@sha256:6eac900151c64c8465ef0e38b27d4ae9d877616230162279727337b47ff5dc08
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21584351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca551e784d546c33bab389a7b90aca0c74fa026194a34cbd4a6805a32fde606f`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 02:50:22 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 02:50:24 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 15 Jul 2020 23:54:07 GMT
COPY file:dbebc61aa00cc3bd336b1fe611a0e32e7ad8b4b311e43c336de691d7c04a47af in / 
# Wed, 15 Jul 2020 23:54:08 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:54:08 GMT
VOLUME [/tmp]
# Wed, 15 Jul 2020 23:54:08 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jul 2020 23:54:08 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e40d0b92fe2d2ef50c6f43f32c33dc117ab26d69a29d74ae15725a379dbde0c2`  
		Last Modified: Fri, 21 Feb 2020 02:51:04 GMT  
		Size: 131.7 KB (131682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c068c5049677b6879089396aa0d2d162ac9697e25bacf333c0596a248bae8a5`  
		Last Modified: Fri, 21 Feb 2020 02:51:04 GMT  
		Size: 327.4 KB (327376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2668a1328cae473e5092f00bde31aa8d95bd00773bd3dbb5bf938539066ec41e`  
		Last Modified: Wed, 15 Jul 2020 23:54:48 GMT  
		Size: 21.1 MB (21125293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.25` - linux; arm variant v6

```console
$ docker pull traefik@sha256:201b3f9b283f6bc734fe33ab3c1c7c428d5878ccf4836be1892f1aea6bd63a9d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20231475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47cc1d1e27878e29edf1fc95fa792416065312621456b2f166e71de4782cae1e`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 03:46:16 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 03:46:17 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 15 Jul 2020 23:07:11 GMT
COPY file:185bd7cda9d632ce86c62da94a8061efac1291f616a72972fcda00ba82e29c4d in / 
# Wed, 15 Jul 2020 23:07:12 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:07:14 GMT
VOLUME [/tmp]
# Wed, 15 Jul 2020 23:07:15 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jul 2020 23:07:16 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:3ea78b0360c0223e83ecbb7336ab0de873d099e2aa889216bc3622c7dc315adc`  
		Last Modified: Tue, 24 Mar 2020 03:47:54 GMT  
		Size: 131.7 KB (131681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd374e140760994a9274b43e4cbf314b61a77acb227eca705d35780bb33a6a07`  
		Last Modified: Tue, 24 Mar 2020 03:47:55 GMT  
		Size: 327.4 KB (327405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5eb8f091d88a8df352ff16fe91d7b9d4a458c1fbb7e28ce7a282293681e2c91`  
		Last Modified: Wed, 15 Jul 2020 23:08:16 GMT  
		Size: 19.8 MB (19772389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.25` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:c98ea0955bb58f169837a6a29663ccec288bc496290aa06d19a63b1922ea44fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.0 MB (19952902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c7f0e9591004fb0d9f0ec32c8b5e3294790b993e054cb774f1b08055583fcde`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 05:55:25 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 05:55:26 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 15 Jul 2020 23:30:24 GMT
COPY file:2004fb63ffb43df9c881281b0e9250dcd15332dde58681121ec9738221528602 in / 
# Wed, 15 Jul 2020 23:30:25 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:30:26 GMT
VOLUME [/tmp]
# Wed, 15 Jul 2020 23:30:27 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jul 2020 23:30:28 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:58ceb9a2a8ba9dd83eef0c2cf887c175911b301df486d142f7d09293605add22`  
		Last Modified: Tue, 24 Mar 2020 05:56:42 GMT  
		Size: 131.7 KB (131676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b9edf48787b0368bb1af04734041d3b374acefa70417bdf0090919056c874d`  
		Last Modified: Tue, 24 Mar 2020 05:56:42 GMT  
		Size: 327.4 KB (327402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100a118a37516ea44966052eb5d2b1de534be63dd7da7443bf69a60c4cf3731d`  
		Last Modified: Wed, 15 Jul 2020 23:31:38 GMT  
		Size: 19.5 MB (19493824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.25-alpine`

```console
$ docker pull traefik@sha256:d4325a60a66c34c4491b7662a71e2b0f5c45cefcb036af8e762f7ccc685b1874
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.25-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:56b5ec0207c9d9bca95b2c25262ff968c1edf4469984000c7550bcf23952827e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24633397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b15dfa7af58e7044de080d1e00c691112ad97424a0d63f7dd81e59ce0ea20beb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:53:41 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.25/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:53:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:53:42 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:53:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:53:42 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:53:42 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16506d32a25436b458a7f443ec1ca0d096d99d3479523c92c247856fc6148c0`  
		Last Modified: Fri, 24 Apr 2020 17:34:15 GMT  
		Size: 694.1 KB (694148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e283b232b00d6def332f0854c0624efc59074fd6f99cf171abe83af71d716739`  
		Last Modified: Wed, 15 Jul 2020 23:54:38 GMT  
		Size: 21.1 MB (21125565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21796958177fa80eb809b5a57c9f547af553cfdc9a0568b4794bac6610af934`  
		Last Modified: Wed, 15 Jul 2020 23:54:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.25-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:b21c79858f578e27cb04a8723686008dc91197fd7cdeb94614935e171871ef7b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23090947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b97db544f1052e42a534853e75d36cb7b6996ec4223752e4187ac4d0bbe5417c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:04:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.25/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:04:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:04:53 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:04:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:04:55 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:04:56 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a36cf46e6cb6a8028db7cb68482816e710935254a7d463897840713066cf5ba`  
		Last Modified: Thu, 23 Apr 2020 22:39:24 GMT  
		Size: 698.1 KB (698086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bfedcce63424119565c9a127a7f8bd82e99ea024f93f2c7427942f3451e3001`  
		Last Modified: Wed, 15 Jul 2020 23:08:01 GMT  
		Size: 19.8 MB (19772557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b24e2aadaecd85cde7ef979c7a6981ae83a7050116df5fcb073bfec4833cc74`  
		Last Modified: Wed, 15 Jul 2020 23:07:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.25-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3798e6eea86039b46b4bf760f5cc4bc6be672ea0b89c9e0be397eddfb16000f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22914773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3940f96616b8f8d03d96c2796404288a054b54b87b587c9f0bc7c90d1ae2d5da`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:24:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.25/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:24:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:24:10 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:24:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:24:12 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:24:13 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff968af61b86e34dc2412293ade430f77b7db53f7f4adb925fec30d3ccbb2876`  
		Last Modified: Fri, 24 Apr 2020 12:43:42 GMT  
		Size: 696.1 KB (696058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380ca995bf3761e50cdb46b03208ac913ea1328566e2eac8ad835867ff78a077`  
		Last Modified: Wed, 15 Jul 2020 23:31:22 GMT  
		Size: 19.5 MB (19493924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d88c62829ac867327a678720b6bcc03c9b9413d196cd15ef2983d4946b9ebb`  
		Last Modified: Wed, 15 Jul 2020 23:31:15 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.25-windowsservercore-1809`

```console
$ docker pull traefik@sha256:7a2e772e8537a92ad67813de222d6fc35d46db70f8c3342c22ca0bcb9f2224a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `traefik:1.7.25-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull traefik@sha256:2447f4bcd451245ad9e3200626d0ad9bc6842f4f6288743c1b1ad4154698b46a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2340473541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d6ce3a7269e05fd8df0e5f6c1f272c24bf8903d1b499bc84306431e5c0ab3a5`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 23:17:53 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.25/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 15 Jul 2020 23:17:54 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:17:56 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jul 2020 23:17:58 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56765e2183d70fbee243e23e45b4dae04f3611ac7bb45d0f237f7141337bb6b1`  
		Last Modified: Wed, 15 Jul 2020 23:19:02 GMT  
		Size: 30.3 MB (30276616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a9aeca829593fbf97e6ddfba27b1f71b9cfdbdc814b9a0c353b82039542a53`  
		Last Modified: Wed, 15 Jul 2020 23:18:57 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13f8ba7125cb8bd4176a652b98db75af122b71acd3aa8f00de1120b8234d009`  
		Last Modified: Wed, 15 Jul 2020 23:18:55 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffbf5581287fcb7681d76485a5bf4e5f1ded4fe51c7e8f2c91d1f5b98df456a`  
		Last Modified: Wed, 15 Jul 2020 23:18:54 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-alpine`

```console
$ docker pull traefik@sha256:d4325a60a66c34c4491b7662a71e2b0f5c45cefcb036af8e762f7ccc685b1874
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:56b5ec0207c9d9bca95b2c25262ff968c1edf4469984000c7550bcf23952827e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24633397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b15dfa7af58e7044de080d1e00c691112ad97424a0d63f7dd81e59ce0ea20beb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:53:41 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.25/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:53:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:53:42 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:53:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:53:42 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:53:42 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16506d32a25436b458a7f443ec1ca0d096d99d3479523c92c247856fc6148c0`  
		Last Modified: Fri, 24 Apr 2020 17:34:15 GMT  
		Size: 694.1 KB (694148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e283b232b00d6def332f0854c0624efc59074fd6f99cf171abe83af71d716739`  
		Last Modified: Wed, 15 Jul 2020 23:54:38 GMT  
		Size: 21.1 MB (21125565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21796958177fa80eb809b5a57c9f547af553cfdc9a0568b4794bac6610af934`  
		Last Modified: Wed, 15 Jul 2020 23:54:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:b21c79858f578e27cb04a8723686008dc91197fd7cdeb94614935e171871ef7b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23090947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b97db544f1052e42a534853e75d36cb7b6996ec4223752e4187ac4d0bbe5417c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:04:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.25/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:04:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:04:53 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:04:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:04:55 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:04:56 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a36cf46e6cb6a8028db7cb68482816e710935254a7d463897840713066cf5ba`  
		Last Modified: Thu, 23 Apr 2020 22:39:24 GMT  
		Size: 698.1 KB (698086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bfedcce63424119565c9a127a7f8bd82e99ea024f93f2c7427942f3451e3001`  
		Last Modified: Wed, 15 Jul 2020 23:08:01 GMT  
		Size: 19.8 MB (19772557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b24e2aadaecd85cde7ef979c7a6981ae83a7050116df5fcb073bfec4833cc74`  
		Last Modified: Wed, 15 Jul 2020 23:07:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3798e6eea86039b46b4bf760f5cc4bc6be672ea0b89c9e0be397eddfb16000f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22914773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3940f96616b8f8d03d96c2796404288a054b54b87b587c9f0bc7c90d1ae2d5da`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:24:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.25/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:24:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:24:10 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:24:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:24:12 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:24:13 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff968af61b86e34dc2412293ade430f77b7db53f7f4adb925fec30d3ccbb2876`  
		Last Modified: Fri, 24 Apr 2020 12:43:42 GMT  
		Size: 696.1 KB (696058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380ca995bf3761e50cdb46b03208ac913ea1328566e2eac8ad835867ff78a077`  
		Last Modified: Wed, 15 Jul 2020 23:31:22 GMT  
		Size: 19.5 MB (19493924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d88c62829ac867327a678720b6bcc03c9b9413d196cd15ef2983d4946b9ebb`  
		Last Modified: Wed, 15 Jul 2020 23:31:15 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:7a2e772e8537a92ad67813de222d6fc35d46db70f8c3342c22ca0bcb9f2224a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `traefik:1.7-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull traefik@sha256:2447f4bcd451245ad9e3200626d0ad9bc6842f4f6288743c1b1ad4154698b46a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2340473541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d6ce3a7269e05fd8df0e5f6c1f272c24bf8903d1b499bc84306431e5c0ab3a5`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 23:17:53 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.25/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 15 Jul 2020 23:17:54 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:17:56 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jul 2020 23:17:58 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56765e2183d70fbee243e23e45b4dae04f3611ac7bb45d0f237f7141337bb6b1`  
		Last Modified: Wed, 15 Jul 2020 23:19:02 GMT  
		Size: 30.3 MB (30276616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a9aeca829593fbf97e6ddfba27b1f71b9cfdbdc814b9a0c353b82039542a53`  
		Last Modified: Wed, 15 Jul 2020 23:18:57 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13f8ba7125cb8bd4176a652b98db75af122b71acd3aa8f00de1120b8234d009`  
		Last Modified: Wed, 15 Jul 2020 23:18:55 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffbf5581287fcb7681d76485a5bf4e5f1ded4fe51c7e8f2c91d1f5b98df456a`  
		Last Modified: Wed, 15 Jul 2020 23:18:54 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.2`

```console
$ docker pull traefik@sha256:2dcdde75212d0117ef1360df5c532a2ec8bb97c386987b2bc66d973bca5003b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.2` - linux; amd64

```console
$ docker pull traefik@sha256:55f1b5e719c6e0f2d650e921463a87c8a4024236afb4991aea632df7ef942663
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25167013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de086c281ea7b4116c64a917309e249ae9063c663cd8e41c234bc54b88cfcd2c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Jul 2020 19:22:47 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.7/traefik_v2.2.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Jul 2020 19:22:47 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Jul 2020 19:22:47 GMT
EXPOSE 80
# Mon, 20 Jul 2020 19:22:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Jul 2020 19:22:48 GMT
CMD ["traefik"]
# Mon, 20 Jul 2020 19:22:48 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16506d32a25436b458a7f443ec1ca0d096d99d3479523c92c247856fc6148c0`  
		Last Modified: Fri, 24 Apr 2020 17:34:15 GMT  
		Size: 694.1 KB (694148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd583f1fc97ea2229f7e54f3b224e77b1b35f9e130dead096b58331b74427999`  
		Last Modified: Mon, 20 Jul 2020 19:23:12 GMT  
		Size: 21.7 MB (21659180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb2b75fe8e63b50ed1bb2728995b03b38ae981345ce246cececaf4384f5a9a1`  
		Last Modified: Mon, 20 Jul 2020 19:23:07 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.2` - linux; arm variant v6

```console
$ docker pull traefik@sha256:1dd33a92c9604ced7cfc03c9ad6653aa5d00a26a5e0a825f89ada10b052fb236
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.7 MB (23663447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41954059dfb2a60ecee9e006f90e5e8e9ec6d2174e65608e2518f801dc5df657`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Jul 2020 18:50:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.7/traefik_v2.2.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Jul 2020 18:50:32 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Jul 2020 18:50:32 GMT
EXPOSE 80
# Mon, 20 Jul 2020 18:50:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Jul 2020 18:50:34 GMT
CMD ["traefik"]
# Mon, 20 Jul 2020 18:50:35 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a36cf46e6cb6a8028db7cb68482816e710935254a7d463897840713066cf5ba`  
		Last Modified: Thu, 23 Apr 2020 22:39:24 GMT  
		Size: 698.1 KB (698086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ee7c01f51a7c41cc870b283b66ccd0dee4dfc7e0e9c1ca957d73969dc26691`  
		Last Modified: Mon, 20 Jul 2020 18:51:19 GMT  
		Size: 20.3 MB (20345057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ca186cb1c339d1fd77800b7788583c0d6b0309bda439b921d497a6f2030dc`  
		Last Modified: Mon, 20 Jul 2020 18:51:11 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.2` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:ae6a9e07e0c03df672e5fe90ade2f5a56ea27f1f0e30e2a13bb49d8cbdc3e7c9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23423015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f69c73e81ebad70c08ca34291273b3a3b4bb3b4b5f9a5acbd9fc3433c157e19`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Jul 2020 19:47:40 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.7/traefik_v2.2.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Jul 2020 19:47:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Jul 2020 19:47:42 GMT
EXPOSE 80
# Mon, 20 Jul 2020 19:47:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Jul 2020 19:47:46 GMT
CMD ["traefik"]
# Mon, 20 Jul 2020 19:47:46 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff968af61b86e34dc2412293ade430f77b7db53f7f4adb925fec30d3ccbb2876`  
		Last Modified: Fri, 24 Apr 2020 12:43:42 GMT  
		Size: 696.1 KB (696058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2ba74a0f32fa0e26ecf336f6d70bc0d0a8a08a20062643dd9ac00bed14efa6`  
		Last Modified: Mon, 20 Jul 2020 19:48:27 GMT  
		Size: 20.0 MB (20002164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569fe01719a75603ca3d8c344ac5ec7d52199626d3240e48bf9e947a18b21810`  
		Last Modified: Mon, 20 Jul 2020 19:48:16 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.2.7`

```console
$ docker pull traefik@sha256:2dcdde75212d0117ef1360df5c532a2ec8bb97c386987b2bc66d973bca5003b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.2.7` - linux; amd64

```console
$ docker pull traefik@sha256:55f1b5e719c6e0f2d650e921463a87c8a4024236afb4991aea632df7ef942663
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25167013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de086c281ea7b4116c64a917309e249ae9063c663cd8e41c234bc54b88cfcd2c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Jul 2020 19:22:47 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.7/traefik_v2.2.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Jul 2020 19:22:47 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Jul 2020 19:22:47 GMT
EXPOSE 80
# Mon, 20 Jul 2020 19:22:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Jul 2020 19:22:48 GMT
CMD ["traefik"]
# Mon, 20 Jul 2020 19:22:48 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16506d32a25436b458a7f443ec1ca0d096d99d3479523c92c247856fc6148c0`  
		Last Modified: Fri, 24 Apr 2020 17:34:15 GMT  
		Size: 694.1 KB (694148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd583f1fc97ea2229f7e54f3b224e77b1b35f9e130dead096b58331b74427999`  
		Last Modified: Mon, 20 Jul 2020 19:23:12 GMT  
		Size: 21.7 MB (21659180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb2b75fe8e63b50ed1bb2728995b03b38ae981345ce246cececaf4384f5a9a1`  
		Last Modified: Mon, 20 Jul 2020 19:23:07 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.2.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:1dd33a92c9604ced7cfc03c9ad6653aa5d00a26a5e0a825f89ada10b052fb236
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.7 MB (23663447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41954059dfb2a60ecee9e006f90e5e8e9ec6d2174e65608e2518f801dc5df657`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Jul 2020 18:50:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.7/traefik_v2.2.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Jul 2020 18:50:32 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Jul 2020 18:50:32 GMT
EXPOSE 80
# Mon, 20 Jul 2020 18:50:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Jul 2020 18:50:34 GMT
CMD ["traefik"]
# Mon, 20 Jul 2020 18:50:35 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a36cf46e6cb6a8028db7cb68482816e710935254a7d463897840713066cf5ba`  
		Last Modified: Thu, 23 Apr 2020 22:39:24 GMT  
		Size: 698.1 KB (698086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ee7c01f51a7c41cc870b283b66ccd0dee4dfc7e0e9c1ca957d73969dc26691`  
		Last Modified: Mon, 20 Jul 2020 18:51:19 GMT  
		Size: 20.3 MB (20345057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ca186cb1c339d1fd77800b7788583c0d6b0309bda439b921d497a6f2030dc`  
		Last Modified: Mon, 20 Jul 2020 18:51:11 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.2.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:ae6a9e07e0c03df672e5fe90ade2f5a56ea27f1f0e30e2a13bb49d8cbdc3e7c9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23423015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f69c73e81ebad70c08ca34291273b3a3b4bb3b4b5f9a5acbd9fc3433c157e19`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Jul 2020 19:47:40 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.7/traefik_v2.2.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Jul 2020 19:47:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Jul 2020 19:47:42 GMT
EXPOSE 80
# Mon, 20 Jul 2020 19:47:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Jul 2020 19:47:46 GMT
CMD ["traefik"]
# Mon, 20 Jul 2020 19:47:46 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff968af61b86e34dc2412293ade430f77b7db53f7f4adb925fec30d3ccbb2876`  
		Last Modified: Fri, 24 Apr 2020 12:43:42 GMT  
		Size: 696.1 KB (696058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2ba74a0f32fa0e26ecf336f6d70bc0d0a8a08a20062643dd9ac00bed14efa6`  
		Last Modified: Mon, 20 Jul 2020 19:48:27 GMT  
		Size: 20.0 MB (20002164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569fe01719a75603ca3d8c344ac5ec7d52199626d3240e48bf9e947a18b21810`  
		Last Modified: Mon, 20 Jul 2020 19:48:16 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.2.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:fda8b53c30a901acfa91388660d2d85dfb77bcd49f7a3fe66d6d3c27c6710ac2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `traefik:2.2.7-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull traefik@sha256:f3c6b74c8cee89d7dd612c1f545a67746f57cbddabe650718c0d3e91af5fbc5f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2340995387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6abec4b0661abb8b7e71d04e842c7bc38a5e9afad4991089c95c19107c611a1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 20 Jul 2020 19:15:37 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.2.7/traefik_v2.2.7_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 20 Jul 2020 19:15:39 GMT
EXPOSE 80
# Mon, 20 Jul 2020 19:15:40 GMT
ENTRYPOINT ["/traefik"]
# Mon, 20 Jul 2020 19:15:42 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0247512bb5646fd88951141a0338afcbabb2130655250cc3959d27438ef1fb`  
		Last Modified: Mon, 20 Jul 2020 19:16:17 GMT  
		Size: 30.8 MB (30798531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e1f70926eb835a5f2a15b7eb3a699976603074073a3ec7e8e693221740f56f`  
		Last Modified: Mon, 20 Jul 2020 19:16:10 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1821ea1f642148d720fd6f4cfe40d3383d8b12c6c85e8e3cddd726f8cfc8b2b1`  
		Last Modified: Mon, 20 Jul 2020 19:16:09 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a2388b729f036c4dbf707e9e9a283d3a27987b149789c94b0307c5502febd1`  
		Last Modified: Mon, 20 Jul 2020 19:16:09 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:fda8b53c30a901acfa91388660d2d85dfb77bcd49f7a3fe66d6d3c27c6710ac2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `traefik:2.2-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull traefik@sha256:f3c6b74c8cee89d7dd612c1f545a67746f57cbddabe650718c0d3e91af5fbc5f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2340995387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6abec4b0661abb8b7e71d04e842c7bc38a5e9afad4991089c95c19107c611a1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 20 Jul 2020 19:15:37 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.2.7/traefik_v2.2.7_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 20 Jul 2020 19:15:39 GMT
EXPOSE 80
# Mon, 20 Jul 2020 19:15:40 GMT
ENTRYPOINT ["/traefik"]
# Mon, 20 Jul 2020 19:15:42 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0247512bb5646fd88951141a0338afcbabb2130655250cc3959d27438ef1fb`  
		Last Modified: Mon, 20 Jul 2020 19:16:17 GMT  
		Size: 30.8 MB (30798531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e1f70926eb835a5f2a15b7eb3a699976603074073a3ec7e8e693221740f56f`  
		Last Modified: Mon, 20 Jul 2020 19:16:10 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1821ea1f642148d720fd6f4cfe40d3383d8b12c6c85e8e3cddd726f8cfc8b2b1`  
		Last Modified: Mon, 20 Jul 2020 19:16:09 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a2388b729f036c4dbf707e9e9a283d3a27987b149789c94b0307c5502febd1`  
		Last Modified: Mon, 20 Jul 2020 19:16:09 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.3`

```console
$ docker pull traefik@sha256:b08601a937c1a160717e4ed6e0f4bc9ad0dea023de1ab309868cdf78164f9a33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.3` - linux; amd64

```console
$ docker pull traefik@sha256:b50cb55e6800df703f31b9a312d018558fc2286f829510f7da3de44a40aa74b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.9 MB (29942216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50a95f228e71630ffab61595fc050ce34c6013d6b9367440faef4e4f59d0e102`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:53:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc2/traefik_v2.3.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:53:34 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:53:34 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:53:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:53:35 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:53:35 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16506d32a25436b458a7f443ec1ca0d096d99d3479523c92c247856fc6148c0`  
		Last Modified: Fri, 24 Apr 2020 17:34:15 GMT  
		Size: 694.1 KB (694148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8f355ffe1c3315a63e73b1cb926b7f380eaa3ab4e9780add467a08709ef778`  
		Last Modified: Wed, 15 Jul 2020 23:54:29 GMT  
		Size: 26.4 MB (26434385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bdc521c6883d93f2893812825a3c6df9ac3959d1bf6c3ab800fcd311d8429a7`  
		Last Modified: Wed, 15 Jul 2020 23:54:24 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.3` - linux; arm variant v6

```console
$ docker pull traefik@sha256:09f2d34f7a32514f088d18ed0234527aeacd157d88187e115eed94c92db13e35
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.2 MB (28167652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab91012db5f2689da6b31247abefc6ca69082c5647a7f08b8439120169e69d9a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:04:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc2/traefik_v2.3.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:04:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:04:34 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:04:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:04:36 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:04:37 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a36cf46e6cb6a8028db7cb68482816e710935254a7d463897840713066cf5ba`  
		Last Modified: Thu, 23 Apr 2020 22:39:24 GMT  
		Size: 698.1 KB (698086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57bd030c3232794b6b0a553c8a0d9718f4c28235b71183f4ea6504924bd1782`  
		Last Modified: Wed, 15 Jul 2020 23:07:46 GMT  
		Size: 24.8 MB (24849262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eedc73b5df0ec289099eb44ad5b35b1b665275fb28bc869874f47e7f9279b9cd`  
		Last Modified: Wed, 15 Jul 2020 23:07:37 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.3` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:688de2b75dd901810244869b8bb7e3f6a437c9bef192be400d0dddc81a5e7606
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27751412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:982d3b3da00ee7a3fb892bcced519c84d83ba6a3a4e8969c30048e8291034812`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:23:55 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc2/traefik_v2.3.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:23:55 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:23:56 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:23:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:23:57 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:23:58 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff968af61b86e34dc2412293ade430f77b7db53f7f4adb925fec30d3ccbb2876`  
		Last Modified: Fri, 24 Apr 2020 12:43:42 GMT  
		Size: 696.1 KB (696058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974bdc9a43ec2151a237ff8d3b92d85e8b1a08d8f626c882203ca71b34e044ba`  
		Last Modified: Wed, 15 Jul 2020 23:31:05 GMT  
		Size: 24.3 MB (24330564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f12cd4c4b7843cbe81d3f484e87bf7e77cfaa32bbe47012036d2bb4956b79c`  
		Last Modified: Wed, 15 Jul 2020 23:30:57 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.3.0-rc2`

```console
$ docker pull traefik@sha256:b08601a937c1a160717e4ed6e0f4bc9ad0dea023de1ab309868cdf78164f9a33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.3.0-rc2` - linux; amd64

```console
$ docker pull traefik@sha256:b50cb55e6800df703f31b9a312d018558fc2286f829510f7da3de44a40aa74b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.9 MB (29942216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50a95f228e71630ffab61595fc050ce34c6013d6b9367440faef4e4f59d0e102`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:53:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc2/traefik_v2.3.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:53:34 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:53:34 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:53:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:53:35 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:53:35 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16506d32a25436b458a7f443ec1ca0d096d99d3479523c92c247856fc6148c0`  
		Last Modified: Fri, 24 Apr 2020 17:34:15 GMT  
		Size: 694.1 KB (694148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8f355ffe1c3315a63e73b1cb926b7f380eaa3ab4e9780add467a08709ef778`  
		Last Modified: Wed, 15 Jul 2020 23:54:29 GMT  
		Size: 26.4 MB (26434385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bdc521c6883d93f2893812825a3c6df9ac3959d1bf6c3ab800fcd311d8429a7`  
		Last Modified: Wed, 15 Jul 2020 23:54:24 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.3.0-rc2` - linux; arm variant v6

```console
$ docker pull traefik@sha256:09f2d34f7a32514f088d18ed0234527aeacd157d88187e115eed94c92db13e35
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.2 MB (28167652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab91012db5f2689da6b31247abefc6ca69082c5647a7f08b8439120169e69d9a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:04:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc2/traefik_v2.3.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:04:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:04:34 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:04:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:04:36 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:04:37 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a36cf46e6cb6a8028db7cb68482816e710935254a7d463897840713066cf5ba`  
		Last Modified: Thu, 23 Apr 2020 22:39:24 GMT  
		Size: 698.1 KB (698086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57bd030c3232794b6b0a553c8a0d9718f4c28235b71183f4ea6504924bd1782`  
		Last Modified: Wed, 15 Jul 2020 23:07:46 GMT  
		Size: 24.8 MB (24849262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eedc73b5df0ec289099eb44ad5b35b1b665275fb28bc869874f47e7f9279b9cd`  
		Last Modified: Wed, 15 Jul 2020 23:07:37 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.3.0-rc2` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:688de2b75dd901810244869b8bb7e3f6a437c9bef192be400d0dddc81a5e7606
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27751412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:982d3b3da00ee7a3fb892bcced519c84d83ba6a3a4e8969c30048e8291034812`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:23:55 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc2/traefik_v2.3.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:23:55 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:23:56 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:23:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:23:57 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:23:58 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff968af61b86e34dc2412293ade430f77b7db53f7f4adb925fec30d3ccbb2876`  
		Last Modified: Fri, 24 Apr 2020 12:43:42 GMT  
		Size: 696.1 KB (696058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974bdc9a43ec2151a237ff8d3b92d85e8b1a08d8f626c882203ca71b34e044ba`  
		Last Modified: Wed, 15 Jul 2020 23:31:05 GMT  
		Size: 24.3 MB (24330564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f12cd4c4b7843cbe81d3f484e87bf7e77cfaa32bbe47012036d2bb4956b79c`  
		Last Modified: Wed, 15 Jul 2020 23:30:57 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.3.0-rc2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e68058ecfa80e979dcc2fa6ee920bd8df2bcc50232d39143954f62218bf6a88f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `traefik:2.3.0-rc2-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull traefik@sha256:67b2e308c494d95c2a4bc00dd3367211a36981bb8c696c129ebad6ac3deb2d77
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2345763886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db8373dbd0aa67ba8149ddd07eef0fbec138c15cfb827ca6b4bce35804560b7`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 23:16:31 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.3.0-rc2/traefik_v2.3.0-rc2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 15 Jul 2020 23:16:33 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:16:34 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jul 2020 23:16:36 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb18feaa7bac1bd3b44235da4df5a7b60d9f7ed0d1d73e947b8891cd7caab13`  
		Last Modified: Wed, 15 Jul 2020 23:18:36 GMT  
		Size: 35.6 MB (35567079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f48b12aa3c2e7f28108611083bb84e20d68ebc804f82c72e66bf021afdddb83`  
		Last Modified: Wed, 15 Jul 2020 23:18:28 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788fee2061a681b14cf194dc60865450f05989d62c90f7fa4de355b47d50ace9`  
		Last Modified: Wed, 15 Jul 2020 23:18:28 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd82bd8a7ea907d29fe22de2223c0a05f643dfbe5896ad97e51fed7f541ebde9`  
		Last Modified: Wed, 15 Jul 2020 23:18:28 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.3-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e68058ecfa80e979dcc2fa6ee920bd8df2bcc50232d39143954f62218bf6a88f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `traefik:2.3-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull traefik@sha256:67b2e308c494d95c2a4bc00dd3367211a36981bb8c696c129ebad6ac3deb2d77
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2345763886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db8373dbd0aa67ba8149ddd07eef0fbec138c15cfb827ca6b4bce35804560b7`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 23:16:31 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.3.0-rc2/traefik_v2.3.0-rc2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 15 Jul 2020 23:16:33 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:16:34 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jul 2020 23:16:36 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb18feaa7bac1bd3b44235da4df5a7b60d9f7ed0d1d73e947b8891cd7caab13`  
		Last Modified: Wed, 15 Jul 2020 23:18:36 GMT  
		Size: 35.6 MB (35567079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f48b12aa3c2e7f28108611083bb84e20d68ebc804f82c72e66bf021afdddb83`  
		Last Modified: Wed, 15 Jul 2020 23:18:28 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788fee2061a681b14cf194dc60865450f05989d62c90f7fa4de355b47d50ace9`  
		Last Modified: Wed, 15 Jul 2020 23:18:28 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd82bd8a7ea907d29fe22de2223c0a05f643dfbe5896ad97e51fed7f541ebde9`  
		Last Modified: Wed, 15 Jul 2020 23:18:28 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:chevrotin`

```console
$ docker pull traefik@sha256:2dcdde75212d0117ef1360df5c532a2ec8bb97c386987b2bc66d973bca5003b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:chevrotin` - linux; amd64

```console
$ docker pull traefik@sha256:55f1b5e719c6e0f2d650e921463a87c8a4024236afb4991aea632df7ef942663
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25167013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de086c281ea7b4116c64a917309e249ae9063c663cd8e41c234bc54b88cfcd2c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Jul 2020 19:22:47 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.7/traefik_v2.2.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Jul 2020 19:22:47 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Jul 2020 19:22:47 GMT
EXPOSE 80
# Mon, 20 Jul 2020 19:22:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Jul 2020 19:22:48 GMT
CMD ["traefik"]
# Mon, 20 Jul 2020 19:22:48 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16506d32a25436b458a7f443ec1ca0d096d99d3479523c92c247856fc6148c0`  
		Last Modified: Fri, 24 Apr 2020 17:34:15 GMT  
		Size: 694.1 KB (694148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd583f1fc97ea2229f7e54f3b224e77b1b35f9e130dead096b58331b74427999`  
		Last Modified: Mon, 20 Jul 2020 19:23:12 GMT  
		Size: 21.7 MB (21659180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb2b75fe8e63b50ed1bb2728995b03b38ae981345ce246cececaf4384f5a9a1`  
		Last Modified: Mon, 20 Jul 2020 19:23:07 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:chevrotin` - linux; arm variant v6

```console
$ docker pull traefik@sha256:1dd33a92c9604ced7cfc03c9ad6653aa5d00a26a5e0a825f89ada10b052fb236
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.7 MB (23663447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41954059dfb2a60ecee9e006f90e5e8e9ec6d2174e65608e2518f801dc5df657`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Jul 2020 18:50:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.7/traefik_v2.2.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Jul 2020 18:50:32 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Jul 2020 18:50:32 GMT
EXPOSE 80
# Mon, 20 Jul 2020 18:50:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Jul 2020 18:50:34 GMT
CMD ["traefik"]
# Mon, 20 Jul 2020 18:50:35 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a36cf46e6cb6a8028db7cb68482816e710935254a7d463897840713066cf5ba`  
		Last Modified: Thu, 23 Apr 2020 22:39:24 GMT  
		Size: 698.1 KB (698086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ee7c01f51a7c41cc870b283b66ccd0dee4dfc7e0e9c1ca957d73969dc26691`  
		Last Modified: Mon, 20 Jul 2020 18:51:19 GMT  
		Size: 20.3 MB (20345057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ca186cb1c339d1fd77800b7788583c0d6b0309bda439b921d497a6f2030dc`  
		Last Modified: Mon, 20 Jul 2020 18:51:11 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:chevrotin` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:ae6a9e07e0c03df672e5fe90ade2f5a56ea27f1f0e30e2a13bb49d8cbdc3e7c9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23423015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f69c73e81ebad70c08ca34291273b3a3b4bb3b4b5f9a5acbd9fc3433c157e19`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Jul 2020 19:47:40 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.7/traefik_v2.2.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Jul 2020 19:47:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Jul 2020 19:47:42 GMT
EXPOSE 80
# Mon, 20 Jul 2020 19:47:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Jul 2020 19:47:46 GMT
CMD ["traefik"]
# Mon, 20 Jul 2020 19:47:46 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff968af61b86e34dc2412293ade430f77b7db53f7f4adb925fec30d3ccbb2876`  
		Last Modified: Fri, 24 Apr 2020 12:43:42 GMT  
		Size: 696.1 KB (696058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2ba74a0f32fa0e26ecf336f6d70bc0d0a8a08a20062643dd9ac00bed14efa6`  
		Last Modified: Mon, 20 Jul 2020 19:48:27 GMT  
		Size: 20.0 MB (20002164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569fe01719a75603ca3d8c344ac5ec7d52199626d3240e48bf9e947a18b21810`  
		Last Modified: Mon, 20 Jul 2020 19:48:16 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:chevrotin-windowsservercore-1809`

```console
$ docker pull traefik@sha256:fda8b53c30a901acfa91388660d2d85dfb77bcd49f7a3fe66d6d3c27c6710ac2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `traefik:chevrotin-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull traefik@sha256:f3c6b74c8cee89d7dd612c1f545a67746f57cbddabe650718c0d3e91af5fbc5f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2340995387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6abec4b0661abb8b7e71d04e842c7bc38a5e9afad4991089c95c19107c611a1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 20 Jul 2020 19:15:37 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.2.7/traefik_v2.2.7_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 20 Jul 2020 19:15:39 GMT
EXPOSE 80
# Mon, 20 Jul 2020 19:15:40 GMT
ENTRYPOINT ["/traefik"]
# Mon, 20 Jul 2020 19:15:42 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0247512bb5646fd88951141a0338afcbabb2130655250cc3959d27438ef1fb`  
		Last Modified: Mon, 20 Jul 2020 19:16:17 GMT  
		Size: 30.8 MB (30798531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e1f70926eb835a5f2a15b7eb3a699976603074073a3ec7e8e693221740f56f`  
		Last Modified: Mon, 20 Jul 2020 19:16:10 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1821ea1f642148d720fd6f4cfe40d3383d8b12c6c85e8e3cddd726f8cfc8b2b1`  
		Last Modified: Mon, 20 Jul 2020 19:16:09 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a2388b729f036c4dbf707e9e9a283d3a27987b149789c94b0307c5502febd1`  
		Last Modified: Mon, 20 Jul 2020 19:16:09 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:2dcdde75212d0117ef1360df5c532a2ec8bb97c386987b2bc66d973bca5003b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:55f1b5e719c6e0f2d650e921463a87c8a4024236afb4991aea632df7ef942663
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25167013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de086c281ea7b4116c64a917309e249ae9063c663cd8e41c234bc54b88cfcd2c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Jul 2020 19:22:47 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.7/traefik_v2.2.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Jul 2020 19:22:47 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Jul 2020 19:22:47 GMT
EXPOSE 80
# Mon, 20 Jul 2020 19:22:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Jul 2020 19:22:48 GMT
CMD ["traefik"]
# Mon, 20 Jul 2020 19:22:48 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16506d32a25436b458a7f443ec1ca0d096d99d3479523c92c247856fc6148c0`  
		Last Modified: Fri, 24 Apr 2020 17:34:15 GMT  
		Size: 694.1 KB (694148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd583f1fc97ea2229f7e54f3b224e77b1b35f9e130dead096b58331b74427999`  
		Last Modified: Mon, 20 Jul 2020 19:23:12 GMT  
		Size: 21.7 MB (21659180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb2b75fe8e63b50ed1bb2728995b03b38ae981345ce246cececaf4384f5a9a1`  
		Last Modified: Mon, 20 Jul 2020 19:23:07 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:1dd33a92c9604ced7cfc03c9ad6653aa5d00a26a5e0a825f89ada10b052fb236
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.7 MB (23663447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41954059dfb2a60ecee9e006f90e5e8e9ec6d2174e65608e2518f801dc5df657`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Jul 2020 18:50:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.7/traefik_v2.2.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Jul 2020 18:50:32 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Jul 2020 18:50:32 GMT
EXPOSE 80
# Mon, 20 Jul 2020 18:50:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Jul 2020 18:50:34 GMT
CMD ["traefik"]
# Mon, 20 Jul 2020 18:50:35 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a36cf46e6cb6a8028db7cb68482816e710935254a7d463897840713066cf5ba`  
		Last Modified: Thu, 23 Apr 2020 22:39:24 GMT  
		Size: 698.1 KB (698086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ee7c01f51a7c41cc870b283b66ccd0dee4dfc7e0e9c1ca957d73969dc26691`  
		Last Modified: Mon, 20 Jul 2020 18:51:19 GMT  
		Size: 20.3 MB (20345057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ca186cb1c339d1fd77800b7788583c0d6b0309bda439b921d497a6f2030dc`  
		Last Modified: Mon, 20 Jul 2020 18:51:11 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:ae6a9e07e0c03df672e5fe90ade2f5a56ea27f1f0e30e2a13bb49d8cbdc3e7c9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23423015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f69c73e81ebad70c08ca34291273b3a3b4bb3b4b5f9a5acbd9fc3433c157e19`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Jul 2020 19:47:40 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.7/traefik_v2.2.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Jul 2020 19:47:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Jul 2020 19:47:42 GMT
EXPOSE 80
# Mon, 20 Jul 2020 19:47:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Jul 2020 19:47:46 GMT
CMD ["traefik"]
# Mon, 20 Jul 2020 19:47:46 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff968af61b86e34dc2412293ade430f77b7db53f7f4adb925fec30d3ccbb2876`  
		Last Modified: Fri, 24 Apr 2020 12:43:42 GMT  
		Size: 696.1 KB (696058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2ba74a0f32fa0e26ecf336f6d70bc0d0a8a08a20062643dd9ac00bed14efa6`  
		Last Modified: Mon, 20 Jul 2020 19:48:27 GMT  
		Size: 20.0 MB (20002164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569fe01719a75603ca3d8c344ac5ec7d52199626d3240e48bf9e947a18b21810`  
		Last Modified: Mon, 20 Jul 2020 19:48:16 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles`

```console
$ docker pull traefik@sha256:1fa3e9ee4509211196b926eb90d07ffbdf72d730ff3d8c428ac94f3b1c784783
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles` - linux; amd64

```console
$ docker pull traefik@sha256:6eac900151c64c8465ef0e38b27d4ae9d877616230162279727337b47ff5dc08
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21584351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca551e784d546c33bab389a7b90aca0c74fa026194a34cbd4a6805a32fde606f`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 02:50:22 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 02:50:24 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 15 Jul 2020 23:54:07 GMT
COPY file:dbebc61aa00cc3bd336b1fe611a0e32e7ad8b4b311e43c336de691d7c04a47af in / 
# Wed, 15 Jul 2020 23:54:08 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:54:08 GMT
VOLUME [/tmp]
# Wed, 15 Jul 2020 23:54:08 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jul 2020 23:54:08 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e40d0b92fe2d2ef50c6f43f32c33dc117ab26d69a29d74ae15725a379dbde0c2`  
		Last Modified: Fri, 21 Feb 2020 02:51:04 GMT  
		Size: 131.7 KB (131682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c068c5049677b6879089396aa0d2d162ac9697e25bacf333c0596a248bae8a5`  
		Last Modified: Fri, 21 Feb 2020 02:51:04 GMT  
		Size: 327.4 KB (327376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2668a1328cae473e5092f00bde31aa8d95bd00773bd3dbb5bf938539066ec41e`  
		Last Modified: Wed, 15 Jul 2020 23:54:48 GMT  
		Size: 21.1 MB (21125293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm variant v6

```console
$ docker pull traefik@sha256:201b3f9b283f6bc734fe33ab3c1c7c428d5878ccf4836be1892f1aea6bd63a9d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20231475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47cc1d1e27878e29edf1fc95fa792416065312621456b2f166e71de4782cae1e`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 03:46:16 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 03:46:17 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 15 Jul 2020 23:07:11 GMT
COPY file:185bd7cda9d632ce86c62da94a8061efac1291f616a72972fcda00ba82e29c4d in / 
# Wed, 15 Jul 2020 23:07:12 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:07:14 GMT
VOLUME [/tmp]
# Wed, 15 Jul 2020 23:07:15 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jul 2020 23:07:16 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:3ea78b0360c0223e83ecbb7336ab0de873d099e2aa889216bc3622c7dc315adc`  
		Last Modified: Tue, 24 Mar 2020 03:47:54 GMT  
		Size: 131.7 KB (131681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd374e140760994a9274b43e4cbf314b61a77acb227eca705d35780bb33a6a07`  
		Last Modified: Tue, 24 Mar 2020 03:47:55 GMT  
		Size: 327.4 KB (327405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5eb8f091d88a8df352ff16fe91d7b9d4a458c1fbb7e28ce7a282293681e2c91`  
		Last Modified: Wed, 15 Jul 2020 23:08:16 GMT  
		Size: 19.8 MB (19772389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:c98ea0955bb58f169837a6a29663ccec288bc496290aa06d19a63b1922ea44fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.0 MB (19952902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c7f0e9591004fb0d9f0ec32c8b5e3294790b993e054cb774f1b08055583fcde`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 05:55:25 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 05:55:26 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 15 Jul 2020 23:30:24 GMT
COPY file:2004fb63ffb43df9c881281b0e9250dcd15332dde58681121ec9738221528602 in / 
# Wed, 15 Jul 2020 23:30:25 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:30:26 GMT
VOLUME [/tmp]
# Wed, 15 Jul 2020 23:30:27 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jul 2020 23:30:28 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:58ceb9a2a8ba9dd83eef0c2cf887c175911b301df486d142f7d09293605add22`  
		Last Modified: Tue, 24 Mar 2020 05:56:42 GMT  
		Size: 131.7 KB (131676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b9edf48787b0368bb1af04734041d3b374acefa70417bdf0090919056c874d`  
		Last Modified: Tue, 24 Mar 2020 05:56:42 GMT  
		Size: 327.4 KB (327402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100a118a37516ea44966052eb5d2b1de534be63dd7da7443bf69a60c4cf3731d`  
		Last Modified: Wed, 15 Jul 2020 23:31:38 GMT  
		Size: 19.5 MB (19493824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-alpine`

```console
$ docker pull traefik@sha256:d4325a60a66c34c4491b7662a71e2b0f5c45cefcb036af8e762f7ccc685b1874
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:56b5ec0207c9d9bca95b2c25262ff968c1edf4469984000c7550bcf23952827e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24633397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b15dfa7af58e7044de080d1e00c691112ad97424a0d63f7dd81e59ce0ea20beb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:53:41 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.25/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:53:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:53:42 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:53:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:53:42 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:53:42 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16506d32a25436b458a7f443ec1ca0d096d99d3479523c92c247856fc6148c0`  
		Last Modified: Fri, 24 Apr 2020 17:34:15 GMT  
		Size: 694.1 KB (694148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e283b232b00d6def332f0854c0624efc59074fd6f99cf171abe83af71d716739`  
		Last Modified: Wed, 15 Jul 2020 23:54:38 GMT  
		Size: 21.1 MB (21125565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21796958177fa80eb809b5a57c9f547af553cfdc9a0568b4794bac6610af934`  
		Last Modified: Wed, 15 Jul 2020 23:54:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:b21c79858f578e27cb04a8723686008dc91197fd7cdeb94614935e171871ef7b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23090947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b97db544f1052e42a534853e75d36cb7b6996ec4223752e4187ac4d0bbe5417c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:04:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.25/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:04:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:04:53 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:04:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:04:55 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:04:56 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a36cf46e6cb6a8028db7cb68482816e710935254a7d463897840713066cf5ba`  
		Last Modified: Thu, 23 Apr 2020 22:39:24 GMT  
		Size: 698.1 KB (698086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bfedcce63424119565c9a127a7f8bd82e99ea024f93f2c7427942f3451e3001`  
		Last Modified: Wed, 15 Jul 2020 23:08:01 GMT  
		Size: 19.8 MB (19772557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b24e2aadaecd85cde7ef979c7a6981ae83a7050116df5fcb073bfec4833cc74`  
		Last Modified: Wed, 15 Jul 2020 23:07:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3798e6eea86039b46b4bf760f5cc4bc6be672ea0b89c9e0be397eddfb16000f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22914773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3940f96616b8f8d03d96c2796404288a054b54b87b587c9f0bc7c90d1ae2d5da`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:24:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.25/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:24:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:24:10 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:24:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:24:12 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:24:13 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff968af61b86e34dc2412293ade430f77b7db53f7f4adb925fec30d3ccbb2876`  
		Last Modified: Fri, 24 Apr 2020 12:43:42 GMT  
		Size: 696.1 KB (696058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380ca995bf3761e50cdb46b03208ac913ea1328566e2eac8ad835867ff78a077`  
		Last Modified: Wed, 15 Jul 2020 23:31:22 GMT  
		Size: 19.5 MB (19493924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d88c62829ac867327a678720b6bcc03c9b9413d196cd15ef2983d4946b9ebb`  
		Last Modified: Wed, 15 Jul 2020 23:31:15 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-windowsservercore-1809`

```console
$ docker pull traefik@sha256:7a2e772e8537a92ad67813de222d6fc35d46db70f8c3342c22ca0bcb9f2224a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull traefik@sha256:2447f4bcd451245ad9e3200626d0ad9bc6842f4f6288743c1b1ad4154698b46a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2340473541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d6ce3a7269e05fd8df0e5f6c1f272c24bf8903d1b499bc84306431e5c0ab3a5`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 23:17:53 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.25/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 15 Jul 2020 23:17:54 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:17:56 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jul 2020 23:17:58 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56765e2183d70fbee243e23e45b4dae04f3611ac7bb45d0f237f7141337bb6b1`  
		Last Modified: Wed, 15 Jul 2020 23:19:02 GMT  
		Size: 30.3 MB (30276616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a9aeca829593fbf97e6ddfba27b1f71b9cfdbdc814b9a0c353b82039542a53`  
		Last Modified: Wed, 15 Jul 2020 23:18:57 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13f8ba7125cb8bd4176a652b98db75af122b71acd3aa8f00de1120b8234d009`  
		Last Modified: Wed, 15 Jul 2020 23:18:55 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffbf5581287fcb7681d76485a5bf4e5f1ded4fe51c7e8f2c91d1f5b98df456a`  
		Last Modified: Wed, 15 Jul 2020 23:18:54 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:picodon`

```console
$ docker pull traefik@sha256:b08601a937c1a160717e4ed6e0f4bc9ad0dea023de1ab309868cdf78164f9a33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:picodon` - linux; amd64

```console
$ docker pull traefik@sha256:b50cb55e6800df703f31b9a312d018558fc2286f829510f7da3de44a40aa74b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.9 MB (29942216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50a95f228e71630ffab61595fc050ce34c6013d6b9367440faef4e4f59d0e102`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:53:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc2/traefik_v2.3.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:53:34 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:53:34 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:53:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:53:35 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:53:35 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16506d32a25436b458a7f443ec1ca0d096d99d3479523c92c247856fc6148c0`  
		Last Modified: Fri, 24 Apr 2020 17:34:15 GMT  
		Size: 694.1 KB (694148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8f355ffe1c3315a63e73b1cb926b7f380eaa3ab4e9780add467a08709ef778`  
		Last Modified: Wed, 15 Jul 2020 23:54:29 GMT  
		Size: 26.4 MB (26434385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bdc521c6883d93f2893812825a3c6df9ac3959d1bf6c3ab800fcd311d8429a7`  
		Last Modified: Wed, 15 Jul 2020 23:54:24 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:picodon` - linux; arm variant v6

```console
$ docker pull traefik@sha256:09f2d34f7a32514f088d18ed0234527aeacd157d88187e115eed94c92db13e35
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.2 MB (28167652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab91012db5f2689da6b31247abefc6ca69082c5647a7f08b8439120169e69d9a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:04:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc2/traefik_v2.3.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:04:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:04:34 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:04:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:04:36 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:04:37 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a36cf46e6cb6a8028db7cb68482816e710935254a7d463897840713066cf5ba`  
		Last Modified: Thu, 23 Apr 2020 22:39:24 GMT  
		Size: 698.1 KB (698086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57bd030c3232794b6b0a553c8a0d9718f4c28235b71183f4ea6504924bd1782`  
		Last Modified: Wed, 15 Jul 2020 23:07:46 GMT  
		Size: 24.8 MB (24849262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eedc73b5df0ec289099eb44ad5b35b1b665275fb28bc869874f47e7f9279b9cd`  
		Last Modified: Wed, 15 Jul 2020 23:07:37 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:picodon` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:688de2b75dd901810244869b8bb7e3f6a437c9bef192be400d0dddc81a5e7606
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27751412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:982d3b3da00ee7a3fb892bcced519c84d83ba6a3a4e8969c30048e8291034812`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:23:55 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc2/traefik_v2.3.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:23:55 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:23:56 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:23:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:23:57 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:23:58 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff968af61b86e34dc2412293ade430f77b7db53f7f4adb925fec30d3ccbb2876`  
		Last Modified: Fri, 24 Apr 2020 12:43:42 GMT  
		Size: 696.1 KB (696058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974bdc9a43ec2151a237ff8d3b92d85e8b1a08d8f626c882203ca71b34e044ba`  
		Last Modified: Wed, 15 Jul 2020 23:31:05 GMT  
		Size: 24.3 MB (24330564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f12cd4c4b7843cbe81d3f484e87bf7e77cfaa32bbe47012036d2bb4956b79c`  
		Last Modified: Wed, 15 Jul 2020 23:30:57 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:picodon-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e68058ecfa80e979dcc2fa6ee920bd8df2bcc50232d39143954f62218bf6a88f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `traefik:picodon-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull traefik@sha256:67b2e308c494d95c2a4bc00dd3367211a36981bb8c696c129ebad6ac3deb2d77
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2345763886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db8373dbd0aa67ba8149ddd07eef0fbec138c15cfb827ca6b4bce35804560b7`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 23:16:31 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.3.0-rc2/traefik_v2.3.0-rc2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 15 Jul 2020 23:16:33 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:16:34 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jul 2020 23:16:36 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb18feaa7bac1bd3b44235da4df5a7b60d9f7ed0d1d73e947b8891cd7caab13`  
		Last Modified: Wed, 15 Jul 2020 23:18:36 GMT  
		Size: 35.6 MB (35567079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f48b12aa3c2e7f28108611083bb84e20d68ebc804f82c72e66bf021afdddb83`  
		Last Modified: Wed, 15 Jul 2020 23:18:28 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788fee2061a681b14cf194dc60865450f05989d62c90f7fa4de355b47d50ace9`  
		Last Modified: Wed, 15 Jul 2020 23:18:28 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd82bd8a7ea907d29fe22de2223c0a05f643dfbe5896ad97e51fed7f541ebde9`  
		Last Modified: Wed, 15 Jul 2020 23:18:28 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7`

```console
$ docker pull traefik@sha256:1fa3e9ee4509211196b926eb90d07ffbdf72d730ff3d8c428ac94f3b1c784783
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7` - linux; amd64

```console
$ docker pull traefik@sha256:6eac900151c64c8465ef0e38b27d4ae9d877616230162279727337b47ff5dc08
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21584351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca551e784d546c33bab389a7b90aca0c74fa026194a34cbd4a6805a32fde606f`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 02:50:22 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 02:50:24 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 15 Jul 2020 23:54:07 GMT
COPY file:dbebc61aa00cc3bd336b1fe611a0e32e7ad8b4b311e43c336de691d7c04a47af in / 
# Wed, 15 Jul 2020 23:54:08 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:54:08 GMT
VOLUME [/tmp]
# Wed, 15 Jul 2020 23:54:08 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jul 2020 23:54:08 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e40d0b92fe2d2ef50c6f43f32c33dc117ab26d69a29d74ae15725a379dbde0c2`  
		Last Modified: Fri, 21 Feb 2020 02:51:04 GMT  
		Size: 131.7 KB (131682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c068c5049677b6879089396aa0d2d162ac9697e25bacf333c0596a248bae8a5`  
		Last Modified: Fri, 21 Feb 2020 02:51:04 GMT  
		Size: 327.4 KB (327376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2668a1328cae473e5092f00bde31aa8d95bd00773bd3dbb5bf938539066ec41e`  
		Last Modified: Wed, 15 Jul 2020 23:54:48 GMT  
		Size: 21.1 MB (21125293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:201b3f9b283f6bc734fe33ab3c1c7c428d5878ccf4836be1892f1aea6bd63a9d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20231475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47cc1d1e27878e29edf1fc95fa792416065312621456b2f166e71de4782cae1e`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 03:46:16 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 03:46:17 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 15 Jul 2020 23:07:11 GMT
COPY file:185bd7cda9d632ce86c62da94a8061efac1291f616a72972fcda00ba82e29c4d in / 
# Wed, 15 Jul 2020 23:07:12 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:07:14 GMT
VOLUME [/tmp]
# Wed, 15 Jul 2020 23:07:15 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jul 2020 23:07:16 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:3ea78b0360c0223e83ecbb7336ab0de873d099e2aa889216bc3622c7dc315adc`  
		Last Modified: Tue, 24 Mar 2020 03:47:54 GMT  
		Size: 131.7 KB (131681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd374e140760994a9274b43e4cbf314b61a77acb227eca705d35780bb33a6a07`  
		Last Modified: Tue, 24 Mar 2020 03:47:55 GMT  
		Size: 327.4 KB (327405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5eb8f091d88a8df352ff16fe91d7b9d4a458c1fbb7e28ce7a282293681e2c91`  
		Last Modified: Wed, 15 Jul 2020 23:08:16 GMT  
		Size: 19.8 MB (19772389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:c98ea0955bb58f169837a6a29663ccec288bc496290aa06d19a63b1922ea44fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.0 MB (19952902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c7f0e9591004fb0d9f0ec32c8b5e3294790b993e054cb774f1b08055583fcde`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 05:55:25 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 05:55:26 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 15 Jul 2020 23:30:24 GMT
COPY file:2004fb63ffb43df9c881281b0e9250dcd15332dde58681121ec9738221528602 in / 
# Wed, 15 Jul 2020 23:30:25 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:30:26 GMT
VOLUME [/tmp]
# Wed, 15 Jul 2020 23:30:27 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jul 2020 23:30:28 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:58ceb9a2a8ba9dd83eef0c2cf887c175911b301df486d142f7d09293605add22`  
		Last Modified: Tue, 24 Mar 2020 05:56:42 GMT  
		Size: 131.7 KB (131676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b9edf48787b0368bb1af04734041d3b374acefa70417bdf0090919056c874d`  
		Last Modified: Tue, 24 Mar 2020 05:56:42 GMT  
		Size: 327.4 KB (327402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100a118a37516ea44966052eb5d2b1de534be63dd7da7443bf69a60c4cf3731d`  
		Last Modified: Wed, 15 Jul 2020 23:31:38 GMT  
		Size: 19.5 MB (19493824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.25`

```console
$ docker pull traefik@sha256:1fa3e9ee4509211196b926eb90d07ffbdf72d730ff3d8c428ac94f3b1c784783
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.25` - linux; amd64

```console
$ docker pull traefik@sha256:6eac900151c64c8465ef0e38b27d4ae9d877616230162279727337b47ff5dc08
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21584351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca551e784d546c33bab389a7b90aca0c74fa026194a34cbd4a6805a32fde606f`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 02:50:22 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 02:50:24 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 15 Jul 2020 23:54:07 GMT
COPY file:dbebc61aa00cc3bd336b1fe611a0e32e7ad8b4b311e43c336de691d7c04a47af in / 
# Wed, 15 Jul 2020 23:54:08 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:54:08 GMT
VOLUME [/tmp]
# Wed, 15 Jul 2020 23:54:08 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jul 2020 23:54:08 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e40d0b92fe2d2ef50c6f43f32c33dc117ab26d69a29d74ae15725a379dbde0c2`  
		Last Modified: Fri, 21 Feb 2020 02:51:04 GMT  
		Size: 131.7 KB (131682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c068c5049677b6879089396aa0d2d162ac9697e25bacf333c0596a248bae8a5`  
		Last Modified: Fri, 21 Feb 2020 02:51:04 GMT  
		Size: 327.4 KB (327376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2668a1328cae473e5092f00bde31aa8d95bd00773bd3dbb5bf938539066ec41e`  
		Last Modified: Wed, 15 Jul 2020 23:54:48 GMT  
		Size: 21.1 MB (21125293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.25` - linux; arm variant v6

```console
$ docker pull traefik@sha256:201b3f9b283f6bc734fe33ab3c1c7c428d5878ccf4836be1892f1aea6bd63a9d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20231475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47cc1d1e27878e29edf1fc95fa792416065312621456b2f166e71de4782cae1e`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 03:46:16 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 03:46:17 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 15 Jul 2020 23:07:11 GMT
COPY file:185bd7cda9d632ce86c62da94a8061efac1291f616a72972fcda00ba82e29c4d in / 
# Wed, 15 Jul 2020 23:07:12 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:07:14 GMT
VOLUME [/tmp]
# Wed, 15 Jul 2020 23:07:15 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jul 2020 23:07:16 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:3ea78b0360c0223e83ecbb7336ab0de873d099e2aa889216bc3622c7dc315adc`  
		Last Modified: Tue, 24 Mar 2020 03:47:54 GMT  
		Size: 131.7 KB (131681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd374e140760994a9274b43e4cbf314b61a77acb227eca705d35780bb33a6a07`  
		Last Modified: Tue, 24 Mar 2020 03:47:55 GMT  
		Size: 327.4 KB (327405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5eb8f091d88a8df352ff16fe91d7b9d4a458c1fbb7e28ce7a282293681e2c91`  
		Last Modified: Wed, 15 Jul 2020 23:08:16 GMT  
		Size: 19.8 MB (19772389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.25` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:c98ea0955bb58f169837a6a29663ccec288bc496290aa06d19a63b1922ea44fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.0 MB (19952902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c7f0e9591004fb0d9f0ec32c8b5e3294790b993e054cb774f1b08055583fcde`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 05:55:25 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 05:55:26 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 15 Jul 2020 23:30:24 GMT
COPY file:2004fb63ffb43df9c881281b0e9250dcd15332dde58681121ec9738221528602 in / 
# Wed, 15 Jul 2020 23:30:25 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:30:26 GMT
VOLUME [/tmp]
# Wed, 15 Jul 2020 23:30:27 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jul 2020 23:30:28 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:58ceb9a2a8ba9dd83eef0c2cf887c175911b301df486d142f7d09293605add22`  
		Last Modified: Tue, 24 Mar 2020 05:56:42 GMT  
		Size: 131.7 KB (131676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b9edf48787b0368bb1af04734041d3b374acefa70417bdf0090919056c874d`  
		Last Modified: Tue, 24 Mar 2020 05:56:42 GMT  
		Size: 327.4 KB (327402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100a118a37516ea44966052eb5d2b1de534be63dd7da7443bf69a60c4cf3731d`  
		Last Modified: Wed, 15 Jul 2020 23:31:38 GMT  
		Size: 19.5 MB (19493824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.25-alpine`

```console
$ docker pull traefik@sha256:d4325a60a66c34c4491b7662a71e2b0f5c45cefcb036af8e762f7ccc685b1874
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.25-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:56b5ec0207c9d9bca95b2c25262ff968c1edf4469984000c7550bcf23952827e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24633397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b15dfa7af58e7044de080d1e00c691112ad97424a0d63f7dd81e59ce0ea20beb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:53:41 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.25/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:53:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:53:42 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:53:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:53:42 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:53:42 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16506d32a25436b458a7f443ec1ca0d096d99d3479523c92c247856fc6148c0`  
		Last Modified: Fri, 24 Apr 2020 17:34:15 GMT  
		Size: 694.1 KB (694148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e283b232b00d6def332f0854c0624efc59074fd6f99cf171abe83af71d716739`  
		Last Modified: Wed, 15 Jul 2020 23:54:38 GMT  
		Size: 21.1 MB (21125565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21796958177fa80eb809b5a57c9f547af553cfdc9a0568b4794bac6610af934`  
		Last Modified: Wed, 15 Jul 2020 23:54:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.25-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:b21c79858f578e27cb04a8723686008dc91197fd7cdeb94614935e171871ef7b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23090947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b97db544f1052e42a534853e75d36cb7b6996ec4223752e4187ac4d0bbe5417c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:04:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.25/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:04:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:04:53 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:04:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:04:55 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:04:56 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a36cf46e6cb6a8028db7cb68482816e710935254a7d463897840713066cf5ba`  
		Last Modified: Thu, 23 Apr 2020 22:39:24 GMT  
		Size: 698.1 KB (698086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bfedcce63424119565c9a127a7f8bd82e99ea024f93f2c7427942f3451e3001`  
		Last Modified: Wed, 15 Jul 2020 23:08:01 GMT  
		Size: 19.8 MB (19772557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b24e2aadaecd85cde7ef979c7a6981ae83a7050116df5fcb073bfec4833cc74`  
		Last Modified: Wed, 15 Jul 2020 23:07:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.25-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3798e6eea86039b46b4bf760f5cc4bc6be672ea0b89c9e0be397eddfb16000f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22914773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3940f96616b8f8d03d96c2796404288a054b54b87b587c9f0bc7c90d1ae2d5da`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:24:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.25/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:24:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:24:10 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:24:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:24:12 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:24:13 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff968af61b86e34dc2412293ade430f77b7db53f7f4adb925fec30d3ccbb2876`  
		Last Modified: Fri, 24 Apr 2020 12:43:42 GMT  
		Size: 696.1 KB (696058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380ca995bf3761e50cdb46b03208ac913ea1328566e2eac8ad835867ff78a077`  
		Last Modified: Wed, 15 Jul 2020 23:31:22 GMT  
		Size: 19.5 MB (19493924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d88c62829ac867327a678720b6bcc03c9b9413d196cd15ef2983d4946b9ebb`  
		Last Modified: Wed, 15 Jul 2020 23:31:15 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.25-windowsservercore-1809`

```console
$ docker pull traefik@sha256:7a2e772e8537a92ad67813de222d6fc35d46db70f8c3342c22ca0bcb9f2224a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `traefik:v1.7.25-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull traefik@sha256:2447f4bcd451245ad9e3200626d0ad9bc6842f4f6288743c1b1ad4154698b46a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2340473541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d6ce3a7269e05fd8df0e5f6c1f272c24bf8903d1b499bc84306431e5c0ab3a5`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 23:17:53 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.25/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 15 Jul 2020 23:17:54 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:17:56 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jul 2020 23:17:58 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56765e2183d70fbee243e23e45b4dae04f3611ac7bb45d0f237f7141337bb6b1`  
		Last Modified: Wed, 15 Jul 2020 23:19:02 GMT  
		Size: 30.3 MB (30276616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a9aeca829593fbf97e6ddfba27b1f71b9cfdbdc814b9a0c353b82039542a53`  
		Last Modified: Wed, 15 Jul 2020 23:18:57 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13f8ba7125cb8bd4176a652b98db75af122b71acd3aa8f00de1120b8234d009`  
		Last Modified: Wed, 15 Jul 2020 23:18:55 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffbf5581287fcb7681d76485a5bf4e5f1ded4fe51c7e8f2c91d1f5b98df456a`  
		Last Modified: Wed, 15 Jul 2020 23:18:54 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-alpine`

```console
$ docker pull traefik@sha256:d4325a60a66c34c4491b7662a71e2b0f5c45cefcb036af8e762f7ccc685b1874
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:56b5ec0207c9d9bca95b2c25262ff968c1edf4469984000c7550bcf23952827e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24633397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b15dfa7af58e7044de080d1e00c691112ad97424a0d63f7dd81e59ce0ea20beb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:53:41 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.25/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:53:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:53:42 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:53:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:53:42 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:53:42 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16506d32a25436b458a7f443ec1ca0d096d99d3479523c92c247856fc6148c0`  
		Last Modified: Fri, 24 Apr 2020 17:34:15 GMT  
		Size: 694.1 KB (694148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e283b232b00d6def332f0854c0624efc59074fd6f99cf171abe83af71d716739`  
		Last Modified: Wed, 15 Jul 2020 23:54:38 GMT  
		Size: 21.1 MB (21125565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21796958177fa80eb809b5a57c9f547af553cfdc9a0568b4794bac6610af934`  
		Last Modified: Wed, 15 Jul 2020 23:54:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:b21c79858f578e27cb04a8723686008dc91197fd7cdeb94614935e171871ef7b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23090947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b97db544f1052e42a534853e75d36cb7b6996ec4223752e4187ac4d0bbe5417c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:04:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.25/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:04:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:04:53 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:04:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:04:55 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:04:56 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a36cf46e6cb6a8028db7cb68482816e710935254a7d463897840713066cf5ba`  
		Last Modified: Thu, 23 Apr 2020 22:39:24 GMT  
		Size: 698.1 KB (698086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bfedcce63424119565c9a127a7f8bd82e99ea024f93f2c7427942f3451e3001`  
		Last Modified: Wed, 15 Jul 2020 23:08:01 GMT  
		Size: 19.8 MB (19772557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b24e2aadaecd85cde7ef979c7a6981ae83a7050116df5fcb073bfec4833cc74`  
		Last Modified: Wed, 15 Jul 2020 23:07:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3798e6eea86039b46b4bf760f5cc4bc6be672ea0b89c9e0be397eddfb16000f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22914773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3940f96616b8f8d03d96c2796404288a054b54b87b587c9f0bc7c90d1ae2d5da`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:24:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.25/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:24:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:24:10 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:24:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:24:12 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:24:13 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff968af61b86e34dc2412293ade430f77b7db53f7f4adb925fec30d3ccbb2876`  
		Last Modified: Fri, 24 Apr 2020 12:43:42 GMT  
		Size: 696.1 KB (696058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380ca995bf3761e50cdb46b03208ac913ea1328566e2eac8ad835867ff78a077`  
		Last Modified: Wed, 15 Jul 2020 23:31:22 GMT  
		Size: 19.5 MB (19493924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d88c62829ac867327a678720b6bcc03c9b9413d196cd15ef2983d4946b9ebb`  
		Last Modified: Wed, 15 Jul 2020 23:31:15 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:7a2e772e8537a92ad67813de222d6fc35d46db70f8c3342c22ca0bcb9f2224a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `traefik:v1.7-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull traefik@sha256:2447f4bcd451245ad9e3200626d0ad9bc6842f4f6288743c1b1ad4154698b46a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2340473541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d6ce3a7269e05fd8df0e5f6c1f272c24bf8903d1b499bc84306431e5c0ab3a5`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 23:17:53 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.25/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 15 Jul 2020 23:17:54 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:17:56 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jul 2020 23:17:58 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.25 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56765e2183d70fbee243e23e45b4dae04f3611ac7bb45d0f237f7141337bb6b1`  
		Last Modified: Wed, 15 Jul 2020 23:19:02 GMT  
		Size: 30.3 MB (30276616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a9aeca829593fbf97e6ddfba27b1f71b9cfdbdc814b9a0c353b82039542a53`  
		Last Modified: Wed, 15 Jul 2020 23:18:57 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13f8ba7125cb8bd4176a652b98db75af122b71acd3aa8f00de1120b8234d009`  
		Last Modified: Wed, 15 Jul 2020 23:18:55 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffbf5581287fcb7681d76485a5bf4e5f1ded4fe51c7e8f2c91d1f5b98df456a`  
		Last Modified: Wed, 15 Jul 2020 23:18:54 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.2`

```console
$ docker pull traefik@sha256:2dcdde75212d0117ef1360df5c532a2ec8bb97c386987b2bc66d973bca5003b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.2` - linux; amd64

```console
$ docker pull traefik@sha256:55f1b5e719c6e0f2d650e921463a87c8a4024236afb4991aea632df7ef942663
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25167013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de086c281ea7b4116c64a917309e249ae9063c663cd8e41c234bc54b88cfcd2c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Jul 2020 19:22:47 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.7/traefik_v2.2.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Jul 2020 19:22:47 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Jul 2020 19:22:47 GMT
EXPOSE 80
# Mon, 20 Jul 2020 19:22:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Jul 2020 19:22:48 GMT
CMD ["traefik"]
# Mon, 20 Jul 2020 19:22:48 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16506d32a25436b458a7f443ec1ca0d096d99d3479523c92c247856fc6148c0`  
		Last Modified: Fri, 24 Apr 2020 17:34:15 GMT  
		Size: 694.1 KB (694148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd583f1fc97ea2229f7e54f3b224e77b1b35f9e130dead096b58331b74427999`  
		Last Modified: Mon, 20 Jul 2020 19:23:12 GMT  
		Size: 21.7 MB (21659180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb2b75fe8e63b50ed1bb2728995b03b38ae981345ce246cececaf4384f5a9a1`  
		Last Modified: Mon, 20 Jul 2020 19:23:07 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.2` - linux; arm variant v6

```console
$ docker pull traefik@sha256:1dd33a92c9604ced7cfc03c9ad6653aa5d00a26a5e0a825f89ada10b052fb236
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.7 MB (23663447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41954059dfb2a60ecee9e006f90e5e8e9ec6d2174e65608e2518f801dc5df657`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Jul 2020 18:50:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.7/traefik_v2.2.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Jul 2020 18:50:32 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Jul 2020 18:50:32 GMT
EXPOSE 80
# Mon, 20 Jul 2020 18:50:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Jul 2020 18:50:34 GMT
CMD ["traefik"]
# Mon, 20 Jul 2020 18:50:35 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a36cf46e6cb6a8028db7cb68482816e710935254a7d463897840713066cf5ba`  
		Last Modified: Thu, 23 Apr 2020 22:39:24 GMT  
		Size: 698.1 KB (698086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ee7c01f51a7c41cc870b283b66ccd0dee4dfc7e0e9c1ca957d73969dc26691`  
		Last Modified: Mon, 20 Jul 2020 18:51:19 GMT  
		Size: 20.3 MB (20345057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ca186cb1c339d1fd77800b7788583c0d6b0309bda439b921d497a6f2030dc`  
		Last Modified: Mon, 20 Jul 2020 18:51:11 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.2` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:ae6a9e07e0c03df672e5fe90ade2f5a56ea27f1f0e30e2a13bb49d8cbdc3e7c9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23423015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f69c73e81ebad70c08ca34291273b3a3b4bb3b4b5f9a5acbd9fc3433c157e19`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Jul 2020 19:47:40 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.7/traefik_v2.2.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Jul 2020 19:47:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Jul 2020 19:47:42 GMT
EXPOSE 80
# Mon, 20 Jul 2020 19:47:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Jul 2020 19:47:46 GMT
CMD ["traefik"]
# Mon, 20 Jul 2020 19:47:46 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff968af61b86e34dc2412293ade430f77b7db53f7f4adb925fec30d3ccbb2876`  
		Last Modified: Fri, 24 Apr 2020 12:43:42 GMT  
		Size: 696.1 KB (696058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2ba74a0f32fa0e26ecf336f6d70bc0d0a8a08a20062643dd9ac00bed14efa6`  
		Last Modified: Mon, 20 Jul 2020 19:48:27 GMT  
		Size: 20.0 MB (20002164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569fe01719a75603ca3d8c344ac5ec7d52199626d3240e48bf9e947a18b21810`  
		Last Modified: Mon, 20 Jul 2020 19:48:16 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.2.7`

```console
$ docker pull traefik@sha256:2dcdde75212d0117ef1360df5c532a2ec8bb97c386987b2bc66d973bca5003b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.2.7` - linux; amd64

```console
$ docker pull traefik@sha256:55f1b5e719c6e0f2d650e921463a87c8a4024236afb4991aea632df7ef942663
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25167013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de086c281ea7b4116c64a917309e249ae9063c663cd8e41c234bc54b88cfcd2c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Jul 2020 19:22:47 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.7/traefik_v2.2.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Jul 2020 19:22:47 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Jul 2020 19:22:47 GMT
EXPOSE 80
# Mon, 20 Jul 2020 19:22:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Jul 2020 19:22:48 GMT
CMD ["traefik"]
# Mon, 20 Jul 2020 19:22:48 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16506d32a25436b458a7f443ec1ca0d096d99d3479523c92c247856fc6148c0`  
		Last Modified: Fri, 24 Apr 2020 17:34:15 GMT  
		Size: 694.1 KB (694148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd583f1fc97ea2229f7e54f3b224e77b1b35f9e130dead096b58331b74427999`  
		Last Modified: Mon, 20 Jul 2020 19:23:12 GMT  
		Size: 21.7 MB (21659180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb2b75fe8e63b50ed1bb2728995b03b38ae981345ce246cececaf4384f5a9a1`  
		Last Modified: Mon, 20 Jul 2020 19:23:07 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.2.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:1dd33a92c9604ced7cfc03c9ad6653aa5d00a26a5e0a825f89ada10b052fb236
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.7 MB (23663447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41954059dfb2a60ecee9e006f90e5e8e9ec6d2174e65608e2518f801dc5df657`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Jul 2020 18:50:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.7/traefik_v2.2.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Jul 2020 18:50:32 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Jul 2020 18:50:32 GMT
EXPOSE 80
# Mon, 20 Jul 2020 18:50:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Jul 2020 18:50:34 GMT
CMD ["traefik"]
# Mon, 20 Jul 2020 18:50:35 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a36cf46e6cb6a8028db7cb68482816e710935254a7d463897840713066cf5ba`  
		Last Modified: Thu, 23 Apr 2020 22:39:24 GMT  
		Size: 698.1 KB (698086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ee7c01f51a7c41cc870b283b66ccd0dee4dfc7e0e9c1ca957d73969dc26691`  
		Last Modified: Mon, 20 Jul 2020 18:51:19 GMT  
		Size: 20.3 MB (20345057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ca186cb1c339d1fd77800b7788583c0d6b0309bda439b921d497a6f2030dc`  
		Last Modified: Mon, 20 Jul 2020 18:51:11 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.2.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:ae6a9e07e0c03df672e5fe90ade2f5a56ea27f1f0e30e2a13bb49d8cbdc3e7c9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23423015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f69c73e81ebad70c08ca34291273b3a3b4bb3b4b5f9a5acbd9fc3433c157e19`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Jul 2020 19:47:40 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.7/traefik_v2.2.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Jul 2020 19:47:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Jul 2020 19:47:42 GMT
EXPOSE 80
# Mon, 20 Jul 2020 19:47:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Jul 2020 19:47:46 GMT
CMD ["traefik"]
# Mon, 20 Jul 2020 19:47:46 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff968af61b86e34dc2412293ade430f77b7db53f7f4adb925fec30d3ccbb2876`  
		Last Modified: Fri, 24 Apr 2020 12:43:42 GMT  
		Size: 696.1 KB (696058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2ba74a0f32fa0e26ecf336f6d70bc0d0a8a08a20062643dd9ac00bed14efa6`  
		Last Modified: Mon, 20 Jul 2020 19:48:27 GMT  
		Size: 20.0 MB (20002164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569fe01719a75603ca3d8c344ac5ec7d52199626d3240e48bf9e947a18b21810`  
		Last Modified: Mon, 20 Jul 2020 19:48:16 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.2.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:fda8b53c30a901acfa91388660d2d85dfb77bcd49f7a3fe66d6d3c27c6710ac2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `traefik:v2.2.7-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull traefik@sha256:f3c6b74c8cee89d7dd612c1f545a67746f57cbddabe650718c0d3e91af5fbc5f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2340995387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6abec4b0661abb8b7e71d04e842c7bc38a5e9afad4991089c95c19107c611a1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 20 Jul 2020 19:15:37 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.2.7/traefik_v2.2.7_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 20 Jul 2020 19:15:39 GMT
EXPOSE 80
# Mon, 20 Jul 2020 19:15:40 GMT
ENTRYPOINT ["/traefik"]
# Mon, 20 Jul 2020 19:15:42 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0247512bb5646fd88951141a0338afcbabb2130655250cc3959d27438ef1fb`  
		Last Modified: Mon, 20 Jul 2020 19:16:17 GMT  
		Size: 30.8 MB (30798531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e1f70926eb835a5f2a15b7eb3a699976603074073a3ec7e8e693221740f56f`  
		Last Modified: Mon, 20 Jul 2020 19:16:10 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1821ea1f642148d720fd6f4cfe40d3383d8b12c6c85e8e3cddd726f8cfc8b2b1`  
		Last Modified: Mon, 20 Jul 2020 19:16:09 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a2388b729f036c4dbf707e9e9a283d3a27987b149789c94b0307c5502febd1`  
		Last Modified: Mon, 20 Jul 2020 19:16:09 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:fda8b53c30a901acfa91388660d2d85dfb77bcd49f7a3fe66d6d3c27c6710ac2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `traefik:v2.2-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull traefik@sha256:f3c6b74c8cee89d7dd612c1f545a67746f57cbddabe650718c0d3e91af5fbc5f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2340995387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6abec4b0661abb8b7e71d04e842c7bc38a5e9afad4991089c95c19107c611a1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 20 Jul 2020 19:15:37 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.2.7/traefik_v2.2.7_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 20 Jul 2020 19:15:39 GMT
EXPOSE 80
# Mon, 20 Jul 2020 19:15:40 GMT
ENTRYPOINT ["/traefik"]
# Mon, 20 Jul 2020 19:15:42 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0247512bb5646fd88951141a0338afcbabb2130655250cc3959d27438ef1fb`  
		Last Modified: Mon, 20 Jul 2020 19:16:17 GMT  
		Size: 30.8 MB (30798531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e1f70926eb835a5f2a15b7eb3a699976603074073a3ec7e8e693221740f56f`  
		Last Modified: Mon, 20 Jul 2020 19:16:10 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1821ea1f642148d720fd6f4cfe40d3383d8b12c6c85e8e3cddd726f8cfc8b2b1`  
		Last Modified: Mon, 20 Jul 2020 19:16:09 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a2388b729f036c4dbf707e9e9a283d3a27987b149789c94b0307c5502febd1`  
		Last Modified: Mon, 20 Jul 2020 19:16:09 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.3`

```console
$ docker pull traefik@sha256:b08601a937c1a160717e4ed6e0f4bc9ad0dea023de1ab309868cdf78164f9a33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.3` - linux; amd64

```console
$ docker pull traefik@sha256:b50cb55e6800df703f31b9a312d018558fc2286f829510f7da3de44a40aa74b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.9 MB (29942216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50a95f228e71630ffab61595fc050ce34c6013d6b9367440faef4e4f59d0e102`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:53:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc2/traefik_v2.3.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:53:34 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:53:34 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:53:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:53:35 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:53:35 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16506d32a25436b458a7f443ec1ca0d096d99d3479523c92c247856fc6148c0`  
		Last Modified: Fri, 24 Apr 2020 17:34:15 GMT  
		Size: 694.1 KB (694148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8f355ffe1c3315a63e73b1cb926b7f380eaa3ab4e9780add467a08709ef778`  
		Last Modified: Wed, 15 Jul 2020 23:54:29 GMT  
		Size: 26.4 MB (26434385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bdc521c6883d93f2893812825a3c6df9ac3959d1bf6c3ab800fcd311d8429a7`  
		Last Modified: Wed, 15 Jul 2020 23:54:24 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.3` - linux; arm variant v6

```console
$ docker pull traefik@sha256:09f2d34f7a32514f088d18ed0234527aeacd157d88187e115eed94c92db13e35
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.2 MB (28167652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab91012db5f2689da6b31247abefc6ca69082c5647a7f08b8439120169e69d9a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:04:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc2/traefik_v2.3.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:04:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:04:34 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:04:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:04:36 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:04:37 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a36cf46e6cb6a8028db7cb68482816e710935254a7d463897840713066cf5ba`  
		Last Modified: Thu, 23 Apr 2020 22:39:24 GMT  
		Size: 698.1 KB (698086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57bd030c3232794b6b0a553c8a0d9718f4c28235b71183f4ea6504924bd1782`  
		Last Modified: Wed, 15 Jul 2020 23:07:46 GMT  
		Size: 24.8 MB (24849262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eedc73b5df0ec289099eb44ad5b35b1b665275fb28bc869874f47e7f9279b9cd`  
		Last Modified: Wed, 15 Jul 2020 23:07:37 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.3` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:688de2b75dd901810244869b8bb7e3f6a437c9bef192be400d0dddc81a5e7606
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27751412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:982d3b3da00ee7a3fb892bcced519c84d83ba6a3a4e8969c30048e8291034812`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:23:55 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc2/traefik_v2.3.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:23:55 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:23:56 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:23:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:23:57 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:23:58 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff968af61b86e34dc2412293ade430f77b7db53f7f4adb925fec30d3ccbb2876`  
		Last Modified: Fri, 24 Apr 2020 12:43:42 GMT  
		Size: 696.1 KB (696058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974bdc9a43ec2151a237ff8d3b92d85e8b1a08d8f626c882203ca71b34e044ba`  
		Last Modified: Wed, 15 Jul 2020 23:31:05 GMT  
		Size: 24.3 MB (24330564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f12cd4c4b7843cbe81d3f484e87bf7e77cfaa32bbe47012036d2bb4956b79c`  
		Last Modified: Wed, 15 Jul 2020 23:30:57 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.3.0-rc2`

```console
$ docker pull traefik@sha256:b08601a937c1a160717e4ed6e0f4bc9ad0dea023de1ab309868cdf78164f9a33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.3.0-rc2` - linux; amd64

```console
$ docker pull traefik@sha256:b50cb55e6800df703f31b9a312d018558fc2286f829510f7da3de44a40aa74b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.9 MB (29942216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50a95f228e71630ffab61595fc050ce34c6013d6b9367440faef4e4f59d0e102`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:53:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc2/traefik_v2.3.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:53:34 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:53:34 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:53:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:53:35 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:53:35 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16506d32a25436b458a7f443ec1ca0d096d99d3479523c92c247856fc6148c0`  
		Last Modified: Fri, 24 Apr 2020 17:34:15 GMT  
		Size: 694.1 KB (694148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8f355ffe1c3315a63e73b1cb926b7f380eaa3ab4e9780add467a08709ef778`  
		Last Modified: Wed, 15 Jul 2020 23:54:29 GMT  
		Size: 26.4 MB (26434385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bdc521c6883d93f2893812825a3c6df9ac3959d1bf6c3ab800fcd311d8429a7`  
		Last Modified: Wed, 15 Jul 2020 23:54:24 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.3.0-rc2` - linux; arm variant v6

```console
$ docker pull traefik@sha256:09f2d34f7a32514f088d18ed0234527aeacd157d88187e115eed94c92db13e35
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.2 MB (28167652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab91012db5f2689da6b31247abefc6ca69082c5647a7f08b8439120169e69d9a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:04:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc2/traefik_v2.3.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:04:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:04:34 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:04:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:04:36 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:04:37 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a36cf46e6cb6a8028db7cb68482816e710935254a7d463897840713066cf5ba`  
		Last Modified: Thu, 23 Apr 2020 22:39:24 GMT  
		Size: 698.1 KB (698086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57bd030c3232794b6b0a553c8a0d9718f4c28235b71183f4ea6504924bd1782`  
		Last Modified: Wed, 15 Jul 2020 23:07:46 GMT  
		Size: 24.8 MB (24849262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eedc73b5df0ec289099eb44ad5b35b1b665275fb28bc869874f47e7f9279b9cd`  
		Last Modified: Wed, 15 Jul 2020 23:07:37 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.3.0-rc2` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:688de2b75dd901810244869b8bb7e3f6a437c9bef192be400d0dddc81a5e7606
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27751412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:982d3b3da00ee7a3fb892bcced519c84d83ba6a3a4e8969c30048e8291034812`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Jul 2020 23:23:55 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc2/traefik_v2.3.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Jul 2020 23:23:55 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Jul 2020 23:23:56 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:23:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 23:23:57 GMT
CMD ["traefik"]
# Wed, 15 Jul 2020 23:23:58 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff968af61b86e34dc2412293ade430f77b7db53f7f4adb925fec30d3ccbb2876`  
		Last Modified: Fri, 24 Apr 2020 12:43:42 GMT  
		Size: 696.1 KB (696058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974bdc9a43ec2151a237ff8d3b92d85e8b1a08d8f626c882203ca71b34e044ba`  
		Last Modified: Wed, 15 Jul 2020 23:31:05 GMT  
		Size: 24.3 MB (24330564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f12cd4c4b7843cbe81d3f484e87bf7e77cfaa32bbe47012036d2bb4956b79c`  
		Last Modified: Wed, 15 Jul 2020 23:30:57 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.3.0-rc2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e68058ecfa80e979dcc2fa6ee920bd8df2bcc50232d39143954f62218bf6a88f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `traefik:v2.3.0-rc2-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull traefik@sha256:67b2e308c494d95c2a4bc00dd3367211a36981bb8c696c129ebad6ac3deb2d77
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2345763886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db8373dbd0aa67ba8149ddd07eef0fbec138c15cfb827ca6b4bce35804560b7`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 23:16:31 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.3.0-rc2/traefik_v2.3.0-rc2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 15 Jul 2020 23:16:33 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:16:34 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jul 2020 23:16:36 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb18feaa7bac1bd3b44235da4df5a7b60d9f7ed0d1d73e947b8891cd7caab13`  
		Last Modified: Wed, 15 Jul 2020 23:18:36 GMT  
		Size: 35.6 MB (35567079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f48b12aa3c2e7f28108611083bb84e20d68ebc804f82c72e66bf021afdddb83`  
		Last Modified: Wed, 15 Jul 2020 23:18:28 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788fee2061a681b14cf194dc60865450f05989d62c90f7fa4de355b47d50ace9`  
		Last Modified: Wed, 15 Jul 2020 23:18:28 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd82bd8a7ea907d29fe22de2223c0a05f643dfbe5896ad97e51fed7f541ebde9`  
		Last Modified: Wed, 15 Jul 2020 23:18:28 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.3-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e68058ecfa80e979dcc2fa6ee920bd8df2bcc50232d39143954f62218bf6a88f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `traefik:v2.3-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull traefik@sha256:67b2e308c494d95c2a4bc00dd3367211a36981bb8c696c129ebad6ac3deb2d77
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2345763886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db8373dbd0aa67ba8149ddd07eef0fbec138c15cfb827ca6b4bce35804560b7`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 23:16:31 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.3.0-rc2/traefik_v2.3.0-rc2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 15 Jul 2020 23:16:33 GMT
EXPOSE 80
# Wed, 15 Jul 2020 23:16:34 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jul 2020 23:16:36 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb18feaa7bac1bd3b44235da4df5a7b60d9f7ed0d1d73e947b8891cd7caab13`  
		Last Modified: Wed, 15 Jul 2020 23:18:36 GMT  
		Size: 35.6 MB (35567079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f48b12aa3c2e7f28108611083bb84e20d68ebc804f82c72e66bf021afdddb83`  
		Last Modified: Wed, 15 Jul 2020 23:18:28 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788fee2061a681b14cf194dc60865450f05989d62c90f7fa4de355b47d50ace9`  
		Last Modified: Wed, 15 Jul 2020 23:18:28 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd82bd8a7ea907d29fe22de2223c0a05f643dfbe5896ad97e51fed7f541ebde9`  
		Last Modified: Wed, 15 Jul 2020 23:18:28 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:fda8b53c30a901acfa91388660d2d85dfb77bcd49f7a3fe66d6d3c27c6710ac2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull traefik@sha256:f3c6b74c8cee89d7dd612c1f545a67746f57cbddabe650718c0d3e91af5fbc5f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2340995387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6abec4b0661abb8b7e71d04e842c7bc38a5e9afad4991089c95c19107c611a1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 20 Jul 2020 19:15:37 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.2.7/traefik_v2.2.7_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 20 Jul 2020 19:15:39 GMT
EXPOSE 80
# Mon, 20 Jul 2020 19:15:40 GMT
ENTRYPOINT ["/traefik"]
# Mon, 20 Jul 2020 19:15:42 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0247512bb5646fd88951141a0338afcbabb2130655250cc3959d27438ef1fb`  
		Last Modified: Mon, 20 Jul 2020 19:16:17 GMT  
		Size: 30.8 MB (30798531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e1f70926eb835a5f2a15b7eb3a699976603074073a3ec7e8e693221740f56f`  
		Last Modified: Mon, 20 Jul 2020 19:16:10 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1821ea1f642148d720fd6f4cfe40d3383d8b12c6c85e8e3cddd726f8cfc8b2b1`  
		Last Modified: Mon, 20 Jul 2020 19:16:09 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a2388b729f036c4dbf707e9e9a283d3a27987b149789c94b0307c5502febd1`  
		Last Modified: Mon, 20 Jul 2020 19:16:09 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
