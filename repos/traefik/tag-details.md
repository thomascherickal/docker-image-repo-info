<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:1.7`](#traefik17)
-	[`traefik:1.7.26`](#traefik1726)
-	[`traefik:1.7.26-alpine`](#traefik1726-alpine)
-	[`traefik:1.7.26-windowsservercore-1809`](#traefik1726-windowsservercore-1809)
-	[`traefik:1.7-alpine`](#traefik17-alpine)
-	[`traefik:1.7-windowsservercore-1809`](#traefik17-windowsservercore-1809)
-	[`traefik:2.2`](#traefik22)
-	[`traefik:2.2.8`](#traefik228)
-	[`traefik:2.2.8-windowsservercore-1809`](#traefik228-windowsservercore-1809)
-	[`traefik:2.2-windowsservercore-1809`](#traefik22-windowsservercore-1809)
-	[`traefik:2.3`](#traefik23)
-	[`traefik:2.3.0-rc4`](#traefik230-rc4)
-	[`traefik:2.3.0-rc4-windowsservercore-1809`](#traefik230-rc4-windowsservercore-1809)
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
-	[`traefik:v1.7.26`](#traefikv1726)
-	[`traefik:v1.7.26-alpine`](#traefikv1726-alpine)
-	[`traefik:v1.7.26-windowsservercore-1809`](#traefikv1726-windowsservercore-1809)
-	[`traefik:v1.7-alpine`](#traefikv17-alpine)
-	[`traefik:v1.7-windowsservercore-1809`](#traefikv17-windowsservercore-1809)
-	[`traefik:v2.2`](#traefikv22)
-	[`traefik:v2.2.8`](#traefikv228)
-	[`traefik:v2.2.8-windowsservercore-1809`](#traefikv228-windowsservercore-1809)
-	[`traefik:v2.2-windowsservercore-1809`](#traefikv22-windowsservercore-1809)
-	[`traefik:v2.3`](#traefikv23)
-	[`traefik:v2.3.0-rc4`](#traefikv230-rc4)
-	[`traefik:v2.3.0-rc4-windowsservercore-1809`](#traefikv230-rc4-windowsservercore-1809)
-	[`traefik:v2.3-windowsservercore-1809`](#traefikv23-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:1.7`

```console
$ docker pull traefik@sha256:17067dcaa6b2fca1cf7b4aff8aee13ca55cb43a13e47645598567f9bd09ec128
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7` - linux; amd64

```console
$ docker pull traefik@sha256:3517b63d7a9cd49b7237882fb7c260589b58163c4082d3a37de55a0d93311718
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21585385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80ab7ee8304c003a86093c588d645758bfed1ac563263e12516c798014a4fc10`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 02:50:22 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 02:50:24 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 29 Jul 2020 00:20:43 GMT
COPY file:8e3cf7c133ac957e81d3eb831160ad827bfde058f356d7ac234b8c5ae307e37a in / 
# Wed, 29 Jul 2020 00:20:44 GMT
EXPOSE 80
# Wed, 29 Jul 2020 00:20:44 GMT
VOLUME [/tmp]
# Wed, 29 Jul 2020 00:20:44 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Jul 2020 00:20:44 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:8bcf82fc850436ad04fd66371e38f7611fe76a22b78f47f57ddb8908aa3d6001`  
		Last Modified: Wed, 29 Jul 2020 00:21:33 GMT  
		Size: 21.1 MB (21126327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:200bc13e0e03c532ea237fcc9f0c4f22416b91512a21c11cff0ecfa61a75d1f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20232026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c47b44829bfc497b7e5f3a9777a71f42e165db80fee23dcdb4de56014db3334e`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 03:46:16 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 03:46:17 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 28 Jul 2020 23:56:22 GMT
COPY file:a02ffe991352ee1f8abb077135ea9d27557e8b364fb712a42ccb2865e08df3cc in / 
# Tue, 28 Jul 2020 23:56:25 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:56:26 GMT
VOLUME [/tmp]
# Tue, 28 Jul 2020 23:56:27 GMT
ENTRYPOINT ["/traefik"]
# Tue, 28 Jul 2020 23:56:28 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:5b7ba63f15824a6daa3f73b57bd9fb04ea01b471f646b703dd08620f13e22d9c`  
		Last Modified: Tue, 28 Jul 2020 23:57:53 GMT  
		Size: 19.8 MB (19772940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:d46ed499e4b8c1c9dffea750abe7ad35fba0c431165a394e10283810d33b8d29
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.0 MB (19952059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b691bd363853ce10cedfbe29ea1e8d1e88d7e8eb01da6a3e1baa469c745a1302`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 05:55:25 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 05:55:26 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 29 Jul 2020 00:00:50 GMT
COPY file:f592954af2951d1a2538b1945366cb995f49638c7ef8b561b6961e0f8023197a in / 
# Wed, 29 Jul 2020 00:00:51 GMT
EXPOSE 80
# Wed, 29 Jul 2020 00:00:51 GMT
VOLUME [/tmp]
# Wed, 29 Jul 2020 00:00:52 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Jul 2020 00:00:53 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:fe3d477ed11470c756d1112d559be2ea65e2bbdcc367345ed45d17401a98474e`  
		Last Modified: Wed, 29 Jul 2020 00:02:17 GMT  
		Size: 19.5 MB (19492981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.26`

```console
$ docker pull traefik@sha256:17067dcaa6b2fca1cf7b4aff8aee13ca55cb43a13e47645598567f9bd09ec128
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.26` - linux; amd64

```console
$ docker pull traefik@sha256:3517b63d7a9cd49b7237882fb7c260589b58163c4082d3a37de55a0d93311718
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21585385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80ab7ee8304c003a86093c588d645758bfed1ac563263e12516c798014a4fc10`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 02:50:22 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 02:50:24 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 29 Jul 2020 00:20:43 GMT
COPY file:8e3cf7c133ac957e81d3eb831160ad827bfde058f356d7ac234b8c5ae307e37a in / 
# Wed, 29 Jul 2020 00:20:44 GMT
EXPOSE 80
# Wed, 29 Jul 2020 00:20:44 GMT
VOLUME [/tmp]
# Wed, 29 Jul 2020 00:20:44 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Jul 2020 00:20:44 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:8bcf82fc850436ad04fd66371e38f7611fe76a22b78f47f57ddb8908aa3d6001`  
		Last Modified: Wed, 29 Jul 2020 00:21:33 GMT  
		Size: 21.1 MB (21126327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.26` - linux; arm variant v6

```console
$ docker pull traefik@sha256:200bc13e0e03c532ea237fcc9f0c4f22416b91512a21c11cff0ecfa61a75d1f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20232026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c47b44829bfc497b7e5f3a9777a71f42e165db80fee23dcdb4de56014db3334e`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 03:46:16 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 03:46:17 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 28 Jul 2020 23:56:22 GMT
COPY file:a02ffe991352ee1f8abb077135ea9d27557e8b364fb712a42ccb2865e08df3cc in / 
# Tue, 28 Jul 2020 23:56:25 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:56:26 GMT
VOLUME [/tmp]
# Tue, 28 Jul 2020 23:56:27 GMT
ENTRYPOINT ["/traefik"]
# Tue, 28 Jul 2020 23:56:28 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:5b7ba63f15824a6daa3f73b57bd9fb04ea01b471f646b703dd08620f13e22d9c`  
		Last Modified: Tue, 28 Jul 2020 23:57:53 GMT  
		Size: 19.8 MB (19772940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.26` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:d46ed499e4b8c1c9dffea750abe7ad35fba0c431165a394e10283810d33b8d29
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.0 MB (19952059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b691bd363853ce10cedfbe29ea1e8d1e88d7e8eb01da6a3e1baa469c745a1302`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 05:55:25 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 05:55:26 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 29 Jul 2020 00:00:50 GMT
COPY file:f592954af2951d1a2538b1945366cb995f49638c7ef8b561b6961e0f8023197a in / 
# Wed, 29 Jul 2020 00:00:51 GMT
EXPOSE 80
# Wed, 29 Jul 2020 00:00:51 GMT
VOLUME [/tmp]
# Wed, 29 Jul 2020 00:00:52 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Jul 2020 00:00:53 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:fe3d477ed11470c756d1112d559be2ea65e2bbdcc367345ed45d17401a98474e`  
		Last Modified: Wed, 29 Jul 2020 00:02:17 GMT  
		Size: 19.5 MB (19492981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.26-alpine`

```console
$ docker pull traefik@sha256:0da45cd2c37ec826012e0f2d8a3a4ac0a7be4240a4942a6e40e3aae0f6fb205f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.26-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:3cbe9e62ef26a9ac17b25702754dfbf56dd346850170be90eabd370f24190ef1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24634355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c36f69007d987e4ed093711f4f306b52ce63b1c19f5ffacd49a1aea1f717e527`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Jul 2020 00:20:25 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Jul 2020 00:20:25 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Jul 2020 00:20:25 GMT
EXPOSE 80
# Wed, 29 Jul 2020 00:20:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Jul 2020 00:20:26 GMT
CMD ["traefik"]
# Wed, 29 Jul 2020 00:20:26 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:5bb03716fa366c58de14b0fc81a50daf51f39175c928558e3e82017b5999f233`  
		Last Modified: Wed, 29 Jul 2020 00:21:23 GMT  
		Size: 21.1 MB (21126524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c61f1414a3fbacefede004c9c340def8b1c393630a1c2241a0c9196692c574`  
		Last Modified: Wed, 29 Jul 2020 00:21:19 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.26-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:d77a05164ca7fbf64eb55feb97bd9e3d1dfaed181d23bc172d1602203b036b28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23091373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f84ddfeb559adfb1011610755afdd099c865a8de51b045331d848b1a58077bc6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 28 Jul 2020 23:51:46 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 28 Jul 2020 23:51:47 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 28 Jul 2020 23:51:48 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:51:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Jul 2020 23:51:52 GMT
CMD ["traefik"]
# Tue, 28 Jul 2020 23:51:55 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:bf46db6761515f08f18c5396f51c8d5fd2ae1c385ff5c12113336ffb79684420`  
		Last Modified: Tue, 28 Jul 2020 23:57:37 GMT  
		Size: 19.8 MB (19772984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0368cab0ca49479d26c28e4638f00e78884190c43adf25a35b647ffc70e1209f`  
		Last Modified: Tue, 28 Jul 2020 23:57:30 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.26-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7805105ced1b07c019cb3c420705bb105b1d8da381b76869db624e521af05592
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22913978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6548e0334e123554f38144482ac92954e0ed970de05727c2d7b6e371f0cda8f9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 28 Jul 2020 23:50:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 28 Jul 2020 23:50:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 28 Jul 2020 23:50:28 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:50:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Jul 2020 23:50:29 GMT
CMD ["traefik"]
# Tue, 28 Jul 2020 23:50:30 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:7f9ba2c08e62ba40494711c8f4e4d32d3d297940e5c04ceaa0594de58ced1744`  
		Last Modified: Wed, 29 Jul 2020 00:02:01 GMT  
		Size: 19.5 MB (19493128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3295e2c39b2f8f9a497a542502857a9b10a07977734f37c658f79d6e1a71c57b`  
		Last Modified: Wed, 29 Jul 2020 00:01:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.26-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f8f03683732d73c7d9a288627158d8f30579255aab4662d54201486e07a7f9dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `traefik:1.7.26-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull traefik@sha256:cd065335be88e46f537b005bcdd09e1c8eafeb1ad3674a12011635e30b5c8652
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2366139069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37b2f4d0fbf437493bbfd55b018ebf33649e751c25151ae05ff55009c5a70419`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:47:45 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 12 Aug 2020 18:47:47 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:47:48 GMT
ENTRYPOINT ["/traefik"]
# Wed, 12 Aug 2020 18:47:49 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298e1db6a0b5b538cab98a96f8c4650e4fccee26fb0e75f0582d210e0dc7af6d`  
		Last Modified: Wed, 12 Aug 2020 18:49:14 GMT  
		Size: 30.3 MB (30267520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699a7485ed05f7d7c0614726620e754f884bdd13f33bdd82cf017ede4c96a631`  
		Last Modified: Wed, 12 Aug 2020 18:49:06 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d222b7829a182578922580c28dbd3b0cd98374c8c5508b777df5d6a9e6763d0c`  
		Last Modified: Wed, 12 Aug 2020 18:49:06 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba55ff7183a9e35465c15ca0f795637c77bf77b5d338053acb7b5b1f05434e0`  
		Last Modified: Wed, 12 Aug 2020 18:49:06 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-alpine`

```console
$ docker pull traefik@sha256:0da45cd2c37ec826012e0f2d8a3a4ac0a7be4240a4942a6e40e3aae0f6fb205f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:3cbe9e62ef26a9ac17b25702754dfbf56dd346850170be90eabd370f24190ef1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24634355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c36f69007d987e4ed093711f4f306b52ce63b1c19f5ffacd49a1aea1f717e527`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Jul 2020 00:20:25 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Jul 2020 00:20:25 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Jul 2020 00:20:25 GMT
EXPOSE 80
# Wed, 29 Jul 2020 00:20:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Jul 2020 00:20:26 GMT
CMD ["traefik"]
# Wed, 29 Jul 2020 00:20:26 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:5bb03716fa366c58de14b0fc81a50daf51f39175c928558e3e82017b5999f233`  
		Last Modified: Wed, 29 Jul 2020 00:21:23 GMT  
		Size: 21.1 MB (21126524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c61f1414a3fbacefede004c9c340def8b1c393630a1c2241a0c9196692c574`  
		Last Modified: Wed, 29 Jul 2020 00:21:19 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:d77a05164ca7fbf64eb55feb97bd9e3d1dfaed181d23bc172d1602203b036b28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23091373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f84ddfeb559adfb1011610755afdd099c865a8de51b045331d848b1a58077bc6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 28 Jul 2020 23:51:46 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 28 Jul 2020 23:51:47 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 28 Jul 2020 23:51:48 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:51:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Jul 2020 23:51:52 GMT
CMD ["traefik"]
# Tue, 28 Jul 2020 23:51:55 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:bf46db6761515f08f18c5396f51c8d5fd2ae1c385ff5c12113336ffb79684420`  
		Last Modified: Tue, 28 Jul 2020 23:57:37 GMT  
		Size: 19.8 MB (19772984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0368cab0ca49479d26c28e4638f00e78884190c43adf25a35b647ffc70e1209f`  
		Last Modified: Tue, 28 Jul 2020 23:57:30 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7805105ced1b07c019cb3c420705bb105b1d8da381b76869db624e521af05592
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22913978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6548e0334e123554f38144482ac92954e0ed970de05727c2d7b6e371f0cda8f9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 28 Jul 2020 23:50:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 28 Jul 2020 23:50:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 28 Jul 2020 23:50:28 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:50:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Jul 2020 23:50:29 GMT
CMD ["traefik"]
# Tue, 28 Jul 2020 23:50:30 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:7f9ba2c08e62ba40494711c8f4e4d32d3d297940e5c04ceaa0594de58ced1744`  
		Last Modified: Wed, 29 Jul 2020 00:02:01 GMT  
		Size: 19.5 MB (19493128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3295e2c39b2f8f9a497a542502857a9b10a07977734f37c658f79d6e1a71c57b`  
		Last Modified: Wed, 29 Jul 2020 00:01:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f8f03683732d73c7d9a288627158d8f30579255aab4662d54201486e07a7f9dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `traefik:1.7-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull traefik@sha256:cd065335be88e46f537b005bcdd09e1c8eafeb1ad3674a12011635e30b5c8652
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2366139069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37b2f4d0fbf437493bbfd55b018ebf33649e751c25151ae05ff55009c5a70419`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:47:45 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 12 Aug 2020 18:47:47 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:47:48 GMT
ENTRYPOINT ["/traefik"]
# Wed, 12 Aug 2020 18:47:49 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298e1db6a0b5b538cab98a96f8c4650e4fccee26fb0e75f0582d210e0dc7af6d`  
		Last Modified: Wed, 12 Aug 2020 18:49:14 GMT  
		Size: 30.3 MB (30267520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699a7485ed05f7d7c0614726620e754f884bdd13f33bdd82cf017ede4c96a631`  
		Last Modified: Wed, 12 Aug 2020 18:49:06 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d222b7829a182578922580c28dbd3b0cd98374c8c5508b777df5d6a9e6763d0c`  
		Last Modified: Wed, 12 Aug 2020 18:49:06 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba55ff7183a9e35465c15ca0f795637c77bf77b5d338053acb7b5b1f05434e0`  
		Last Modified: Wed, 12 Aug 2020 18:49:06 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.2`

```console
$ docker pull traefik@sha256:f5af5a5ce17fc3e353b507e8acce65d7f28126408a8c92dc3cac246d023dc9e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.2` - linux; amd64

```console
$ docker pull traefik@sha256:2468d73cafe08a8973ac3d4e7d0163c1e86c36c8b1bc1f212fdf88999a799fb5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25167674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6e6fde072260f39a81ffcd1eaaa9e0f3aa8de874d1805a14e7315f0e19c344b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Jul 2020 00:20:17 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.8/traefik_v2.2.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Jul 2020 00:20:17 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Jul 2020 00:20:17 GMT
EXPOSE 80
# Wed, 29 Jul 2020 00:20:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Jul 2020 00:20:18 GMT
CMD ["traefik"]
# Wed, 29 Jul 2020 00:20:18 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:1f5ad3441e7363549035f66e706f206a0de236b858cf33c9cd9ff8dcdd18e1a7`  
		Last Modified: Wed, 29 Jul 2020 00:21:13 GMT  
		Size: 21.7 MB (21659842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636569b0d16cb280926eb5f6d661be7cb1d4476a31d45328398e644f07119b3c`  
		Last Modified: Wed, 29 Jul 2020 00:21:09 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.2` - linux; arm variant v6

```console
$ docker pull traefik@sha256:fa4de82729f8fccc89108cf8e8e23032173a461dd4b8a6a2f717be05254bce6c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.7 MB (23663705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8161e01e718ca849737d9eb3777995c1c86c0b8e361ddd66bf36bec4162f102`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 28 Jul 2020 23:51:19 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.8/traefik_v2.2.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 28 Jul 2020 23:51:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 28 Jul 2020 23:51:24 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:51:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Jul 2020 23:51:28 GMT
CMD ["traefik"]
# Tue, 28 Jul 2020 23:51:30 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9fd7ea12487aad43f479ff4ed630cfdcad68a675a840c616be0a8d9e6bbff967`  
		Last Modified: Tue, 28 Jul 2020 23:57:20 GMT  
		Size: 20.3 MB (20345315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a709b83326f37f60b72767971160e15dacb81aa1c252ad8d48d22a54fcaed7cf`  
		Last Modified: Tue, 28 Jul 2020 23:57:13 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.2` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9a56dab619dbd6617ce626f247bcb5f4c5c47b6b1a1c1c2d7ad1ffa842d1feaf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23422892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fb444508581ad8942228a15b26ae157f4624dc050768480e286472439499f40`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 28 Jul 2020 23:50:09 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.8/traefik_v2.2.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 28 Jul 2020 23:50:10 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 28 Jul 2020 23:50:12 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:50:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Jul 2020 23:50:13 GMT
CMD ["traefik"]
# Tue, 28 Jul 2020 23:50:14 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:04d6b3ba19b9cdbee340681e37ccbf55756f6547a8ea2176e084d2d38d900b43`  
		Last Modified: Wed, 29 Jul 2020 00:01:42 GMT  
		Size: 20.0 MB (20002042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5632834be9cd878f2629d7e53d9c353cad96bda6be58e6afcdab6fb8477bbd`  
		Last Modified: Wed, 29 Jul 2020 00:01:37 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.2.8`

```console
$ docker pull traefik@sha256:f5af5a5ce17fc3e353b507e8acce65d7f28126408a8c92dc3cac246d023dc9e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.2.8` - linux; amd64

```console
$ docker pull traefik@sha256:2468d73cafe08a8973ac3d4e7d0163c1e86c36c8b1bc1f212fdf88999a799fb5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25167674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6e6fde072260f39a81ffcd1eaaa9e0f3aa8de874d1805a14e7315f0e19c344b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Jul 2020 00:20:17 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.8/traefik_v2.2.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Jul 2020 00:20:17 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Jul 2020 00:20:17 GMT
EXPOSE 80
# Wed, 29 Jul 2020 00:20:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Jul 2020 00:20:18 GMT
CMD ["traefik"]
# Wed, 29 Jul 2020 00:20:18 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:1f5ad3441e7363549035f66e706f206a0de236b858cf33c9cd9ff8dcdd18e1a7`  
		Last Modified: Wed, 29 Jul 2020 00:21:13 GMT  
		Size: 21.7 MB (21659842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636569b0d16cb280926eb5f6d661be7cb1d4476a31d45328398e644f07119b3c`  
		Last Modified: Wed, 29 Jul 2020 00:21:09 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.2.8` - linux; arm variant v6

```console
$ docker pull traefik@sha256:fa4de82729f8fccc89108cf8e8e23032173a461dd4b8a6a2f717be05254bce6c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.7 MB (23663705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8161e01e718ca849737d9eb3777995c1c86c0b8e361ddd66bf36bec4162f102`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 28 Jul 2020 23:51:19 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.8/traefik_v2.2.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 28 Jul 2020 23:51:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 28 Jul 2020 23:51:24 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:51:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Jul 2020 23:51:28 GMT
CMD ["traefik"]
# Tue, 28 Jul 2020 23:51:30 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9fd7ea12487aad43f479ff4ed630cfdcad68a675a840c616be0a8d9e6bbff967`  
		Last Modified: Tue, 28 Jul 2020 23:57:20 GMT  
		Size: 20.3 MB (20345315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a709b83326f37f60b72767971160e15dacb81aa1c252ad8d48d22a54fcaed7cf`  
		Last Modified: Tue, 28 Jul 2020 23:57:13 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.2.8` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9a56dab619dbd6617ce626f247bcb5f4c5c47b6b1a1c1c2d7ad1ffa842d1feaf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23422892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fb444508581ad8942228a15b26ae157f4624dc050768480e286472439499f40`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 28 Jul 2020 23:50:09 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.8/traefik_v2.2.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 28 Jul 2020 23:50:10 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 28 Jul 2020 23:50:12 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:50:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Jul 2020 23:50:13 GMT
CMD ["traefik"]
# Tue, 28 Jul 2020 23:50:14 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:04d6b3ba19b9cdbee340681e37ccbf55756f6547a8ea2176e084d2d38d900b43`  
		Last Modified: Wed, 29 Jul 2020 00:01:42 GMT  
		Size: 20.0 MB (20002042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5632834be9cd878f2629d7e53d9c353cad96bda6be58e6afcdab6fb8477bbd`  
		Last Modified: Wed, 29 Jul 2020 00:01:37 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.2.8-windowsservercore-1809`

```console
$ docker pull traefik@sha256:cdc3dbe8b06277ebd96943b994a7cc23d2b9373e1e785276d64f82085219bf16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `traefik:2.2.8-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull traefik@sha256:a17b61b8c1e1d7573b98844eaec3a7f0c503d85f0705d3ab642585bbdc9d888a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2366658561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e061a005c81a3df8c7000f7c9ad6aecbe3761839b3adc998b9cb996776ba824`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:46:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.2.8/traefik_v2.2.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 12 Aug 2020 18:46:47 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:46:48 GMT
ENTRYPOINT ["/traefik"]
# Wed, 12 Aug 2020 18:46:49 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7698fba9396d0c8aabdaeb88d228a02d13fa7eccb8c50cc8ad141232de6d5d`  
		Last Modified: Wed, 12 Aug 2020 18:48:47 GMT  
		Size: 30.8 MB (30787030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70187a11409864df9161ffb451d7cb5cee8d45ce3aa9bf78a9ac1b8569d0513c`  
		Last Modified: Wed, 12 Aug 2020 18:48:40 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0acd47024a509c5b6df0032fae59357c838b124c17ea1d510d233a548fb58459`  
		Last Modified: Wed, 12 Aug 2020 18:48:39 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b66a39bbb90e279df94df561cd2e7c19ec45604bfcddce75254a78d67cf18a`  
		Last Modified: Wed, 12 Aug 2020 18:48:40 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:cdc3dbe8b06277ebd96943b994a7cc23d2b9373e1e785276d64f82085219bf16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `traefik:2.2-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull traefik@sha256:a17b61b8c1e1d7573b98844eaec3a7f0c503d85f0705d3ab642585bbdc9d888a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2366658561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e061a005c81a3df8c7000f7c9ad6aecbe3761839b3adc998b9cb996776ba824`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:46:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.2.8/traefik_v2.2.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 12 Aug 2020 18:46:47 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:46:48 GMT
ENTRYPOINT ["/traefik"]
# Wed, 12 Aug 2020 18:46:49 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7698fba9396d0c8aabdaeb88d228a02d13fa7eccb8c50cc8ad141232de6d5d`  
		Last Modified: Wed, 12 Aug 2020 18:48:47 GMT  
		Size: 30.8 MB (30787030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70187a11409864df9161ffb451d7cb5cee8d45ce3aa9bf78a9ac1b8569d0513c`  
		Last Modified: Wed, 12 Aug 2020 18:48:40 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0acd47024a509c5b6df0032fae59357c838b124c17ea1d510d233a548fb58459`  
		Last Modified: Wed, 12 Aug 2020 18:48:39 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b66a39bbb90e279df94df561cd2e7c19ec45604bfcddce75254a78d67cf18a`  
		Last Modified: Wed, 12 Aug 2020 18:48:40 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.3`

```console
$ docker pull traefik@sha256:302e1214da614f62b8cdc930daf285bc9d8165ac15e0953309161de06a589fb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.3` - linux; amd64

```console
$ docker pull traefik@sha256:3f5c5a46ccff636a9e726961f123638bd6854191040072d860fc15bbcee3e184
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28052206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:926633bd017b112d1ee29780353bd3898e2f5f4a3b4749e8c4070ab765708bc4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 19 Aug 2020 21:12:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc4/traefik_v2.3.0-rc4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 19 Aug 2020 21:12:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 19 Aug 2020 21:12:05 GMT
EXPOSE 80
# Wed, 19 Aug 2020 21:12:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Aug 2020 21:12:05 GMT
CMD ["traefik"]
# Wed, 19 Aug 2020 21:12:05 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:8843362db2d6c7cba5a5ac00938528154d1b876fe944ae136e0c6cd5d390e4f4`  
		Last Modified: Wed, 19 Aug 2020 21:12:38 GMT  
		Size: 24.5 MB (24544374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685edc151199f805d0e1910cd68e68161fbc81369caf76102ebed3176760a338`  
		Last Modified: Wed, 19 Aug 2020 21:12:32 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.3` - linux; arm variant v6

```console
$ docker pull traefik@sha256:c85e11c5d0332ddc75b8a70c5fcd19540794ae68a86df0fb7c957fec76074a65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.2 MB (26178413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f6d814c93b2dcc172081103002e7c5ff94bd1b8fec1210b28caca91353fdb66`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 19 Aug 2020 21:04:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc4/traefik_v2.3.0-rc4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 19 Aug 2020 21:04:07 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 19 Aug 2020 21:04:09 GMT
EXPOSE 80
# Wed, 19 Aug 2020 21:04:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Aug 2020 21:04:12 GMT
CMD ["traefik"]
# Wed, 19 Aug 2020 21:04:15 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:a2d52f51ca6c71d0c3f5144f84c3099bd4831769fa83c8d072c6b67b89c61321`  
		Last Modified: Wed, 19 Aug 2020 21:04:59 GMT  
		Size: 22.9 MB (22860023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6497bf20f1fdcc8800a01dd9f26e77ac3f1236f6627bbd64100ec7926f84e2c2`  
		Last Modified: Wed, 19 Aug 2020 21:04:52 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.3` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:14b29b6c8bd7c722e1dd0e06f9f0a7e37db3a5d8467496cfde55b13073656702
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27754805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bce20c5287082213e632bc7034a39e3e84efd677922b395fd4c5d13843dfa62`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 28 Jul 2020 23:49:54 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc3/traefik_v2.3.0-rc3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 28 Jul 2020 23:49:55 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 28 Jul 2020 23:49:56 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:49:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Jul 2020 23:49:57 GMT
CMD ["traefik"]
# Tue, 28 Jul 2020 23:49:58 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b32d16371e8f6c49f7eb4c9ae55be6a35d152399c37508b5a81eb631bdd0f182`  
		Last Modified: Wed, 29 Jul 2020 00:01:25 GMT  
		Size: 24.3 MB (24333955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3bbea951e4557c6db83dc8f3fa25298592630e9292fe53c8f4ebcadce74658b`  
		Last Modified: Wed, 29 Jul 2020 00:01:18 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.3.0-rc4`

```console
$ docker pull traefik@sha256:587a1920014de5051d3dbeefc6eb0f9d4162dd4d485778fe3a2926f1e3b25d05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6

### `traefik:2.3.0-rc4` - linux; amd64

```console
$ docker pull traefik@sha256:3f5c5a46ccff636a9e726961f123638bd6854191040072d860fc15bbcee3e184
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28052206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:926633bd017b112d1ee29780353bd3898e2f5f4a3b4749e8c4070ab765708bc4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 19 Aug 2020 21:12:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc4/traefik_v2.3.0-rc4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 19 Aug 2020 21:12:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 19 Aug 2020 21:12:05 GMT
EXPOSE 80
# Wed, 19 Aug 2020 21:12:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Aug 2020 21:12:05 GMT
CMD ["traefik"]
# Wed, 19 Aug 2020 21:12:05 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:8843362db2d6c7cba5a5ac00938528154d1b876fe944ae136e0c6cd5d390e4f4`  
		Last Modified: Wed, 19 Aug 2020 21:12:38 GMT  
		Size: 24.5 MB (24544374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685edc151199f805d0e1910cd68e68161fbc81369caf76102ebed3176760a338`  
		Last Modified: Wed, 19 Aug 2020 21:12:32 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.3.0-rc4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:c85e11c5d0332ddc75b8a70c5fcd19540794ae68a86df0fb7c957fec76074a65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.2 MB (26178413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f6d814c93b2dcc172081103002e7c5ff94bd1b8fec1210b28caca91353fdb66`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 19 Aug 2020 21:04:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc4/traefik_v2.3.0-rc4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 19 Aug 2020 21:04:07 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 19 Aug 2020 21:04:09 GMT
EXPOSE 80
# Wed, 19 Aug 2020 21:04:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Aug 2020 21:04:12 GMT
CMD ["traefik"]
# Wed, 19 Aug 2020 21:04:15 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:a2d52f51ca6c71d0c3f5144f84c3099bd4831769fa83c8d072c6b67b89c61321`  
		Last Modified: Wed, 19 Aug 2020 21:04:59 GMT  
		Size: 22.9 MB (22860023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6497bf20f1fdcc8800a01dd9f26e77ac3f1236f6627bbd64100ec7926f84e2c2`  
		Last Modified: Wed, 19 Aug 2020 21:04:52 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.3.0-rc4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:5c9e5afb0e7accad59b5f89929d130a728a8fbcd78c6d7d3e676a7c091d2c942
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `traefik:2.3.0-rc4-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull traefik@sha256:19d714a6298146cab0bf90c4909d2e6addc448b76539b8f6653737c41380ce61
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2369930817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0193116892fbe1dd8a1a7327fb2197ef5d1e6728bb04c6ce6846064f1375fe63`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 19 Aug 2020 20:16:01 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.3.0-rc4/traefik_v2.3.0-rc4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 19 Aug 2020 20:16:02 GMT
EXPOSE 80
# Wed, 19 Aug 2020 20:16:03 GMT
ENTRYPOINT ["/traefik"]
# Wed, 19 Aug 2020 20:16:04 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4b935273c9edf14dff5895c90155812d7052eb98cdde597989fb945e41a600`  
		Last Modified: Wed, 19 Aug 2020 20:16:51 GMT  
		Size: 34.1 MB (34059255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982afb2946804976c1bbfe8b800b61fce8c6b9ec3bd9bb7951c013285b70d035`  
		Last Modified: Wed, 19 Aug 2020 20:16:43 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b41b5d9e95faa94a24fc8746bcf52d32b83a2c0199bd871711259bd69287298`  
		Last Modified: Wed, 19 Aug 2020 20:16:43 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e22963c3d8d4509fa45f3351a0348edcfd1dbbdb3502373ef7feed8503ca96`  
		Last Modified: Wed, 19 Aug 2020 20:16:43 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.3-windowsservercore-1809`

```console
$ docker pull traefik@sha256:5c9e5afb0e7accad59b5f89929d130a728a8fbcd78c6d7d3e676a7c091d2c942
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `traefik:2.3-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull traefik@sha256:19d714a6298146cab0bf90c4909d2e6addc448b76539b8f6653737c41380ce61
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2369930817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0193116892fbe1dd8a1a7327fb2197ef5d1e6728bb04c6ce6846064f1375fe63`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 19 Aug 2020 20:16:01 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.3.0-rc4/traefik_v2.3.0-rc4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 19 Aug 2020 20:16:02 GMT
EXPOSE 80
# Wed, 19 Aug 2020 20:16:03 GMT
ENTRYPOINT ["/traefik"]
# Wed, 19 Aug 2020 20:16:04 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4b935273c9edf14dff5895c90155812d7052eb98cdde597989fb945e41a600`  
		Last Modified: Wed, 19 Aug 2020 20:16:51 GMT  
		Size: 34.1 MB (34059255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982afb2946804976c1bbfe8b800b61fce8c6b9ec3bd9bb7951c013285b70d035`  
		Last Modified: Wed, 19 Aug 2020 20:16:43 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b41b5d9e95faa94a24fc8746bcf52d32b83a2c0199bd871711259bd69287298`  
		Last Modified: Wed, 19 Aug 2020 20:16:43 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e22963c3d8d4509fa45f3351a0348edcfd1dbbdb3502373ef7feed8503ca96`  
		Last Modified: Wed, 19 Aug 2020 20:16:43 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:chevrotin`

```console
$ docker pull traefik@sha256:f5af5a5ce17fc3e353b507e8acce65d7f28126408a8c92dc3cac246d023dc9e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:chevrotin` - linux; amd64

```console
$ docker pull traefik@sha256:2468d73cafe08a8973ac3d4e7d0163c1e86c36c8b1bc1f212fdf88999a799fb5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25167674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6e6fde072260f39a81ffcd1eaaa9e0f3aa8de874d1805a14e7315f0e19c344b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Jul 2020 00:20:17 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.8/traefik_v2.2.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Jul 2020 00:20:17 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Jul 2020 00:20:17 GMT
EXPOSE 80
# Wed, 29 Jul 2020 00:20:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Jul 2020 00:20:18 GMT
CMD ["traefik"]
# Wed, 29 Jul 2020 00:20:18 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:1f5ad3441e7363549035f66e706f206a0de236b858cf33c9cd9ff8dcdd18e1a7`  
		Last Modified: Wed, 29 Jul 2020 00:21:13 GMT  
		Size: 21.7 MB (21659842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636569b0d16cb280926eb5f6d661be7cb1d4476a31d45328398e644f07119b3c`  
		Last Modified: Wed, 29 Jul 2020 00:21:09 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:chevrotin` - linux; arm variant v6

```console
$ docker pull traefik@sha256:fa4de82729f8fccc89108cf8e8e23032173a461dd4b8a6a2f717be05254bce6c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.7 MB (23663705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8161e01e718ca849737d9eb3777995c1c86c0b8e361ddd66bf36bec4162f102`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 28 Jul 2020 23:51:19 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.8/traefik_v2.2.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 28 Jul 2020 23:51:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 28 Jul 2020 23:51:24 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:51:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Jul 2020 23:51:28 GMT
CMD ["traefik"]
# Tue, 28 Jul 2020 23:51:30 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9fd7ea12487aad43f479ff4ed630cfdcad68a675a840c616be0a8d9e6bbff967`  
		Last Modified: Tue, 28 Jul 2020 23:57:20 GMT  
		Size: 20.3 MB (20345315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a709b83326f37f60b72767971160e15dacb81aa1c252ad8d48d22a54fcaed7cf`  
		Last Modified: Tue, 28 Jul 2020 23:57:13 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:chevrotin` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9a56dab619dbd6617ce626f247bcb5f4c5c47b6b1a1c1c2d7ad1ffa842d1feaf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23422892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fb444508581ad8942228a15b26ae157f4624dc050768480e286472439499f40`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 28 Jul 2020 23:50:09 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.8/traefik_v2.2.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 28 Jul 2020 23:50:10 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 28 Jul 2020 23:50:12 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:50:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Jul 2020 23:50:13 GMT
CMD ["traefik"]
# Tue, 28 Jul 2020 23:50:14 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:04d6b3ba19b9cdbee340681e37ccbf55756f6547a8ea2176e084d2d38d900b43`  
		Last Modified: Wed, 29 Jul 2020 00:01:42 GMT  
		Size: 20.0 MB (20002042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5632834be9cd878f2629d7e53d9c353cad96bda6be58e6afcdab6fb8477bbd`  
		Last Modified: Wed, 29 Jul 2020 00:01:37 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:chevrotin-windowsservercore-1809`

```console
$ docker pull traefik@sha256:cdc3dbe8b06277ebd96943b994a7cc23d2b9373e1e785276d64f82085219bf16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `traefik:chevrotin-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull traefik@sha256:a17b61b8c1e1d7573b98844eaec3a7f0c503d85f0705d3ab642585bbdc9d888a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2366658561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e061a005c81a3df8c7000f7c9ad6aecbe3761839b3adc998b9cb996776ba824`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:46:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.2.8/traefik_v2.2.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 12 Aug 2020 18:46:47 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:46:48 GMT
ENTRYPOINT ["/traefik"]
# Wed, 12 Aug 2020 18:46:49 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7698fba9396d0c8aabdaeb88d228a02d13fa7eccb8c50cc8ad141232de6d5d`  
		Last Modified: Wed, 12 Aug 2020 18:48:47 GMT  
		Size: 30.8 MB (30787030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70187a11409864df9161ffb451d7cb5cee8d45ce3aa9bf78a9ac1b8569d0513c`  
		Last Modified: Wed, 12 Aug 2020 18:48:40 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0acd47024a509c5b6df0032fae59357c838b124c17ea1d510d233a548fb58459`  
		Last Modified: Wed, 12 Aug 2020 18:48:39 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b66a39bbb90e279df94df561cd2e7c19ec45604bfcddce75254a78d67cf18a`  
		Last Modified: Wed, 12 Aug 2020 18:48:40 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:f5af5a5ce17fc3e353b507e8acce65d7f28126408a8c92dc3cac246d023dc9e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:2468d73cafe08a8973ac3d4e7d0163c1e86c36c8b1bc1f212fdf88999a799fb5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25167674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6e6fde072260f39a81ffcd1eaaa9e0f3aa8de874d1805a14e7315f0e19c344b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Jul 2020 00:20:17 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.8/traefik_v2.2.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Jul 2020 00:20:17 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Jul 2020 00:20:17 GMT
EXPOSE 80
# Wed, 29 Jul 2020 00:20:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Jul 2020 00:20:18 GMT
CMD ["traefik"]
# Wed, 29 Jul 2020 00:20:18 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:1f5ad3441e7363549035f66e706f206a0de236b858cf33c9cd9ff8dcdd18e1a7`  
		Last Modified: Wed, 29 Jul 2020 00:21:13 GMT  
		Size: 21.7 MB (21659842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636569b0d16cb280926eb5f6d661be7cb1d4476a31d45328398e644f07119b3c`  
		Last Modified: Wed, 29 Jul 2020 00:21:09 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:fa4de82729f8fccc89108cf8e8e23032173a461dd4b8a6a2f717be05254bce6c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.7 MB (23663705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8161e01e718ca849737d9eb3777995c1c86c0b8e361ddd66bf36bec4162f102`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 28 Jul 2020 23:51:19 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.8/traefik_v2.2.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 28 Jul 2020 23:51:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 28 Jul 2020 23:51:24 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:51:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Jul 2020 23:51:28 GMT
CMD ["traefik"]
# Tue, 28 Jul 2020 23:51:30 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9fd7ea12487aad43f479ff4ed630cfdcad68a675a840c616be0a8d9e6bbff967`  
		Last Modified: Tue, 28 Jul 2020 23:57:20 GMT  
		Size: 20.3 MB (20345315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a709b83326f37f60b72767971160e15dacb81aa1c252ad8d48d22a54fcaed7cf`  
		Last Modified: Tue, 28 Jul 2020 23:57:13 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9a56dab619dbd6617ce626f247bcb5f4c5c47b6b1a1c1c2d7ad1ffa842d1feaf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23422892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fb444508581ad8942228a15b26ae157f4624dc050768480e286472439499f40`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 28 Jul 2020 23:50:09 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.8/traefik_v2.2.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 28 Jul 2020 23:50:10 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 28 Jul 2020 23:50:12 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:50:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Jul 2020 23:50:13 GMT
CMD ["traefik"]
# Tue, 28 Jul 2020 23:50:14 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:04d6b3ba19b9cdbee340681e37ccbf55756f6547a8ea2176e084d2d38d900b43`  
		Last Modified: Wed, 29 Jul 2020 00:01:42 GMT  
		Size: 20.0 MB (20002042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5632834be9cd878f2629d7e53d9c353cad96bda6be58e6afcdab6fb8477bbd`  
		Last Modified: Wed, 29 Jul 2020 00:01:37 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles`

```console
$ docker pull traefik@sha256:17067dcaa6b2fca1cf7b4aff8aee13ca55cb43a13e47645598567f9bd09ec128
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles` - linux; amd64

```console
$ docker pull traefik@sha256:3517b63d7a9cd49b7237882fb7c260589b58163c4082d3a37de55a0d93311718
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21585385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80ab7ee8304c003a86093c588d645758bfed1ac563263e12516c798014a4fc10`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 02:50:22 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 02:50:24 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 29 Jul 2020 00:20:43 GMT
COPY file:8e3cf7c133ac957e81d3eb831160ad827bfde058f356d7ac234b8c5ae307e37a in / 
# Wed, 29 Jul 2020 00:20:44 GMT
EXPOSE 80
# Wed, 29 Jul 2020 00:20:44 GMT
VOLUME [/tmp]
# Wed, 29 Jul 2020 00:20:44 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Jul 2020 00:20:44 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:8bcf82fc850436ad04fd66371e38f7611fe76a22b78f47f57ddb8908aa3d6001`  
		Last Modified: Wed, 29 Jul 2020 00:21:33 GMT  
		Size: 21.1 MB (21126327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm variant v6

```console
$ docker pull traefik@sha256:200bc13e0e03c532ea237fcc9f0c4f22416b91512a21c11cff0ecfa61a75d1f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20232026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c47b44829bfc497b7e5f3a9777a71f42e165db80fee23dcdb4de56014db3334e`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 03:46:16 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 03:46:17 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 28 Jul 2020 23:56:22 GMT
COPY file:a02ffe991352ee1f8abb077135ea9d27557e8b364fb712a42ccb2865e08df3cc in / 
# Tue, 28 Jul 2020 23:56:25 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:56:26 GMT
VOLUME [/tmp]
# Tue, 28 Jul 2020 23:56:27 GMT
ENTRYPOINT ["/traefik"]
# Tue, 28 Jul 2020 23:56:28 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:5b7ba63f15824a6daa3f73b57bd9fb04ea01b471f646b703dd08620f13e22d9c`  
		Last Modified: Tue, 28 Jul 2020 23:57:53 GMT  
		Size: 19.8 MB (19772940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:d46ed499e4b8c1c9dffea750abe7ad35fba0c431165a394e10283810d33b8d29
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.0 MB (19952059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b691bd363853ce10cedfbe29ea1e8d1e88d7e8eb01da6a3e1baa469c745a1302`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 05:55:25 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 05:55:26 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 29 Jul 2020 00:00:50 GMT
COPY file:f592954af2951d1a2538b1945366cb995f49638c7ef8b561b6961e0f8023197a in / 
# Wed, 29 Jul 2020 00:00:51 GMT
EXPOSE 80
# Wed, 29 Jul 2020 00:00:51 GMT
VOLUME [/tmp]
# Wed, 29 Jul 2020 00:00:52 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Jul 2020 00:00:53 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:fe3d477ed11470c756d1112d559be2ea65e2bbdcc367345ed45d17401a98474e`  
		Last Modified: Wed, 29 Jul 2020 00:02:17 GMT  
		Size: 19.5 MB (19492981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-alpine`

```console
$ docker pull traefik@sha256:0da45cd2c37ec826012e0f2d8a3a4ac0a7be4240a4942a6e40e3aae0f6fb205f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:3cbe9e62ef26a9ac17b25702754dfbf56dd346850170be90eabd370f24190ef1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24634355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c36f69007d987e4ed093711f4f306b52ce63b1c19f5ffacd49a1aea1f717e527`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Jul 2020 00:20:25 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Jul 2020 00:20:25 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Jul 2020 00:20:25 GMT
EXPOSE 80
# Wed, 29 Jul 2020 00:20:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Jul 2020 00:20:26 GMT
CMD ["traefik"]
# Wed, 29 Jul 2020 00:20:26 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:5bb03716fa366c58de14b0fc81a50daf51f39175c928558e3e82017b5999f233`  
		Last Modified: Wed, 29 Jul 2020 00:21:23 GMT  
		Size: 21.1 MB (21126524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c61f1414a3fbacefede004c9c340def8b1c393630a1c2241a0c9196692c574`  
		Last Modified: Wed, 29 Jul 2020 00:21:19 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:d77a05164ca7fbf64eb55feb97bd9e3d1dfaed181d23bc172d1602203b036b28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23091373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f84ddfeb559adfb1011610755afdd099c865a8de51b045331d848b1a58077bc6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 28 Jul 2020 23:51:46 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 28 Jul 2020 23:51:47 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 28 Jul 2020 23:51:48 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:51:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Jul 2020 23:51:52 GMT
CMD ["traefik"]
# Tue, 28 Jul 2020 23:51:55 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:bf46db6761515f08f18c5396f51c8d5fd2ae1c385ff5c12113336ffb79684420`  
		Last Modified: Tue, 28 Jul 2020 23:57:37 GMT  
		Size: 19.8 MB (19772984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0368cab0ca49479d26c28e4638f00e78884190c43adf25a35b647ffc70e1209f`  
		Last Modified: Tue, 28 Jul 2020 23:57:30 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7805105ced1b07c019cb3c420705bb105b1d8da381b76869db624e521af05592
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22913978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6548e0334e123554f38144482ac92954e0ed970de05727c2d7b6e371f0cda8f9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 28 Jul 2020 23:50:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 28 Jul 2020 23:50:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 28 Jul 2020 23:50:28 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:50:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Jul 2020 23:50:29 GMT
CMD ["traefik"]
# Tue, 28 Jul 2020 23:50:30 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:7f9ba2c08e62ba40494711c8f4e4d32d3d297940e5c04ceaa0594de58ced1744`  
		Last Modified: Wed, 29 Jul 2020 00:02:01 GMT  
		Size: 19.5 MB (19493128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3295e2c39b2f8f9a497a542502857a9b10a07977734f37c658f79d6e1a71c57b`  
		Last Modified: Wed, 29 Jul 2020 00:01:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f8f03683732d73c7d9a288627158d8f30579255aab4662d54201486e07a7f9dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull traefik@sha256:cd065335be88e46f537b005bcdd09e1c8eafeb1ad3674a12011635e30b5c8652
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2366139069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37b2f4d0fbf437493bbfd55b018ebf33649e751c25151ae05ff55009c5a70419`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:47:45 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 12 Aug 2020 18:47:47 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:47:48 GMT
ENTRYPOINT ["/traefik"]
# Wed, 12 Aug 2020 18:47:49 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298e1db6a0b5b538cab98a96f8c4650e4fccee26fb0e75f0582d210e0dc7af6d`  
		Last Modified: Wed, 12 Aug 2020 18:49:14 GMT  
		Size: 30.3 MB (30267520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699a7485ed05f7d7c0614726620e754f884bdd13f33bdd82cf017ede4c96a631`  
		Last Modified: Wed, 12 Aug 2020 18:49:06 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d222b7829a182578922580c28dbd3b0cd98374c8c5508b777df5d6a9e6763d0c`  
		Last Modified: Wed, 12 Aug 2020 18:49:06 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba55ff7183a9e35465c15ca0f795637c77bf77b5d338053acb7b5b1f05434e0`  
		Last Modified: Wed, 12 Aug 2020 18:49:06 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:picodon`

```console
$ docker pull traefik@sha256:302e1214da614f62b8cdc930daf285bc9d8165ac15e0953309161de06a589fb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:picodon` - linux; amd64

```console
$ docker pull traefik@sha256:3f5c5a46ccff636a9e726961f123638bd6854191040072d860fc15bbcee3e184
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28052206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:926633bd017b112d1ee29780353bd3898e2f5f4a3b4749e8c4070ab765708bc4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 19 Aug 2020 21:12:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc4/traefik_v2.3.0-rc4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 19 Aug 2020 21:12:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 19 Aug 2020 21:12:05 GMT
EXPOSE 80
# Wed, 19 Aug 2020 21:12:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Aug 2020 21:12:05 GMT
CMD ["traefik"]
# Wed, 19 Aug 2020 21:12:05 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:8843362db2d6c7cba5a5ac00938528154d1b876fe944ae136e0c6cd5d390e4f4`  
		Last Modified: Wed, 19 Aug 2020 21:12:38 GMT  
		Size: 24.5 MB (24544374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685edc151199f805d0e1910cd68e68161fbc81369caf76102ebed3176760a338`  
		Last Modified: Wed, 19 Aug 2020 21:12:32 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:picodon` - linux; arm variant v6

```console
$ docker pull traefik@sha256:c85e11c5d0332ddc75b8a70c5fcd19540794ae68a86df0fb7c957fec76074a65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.2 MB (26178413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f6d814c93b2dcc172081103002e7c5ff94bd1b8fec1210b28caca91353fdb66`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 19 Aug 2020 21:04:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc4/traefik_v2.3.0-rc4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 19 Aug 2020 21:04:07 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 19 Aug 2020 21:04:09 GMT
EXPOSE 80
# Wed, 19 Aug 2020 21:04:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Aug 2020 21:04:12 GMT
CMD ["traefik"]
# Wed, 19 Aug 2020 21:04:15 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:a2d52f51ca6c71d0c3f5144f84c3099bd4831769fa83c8d072c6b67b89c61321`  
		Last Modified: Wed, 19 Aug 2020 21:04:59 GMT  
		Size: 22.9 MB (22860023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6497bf20f1fdcc8800a01dd9f26e77ac3f1236f6627bbd64100ec7926f84e2c2`  
		Last Modified: Wed, 19 Aug 2020 21:04:52 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:picodon` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:14b29b6c8bd7c722e1dd0e06f9f0a7e37db3a5d8467496cfde55b13073656702
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27754805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bce20c5287082213e632bc7034a39e3e84efd677922b395fd4c5d13843dfa62`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 28 Jul 2020 23:49:54 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc3/traefik_v2.3.0-rc3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 28 Jul 2020 23:49:55 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 28 Jul 2020 23:49:56 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:49:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Jul 2020 23:49:57 GMT
CMD ["traefik"]
# Tue, 28 Jul 2020 23:49:58 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b32d16371e8f6c49f7eb4c9ae55be6a35d152399c37508b5a81eb631bdd0f182`  
		Last Modified: Wed, 29 Jul 2020 00:01:25 GMT  
		Size: 24.3 MB (24333955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3bbea951e4557c6db83dc8f3fa25298592630e9292fe53c8f4ebcadce74658b`  
		Last Modified: Wed, 29 Jul 2020 00:01:18 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:picodon-windowsservercore-1809`

```console
$ docker pull traefik@sha256:5c9e5afb0e7accad59b5f89929d130a728a8fbcd78c6d7d3e676a7c091d2c942
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `traefik:picodon-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull traefik@sha256:19d714a6298146cab0bf90c4909d2e6addc448b76539b8f6653737c41380ce61
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2369930817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0193116892fbe1dd8a1a7327fb2197ef5d1e6728bb04c6ce6846064f1375fe63`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 19 Aug 2020 20:16:01 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.3.0-rc4/traefik_v2.3.0-rc4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 19 Aug 2020 20:16:02 GMT
EXPOSE 80
# Wed, 19 Aug 2020 20:16:03 GMT
ENTRYPOINT ["/traefik"]
# Wed, 19 Aug 2020 20:16:04 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4b935273c9edf14dff5895c90155812d7052eb98cdde597989fb945e41a600`  
		Last Modified: Wed, 19 Aug 2020 20:16:51 GMT  
		Size: 34.1 MB (34059255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982afb2946804976c1bbfe8b800b61fce8c6b9ec3bd9bb7951c013285b70d035`  
		Last Modified: Wed, 19 Aug 2020 20:16:43 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b41b5d9e95faa94a24fc8746bcf52d32b83a2c0199bd871711259bd69287298`  
		Last Modified: Wed, 19 Aug 2020 20:16:43 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e22963c3d8d4509fa45f3351a0348edcfd1dbbdb3502373ef7feed8503ca96`  
		Last Modified: Wed, 19 Aug 2020 20:16:43 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7`

```console
$ docker pull traefik@sha256:17067dcaa6b2fca1cf7b4aff8aee13ca55cb43a13e47645598567f9bd09ec128
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7` - linux; amd64

```console
$ docker pull traefik@sha256:3517b63d7a9cd49b7237882fb7c260589b58163c4082d3a37de55a0d93311718
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21585385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80ab7ee8304c003a86093c588d645758bfed1ac563263e12516c798014a4fc10`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 02:50:22 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 02:50:24 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 29 Jul 2020 00:20:43 GMT
COPY file:8e3cf7c133ac957e81d3eb831160ad827bfde058f356d7ac234b8c5ae307e37a in / 
# Wed, 29 Jul 2020 00:20:44 GMT
EXPOSE 80
# Wed, 29 Jul 2020 00:20:44 GMT
VOLUME [/tmp]
# Wed, 29 Jul 2020 00:20:44 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Jul 2020 00:20:44 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:8bcf82fc850436ad04fd66371e38f7611fe76a22b78f47f57ddb8908aa3d6001`  
		Last Modified: Wed, 29 Jul 2020 00:21:33 GMT  
		Size: 21.1 MB (21126327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:200bc13e0e03c532ea237fcc9f0c4f22416b91512a21c11cff0ecfa61a75d1f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20232026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c47b44829bfc497b7e5f3a9777a71f42e165db80fee23dcdb4de56014db3334e`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 03:46:16 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 03:46:17 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 28 Jul 2020 23:56:22 GMT
COPY file:a02ffe991352ee1f8abb077135ea9d27557e8b364fb712a42ccb2865e08df3cc in / 
# Tue, 28 Jul 2020 23:56:25 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:56:26 GMT
VOLUME [/tmp]
# Tue, 28 Jul 2020 23:56:27 GMT
ENTRYPOINT ["/traefik"]
# Tue, 28 Jul 2020 23:56:28 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:5b7ba63f15824a6daa3f73b57bd9fb04ea01b471f646b703dd08620f13e22d9c`  
		Last Modified: Tue, 28 Jul 2020 23:57:53 GMT  
		Size: 19.8 MB (19772940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:d46ed499e4b8c1c9dffea750abe7ad35fba0c431165a394e10283810d33b8d29
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.0 MB (19952059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b691bd363853ce10cedfbe29ea1e8d1e88d7e8eb01da6a3e1baa469c745a1302`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 05:55:25 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 05:55:26 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 29 Jul 2020 00:00:50 GMT
COPY file:f592954af2951d1a2538b1945366cb995f49638c7ef8b561b6961e0f8023197a in / 
# Wed, 29 Jul 2020 00:00:51 GMT
EXPOSE 80
# Wed, 29 Jul 2020 00:00:51 GMT
VOLUME [/tmp]
# Wed, 29 Jul 2020 00:00:52 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Jul 2020 00:00:53 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:fe3d477ed11470c756d1112d559be2ea65e2bbdcc367345ed45d17401a98474e`  
		Last Modified: Wed, 29 Jul 2020 00:02:17 GMT  
		Size: 19.5 MB (19492981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.26`

```console
$ docker pull traefik@sha256:17067dcaa6b2fca1cf7b4aff8aee13ca55cb43a13e47645598567f9bd09ec128
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.26` - linux; amd64

```console
$ docker pull traefik@sha256:3517b63d7a9cd49b7237882fb7c260589b58163c4082d3a37de55a0d93311718
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21585385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80ab7ee8304c003a86093c588d645758bfed1ac563263e12516c798014a4fc10`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 02:50:22 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 02:50:24 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 29 Jul 2020 00:20:43 GMT
COPY file:8e3cf7c133ac957e81d3eb831160ad827bfde058f356d7ac234b8c5ae307e37a in / 
# Wed, 29 Jul 2020 00:20:44 GMT
EXPOSE 80
# Wed, 29 Jul 2020 00:20:44 GMT
VOLUME [/tmp]
# Wed, 29 Jul 2020 00:20:44 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Jul 2020 00:20:44 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:8bcf82fc850436ad04fd66371e38f7611fe76a22b78f47f57ddb8908aa3d6001`  
		Last Modified: Wed, 29 Jul 2020 00:21:33 GMT  
		Size: 21.1 MB (21126327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.26` - linux; arm variant v6

```console
$ docker pull traefik@sha256:200bc13e0e03c532ea237fcc9f0c4f22416b91512a21c11cff0ecfa61a75d1f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20232026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c47b44829bfc497b7e5f3a9777a71f42e165db80fee23dcdb4de56014db3334e`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 03:46:16 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 03:46:17 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 28 Jul 2020 23:56:22 GMT
COPY file:a02ffe991352ee1f8abb077135ea9d27557e8b364fb712a42ccb2865e08df3cc in / 
# Tue, 28 Jul 2020 23:56:25 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:56:26 GMT
VOLUME [/tmp]
# Tue, 28 Jul 2020 23:56:27 GMT
ENTRYPOINT ["/traefik"]
# Tue, 28 Jul 2020 23:56:28 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:5b7ba63f15824a6daa3f73b57bd9fb04ea01b471f646b703dd08620f13e22d9c`  
		Last Modified: Tue, 28 Jul 2020 23:57:53 GMT  
		Size: 19.8 MB (19772940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.26` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:d46ed499e4b8c1c9dffea750abe7ad35fba0c431165a394e10283810d33b8d29
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.0 MB (19952059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b691bd363853ce10cedfbe29ea1e8d1e88d7e8eb01da6a3e1baa469c745a1302`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 05:55:25 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 05:55:26 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 29 Jul 2020 00:00:50 GMT
COPY file:f592954af2951d1a2538b1945366cb995f49638c7ef8b561b6961e0f8023197a in / 
# Wed, 29 Jul 2020 00:00:51 GMT
EXPOSE 80
# Wed, 29 Jul 2020 00:00:51 GMT
VOLUME [/tmp]
# Wed, 29 Jul 2020 00:00:52 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Jul 2020 00:00:53 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:fe3d477ed11470c756d1112d559be2ea65e2bbdcc367345ed45d17401a98474e`  
		Last Modified: Wed, 29 Jul 2020 00:02:17 GMT  
		Size: 19.5 MB (19492981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.26-alpine`

```console
$ docker pull traefik@sha256:0da45cd2c37ec826012e0f2d8a3a4ac0a7be4240a4942a6e40e3aae0f6fb205f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.26-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:3cbe9e62ef26a9ac17b25702754dfbf56dd346850170be90eabd370f24190ef1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24634355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c36f69007d987e4ed093711f4f306b52ce63b1c19f5ffacd49a1aea1f717e527`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Jul 2020 00:20:25 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Jul 2020 00:20:25 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Jul 2020 00:20:25 GMT
EXPOSE 80
# Wed, 29 Jul 2020 00:20:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Jul 2020 00:20:26 GMT
CMD ["traefik"]
# Wed, 29 Jul 2020 00:20:26 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:5bb03716fa366c58de14b0fc81a50daf51f39175c928558e3e82017b5999f233`  
		Last Modified: Wed, 29 Jul 2020 00:21:23 GMT  
		Size: 21.1 MB (21126524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c61f1414a3fbacefede004c9c340def8b1c393630a1c2241a0c9196692c574`  
		Last Modified: Wed, 29 Jul 2020 00:21:19 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.26-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:d77a05164ca7fbf64eb55feb97bd9e3d1dfaed181d23bc172d1602203b036b28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23091373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f84ddfeb559adfb1011610755afdd099c865a8de51b045331d848b1a58077bc6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 28 Jul 2020 23:51:46 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 28 Jul 2020 23:51:47 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 28 Jul 2020 23:51:48 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:51:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Jul 2020 23:51:52 GMT
CMD ["traefik"]
# Tue, 28 Jul 2020 23:51:55 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:bf46db6761515f08f18c5396f51c8d5fd2ae1c385ff5c12113336ffb79684420`  
		Last Modified: Tue, 28 Jul 2020 23:57:37 GMT  
		Size: 19.8 MB (19772984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0368cab0ca49479d26c28e4638f00e78884190c43adf25a35b647ffc70e1209f`  
		Last Modified: Tue, 28 Jul 2020 23:57:30 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.26-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7805105ced1b07c019cb3c420705bb105b1d8da381b76869db624e521af05592
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22913978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6548e0334e123554f38144482ac92954e0ed970de05727c2d7b6e371f0cda8f9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 28 Jul 2020 23:50:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 28 Jul 2020 23:50:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 28 Jul 2020 23:50:28 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:50:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Jul 2020 23:50:29 GMT
CMD ["traefik"]
# Tue, 28 Jul 2020 23:50:30 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:7f9ba2c08e62ba40494711c8f4e4d32d3d297940e5c04ceaa0594de58ced1744`  
		Last Modified: Wed, 29 Jul 2020 00:02:01 GMT  
		Size: 19.5 MB (19493128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3295e2c39b2f8f9a497a542502857a9b10a07977734f37c658f79d6e1a71c57b`  
		Last Modified: Wed, 29 Jul 2020 00:01:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.26-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f8f03683732d73c7d9a288627158d8f30579255aab4662d54201486e07a7f9dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `traefik:v1.7.26-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull traefik@sha256:cd065335be88e46f537b005bcdd09e1c8eafeb1ad3674a12011635e30b5c8652
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2366139069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37b2f4d0fbf437493bbfd55b018ebf33649e751c25151ae05ff55009c5a70419`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:47:45 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 12 Aug 2020 18:47:47 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:47:48 GMT
ENTRYPOINT ["/traefik"]
# Wed, 12 Aug 2020 18:47:49 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298e1db6a0b5b538cab98a96f8c4650e4fccee26fb0e75f0582d210e0dc7af6d`  
		Last Modified: Wed, 12 Aug 2020 18:49:14 GMT  
		Size: 30.3 MB (30267520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699a7485ed05f7d7c0614726620e754f884bdd13f33bdd82cf017ede4c96a631`  
		Last Modified: Wed, 12 Aug 2020 18:49:06 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d222b7829a182578922580c28dbd3b0cd98374c8c5508b777df5d6a9e6763d0c`  
		Last Modified: Wed, 12 Aug 2020 18:49:06 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba55ff7183a9e35465c15ca0f795637c77bf77b5d338053acb7b5b1f05434e0`  
		Last Modified: Wed, 12 Aug 2020 18:49:06 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-alpine`

```console
$ docker pull traefik@sha256:0da45cd2c37ec826012e0f2d8a3a4ac0a7be4240a4942a6e40e3aae0f6fb205f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:3cbe9e62ef26a9ac17b25702754dfbf56dd346850170be90eabd370f24190ef1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24634355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c36f69007d987e4ed093711f4f306b52ce63b1c19f5ffacd49a1aea1f717e527`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Jul 2020 00:20:25 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Jul 2020 00:20:25 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Jul 2020 00:20:25 GMT
EXPOSE 80
# Wed, 29 Jul 2020 00:20:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Jul 2020 00:20:26 GMT
CMD ["traefik"]
# Wed, 29 Jul 2020 00:20:26 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:5bb03716fa366c58de14b0fc81a50daf51f39175c928558e3e82017b5999f233`  
		Last Modified: Wed, 29 Jul 2020 00:21:23 GMT  
		Size: 21.1 MB (21126524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c61f1414a3fbacefede004c9c340def8b1c393630a1c2241a0c9196692c574`  
		Last Modified: Wed, 29 Jul 2020 00:21:19 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:d77a05164ca7fbf64eb55feb97bd9e3d1dfaed181d23bc172d1602203b036b28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23091373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f84ddfeb559adfb1011610755afdd099c865a8de51b045331d848b1a58077bc6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 28 Jul 2020 23:51:46 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 28 Jul 2020 23:51:47 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 28 Jul 2020 23:51:48 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:51:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Jul 2020 23:51:52 GMT
CMD ["traefik"]
# Tue, 28 Jul 2020 23:51:55 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:bf46db6761515f08f18c5396f51c8d5fd2ae1c385ff5c12113336ffb79684420`  
		Last Modified: Tue, 28 Jul 2020 23:57:37 GMT  
		Size: 19.8 MB (19772984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0368cab0ca49479d26c28e4638f00e78884190c43adf25a35b647ffc70e1209f`  
		Last Modified: Tue, 28 Jul 2020 23:57:30 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7805105ced1b07c019cb3c420705bb105b1d8da381b76869db624e521af05592
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22913978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6548e0334e123554f38144482ac92954e0ed970de05727c2d7b6e371f0cda8f9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 28 Jul 2020 23:50:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 28 Jul 2020 23:50:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 28 Jul 2020 23:50:28 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:50:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Jul 2020 23:50:29 GMT
CMD ["traefik"]
# Tue, 28 Jul 2020 23:50:30 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:7f9ba2c08e62ba40494711c8f4e4d32d3d297940e5c04ceaa0594de58ced1744`  
		Last Modified: Wed, 29 Jul 2020 00:02:01 GMT  
		Size: 19.5 MB (19493128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3295e2c39b2f8f9a497a542502857a9b10a07977734f37c658f79d6e1a71c57b`  
		Last Modified: Wed, 29 Jul 2020 00:01:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f8f03683732d73c7d9a288627158d8f30579255aab4662d54201486e07a7f9dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `traefik:v1.7-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull traefik@sha256:cd065335be88e46f537b005bcdd09e1c8eafeb1ad3674a12011635e30b5c8652
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2366139069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37b2f4d0fbf437493bbfd55b018ebf33649e751c25151ae05ff55009c5a70419`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:47:45 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 12 Aug 2020 18:47:47 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:47:48 GMT
ENTRYPOINT ["/traefik"]
# Wed, 12 Aug 2020 18:47:49 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298e1db6a0b5b538cab98a96f8c4650e4fccee26fb0e75f0582d210e0dc7af6d`  
		Last Modified: Wed, 12 Aug 2020 18:49:14 GMT  
		Size: 30.3 MB (30267520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699a7485ed05f7d7c0614726620e754f884bdd13f33bdd82cf017ede4c96a631`  
		Last Modified: Wed, 12 Aug 2020 18:49:06 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d222b7829a182578922580c28dbd3b0cd98374c8c5508b777df5d6a9e6763d0c`  
		Last Modified: Wed, 12 Aug 2020 18:49:06 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba55ff7183a9e35465c15ca0f795637c77bf77b5d338053acb7b5b1f05434e0`  
		Last Modified: Wed, 12 Aug 2020 18:49:06 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.2`

```console
$ docker pull traefik@sha256:f5af5a5ce17fc3e353b507e8acce65d7f28126408a8c92dc3cac246d023dc9e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.2` - linux; amd64

```console
$ docker pull traefik@sha256:2468d73cafe08a8973ac3d4e7d0163c1e86c36c8b1bc1f212fdf88999a799fb5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25167674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6e6fde072260f39a81ffcd1eaaa9e0f3aa8de874d1805a14e7315f0e19c344b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Jul 2020 00:20:17 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.8/traefik_v2.2.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Jul 2020 00:20:17 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Jul 2020 00:20:17 GMT
EXPOSE 80
# Wed, 29 Jul 2020 00:20:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Jul 2020 00:20:18 GMT
CMD ["traefik"]
# Wed, 29 Jul 2020 00:20:18 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:1f5ad3441e7363549035f66e706f206a0de236b858cf33c9cd9ff8dcdd18e1a7`  
		Last Modified: Wed, 29 Jul 2020 00:21:13 GMT  
		Size: 21.7 MB (21659842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636569b0d16cb280926eb5f6d661be7cb1d4476a31d45328398e644f07119b3c`  
		Last Modified: Wed, 29 Jul 2020 00:21:09 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.2` - linux; arm variant v6

```console
$ docker pull traefik@sha256:fa4de82729f8fccc89108cf8e8e23032173a461dd4b8a6a2f717be05254bce6c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.7 MB (23663705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8161e01e718ca849737d9eb3777995c1c86c0b8e361ddd66bf36bec4162f102`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 28 Jul 2020 23:51:19 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.8/traefik_v2.2.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 28 Jul 2020 23:51:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 28 Jul 2020 23:51:24 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:51:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Jul 2020 23:51:28 GMT
CMD ["traefik"]
# Tue, 28 Jul 2020 23:51:30 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9fd7ea12487aad43f479ff4ed630cfdcad68a675a840c616be0a8d9e6bbff967`  
		Last Modified: Tue, 28 Jul 2020 23:57:20 GMT  
		Size: 20.3 MB (20345315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a709b83326f37f60b72767971160e15dacb81aa1c252ad8d48d22a54fcaed7cf`  
		Last Modified: Tue, 28 Jul 2020 23:57:13 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.2` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9a56dab619dbd6617ce626f247bcb5f4c5c47b6b1a1c1c2d7ad1ffa842d1feaf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23422892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fb444508581ad8942228a15b26ae157f4624dc050768480e286472439499f40`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 28 Jul 2020 23:50:09 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.8/traefik_v2.2.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 28 Jul 2020 23:50:10 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 28 Jul 2020 23:50:12 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:50:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Jul 2020 23:50:13 GMT
CMD ["traefik"]
# Tue, 28 Jul 2020 23:50:14 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:04d6b3ba19b9cdbee340681e37ccbf55756f6547a8ea2176e084d2d38d900b43`  
		Last Modified: Wed, 29 Jul 2020 00:01:42 GMT  
		Size: 20.0 MB (20002042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5632834be9cd878f2629d7e53d9c353cad96bda6be58e6afcdab6fb8477bbd`  
		Last Modified: Wed, 29 Jul 2020 00:01:37 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.2.8`

```console
$ docker pull traefik@sha256:f5af5a5ce17fc3e353b507e8acce65d7f28126408a8c92dc3cac246d023dc9e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.2.8` - linux; amd64

```console
$ docker pull traefik@sha256:2468d73cafe08a8973ac3d4e7d0163c1e86c36c8b1bc1f212fdf88999a799fb5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25167674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6e6fde072260f39a81ffcd1eaaa9e0f3aa8de874d1805a14e7315f0e19c344b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Jul 2020 00:20:17 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.8/traefik_v2.2.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Jul 2020 00:20:17 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Jul 2020 00:20:17 GMT
EXPOSE 80
# Wed, 29 Jul 2020 00:20:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Jul 2020 00:20:18 GMT
CMD ["traefik"]
# Wed, 29 Jul 2020 00:20:18 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:1f5ad3441e7363549035f66e706f206a0de236b858cf33c9cd9ff8dcdd18e1a7`  
		Last Modified: Wed, 29 Jul 2020 00:21:13 GMT  
		Size: 21.7 MB (21659842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636569b0d16cb280926eb5f6d661be7cb1d4476a31d45328398e644f07119b3c`  
		Last Modified: Wed, 29 Jul 2020 00:21:09 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.2.8` - linux; arm variant v6

```console
$ docker pull traefik@sha256:fa4de82729f8fccc89108cf8e8e23032173a461dd4b8a6a2f717be05254bce6c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.7 MB (23663705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8161e01e718ca849737d9eb3777995c1c86c0b8e361ddd66bf36bec4162f102`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 28 Jul 2020 23:51:19 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.8/traefik_v2.2.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 28 Jul 2020 23:51:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 28 Jul 2020 23:51:24 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:51:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Jul 2020 23:51:28 GMT
CMD ["traefik"]
# Tue, 28 Jul 2020 23:51:30 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9fd7ea12487aad43f479ff4ed630cfdcad68a675a840c616be0a8d9e6bbff967`  
		Last Modified: Tue, 28 Jul 2020 23:57:20 GMT  
		Size: 20.3 MB (20345315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a709b83326f37f60b72767971160e15dacb81aa1c252ad8d48d22a54fcaed7cf`  
		Last Modified: Tue, 28 Jul 2020 23:57:13 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.2.8` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9a56dab619dbd6617ce626f247bcb5f4c5c47b6b1a1c1c2d7ad1ffa842d1feaf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23422892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fb444508581ad8942228a15b26ae157f4624dc050768480e286472439499f40`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 28 Jul 2020 23:50:09 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.8/traefik_v2.2.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 28 Jul 2020 23:50:10 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 28 Jul 2020 23:50:12 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:50:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Jul 2020 23:50:13 GMT
CMD ["traefik"]
# Tue, 28 Jul 2020 23:50:14 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:04d6b3ba19b9cdbee340681e37ccbf55756f6547a8ea2176e084d2d38d900b43`  
		Last Modified: Wed, 29 Jul 2020 00:01:42 GMT  
		Size: 20.0 MB (20002042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5632834be9cd878f2629d7e53d9c353cad96bda6be58e6afcdab6fb8477bbd`  
		Last Modified: Wed, 29 Jul 2020 00:01:37 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.2.8-windowsservercore-1809`

```console
$ docker pull traefik@sha256:cdc3dbe8b06277ebd96943b994a7cc23d2b9373e1e785276d64f82085219bf16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `traefik:v2.2.8-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull traefik@sha256:a17b61b8c1e1d7573b98844eaec3a7f0c503d85f0705d3ab642585bbdc9d888a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2366658561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e061a005c81a3df8c7000f7c9ad6aecbe3761839b3adc998b9cb996776ba824`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:46:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.2.8/traefik_v2.2.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 12 Aug 2020 18:46:47 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:46:48 GMT
ENTRYPOINT ["/traefik"]
# Wed, 12 Aug 2020 18:46:49 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7698fba9396d0c8aabdaeb88d228a02d13fa7eccb8c50cc8ad141232de6d5d`  
		Last Modified: Wed, 12 Aug 2020 18:48:47 GMT  
		Size: 30.8 MB (30787030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70187a11409864df9161ffb451d7cb5cee8d45ce3aa9bf78a9ac1b8569d0513c`  
		Last Modified: Wed, 12 Aug 2020 18:48:40 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0acd47024a509c5b6df0032fae59357c838b124c17ea1d510d233a548fb58459`  
		Last Modified: Wed, 12 Aug 2020 18:48:39 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b66a39bbb90e279df94df561cd2e7c19ec45604bfcddce75254a78d67cf18a`  
		Last Modified: Wed, 12 Aug 2020 18:48:40 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:cdc3dbe8b06277ebd96943b994a7cc23d2b9373e1e785276d64f82085219bf16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `traefik:v2.2-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull traefik@sha256:a17b61b8c1e1d7573b98844eaec3a7f0c503d85f0705d3ab642585bbdc9d888a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2366658561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e061a005c81a3df8c7000f7c9ad6aecbe3761839b3adc998b9cb996776ba824`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:46:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.2.8/traefik_v2.2.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 12 Aug 2020 18:46:47 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:46:48 GMT
ENTRYPOINT ["/traefik"]
# Wed, 12 Aug 2020 18:46:49 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7698fba9396d0c8aabdaeb88d228a02d13fa7eccb8c50cc8ad141232de6d5d`  
		Last Modified: Wed, 12 Aug 2020 18:48:47 GMT  
		Size: 30.8 MB (30787030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70187a11409864df9161ffb451d7cb5cee8d45ce3aa9bf78a9ac1b8569d0513c`  
		Last Modified: Wed, 12 Aug 2020 18:48:40 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0acd47024a509c5b6df0032fae59357c838b124c17ea1d510d233a548fb58459`  
		Last Modified: Wed, 12 Aug 2020 18:48:39 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b66a39bbb90e279df94df561cd2e7c19ec45604bfcddce75254a78d67cf18a`  
		Last Modified: Wed, 12 Aug 2020 18:48:40 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.3`

```console
$ docker pull traefik@sha256:302e1214da614f62b8cdc930daf285bc9d8165ac15e0953309161de06a589fb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.3` - linux; amd64

```console
$ docker pull traefik@sha256:3f5c5a46ccff636a9e726961f123638bd6854191040072d860fc15bbcee3e184
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28052206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:926633bd017b112d1ee29780353bd3898e2f5f4a3b4749e8c4070ab765708bc4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 19 Aug 2020 21:12:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc4/traefik_v2.3.0-rc4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 19 Aug 2020 21:12:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 19 Aug 2020 21:12:05 GMT
EXPOSE 80
# Wed, 19 Aug 2020 21:12:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Aug 2020 21:12:05 GMT
CMD ["traefik"]
# Wed, 19 Aug 2020 21:12:05 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:8843362db2d6c7cba5a5ac00938528154d1b876fe944ae136e0c6cd5d390e4f4`  
		Last Modified: Wed, 19 Aug 2020 21:12:38 GMT  
		Size: 24.5 MB (24544374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685edc151199f805d0e1910cd68e68161fbc81369caf76102ebed3176760a338`  
		Last Modified: Wed, 19 Aug 2020 21:12:32 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.3` - linux; arm variant v6

```console
$ docker pull traefik@sha256:c85e11c5d0332ddc75b8a70c5fcd19540794ae68a86df0fb7c957fec76074a65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.2 MB (26178413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f6d814c93b2dcc172081103002e7c5ff94bd1b8fec1210b28caca91353fdb66`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 19 Aug 2020 21:04:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc4/traefik_v2.3.0-rc4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 19 Aug 2020 21:04:07 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 19 Aug 2020 21:04:09 GMT
EXPOSE 80
# Wed, 19 Aug 2020 21:04:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Aug 2020 21:04:12 GMT
CMD ["traefik"]
# Wed, 19 Aug 2020 21:04:15 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:a2d52f51ca6c71d0c3f5144f84c3099bd4831769fa83c8d072c6b67b89c61321`  
		Last Modified: Wed, 19 Aug 2020 21:04:59 GMT  
		Size: 22.9 MB (22860023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6497bf20f1fdcc8800a01dd9f26e77ac3f1236f6627bbd64100ec7926f84e2c2`  
		Last Modified: Wed, 19 Aug 2020 21:04:52 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.3` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:14b29b6c8bd7c722e1dd0e06f9f0a7e37db3a5d8467496cfde55b13073656702
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27754805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bce20c5287082213e632bc7034a39e3e84efd677922b395fd4c5d13843dfa62`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 28 Jul 2020 23:49:54 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc3/traefik_v2.3.0-rc3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 28 Jul 2020 23:49:55 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 28 Jul 2020 23:49:56 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:49:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Jul 2020 23:49:57 GMT
CMD ["traefik"]
# Tue, 28 Jul 2020 23:49:58 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b32d16371e8f6c49f7eb4c9ae55be6a35d152399c37508b5a81eb631bdd0f182`  
		Last Modified: Wed, 29 Jul 2020 00:01:25 GMT  
		Size: 24.3 MB (24333955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3bbea951e4557c6db83dc8f3fa25298592630e9292fe53c8f4ebcadce74658b`  
		Last Modified: Wed, 29 Jul 2020 00:01:18 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.3.0-rc4`

```console
$ docker pull traefik@sha256:587a1920014de5051d3dbeefc6eb0f9d4162dd4d485778fe3a2926f1e3b25d05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6

### `traefik:v2.3.0-rc4` - linux; amd64

```console
$ docker pull traefik@sha256:3f5c5a46ccff636a9e726961f123638bd6854191040072d860fc15bbcee3e184
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28052206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:926633bd017b112d1ee29780353bd3898e2f5f4a3b4749e8c4070ab765708bc4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 19 Aug 2020 21:12:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc4/traefik_v2.3.0-rc4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 19 Aug 2020 21:12:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 19 Aug 2020 21:12:05 GMT
EXPOSE 80
# Wed, 19 Aug 2020 21:12:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Aug 2020 21:12:05 GMT
CMD ["traefik"]
# Wed, 19 Aug 2020 21:12:05 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:8843362db2d6c7cba5a5ac00938528154d1b876fe944ae136e0c6cd5d390e4f4`  
		Last Modified: Wed, 19 Aug 2020 21:12:38 GMT  
		Size: 24.5 MB (24544374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685edc151199f805d0e1910cd68e68161fbc81369caf76102ebed3176760a338`  
		Last Modified: Wed, 19 Aug 2020 21:12:32 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.3.0-rc4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:c85e11c5d0332ddc75b8a70c5fcd19540794ae68a86df0fb7c957fec76074a65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.2 MB (26178413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f6d814c93b2dcc172081103002e7c5ff94bd1b8fec1210b28caca91353fdb66`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 19 Aug 2020 21:04:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc4/traefik_v2.3.0-rc4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 19 Aug 2020 21:04:07 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 19 Aug 2020 21:04:09 GMT
EXPOSE 80
# Wed, 19 Aug 2020 21:04:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Aug 2020 21:04:12 GMT
CMD ["traefik"]
# Wed, 19 Aug 2020 21:04:15 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:a2d52f51ca6c71d0c3f5144f84c3099bd4831769fa83c8d072c6b67b89c61321`  
		Last Modified: Wed, 19 Aug 2020 21:04:59 GMT  
		Size: 22.9 MB (22860023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6497bf20f1fdcc8800a01dd9f26e77ac3f1236f6627bbd64100ec7926f84e2c2`  
		Last Modified: Wed, 19 Aug 2020 21:04:52 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.3.0-rc4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:5c9e5afb0e7accad59b5f89929d130a728a8fbcd78c6d7d3e676a7c091d2c942
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `traefik:v2.3.0-rc4-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull traefik@sha256:19d714a6298146cab0bf90c4909d2e6addc448b76539b8f6653737c41380ce61
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2369930817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0193116892fbe1dd8a1a7327fb2197ef5d1e6728bb04c6ce6846064f1375fe63`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 19 Aug 2020 20:16:01 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.3.0-rc4/traefik_v2.3.0-rc4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 19 Aug 2020 20:16:02 GMT
EXPOSE 80
# Wed, 19 Aug 2020 20:16:03 GMT
ENTRYPOINT ["/traefik"]
# Wed, 19 Aug 2020 20:16:04 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4b935273c9edf14dff5895c90155812d7052eb98cdde597989fb945e41a600`  
		Last Modified: Wed, 19 Aug 2020 20:16:51 GMT  
		Size: 34.1 MB (34059255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982afb2946804976c1bbfe8b800b61fce8c6b9ec3bd9bb7951c013285b70d035`  
		Last Modified: Wed, 19 Aug 2020 20:16:43 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b41b5d9e95faa94a24fc8746bcf52d32b83a2c0199bd871711259bd69287298`  
		Last Modified: Wed, 19 Aug 2020 20:16:43 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e22963c3d8d4509fa45f3351a0348edcfd1dbbdb3502373ef7feed8503ca96`  
		Last Modified: Wed, 19 Aug 2020 20:16:43 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.3-windowsservercore-1809`

```console
$ docker pull traefik@sha256:5c9e5afb0e7accad59b5f89929d130a728a8fbcd78c6d7d3e676a7c091d2c942
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `traefik:v2.3-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull traefik@sha256:19d714a6298146cab0bf90c4909d2e6addc448b76539b8f6653737c41380ce61
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2369930817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0193116892fbe1dd8a1a7327fb2197ef5d1e6728bb04c6ce6846064f1375fe63`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 19 Aug 2020 20:16:01 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.3.0-rc4/traefik_v2.3.0-rc4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 19 Aug 2020 20:16:02 GMT
EXPOSE 80
# Wed, 19 Aug 2020 20:16:03 GMT
ENTRYPOINT ["/traefik"]
# Wed, 19 Aug 2020 20:16:04 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4b935273c9edf14dff5895c90155812d7052eb98cdde597989fb945e41a600`  
		Last Modified: Wed, 19 Aug 2020 20:16:51 GMT  
		Size: 34.1 MB (34059255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982afb2946804976c1bbfe8b800b61fce8c6b9ec3bd9bb7951c013285b70d035`  
		Last Modified: Wed, 19 Aug 2020 20:16:43 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b41b5d9e95faa94a24fc8746bcf52d32b83a2c0199bd871711259bd69287298`  
		Last Modified: Wed, 19 Aug 2020 20:16:43 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e22963c3d8d4509fa45f3351a0348edcfd1dbbdb3502373ef7feed8503ca96`  
		Last Modified: Wed, 19 Aug 2020 20:16:43 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:cdc3dbe8b06277ebd96943b994a7cc23d2b9373e1e785276d64f82085219bf16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull traefik@sha256:a17b61b8c1e1d7573b98844eaec3a7f0c503d85f0705d3ab642585bbdc9d888a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2366658561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e061a005c81a3df8c7000f7c9ad6aecbe3761839b3adc998b9cb996776ba824`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:46:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.2.8/traefik_v2.2.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 12 Aug 2020 18:46:47 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:46:48 GMT
ENTRYPOINT ["/traefik"]
# Wed, 12 Aug 2020 18:46:49 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7698fba9396d0c8aabdaeb88d228a02d13fa7eccb8c50cc8ad141232de6d5d`  
		Last Modified: Wed, 12 Aug 2020 18:48:47 GMT  
		Size: 30.8 MB (30787030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70187a11409864df9161ffb451d7cb5cee8d45ce3aa9bf78a9ac1b8569d0513c`  
		Last Modified: Wed, 12 Aug 2020 18:48:40 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0acd47024a509c5b6df0032fae59357c838b124c17ea1d510d233a548fb58459`  
		Last Modified: Wed, 12 Aug 2020 18:48:39 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b66a39bbb90e279df94df561cd2e7c19ec45604bfcddce75254a78d67cf18a`  
		Last Modified: Wed, 12 Aug 2020 18:48:40 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
