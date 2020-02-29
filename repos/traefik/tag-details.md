<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:1.7`](#traefik17)
-	[`traefik:1.7.21`](#traefik1721)
-	[`traefik:1.7.21-alpine`](#traefik1721-alpine)
-	[`traefik:1.7.21-windowsservercore-1809`](#traefik1721-windowsservercore-1809)
-	[`traefik:1.7-alpine`](#traefik17-alpine)
-	[`traefik:1.7-windowsservercore-1809`](#traefik17-windowsservercore-1809)
-	[`traefik:2.1`](#traefik21)
-	[`traefik:2.1.6`](#traefik216)
-	[`traefik:2.1.6-windowsservercore-1809`](#traefik216-windowsservercore-1809)
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
-	[`traefik:v2.1.6`](#traefikv216)
-	[`traefik:v2.1.6-windowsservercore-1809`](#traefikv216-windowsservercore-1809)
-	[`traefik:v2.1-windowsservercore-1809`](#traefikv21-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:1.7`

```console
$ docker pull traefik@sha256:58daca9716fa5f7de3c281d42fbba6d07c7037460b9d62a9a80bc1247c9c22db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7` - linux; amd64

```console
$ docker pull traefik@sha256:61a4e3aa686d88ddb394717592e6e2fc0ac3cfa41a18c50c90409aa854ef0de4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.0 MB (24007955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c2555fbcde99f397827cb31e38da922978f9aaa3caa2e754cefe646b383ec3e`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 02:50:22 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 02:50:24 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Fri, 21 Feb 2020 02:50:26 GMT
COPY file:8fa44c20d6e42fb3cd0b6caaeb86722c0e1cd93fb6093d2de8aaf28b28c2f650 in / 
# Fri, 21 Feb 2020 02:50:27 GMT
EXPOSE 80
# Fri, 21 Feb 2020 02:50:27 GMT
VOLUME [/tmp]
# Fri, 21 Feb 2020 02:50:27 GMT
ENTRYPOINT ["/traefik"]
# Fri, 21 Feb 2020 02:50:27 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:f94e0edbd0965ecafc2f2dc4f70ed65894bc6118d9918ab8957a56c346e62174`  
		Last Modified: Fri, 21 Feb 2020 02:51:11 GMT  
		Size: 23.5 MB (23548897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:e077692a927fad30896e298531b9bb63bd9ab26f750f259a6f9fd0dfe60da266
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.5 MB (22497176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8d3fc66811d215539a771ad826f5dcf5caf0e42299529ea0bb4f3cdf7d5dedd`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 20 Feb 2020 23:23:27 GMT
COPY file:f457e8adb6c53dc9a59d4eb315e663a1b1eda09623526a54957ad04390140125 in /etc/ssl/certs/ 
# Thu, 20 Feb 2020 23:23:31 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Thu, 20 Feb 2020 23:23:46 GMT
COPY file:6d3dbbb33aedfd1f5ef6da256d3ecd62ae826e9064d323b8e99debcf83de347d in / 
# Thu, 20 Feb 2020 23:23:56 GMT
EXPOSE 80
# Thu, 20 Feb 2020 23:24:05 GMT
VOLUME [/tmp]
# Thu, 20 Feb 2020 23:24:11 GMT
ENTRYPOINT ["/traefik"]
# Thu, 20 Feb 2020 23:24:19 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:23c1841b8c7860045db6b4a1e02a96e6232417f97062ae42483b8d4658a40d33`  
		Last Modified: Thu, 20 Feb 2020 23:25:15 GMT  
		Size: 131.7 KB (131681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bb0787cb8098772b3249eecfe5cb7694c680eceff4feebcab8358baf7e26557`  
		Last Modified: Thu, 20 Feb 2020 23:25:16 GMT  
		Size: 327.4 KB (327383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07efaf5c8806d641c6b656bf92370fe8ba5086603061f1661d5e80fb4969a2ef`  
		Last Modified: Thu, 20 Feb 2020 23:25:24 GMT  
		Size: 22.0 MB (22038112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:0cb49bbff4def1c014d06bb6e63c4241e6f459128e2cffaf0dde5d5106640e52
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.2 MB (22217495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94ddc0a9c7abadc96d123d0d0049c0e585f867c795d1a2d8c8e2a4393bb06245`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 01:08:43 GMT
COPY file:f457e8adb6c53dc9a59d4eb315e663a1b1eda09623526a54957ad04390140125 in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 01:08:48 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Fri, 21 Feb 2020 01:08:51 GMT
COPY file:387a5fc078877c037ccc2027c5668931f7835f82a2c24234f574014ddcd1fca6 in / 
# Fri, 21 Feb 2020 01:08:56 GMT
EXPOSE 80
# Fri, 21 Feb 2020 01:08:58 GMT
VOLUME [/tmp]
# Fri, 21 Feb 2020 01:09:01 GMT
ENTRYPOINT ["/traefik"]
# Fri, 21 Feb 2020 01:09:04 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e3d3c9facd6ab3f42d5ef511674d7d138ad0107cf47a738ec1ec1c836be5178e`  
		Last Modified: Fri, 21 Feb 2020 01:09:42 GMT  
		Size: 131.7 KB (131684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52950036377454e4b5c9b92233904cd5d12087bbce611bddcda397a500ea6bb`  
		Last Modified: Fri, 21 Feb 2020 01:09:42 GMT  
		Size: 327.4 KB (327408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99824cccc52b292309e2540f7f63bbe94ac6332ef5c79d89239eb6dd5f7c3e1`  
		Last Modified: Fri, 21 Feb 2020 01:09:50 GMT  
		Size: 21.8 MB (21758403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.21`

```console
$ docker pull traefik@sha256:58daca9716fa5f7de3c281d42fbba6d07c7037460b9d62a9a80bc1247c9c22db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.21` - linux; amd64

```console
$ docker pull traefik@sha256:61a4e3aa686d88ddb394717592e6e2fc0ac3cfa41a18c50c90409aa854ef0de4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.0 MB (24007955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c2555fbcde99f397827cb31e38da922978f9aaa3caa2e754cefe646b383ec3e`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 02:50:22 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 02:50:24 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Fri, 21 Feb 2020 02:50:26 GMT
COPY file:8fa44c20d6e42fb3cd0b6caaeb86722c0e1cd93fb6093d2de8aaf28b28c2f650 in / 
# Fri, 21 Feb 2020 02:50:27 GMT
EXPOSE 80
# Fri, 21 Feb 2020 02:50:27 GMT
VOLUME [/tmp]
# Fri, 21 Feb 2020 02:50:27 GMT
ENTRYPOINT ["/traefik"]
# Fri, 21 Feb 2020 02:50:27 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:f94e0edbd0965ecafc2f2dc4f70ed65894bc6118d9918ab8957a56c346e62174`  
		Last Modified: Fri, 21 Feb 2020 02:51:11 GMT  
		Size: 23.5 MB (23548897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.21` - linux; arm variant v6

```console
$ docker pull traefik@sha256:e077692a927fad30896e298531b9bb63bd9ab26f750f259a6f9fd0dfe60da266
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.5 MB (22497176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8d3fc66811d215539a771ad826f5dcf5caf0e42299529ea0bb4f3cdf7d5dedd`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 20 Feb 2020 23:23:27 GMT
COPY file:f457e8adb6c53dc9a59d4eb315e663a1b1eda09623526a54957ad04390140125 in /etc/ssl/certs/ 
# Thu, 20 Feb 2020 23:23:31 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Thu, 20 Feb 2020 23:23:46 GMT
COPY file:6d3dbbb33aedfd1f5ef6da256d3ecd62ae826e9064d323b8e99debcf83de347d in / 
# Thu, 20 Feb 2020 23:23:56 GMT
EXPOSE 80
# Thu, 20 Feb 2020 23:24:05 GMT
VOLUME [/tmp]
# Thu, 20 Feb 2020 23:24:11 GMT
ENTRYPOINT ["/traefik"]
# Thu, 20 Feb 2020 23:24:19 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:23c1841b8c7860045db6b4a1e02a96e6232417f97062ae42483b8d4658a40d33`  
		Last Modified: Thu, 20 Feb 2020 23:25:15 GMT  
		Size: 131.7 KB (131681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bb0787cb8098772b3249eecfe5cb7694c680eceff4feebcab8358baf7e26557`  
		Last Modified: Thu, 20 Feb 2020 23:25:16 GMT  
		Size: 327.4 KB (327383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07efaf5c8806d641c6b656bf92370fe8ba5086603061f1661d5e80fb4969a2ef`  
		Last Modified: Thu, 20 Feb 2020 23:25:24 GMT  
		Size: 22.0 MB (22038112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.21` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:0cb49bbff4def1c014d06bb6e63c4241e6f459128e2cffaf0dde5d5106640e52
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.2 MB (22217495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94ddc0a9c7abadc96d123d0d0049c0e585f867c795d1a2d8c8e2a4393bb06245`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 01:08:43 GMT
COPY file:f457e8adb6c53dc9a59d4eb315e663a1b1eda09623526a54957ad04390140125 in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 01:08:48 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Fri, 21 Feb 2020 01:08:51 GMT
COPY file:387a5fc078877c037ccc2027c5668931f7835f82a2c24234f574014ddcd1fca6 in / 
# Fri, 21 Feb 2020 01:08:56 GMT
EXPOSE 80
# Fri, 21 Feb 2020 01:08:58 GMT
VOLUME [/tmp]
# Fri, 21 Feb 2020 01:09:01 GMT
ENTRYPOINT ["/traefik"]
# Fri, 21 Feb 2020 01:09:04 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e3d3c9facd6ab3f42d5ef511674d7d138ad0107cf47a738ec1ec1c836be5178e`  
		Last Modified: Fri, 21 Feb 2020 01:09:42 GMT  
		Size: 131.7 KB (131684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52950036377454e4b5c9b92233904cd5d12087bbce611bddcda397a500ea6bb`  
		Last Modified: Fri, 21 Feb 2020 01:09:42 GMT  
		Size: 327.4 KB (327408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99824cccc52b292309e2540f7f63bbe94ac6332ef5c79d89239eb6dd5f7c3e1`  
		Last Modified: Fri, 21 Feb 2020 01:09:50 GMT  
		Size: 21.8 MB (21758403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.21-alpine`

```console
$ docker pull traefik@sha256:0e4ac8ae724603898620dbd5eb9cda7ec05f405d25476eb0d32b716b490ba079
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.21-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:c6ce83d760f3b8345f733e5c683150fcbb2be562320d770ef5b5b200430b73af
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27046535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6156ee9118f9e56be7ff7f2502b60f673a0c7d369cbf04c7d86b7f51e160d57`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 21 Feb 2020 02:50:03 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.21/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 21 Feb 2020 02:50:04 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 21 Feb 2020 02:50:04 GMT
EXPOSE 80
# Fri, 21 Feb 2020 02:50:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Feb 2020 02:50:05 GMT
CMD ["traefik"]
# Fri, 21 Feb 2020 02:50:05 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:2573c02b6f16483bdb00538c6e62a28f2b46e281a45995a40759219f7b684033`  
		Last Modified: Fri, 21 Feb 2020 02:50:57 GMT  
		Size: 23.5 MB (23549027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1619fb3841d1976493c12824ab4fa94f75dc863f74bb7ea35a77baf2f3dbb83f`  
		Last Modified: Fri, 21 Feb 2020 02:50:49 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.21-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:738e9b119aaf9d93111c4d106999b761a2aec49107bfcdf56659cb8cb00e3b78
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25354129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:040affe79b0c33f1032773cecdc51b55c3ad16d32129fe19eac901be8b2beca1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 20 Feb 2020 23:19:40 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.21/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 20 Feb 2020 23:19:42 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 20 Feb 2020 23:19:43 GMT
EXPOSE 80
# Thu, 20 Feb 2020 23:19:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 20 Feb 2020 23:19:45 GMT
CMD ["traefik"]
# Thu, 20 Feb 2020 23:19:46 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:a1ef1f9c32d2768d6e21333dea037ba6488a6807bd873790b98d6cbeaa676f20`  
		Last Modified: Thu, 20 Feb 2020 23:25:05 GMT  
		Size: 22.0 MB (22038187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f3959c6f98920f7c6ed79674d03674c30925a6bbe11e2da8f02bcf50ad80da`  
		Last Modified: Thu, 20 Feb 2020 23:24:53 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.21-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:bc9357d03ae91ec11cbfcef34dd85c5512e93dd993220f29e9bcb109ad4e87f8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25177947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:990a43d99f6d8b4cb18362432e9aa459ab4828fc64e8f04f8ca504243af319ec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 21 Feb 2020 01:08:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.21/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 21 Feb 2020 01:08:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 21 Feb 2020 01:08:28 GMT
EXPOSE 80
# Fri, 21 Feb 2020 01:08:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Feb 2020 01:08:29 GMT
CMD ["traefik"]
# Fri, 21 Feb 2020 01:08:31 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b1520ccdb72fc9797850dc1b3891af53fac1a5ab24ff927bd75ff769495a11df`  
		Last Modified: Fri, 21 Feb 2020 01:09:31 GMT  
		Size: 21.8 MB (21758461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b783ed4bba2358b372561bbb9084fea69e6f888bd146459d201471a16c238afc`  
		Last Modified: Fri, 21 Feb 2020 01:09:23 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.21-windowsservercore-1809`

```console
$ docker pull traefik@sha256:9c5d55ab72b6ff7878e90c13f2e4129d555841f40162084aee7262958781cf72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1040; amd64

### `traefik:1.7.21-windowsservercore-1809` - windows version 10.0.17763.1040; amd64

```console
$ docker pull traefik@sha256:95fde4a8ab386660c84b9d41a3a318b8a5a5790b75c72616bcd7370f396c9f86
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2258633790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4f1caafca4ee157eccd61c9e21054adcfd73622794670afec2c7267bf24024d`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 17 Feb 2020 06:57:13 GMT
RUN Install update 1809-amd64
# Thu, 20 Feb 2020 01:13:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 20 Feb 2020 23:23:08 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.21/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 20 Feb 2020 23:23:14 GMT
EXPOSE 80
# Thu, 20 Feb 2020 23:23:16 GMT
ENTRYPOINT ["/traefik"]
# Thu, 20 Feb 2020 23:23:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b5103484a3c3b2578d270f0963d24f36f3cbc7c8c14cea7caffba57e6a661b64`  
		Last Modified: Thu, 20 Feb 2020 23:24:03 GMT  
		Size: 28.1 MB (28125104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7ed7741340e3edcdd2cf93f5ae86ebde4f492b0b5362afd6b45d51d5ccaadd`  
		Last Modified: Thu, 20 Feb 2020 23:23:53 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70eda346bd458bce401d67081efcd6eb552a8fef9aa661ff3663481bdac1eefe`  
		Last Modified: Thu, 20 Feb 2020 23:23:53 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bea84645d19f8e10b033b2203ee00c209fdd8836116ac9faa4a9519d1740cb`  
		Last Modified: Thu, 20 Feb 2020 23:23:53 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-alpine`

```console
$ docker pull traefik@sha256:0e4ac8ae724603898620dbd5eb9cda7ec05f405d25476eb0d32b716b490ba079
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:c6ce83d760f3b8345f733e5c683150fcbb2be562320d770ef5b5b200430b73af
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27046535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6156ee9118f9e56be7ff7f2502b60f673a0c7d369cbf04c7d86b7f51e160d57`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 21 Feb 2020 02:50:03 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.21/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 21 Feb 2020 02:50:04 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 21 Feb 2020 02:50:04 GMT
EXPOSE 80
# Fri, 21 Feb 2020 02:50:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Feb 2020 02:50:05 GMT
CMD ["traefik"]
# Fri, 21 Feb 2020 02:50:05 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:2573c02b6f16483bdb00538c6e62a28f2b46e281a45995a40759219f7b684033`  
		Last Modified: Fri, 21 Feb 2020 02:50:57 GMT  
		Size: 23.5 MB (23549027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1619fb3841d1976493c12824ab4fa94f75dc863f74bb7ea35a77baf2f3dbb83f`  
		Last Modified: Fri, 21 Feb 2020 02:50:49 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:738e9b119aaf9d93111c4d106999b761a2aec49107bfcdf56659cb8cb00e3b78
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25354129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:040affe79b0c33f1032773cecdc51b55c3ad16d32129fe19eac901be8b2beca1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 20 Feb 2020 23:19:40 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.21/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 20 Feb 2020 23:19:42 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 20 Feb 2020 23:19:43 GMT
EXPOSE 80
# Thu, 20 Feb 2020 23:19:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 20 Feb 2020 23:19:45 GMT
CMD ["traefik"]
# Thu, 20 Feb 2020 23:19:46 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:a1ef1f9c32d2768d6e21333dea037ba6488a6807bd873790b98d6cbeaa676f20`  
		Last Modified: Thu, 20 Feb 2020 23:25:05 GMT  
		Size: 22.0 MB (22038187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f3959c6f98920f7c6ed79674d03674c30925a6bbe11e2da8f02bcf50ad80da`  
		Last Modified: Thu, 20 Feb 2020 23:24:53 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:bc9357d03ae91ec11cbfcef34dd85c5512e93dd993220f29e9bcb109ad4e87f8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25177947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:990a43d99f6d8b4cb18362432e9aa459ab4828fc64e8f04f8ca504243af319ec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 21 Feb 2020 01:08:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.21/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 21 Feb 2020 01:08:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 21 Feb 2020 01:08:28 GMT
EXPOSE 80
# Fri, 21 Feb 2020 01:08:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Feb 2020 01:08:29 GMT
CMD ["traefik"]
# Fri, 21 Feb 2020 01:08:31 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b1520ccdb72fc9797850dc1b3891af53fac1a5ab24ff927bd75ff769495a11df`  
		Last Modified: Fri, 21 Feb 2020 01:09:31 GMT  
		Size: 21.8 MB (21758461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b783ed4bba2358b372561bbb9084fea69e6f888bd146459d201471a16c238afc`  
		Last Modified: Fri, 21 Feb 2020 01:09:23 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:9c5d55ab72b6ff7878e90c13f2e4129d555841f40162084aee7262958781cf72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1040; amd64

### `traefik:1.7-windowsservercore-1809` - windows version 10.0.17763.1040; amd64

```console
$ docker pull traefik@sha256:95fde4a8ab386660c84b9d41a3a318b8a5a5790b75c72616bcd7370f396c9f86
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2258633790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4f1caafca4ee157eccd61c9e21054adcfd73622794670afec2c7267bf24024d`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 17 Feb 2020 06:57:13 GMT
RUN Install update 1809-amd64
# Thu, 20 Feb 2020 01:13:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 20 Feb 2020 23:23:08 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.21/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 20 Feb 2020 23:23:14 GMT
EXPOSE 80
# Thu, 20 Feb 2020 23:23:16 GMT
ENTRYPOINT ["/traefik"]
# Thu, 20 Feb 2020 23:23:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b5103484a3c3b2578d270f0963d24f36f3cbc7c8c14cea7caffba57e6a661b64`  
		Last Modified: Thu, 20 Feb 2020 23:24:03 GMT  
		Size: 28.1 MB (28125104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7ed7741340e3edcdd2cf93f5ae86ebde4f492b0b5362afd6b45d51d5ccaadd`  
		Last Modified: Thu, 20 Feb 2020 23:23:53 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70eda346bd458bce401d67081efcd6eb552a8fef9aa661ff3663481bdac1eefe`  
		Last Modified: Thu, 20 Feb 2020 23:23:53 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bea84645d19f8e10b033b2203ee00c209fdd8836116ac9faa4a9519d1740cb`  
		Last Modified: Thu, 20 Feb 2020 23:23:53 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.1`

```console
$ docker pull traefik@sha256:13c5e62a0757bd8bf57c8c36575f7686f06186994ad6d2bda773ed8f140415c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.1` - linux; amd64

```console
$ docker pull traefik@sha256:25a2352b4a1c1a645eac9cf8687976264e1fcded88ce87839895e4a6f1b15a82
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23080492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12609cfc24227160805147219eabc15c9fcc83fec86a72d5d6263c34c1e4c6c3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 28 Feb 2020 23:21:22 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.6/traefik_v2.1.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 28 Feb 2020 23:21:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 28 Feb 2020 23:21:23 GMT
EXPOSE 80
# Fri, 28 Feb 2020 23:21:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Feb 2020 23:21:23 GMT
CMD ["traefik"]
# Fri, 28 Feb 2020 23:21:23 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:f246959e69e132c3c07393e1f4857470594c34f4bc31696f7c1d0b479c4225b9`  
		Last Modified: Fri, 28 Feb 2020 23:21:47 GMT  
		Size: 19.6 MB (19582985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb45f4dca2ffdb237ad2155441cd41ab771be09738a315337fbf4745d412a49f`  
		Last Modified: Fri, 28 Feb 2020 23:21:42 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.1` - linux; arm variant v6

```console
$ docker pull traefik@sha256:9a84a4904925f1a5959777640b5b3d7d777e8ecf70fad03501bcb0d0b1bb5876
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21647505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5212a87ddaba0fea3f9d7a7609146f620b2f08904e9064cbc2f06550e3349d9a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 28 Feb 2020 22:49:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.6/traefik_v2.1.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 28 Feb 2020 22:49:43 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 28 Feb 2020 22:49:44 GMT
EXPOSE 80
# Fri, 28 Feb 2020 22:49:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Feb 2020 22:49:45 GMT
CMD ["traefik"]
# Fri, 28 Feb 2020 22:49:45 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:8bf74f8c820455e9c57f8afba3adbc0b78344d322c7a087ef2aed1bdea66687e`  
		Last Modified: Fri, 28 Feb 2020 22:50:26 GMT  
		Size: 18.3 MB (18331562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60efb704037babbe5325a0482dd8d4fdf485d0e0aed54e9a66d6b16d1f7dc2f0`  
		Last Modified: Fri, 28 Feb 2020 22:50:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:6a69893d63aff5270effc34e516605030578cc3c36cf5afa1b007266414161f3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21448230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e7c15a6013a22978d4996b24cfae44d24a4ed518908a6b547958c59a3ddc78b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 28 Feb 2020 22:42:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.6/traefik_v2.1.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 28 Feb 2020 22:42:37 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 28 Feb 2020 22:42:37 GMT
EXPOSE 80
# Fri, 28 Feb 2020 22:42:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Feb 2020 22:42:39 GMT
CMD ["traefik"]
# Fri, 28 Feb 2020 22:42:39 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:52b1f3e98b82f1ca594ec918a75407d1920e426975edfd8289cd7eb9a2acaa8f`  
		Last Modified: Fri, 28 Feb 2020 22:43:10 GMT  
		Size: 18.0 MB (18028744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006197e30cad84f3d1a363029848ac4fa0782b89916b3db4fcc9b5c97bbedea9`  
		Last Modified: Fri, 28 Feb 2020 22:43:04 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.1.6`

```console
$ docker pull traefik@sha256:13c5e62a0757bd8bf57c8c36575f7686f06186994ad6d2bda773ed8f140415c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.1.6` - linux; amd64

```console
$ docker pull traefik@sha256:25a2352b4a1c1a645eac9cf8687976264e1fcded88ce87839895e4a6f1b15a82
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23080492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12609cfc24227160805147219eabc15c9fcc83fec86a72d5d6263c34c1e4c6c3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 28 Feb 2020 23:21:22 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.6/traefik_v2.1.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 28 Feb 2020 23:21:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 28 Feb 2020 23:21:23 GMT
EXPOSE 80
# Fri, 28 Feb 2020 23:21:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Feb 2020 23:21:23 GMT
CMD ["traefik"]
# Fri, 28 Feb 2020 23:21:23 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:f246959e69e132c3c07393e1f4857470594c34f4bc31696f7c1d0b479c4225b9`  
		Last Modified: Fri, 28 Feb 2020 23:21:47 GMT  
		Size: 19.6 MB (19582985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb45f4dca2ffdb237ad2155441cd41ab771be09738a315337fbf4745d412a49f`  
		Last Modified: Fri, 28 Feb 2020 23:21:42 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.1.6` - linux; arm variant v6

```console
$ docker pull traefik@sha256:9a84a4904925f1a5959777640b5b3d7d777e8ecf70fad03501bcb0d0b1bb5876
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21647505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5212a87ddaba0fea3f9d7a7609146f620b2f08904e9064cbc2f06550e3349d9a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 28 Feb 2020 22:49:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.6/traefik_v2.1.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 28 Feb 2020 22:49:43 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 28 Feb 2020 22:49:44 GMT
EXPOSE 80
# Fri, 28 Feb 2020 22:49:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Feb 2020 22:49:45 GMT
CMD ["traefik"]
# Fri, 28 Feb 2020 22:49:45 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:8bf74f8c820455e9c57f8afba3adbc0b78344d322c7a087ef2aed1bdea66687e`  
		Last Modified: Fri, 28 Feb 2020 22:50:26 GMT  
		Size: 18.3 MB (18331562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60efb704037babbe5325a0482dd8d4fdf485d0e0aed54e9a66d6b16d1f7dc2f0`  
		Last Modified: Fri, 28 Feb 2020 22:50:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.1.6` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:6a69893d63aff5270effc34e516605030578cc3c36cf5afa1b007266414161f3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21448230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e7c15a6013a22978d4996b24cfae44d24a4ed518908a6b547958c59a3ddc78b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 28 Feb 2020 22:42:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.6/traefik_v2.1.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 28 Feb 2020 22:42:37 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 28 Feb 2020 22:42:37 GMT
EXPOSE 80
# Fri, 28 Feb 2020 22:42:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Feb 2020 22:42:39 GMT
CMD ["traefik"]
# Fri, 28 Feb 2020 22:42:39 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:52b1f3e98b82f1ca594ec918a75407d1920e426975edfd8289cd7eb9a2acaa8f`  
		Last Modified: Fri, 28 Feb 2020 22:43:10 GMT  
		Size: 18.0 MB (18028744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006197e30cad84f3d1a363029848ac4fa0782b89916b3db4fcc9b5c97bbedea9`  
		Last Modified: Fri, 28 Feb 2020 22:43:04 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.1.6-windowsservercore-1809`

```console
$ docker pull traefik@sha256:d197841c98f70a5cfcc3aae372d7843eff10045fe38cdadcc5acdf2fd084fc7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1040; amd64

### `traefik:2.1.6-windowsservercore-1809` - windows version 10.0.17763.1040; amd64

```console
$ docker pull traefik@sha256:6ef62e89404c45ea849cd51a5dcfac5732a225572b7fd1679f9345ab21577a7e
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2254677851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f8b8df80a5f009f8eeeba97b27d2069784c291ae48289a714a113adbb942941`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 17 Feb 2020 06:57:13 GMT
RUN Install update 1809-amd64
# Thu, 20 Feb 2020 01:13:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 28 Feb 2020 23:24:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.6/traefik_v2.1.6_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Fri, 28 Feb 2020 23:24:15 GMT
EXPOSE 80
# Fri, 28 Feb 2020 23:24:16 GMT
ENTRYPOINT ["/traefik"]
# Fri, 28 Feb 2020 23:24:18 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b76f678ce4ee0ac830ca2fbfbe9bb25345f876cbb007fe9683043f3cfc54411d`  
		Last Modified: Fri, 28 Feb 2020 23:24:59 GMT  
		Size: 24.2 MB (24169151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48efb386c689e1ece2ee5afa2b9c2a40d015e2bd1fe8166fd5e785b2402b4d7b`  
		Last Modified: Fri, 28 Feb 2020 23:24:53 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b37b2b9555ab0edb0fc149d4c974e6bf124c14c385605002d75cc7521955b00`  
		Last Modified: Fri, 28 Feb 2020 23:24:53 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06a84dcfb78e0a621d3addfd89ebdffd9763f973134ef5433195c6b49c6f33d`  
		Last Modified: Fri, 28 Feb 2020 23:24:53 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:d197841c98f70a5cfcc3aae372d7843eff10045fe38cdadcc5acdf2fd084fc7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1040; amd64

### `traefik:2.1-windowsservercore-1809` - windows version 10.0.17763.1040; amd64

```console
$ docker pull traefik@sha256:6ef62e89404c45ea849cd51a5dcfac5732a225572b7fd1679f9345ab21577a7e
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2254677851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f8b8df80a5f009f8eeeba97b27d2069784c291ae48289a714a113adbb942941`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 17 Feb 2020 06:57:13 GMT
RUN Install update 1809-amd64
# Thu, 20 Feb 2020 01:13:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 28 Feb 2020 23:24:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.6/traefik_v2.1.6_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Fri, 28 Feb 2020 23:24:15 GMT
EXPOSE 80
# Fri, 28 Feb 2020 23:24:16 GMT
ENTRYPOINT ["/traefik"]
# Fri, 28 Feb 2020 23:24:18 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b76f678ce4ee0ac830ca2fbfbe9bb25345f876cbb007fe9683043f3cfc54411d`  
		Last Modified: Fri, 28 Feb 2020 23:24:59 GMT  
		Size: 24.2 MB (24169151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48efb386c689e1ece2ee5afa2b9c2a40d015e2bd1fe8166fd5e785b2402b4d7b`  
		Last Modified: Fri, 28 Feb 2020 23:24:53 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b37b2b9555ab0edb0fc149d4c974e6bf124c14c385605002d75cc7521955b00`  
		Last Modified: Fri, 28 Feb 2020 23:24:53 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06a84dcfb78e0a621d3addfd89ebdffd9763f973134ef5433195c6b49c6f33d`  
		Last Modified: Fri, 28 Feb 2020 23:24:53 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:cantal`

```console
$ docker pull traefik@sha256:13c5e62a0757bd8bf57c8c36575f7686f06186994ad6d2bda773ed8f140415c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:cantal` - linux; amd64

```console
$ docker pull traefik@sha256:25a2352b4a1c1a645eac9cf8687976264e1fcded88ce87839895e4a6f1b15a82
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23080492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12609cfc24227160805147219eabc15c9fcc83fec86a72d5d6263c34c1e4c6c3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 28 Feb 2020 23:21:22 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.6/traefik_v2.1.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 28 Feb 2020 23:21:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 28 Feb 2020 23:21:23 GMT
EXPOSE 80
# Fri, 28 Feb 2020 23:21:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Feb 2020 23:21:23 GMT
CMD ["traefik"]
# Fri, 28 Feb 2020 23:21:23 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:f246959e69e132c3c07393e1f4857470594c34f4bc31696f7c1d0b479c4225b9`  
		Last Modified: Fri, 28 Feb 2020 23:21:47 GMT  
		Size: 19.6 MB (19582985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb45f4dca2ffdb237ad2155441cd41ab771be09738a315337fbf4745d412a49f`  
		Last Modified: Fri, 28 Feb 2020 23:21:42 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:cantal` - linux; arm variant v6

```console
$ docker pull traefik@sha256:9a84a4904925f1a5959777640b5b3d7d777e8ecf70fad03501bcb0d0b1bb5876
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21647505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5212a87ddaba0fea3f9d7a7609146f620b2f08904e9064cbc2f06550e3349d9a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 28 Feb 2020 22:49:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.6/traefik_v2.1.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 28 Feb 2020 22:49:43 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 28 Feb 2020 22:49:44 GMT
EXPOSE 80
# Fri, 28 Feb 2020 22:49:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Feb 2020 22:49:45 GMT
CMD ["traefik"]
# Fri, 28 Feb 2020 22:49:45 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:8bf74f8c820455e9c57f8afba3adbc0b78344d322c7a087ef2aed1bdea66687e`  
		Last Modified: Fri, 28 Feb 2020 22:50:26 GMT  
		Size: 18.3 MB (18331562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60efb704037babbe5325a0482dd8d4fdf485d0e0aed54e9a66d6b16d1f7dc2f0`  
		Last Modified: Fri, 28 Feb 2020 22:50:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:cantal` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:6a69893d63aff5270effc34e516605030578cc3c36cf5afa1b007266414161f3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21448230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e7c15a6013a22978d4996b24cfae44d24a4ed518908a6b547958c59a3ddc78b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 28 Feb 2020 22:42:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.6/traefik_v2.1.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 28 Feb 2020 22:42:37 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 28 Feb 2020 22:42:37 GMT
EXPOSE 80
# Fri, 28 Feb 2020 22:42:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Feb 2020 22:42:39 GMT
CMD ["traefik"]
# Fri, 28 Feb 2020 22:42:39 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:52b1f3e98b82f1ca594ec918a75407d1920e426975edfd8289cd7eb9a2acaa8f`  
		Last Modified: Fri, 28 Feb 2020 22:43:10 GMT  
		Size: 18.0 MB (18028744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006197e30cad84f3d1a363029848ac4fa0782b89916b3db4fcc9b5c97bbedea9`  
		Last Modified: Fri, 28 Feb 2020 22:43:04 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:cantal-windowsservercore-1809`

```console
$ docker pull traefik@sha256:d197841c98f70a5cfcc3aae372d7843eff10045fe38cdadcc5acdf2fd084fc7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1040; amd64

### `traefik:cantal-windowsservercore-1809` - windows version 10.0.17763.1040; amd64

```console
$ docker pull traefik@sha256:6ef62e89404c45ea849cd51a5dcfac5732a225572b7fd1679f9345ab21577a7e
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2254677851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f8b8df80a5f009f8eeeba97b27d2069784c291ae48289a714a113adbb942941`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 17 Feb 2020 06:57:13 GMT
RUN Install update 1809-amd64
# Thu, 20 Feb 2020 01:13:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 28 Feb 2020 23:24:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.6/traefik_v2.1.6_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Fri, 28 Feb 2020 23:24:15 GMT
EXPOSE 80
# Fri, 28 Feb 2020 23:24:16 GMT
ENTRYPOINT ["/traefik"]
# Fri, 28 Feb 2020 23:24:18 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b76f678ce4ee0ac830ca2fbfbe9bb25345f876cbb007fe9683043f3cfc54411d`  
		Last Modified: Fri, 28 Feb 2020 23:24:59 GMT  
		Size: 24.2 MB (24169151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48efb386c689e1ece2ee5afa2b9c2a40d015e2bd1fe8166fd5e785b2402b4d7b`  
		Last Modified: Fri, 28 Feb 2020 23:24:53 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b37b2b9555ab0edb0fc149d4c974e6bf124c14c385605002d75cc7521955b00`  
		Last Modified: Fri, 28 Feb 2020 23:24:53 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06a84dcfb78e0a621d3addfd89ebdffd9763f973134ef5433195c6b49c6f33d`  
		Last Modified: Fri, 28 Feb 2020 23:24:53 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:13c5e62a0757bd8bf57c8c36575f7686f06186994ad6d2bda773ed8f140415c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:25a2352b4a1c1a645eac9cf8687976264e1fcded88ce87839895e4a6f1b15a82
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23080492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12609cfc24227160805147219eabc15c9fcc83fec86a72d5d6263c34c1e4c6c3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 28 Feb 2020 23:21:22 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.6/traefik_v2.1.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 28 Feb 2020 23:21:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 28 Feb 2020 23:21:23 GMT
EXPOSE 80
# Fri, 28 Feb 2020 23:21:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Feb 2020 23:21:23 GMT
CMD ["traefik"]
# Fri, 28 Feb 2020 23:21:23 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:f246959e69e132c3c07393e1f4857470594c34f4bc31696f7c1d0b479c4225b9`  
		Last Modified: Fri, 28 Feb 2020 23:21:47 GMT  
		Size: 19.6 MB (19582985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb45f4dca2ffdb237ad2155441cd41ab771be09738a315337fbf4745d412a49f`  
		Last Modified: Fri, 28 Feb 2020 23:21:42 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:9a84a4904925f1a5959777640b5b3d7d777e8ecf70fad03501bcb0d0b1bb5876
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21647505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5212a87ddaba0fea3f9d7a7609146f620b2f08904e9064cbc2f06550e3349d9a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 28 Feb 2020 22:49:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.6/traefik_v2.1.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 28 Feb 2020 22:49:43 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 28 Feb 2020 22:49:44 GMT
EXPOSE 80
# Fri, 28 Feb 2020 22:49:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Feb 2020 22:49:45 GMT
CMD ["traefik"]
# Fri, 28 Feb 2020 22:49:45 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:8bf74f8c820455e9c57f8afba3adbc0b78344d322c7a087ef2aed1bdea66687e`  
		Last Modified: Fri, 28 Feb 2020 22:50:26 GMT  
		Size: 18.3 MB (18331562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60efb704037babbe5325a0482dd8d4fdf485d0e0aed54e9a66d6b16d1f7dc2f0`  
		Last Modified: Fri, 28 Feb 2020 22:50:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:6a69893d63aff5270effc34e516605030578cc3c36cf5afa1b007266414161f3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21448230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e7c15a6013a22978d4996b24cfae44d24a4ed518908a6b547958c59a3ddc78b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 28 Feb 2020 22:42:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.6/traefik_v2.1.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 28 Feb 2020 22:42:37 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 28 Feb 2020 22:42:37 GMT
EXPOSE 80
# Fri, 28 Feb 2020 22:42:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Feb 2020 22:42:39 GMT
CMD ["traefik"]
# Fri, 28 Feb 2020 22:42:39 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:52b1f3e98b82f1ca594ec918a75407d1920e426975edfd8289cd7eb9a2acaa8f`  
		Last Modified: Fri, 28 Feb 2020 22:43:10 GMT  
		Size: 18.0 MB (18028744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006197e30cad84f3d1a363029848ac4fa0782b89916b3db4fcc9b5c97bbedea9`  
		Last Modified: Fri, 28 Feb 2020 22:43:04 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles`

```console
$ docker pull traefik@sha256:58daca9716fa5f7de3c281d42fbba6d07c7037460b9d62a9a80bc1247c9c22db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles` - linux; amd64

```console
$ docker pull traefik@sha256:61a4e3aa686d88ddb394717592e6e2fc0ac3cfa41a18c50c90409aa854ef0de4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.0 MB (24007955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c2555fbcde99f397827cb31e38da922978f9aaa3caa2e754cefe646b383ec3e`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 02:50:22 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 02:50:24 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Fri, 21 Feb 2020 02:50:26 GMT
COPY file:8fa44c20d6e42fb3cd0b6caaeb86722c0e1cd93fb6093d2de8aaf28b28c2f650 in / 
# Fri, 21 Feb 2020 02:50:27 GMT
EXPOSE 80
# Fri, 21 Feb 2020 02:50:27 GMT
VOLUME [/tmp]
# Fri, 21 Feb 2020 02:50:27 GMT
ENTRYPOINT ["/traefik"]
# Fri, 21 Feb 2020 02:50:27 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:f94e0edbd0965ecafc2f2dc4f70ed65894bc6118d9918ab8957a56c346e62174`  
		Last Modified: Fri, 21 Feb 2020 02:51:11 GMT  
		Size: 23.5 MB (23548897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm variant v6

```console
$ docker pull traefik@sha256:e077692a927fad30896e298531b9bb63bd9ab26f750f259a6f9fd0dfe60da266
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.5 MB (22497176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8d3fc66811d215539a771ad826f5dcf5caf0e42299529ea0bb4f3cdf7d5dedd`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 20 Feb 2020 23:23:27 GMT
COPY file:f457e8adb6c53dc9a59d4eb315e663a1b1eda09623526a54957ad04390140125 in /etc/ssl/certs/ 
# Thu, 20 Feb 2020 23:23:31 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Thu, 20 Feb 2020 23:23:46 GMT
COPY file:6d3dbbb33aedfd1f5ef6da256d3ecd62ae826e9064d323b8e99debcf83de347d in / 
# Thu, 20 Feb 2020 23:23:56 GMT
EXPOSE 80
# Thu, 20 Feb 2020 23:24:05 GMT
VOLUME [/tmp]
# Thu, 20 Feb 2020 23:24:11 GMT
ENTRYPOINT ["/traefik"]
# Thu, 20 Feb 2020 23:24:19 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:23c1841b8c7860045db6b4a1e02a96e6232417f97062ae42483b8d4658a40d33`  
		Last Modified: Thu, 20 Feb 2020 23:25:15 GMT  
		Size: 131.7 KB (131681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bb0787cb8098772b3249eecfe5cb7694c680eceff4feebcab8358baf7e26557`  
		Last Modified: Thu, 20 Feb 2020 23:25:16 GMT  
		Size: 327.4 KB (327383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07efaf5c8806d641c6b656bf92370fe8ba5086603061f1661d5e80fb4969a2ef`  
		Last Modified: Thu, 20 Feb 2020 23:25:24 GMT  
		Size: 22.0 MB (22038112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:0cb49bbff4def1c014d06bb6e63c4241e6f459128e2cffaf0dde5d5106640e52
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.2 MB (22217495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94ddc0a9c7abadc96d123d0d0049c0e585f867c795d1a2d8c8e2a4393bb06245`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 01:08:43 GMT
COPY file:f457e8adb6c53dc9a59d4eb315e663a1b1eda09623526a54957ad04390140125 in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 01:08:48 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Fri, 21 Feb 2020 01:08:51 GMT
COPY file:387a5fc078877c037ccc2027c5668931f7835f82a2c24234f574014ddcd1fca6 in / 
# Fri, 21 Feb 2020 01:08:56 GMT
EXPOSE 80
# Fri, 21 Feb 2020 01:08:58 GMT
VOLUME [/tmp]
# Fri, 21 Feb 2020 01:09:01 GMT
ENTRYPOINT ["/traefik"]
# Fri, 21 Feb 2020 01:09:04 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e3d3c9facd6ab3f42d5ef511674d7d138ad0107cf47a738ec1ec1c836be5178e`  
		Last Modified: Fri, 21 Feb 2020 01:09:42 GMT  
		Size: 131.7 KB (131684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52950036377454e4b5c9b92233904cd5d12087bbce611bddcda397a500ea6bb`  
		Last Modified: Fri, 21 Feb 2020 01:09:42 GMT  
		Size: 327.4 KB (327408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99824cccc52b292309e2540f7f63bbe94ac6332ef5c79d89239eb6dd5f7c3e1`  
		Last Modified: Fri, 21 Feb 2020 01:09:50 GMT  
		Size: 21.8 MB (21758403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-alpine`

```console
$ docker pull traefik@sha256:0e4ac8ae724603898620dbd5eb9cda7ec05f405d25476eb0d32b716b490ba079
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:c6ce83d760f3b8345f733e5c683150fcbb2be562320d770ef5b5b200430b73af
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27046535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6156ee9118f9e56be7ff7f2502b60f673a0c7d369cbf04c7d86b7f51e160d57`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 21 Feb 2020 02:50:03 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.21/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 21 Feb 2020 02:50:04 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 21 Feb 2020 02:50:04 GMT
EXPOSE 80
# Fri, 21 Feb 2020 02:50:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Feb 2020 02:50:05 GMT
CMD ["traefik"]
# Fri, 21 Feb 2020 02:50:05 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:2573c02b6f16483bdb00538c6e62a28f2b46e281a45995a40759219f7b684033`  
		Last Modified: Fri, 21 Feb 2020 02:50:57 GMT  
		Size: 23.5 MB (23549027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1619fb3841d1976493c12824ab4fa94f75dc863f74bb7ea35a77baf2f3dbb83f`  
		Last Modified: Fri, 21 Feb 2020 02:50:49 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:738e9b119aaf9d93111c4d106999b761a2aec49107bfcdf56659cb8cb00e3b78
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25354129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:040affe79b0c33f1032773cecdc51b55c3ad16d32129fe19eac901be8b2beca1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 20 Feb 2020 23:19:40 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.21/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 20 Feb 2020 23:19:42 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 20 Feb 2020 23:19:43 GMT
EXPOSE 80
# Thu, 20 Feb 2020 23:19:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 20 Feb 2020 23:19:45 GMT
CMD ["traefik"]
# Thu, 20 Feb 2020 23:19:46 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:a1ef1f9c32d2768d6e21333dea037ba6488a6807bd873790b98d6cbeaa676f20`  
		Last Modified: Thu, 20 Feb 2020 23:25:05 GMT  
		Size: 22.0 MB (22038187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f3959c6f98920f7c6ed79674d03674c30925a6bbe11e2da8f02bcf50ad80da`  
		Last Modified: Thu, 20 Feb 2020 23:24:53 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:bc9357d03ae91ec11cbfcef34dd85c5512e93dd993220f29e9bcb109ad4e87f8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25177947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:990a43d99f6d8b4cb18362432e9aa459ab4828fc64e8f04f8ca504243af319ec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 21 Feb 2020 01:08:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.21/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 21 Feb 2020 01:08:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 21 Feb 2020 01:08:28 GMT
EXPOSE 80
# Fri, 21 Feb 2020 01:08:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Feb 2020 01:08:29 GMT
CMD ["traefik"]
# Fri, 21 Feb 2020 01:08:31 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b1520ccdb72fc9797850dc1b3891af53fac1a5ab24ff927bd75ff769495a11df`  
		Last Modified: Fri, 21 Feb 2020 01:09:31 GMT  
		Size: 21.8 MB (21758461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b783ed4bba2358b372561bbb9084fea69e6f888bd146459d201471a16c238afc`  
		Last Modified: Fri, 21 Feb 2020 01:09:23 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-windowsservercore-1809`

```console
$ docker pull traefik@sha256:9c5d55ab72b6ff7878e90c13f2e4129d555841f40162084aee7262958781cf72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1040; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.1040; amd64

```console
$ docker pull traefik@sha256:95fde4a8ab386660c84b9d41a3a318b8a5a5790b75c72616bcd7370f396c9f86
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2258633790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4f1caafca4ee157eccd61c9e21054adcfd73622794670afec2c7267bf24024d`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 17 Feb 2020 06:57:13 GMT
RUN Install update 1809-amd64
# Thu, 20 Feb 2020 01:13:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 20 Feb 2020 23:23:08 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.21/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 20 Feb 2020 23:23:14 GMT
EXPOSE 80
# Thu, 20 Feb 2020 23:23:16 GMT
ENTRYPOINT ["/traefik"]
# Thu, 20 Feb 2020 23:23:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b5103484a3c3b2578d270f0963d24f36f3cbc7c8c14cea7caffba57e6a661b64`  
		Last Modified: Thu, 20 Feb 2020 23:24:03 GMT  
		Size: 28.1 MB (28125104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7ed7741340e3edcdd2cf93f5ae86ebde4f492b0b5362afd6b45d51d5ccaadd`  
		Last Modified: Thu, 20 Feb 2020 23:23:53 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70eda346bd458bce401d67081efcd6eb552a8fef9aa661ff3663481bdac1eefe`  
		Last Modified: Thu, 20 Feb 2020 23:23:53 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bea84645d19f8e10b033b2203ee00c209fdd8836116ac9faa4a9519d1740cb`  
		Last Modified: Thu, 20 Feb 2020 23:23:53 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7`

```console
$ docker pull traefik@sha256:58daca9716fa5f7de3c281d42fbba6d07c7037460b9d62a9a80bc1247c9c22db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7` - linux; amd64

```console
$ docker pull traefik@sha256:61a4e3aa686d88ddb394717592e6e2fc0ac3cfa41a18c50c90409aa854ef0de4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.0 MB (24007955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c2555fbcde99f397827cb31e38da922978f9aaa3caa2e754cefe646b383ec3e`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 02:50:22 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 02:50:24 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Fri, 21 Feb 2020 02:50:26 GMT
COPY file:8fa44c20d6e42fb3cd0b6caaeb86722c0e1cd93fb6093d2de8aaf28b28c2f650 in / 
# Fri, 21 Feb 2020 02:50:27 GMT
EXPOSE 80
# Fri, 21 Feb 2020 02:50:27 GMT
VOLUME [/tmp]
# Fri, 21 Feb 2020 02:50:27 GMT
ENTRYPOINT ["/traefik"]
# Fri, 21 Feb 2020 02:50:27 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:f94e0edbd0965ecafc2f2dc4f70ed65894bc6118d9918ab8957a56c346e62174`  
		Last Modified: Fri, 21 Feb 2020 02:51:11 GMT  
		Size: 23.5 MB (23548897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:e077692a927fad30896e298531b9bb63bd9ab26f750f259a6f9fd0dfe60da266
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.5 MB (22497176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8d3fc66811d215539a771ad826f5dcf5caf0e42299529ea0bb4f3cdf7d5dedd`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 20 Feb 2020 23:23:27 GMT
COPY file:f457e8adb6c53dc9a59d4eb315e663a1b1eda09623526a54957ad04390140125 in /etc/ssl/certs/ 
# Thu, 20 Feb 2020 23:23:31 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Thu, 20 Feb 2020 23:23:46 GMT
COPY file:6d3dbbb33aedfd1f5ef6da256d3ecd62ae826e9064d323b8e99debcf83de347d in / 
# Thu, 20 Feb 2020 23:23:56 GMT
EXPOSE 80
# Thu, 20 Feb 2020 23:24:05 GMT
VOLUME [/tmp]
# Thu, 20 Feb 2020 23:24:11 GMT
ENTRYPOINT ["/traefik"]
# Thu, 20 Feb 2020 23:24:19 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:23c1841b8c7860045db6b4a1e02a96e6232417f97062ae42483b8d4658a40d33`  
		Last Modified: Thu, 20 Feb 2020 23:25:15 GMT  
		Size: 131.7 KB (131681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bb0787cb8098772b3249eecfe5cb7694c680eceff4feebcab8358baf7e26557`  
		Last Modified: Thu, 20 Feb 2020 23:25:16 GMT  
		Size: 327.4 KB (327383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07efaf5c8806d641c6b656bf92370fe8ba5086603061f1661d5e80fb4969a2ef`  
		Last Modified: Thu, 20 Feb 2020 23:25:24 GMT  
		Size: 22.0 MB (22038112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:0cb49bbff4def1c014d06bb6e63c4241e6f459128e2cffaf0dde5d5106640e52
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.2 MB (22217495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94ddc0a9c7abadc96d123d0d0049c0e585f867c795d1a2d8c8e2a4393bb06245`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 01:08:43 GMT
COPY file:f457e8adb6c53dc9a59d4eb315e663a1b1eda09623526a54957ad04390140125 in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 01:08:48 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Fri, 21 Feb 2020 01:08:51 GMT
COPY file:387a5fc078877c037ccc2027c5668931f7835f82a2c24234f574014ddcd1fca6 in / 
# Fri, 21 Feb 2020 01:08:56 GMT
EXPOSE 80
# Fri, 21 Feb 2020 01:08:58 GMT
VOLUME [/tmp]
# Fri, 21 Feb 2020 01:09:01 GMT
ENTRYPOINT ["/traefik"]
# Fri, 21 Feb 2020 01:09:04 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e3d3c9facd6ab3f42d5ef511674d7d138ad0107cf47a738ec1ec1c836be5178e`  
		Last Modified: Fri, 21 Feb 2020 01:09:42 GMT  
		Size: 131.7 KB (131684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52950036377454e4b5c9b92233904cd5d12087bbce611bddcda397a500ea6bb`  
		Last Modified: Fri, 21 Feb 2020 01:09:42 GMT  
		Size: 327.4 KB (327408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99824cccc52b292309e2540f7f63bbe94ac6332ef5c79d89239eb6dd5f7c3e1`  
		Last Modified: Fri, 21 Feb 2020 01:09:50 GMT  
		Size: 21.8 MB (21758403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.21`

```console
$ docker pull traefik@sha256:58daca9716fa5f7de3c281d42fbba6d07c7037460b9d62a9a80bc1247c9c22db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.21` - linux; amd64

```console
$ docker pull traefik@sha256:61a4e3aa686d88ddb394717592e6e2fc0ac3cfa41a18c50c90409aa854ef0de4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.0 MB (24007955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c2555fbcde99f397827cb31e38da922978f9aaa3caa2e754cefe646b383ec3e`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 02:50:22 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 02:50:24 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Fri, 21 Feb 2020 02:50:26 GMT
COPY file:8fa44c20d6e42fb3cd0b6caaeb86722c0e1cd93fb6093d2de8aaf28b28c2f650 in / 
# Fri, 21 Feb 2020 02:50:27 GMT
EXPOSE 80
# Fri, 21 Feb 2020 02:50:27 GMT
VOLUME [/tmp]
# Fri, 21 Feb 2020 02:50:27 GMT
ENTRYPOINT ["/traefik"]
# Fri, 21 Feb 2020 02:50:27 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:f94e0edbd0965ecafc2f2dc4f70ed65894bc6118d9918ab8957a56c346e62174`  
		Last Modified: Fri, 21 Feb 2020 02:51:11 GMT  
		Size: 23.5 MB (23548897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.21` - linux; arm variant v6

```console
$ docker pull traefik@sha256:e077692a927fad30896e298531b9bb63bd9ab26f750f259a6f9fd0dfe60da266
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.5 MB (22497176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8d3fc66811d215539a771ad826f5dcf5caf0e42299529ea0bb4f3cdf7d5dedd`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 20 Feb 2020 23:23:27 GMT
COPY file:f457e8adb6c53dc9a59d4eb315e663a1b1eda09623526a54957ad04390140125 in /etc/ssl/certs/ 
# Thu, 20 Feb 2020 23:23:31 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Thu, 20 Feb 2020 23:23:46 GMT
COPY file:6d3dbbb33aedfd1f5ef6da256d3ecd62ae826e9064d323b8e99debcf83de347d in / 
# Thu, 20 Feb 2020 23:23:56 GMT
EXPOSE 80
# Thu, 20 Feb 2020 23:24:05 GMT
VOLUME [/tmp]
# Thu, 20 Feb 2020 23:24:11 GMT
ENTRYPOINT ["/traefik"]
# Thu, 20 Feb 2020 23:24:19 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:23c1841b8c7860045db6b4a1e02a96e6232417f97062ae42483b8d4658a40d33`  
		Last Modified: Thu, 20 Feb 2020 23:25:15 GMT  
		Size: 131.7 KB (131681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bb0787cb8098772b3249eecfe5cb7694c680eceff4feebcab8358baf7e26557`  
		Last Modified: Thu, 20 Feb 2020 23:25:16 GMT  
		Size: 327.4 KB (327383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07efaf5c8806d641c6b656bf92370fe8ba5086603061f1661d5e80fb4969a2ef`  
		Last Modified: Thu, 20 Feb 2020 23:25:24 GMT  
		Size: 22.0 MB (22038112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.21` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:0cb49bbff4def1c014d06bb6e63c4241e6f459128e2cffaf0dde5d5106640e52
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.2 MB (22217495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94ddc0a9c7abadc96d123d0d0049c0e585f867c795d1a2d8c8e2a4393bb06245`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 01:08:43 GMT
COPY file:f457e8adb6c53dc9a59d4eb315e663a1b1eda09623526a54957ad04390140125 in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 01:08:48 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Fri, 21 Feb 2020 01:08:51 GMT
COPY file:387a5fc078877c037ccc2027c5668931f7835f82a2c24234f574014ddcd1fca6 in / 
# Fri, 21 Feb 2020 01:08:56 GMT
EXPOSE 80
# Fri, 21 Feb 2020 01:08:58 GMT
VOLUME [/tmp]
# Fri, 21 Feb 2020 01:09:01 GMT
ENTRYPOINT ["/traefik"]
# Fri, 21 Feb 2020 01:09:04 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e3d3c9facd6ab3f42d5ef511674d7d138ad0107cf47a738ec1ec1c836be5178e`  
		Last Modified: Fri, 21 Feb 2020 01:09:42 GMT  
		Size: 131.7 KB (131684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52950036377454e4b5c9b92233904cd5d12087bbce611bddcda397a500ea6bb`  
		Last Modified: Fri, 21 Feb 2020 01:09:42 GMT  
		Size: 327.4 KB (327408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99824cccc52b292309e2540f7f63bbe94ac6332ef5c79d89239eb6dd5f7c3e1`  
		Last Modified: Fri, 21 Feb 2020 01:09:50 GMT  
		Size: 21.8 MB (21758403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.21-alpine`

```console
$ docker pull traefik@sha256:0e4ac8ae724603898620dbd5eb9cda7ec05f405d25476eb0d32b716b490ba079
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.21-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:c6ce83d760f3b8345f733e5c683150fcbb2be562320d770ef5b5b200430b73af
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27046535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6156ee9118f9e56be7ff7f2502b60f673a0c7d369cbf04c7d86b7f51e160d57`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 21 Feb 2020 02:50:03 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.21/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 21 Feb 2020 02:50:04 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 21 Feb 2020 02:50:04 GMT
EXPOSE 80
# Fri, 21 Feb 2020 02:50:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Feb 2020 02:50:05 GMT
CMD ["traefik"]
# Fri, 21 Feb 2020 02:50:05 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:2573c02b6f16483bdb00538c6e62a28f2b46e281a45995a40759219f7b684033`  
		Last Modified: Fri, 21 Feb 2020 02:50:57 GMT  
		Size: 23.5 MB (23549027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1619fb3841d1976493c12824ab4fa94f75dc863f74bb7ea35a77baf2f3dbb83f`  
		Last Modified: Fri, 21 Feb 2020 02:50:49 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.21-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:738e9b119aaf9d93111c4d106999b761a2aec49107bfcdf56659cb8cb00e3b78
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25354129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:040affe79b0c33f1032773cecdc51b55c3ad16d32129fe19eac901be8b2beca1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 20 Feb 2020 23:19:40 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.21/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 20 Feb 2020 23:19:42 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 20 Feb 2020 23:19:43 GMT
EXPOSE 80
# Thu, 20 Feb 2020 23:19:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 20 Feb 2020 23:19:45 GMT
CMD ["traefik"]
# Thu, 20 Feb 2020 23:19:46 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:a1ef1f9c32d2768d6e21333dea037ba6488a6807bd873790b98d6cbeaa676f20`  
		Last Modified: Thu, 20 Feb 2020 23:25:05 GMT  
		Size: 22.0 MB (22038187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f3959c6f98920f7c6ed79674d03674c30925a6bbe11e2da8f02bcf50ad80da`  
		Last Modified: Thu, 20 Feb 2020 23:24:53 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.21-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:bc9357d03ae91ec11cbfcef34dd85c5512e93dd993220f29e9bcb109ad4e87f8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25177947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:990a43d99f6d8b4cb18362432e9aa459ab4828fc64e8f04f8ca504243af319ec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 21 Feb 2020 01:08:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.21/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 21 Feb 2020 01:08:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 21 Feb 2020 01:08:28 GMT
EXPOSE 80
# Fri, 21 Feb 2020 01:08:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Feb 2020 01:08:29 GMT
CMD ["traefik"]
# Fri, 21 Feb 2020 01:08:31 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b1520ccdb72fc9797850dc1b3891af53fac1a5ab24ff927bd75ff769495a11df`  
		Last Modified: Fri, 21 Feb 2020 01:09:31 GMT  
		Size: 21.8 MB (21758461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b783ed4bba2358b372561bbb9084fea69e6f888bd146459d201471a16c238afc`  
		Last Modified: Fri, 21 Feb 2020 01:09:23 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.21-windowsservercore-1809`

```console
$ docker pull traefik@sha256:9c5d55ab72b6ff7878e90c13f2e4129d555841f40162084aee7262958781cf72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1040; amd64

### `traefik:v1.7.21-windowsservercore-1809` - windows version 10.0.17763.1040; amd64

```console
$ docker pull traefik@sha256:95fde4a8ab386660c84b9d41a3a318b8a5a5790b75c72616bcd7370f396c9f86
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2258633790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4f1caafca4ee157eccd61c9e21054adcfd73622794670afec2c7267bf24024d`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 17 Feb 2020 06:57:13 GMT
RUN Install update 1809-amd64
# Thu, 20 Feb 2020 01:13:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 20 Feb 2020 23:23:08 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.21/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 20 Feb 2020 23:23:14 GMT
EXPOSE 80
# Thu, 20 Feb 2020 23:23:16 GMT
ENTRYPOINT ["/traefik"]
# Thu, 20 Feb 2020 23:23:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b5103484a3c3b2578d270f0963d24f36f3cbc7c8c14cea7caffba57e6a661b64`  
		Last Modified: Thu, 20 Feb 2020 23:24:03 GMT  
		Size: 28.1 MB (28125104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7ed7741340e3edcdd2cf93f5ae86ebde4f492b0b5362afd6b45d51d5ccaadd`  
		Last Modified: Thu, 20 Feb 2020 23:23:53 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70eda346bd458bce401d67081efcd6eb552a8fef9aa661ff3663481bdac1eefe`  
		Last Modified: Thu, 20 Feb 2020 23:23:53 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bea84645d19f8e10b033b2203ee00c209fdd8836116ac9faa4a9519d1740cb`  
		Last Modified: Thu, 20 Feb 2020 23:23:53 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-alpine`

```console
$ docker pull traefik@sha256:0e4ac8ae724603898620dbd5eb9cda7ec05f405d25476eb0d32b716b490ba079
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:c6ce83d760f3b8345f733e5c683150fcbb2be562320d770ef5b5b200430b73af
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27046535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6156ee9118f9e56be7ff7f2502b60f673a0c7d369cbf04c7d86b7f51e160d57`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 21 Feb 2020 02:50:03 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.21/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 21 Feb 2020 02:50:04 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 21 Feb 2020 02:50:04 GMT
EXPOSE 80
# Fri, 21 Feb 2020 02:50:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Feb 2020 02:50:05 GMT
CMD ["traefik"]
# Fri, 21 Feb 2020 02:50:05 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:2573c02b6f16483bdb00538c6e62a28f2b46e281a45995a40759219f7b684033`  
		Last Modified: Fri, 21 Feb 2020 02:50:57 GMT  
		Size: 23.5 MB (23549027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1619fb3841d1976493c12824ab4fa94f75dc863f74bb7ea35a77baf2f3dbb83f`  
		Last Modified: Fri, 21 Feb 2020 02:50:49 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:738e9b119aaf9d93111c4d106999b761a2aec49107bfcdf56659cb8cb00e3b78
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25354129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:040affe79b0c33f1032773cecdc51b55c3ad16d32129fe19eac901be8b2beca1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 20 Feb 2020 23:19:40 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.21/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 20 Feb 2020 23:19:42 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 20 Feb 2020 23:19:43 GMT
EXPOSE 80
# Thu, 20 Feb 2020 23:19:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 20 Feb 2020 23:19:45 GMT
CMD ["traefik"]
# Thu, 20 Feb 2020 23:19:46 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:a1ef1f9c32d2768d6e21333dea037ba6488a6807bd873790b98d6cbeaa676f20`  
		Last Modified: Thu, 20 Feb 2020 23:25:05 GMT  
		Size: 22.0 MB (22038187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f3959c6f98920f7c6ed79674d03674c30925a6bbe11e2da8f02bcf50ad80da`  
		Last Modified: Thu, 20 Feb 2020 23:24:53 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:bc9357d03ae91ec11cbfcef34dd85c5512e93dd993220f29e9bcb109ad4e87f8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25177947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:990a43d99f6d8b4cb18362432e9aa459ab4828fc64e8f04f8ca504243af319ec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 21 Feb 2020 01:08:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.21/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 21 Feb 2020 01:08:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 21 Feb 2020 01:08:28 GMT
EXPOSE 80
# Fri, 21 Feb 2020 01:08:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Feb 2020 01:08:29 GMT
CMD ["traefik"]
# Fri, 21 Feb 2020 01:08:31 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b1520ccdb72fc9797850dc1b3891af53fac1a5ab24ff927bd75ff769495a11df`  
		Last Modified: Fri, 21 Feb 2020 01:09:31 GMT  
		Size: 21.8 MB (21758461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b783ed4bba2358b372561bbb9084fea69e6f888bd146459d201471a16c238afc`  
		Last Modified: Fri, 21 Feb 2020 01:09:23 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:9c5d55ab72b6ff7878e90c13f2e4129d555841f40162084aee7262958781cf72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1040; amd64

### `traefik:v1.7-windowsservercore-1809` - windows version 10.0.17763.1040; amd64

```console
$ docker pull traefik@sha256:95fde4a8ab386660c84b9d41a3a318b8a5a5790b75c72616bcd7370f396c9f86
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2258633790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4f1caafca4ee157eccd61c9e21054adcfd73622794670afec2c7267bf24024d`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 17 Feb 2020 06:57:13 GMT
RUN Install update 1809-amd64
# Thu, 20 Feb 2020 01:13:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 20 Feb 2020 23:23:08 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.21/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 20 Feb 2020 23:23:14 GMT
EXPOSE 80
# Thu, 20 Feb 2020 23:23:16 GMT
ENTRYPOINT ["/traefik"]
# Thu, 20 Feb 2020 23:23:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.21 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b5103484a3c3b2578d270f0963d24f36f3cbc7c8c14cea7caffba57e6a661b64`  
		Last Modified: Thu, 20 Feb 2020 23:24:03 GMT  
		Size: 28.1 MB (28125104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7ed7741340e3edcdd2cf93f5ae86ebde4f492b0b5362afd6b45d51d5ccaadd`  
		Last Modified: Thu, 20 Feb 2020 23:23:53 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70eda346bd458bce401d67081efcd6eb552a8fef9aa661ff3663481bdac1eefe`  
		Last Modified: Thu, 20 Feb 2020 23:23:53 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bea84645d19f8e10b033b2203ee00c209fdd8836116ac9faa4a9519d1740cb`  
		Last Modified: Thu, 20 Feb 2020 23:23:53 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.1`

```console
$ docker pull traefik@sha256:13c5e62a0757bd8bf57c8c36575f7686f06186994ad6d2bda773ed8f140415c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.1` - linux; amd64

```console
$ docker pull traefik@sha256:25a2352b4a1c1a645eac9cf8687976264e1fcded88ce87839895e4a6f1b15a82
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23080492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12609cfc24227160805147219eabc15c9fcc83fec86a72d5d6263c34c1e4c6c3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 28 Feb 2020 23:21:22 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.6/traefik_v2.1.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 28 Feb 2020 23:21:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 28 Feb 2020 23:21:23 GMT
EXPOSE 80
# Fri, 28 Feb 2020 23:21:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Feb 2020 23:21:23 GMT
CMD ["traefik"]
# Fri, 28 Feb 2020 23:21:23 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:f246959e69e132c3c07393e1f4857470594c34f4bc31696f7c1d0b479c4225b9`  
		Last Modified: Fri, 28 Feb 2020 23:21:47 GMT  
		Size: 19.6 MB (19582985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb45f4dca2ffdb237ad2155441cd41ab771be09738a315337fbf4745d412a49f`  
		Last Modified: Fri, 28 Feb 2020 23:21:42 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.1` - linux; arm variant v6

```console
$ docker pull traefik@sha256:9a84a4904925f1a5959777640b5b3d7d777e8ecf70fad03501bcb0d0b1bb5876
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21647505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5212a87ddaba0fea3f9d7a7609146f620b2f08904e9064cbc2f06550e3349d9a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 28 Feb 2020 22:49:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.6/traefik_v2.1.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 28 Feb 2020 22:49:43 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 28 Feb 2020 22:49:44 GMT
EXPOSE 80
# Fri, 28 Feb 2020 22:49:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Feb 2020 22:49:45 GMT
CMD ["traefik"]
# Fri, 28 Feb 2020 22:49:45 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:8bf74f8c820455e9c57f8afba3adbc0b78344d322c7a087ef2aed1bdea66687e`  
		Last Modified: Fri, 28 Feb 2020 22:50:26 GMT  
		Size: 18.3 MB (18331562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60efb704037babbe5325a0482dd8d4fdf485d0e0aed54e9a66d6b16d1f7dc2f0`  
		Last Modified: Fri, 28 Feb 2020 22:50:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:6a69893d63aff5270effc34e516605030578cc3c36cf5afa1b007266414161f3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21448230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e7c15a6013a22978d4996b24cfae44d24a4ed518908a6b547958c59a3ddc78b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 28 Feb 2020 22:42:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.6/traefik_v2.1.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 28 Feb 2020 22:42:37 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 28 Feb 2020 22:42:37 GMT
EXPOSE 80
# Fri, 28 Feb 2020 22:42:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Feb 2020 22:42:39 GMT
CMD ["traefik"]
# Fri, 28 Feb 2020 22:42:39 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:52b1f3e98b82f1ca594ec918a75407d1920e426975edfd8289cd7eb9a2acaa8f`  
		Last Modified: Fri, 28 Feb 2020 22:43:10 GMT  
		Size: 18.0 MB (18028744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006197e30cad84f3d1a363029848ac4fa0782b89916b3db4fcc9b5c97bbedea9`  
		Last Modified: Fri, 28 Feb 2020 22:43:04 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.1.6`

```console
$ docker pull traefik@sha256:13c5e62a0757bd8bf57c8c36575f7686f06186994ad6d2bda773ed8f140415c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.1.6` - linux; amd64

```console
$ docker pull traefik@sha256:25a2352b4a1c1a645eac9cf8687976264e1fcded88ce87839895e4a6f1b15a82
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23080492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12609cfc24227160805147219eabc15c9fcc83fec86a72d5d6263c34c1e4c6c3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 28 Feb 2020 23:21:22 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.6/traefik_v2.1.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 28 Feb 2020 23:21:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 28 Feb 2020 23:21:23 GMT
EXPOSE 80
# Fri, 28 Feb 2020 23:21:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Feb 2020 23:21:23 GMT
CMD ["traefik"]
# Fri, 28 Feb 2020 23:21:23 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:f246959e69e132c3c07393e1f4857470594c34f4bc31696f7c1d0b479c4225b9`  
		Last Modified: Fri, 28 Feb 2020 23:21:47 GMT  
		Size: 19.6 MB (19582985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb45f4dca2ffdb237ad2155441cd41ab771be09738a315337fbf4745d412a49f`  
		Last Modified: Fri, 28 Feb 2020 23:21:42 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.1.6` - linux; arm variant v6

```console
$ docker pull traefik@sha256:9a84a4904925f1a5959777640b5b3d7d777e8ecf70fad03501bcb0d0b1bb5876
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21647505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5212a87ddaba0fea3f9d7a7609146f620b2f08904e9064cbc2f06550e3349d9a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 28 Feb 2020 22:49:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.6/traefik_v2.1.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 28 Feb 2020 22:49:43 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 28 Feb 2020 22:49:44 GMT
EXPOSE 80
# Fri, 28 Feb 2020 22:49:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Feb 2020 22:49:45 GMT
CMD ["traefik"]
# Fri, 28 Feb 2020 22:49:45 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:8bf74f8c820455e9c57f8afba3adbc0b78344d322c7a087ef2aed1bdea66687e`  
		Last Modified: Fri, 28 Feb 2020 22:50:26 GMT  
		Size: 18.3 MB (18331562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60efb704037babbe5325a0482dd8d4fdf485d0e0aed54e9a66d6b16d1f7dc2f0`  
		Last Modified: Fri, 28 Feb 2020 22:50:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.1.6` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:6a69893d63aff5270effc34e516605030578cc3c36cf5afa1b007266414161f3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21448230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e7c15a6013a22978d4996b24cfae44d24a4ed518908a6b547958c59a3ddc78b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 28 Feb 2020 22:42:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.6/traefik_v2.1.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 28 Feb 2020 22:42:37 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 28 Feb 2020 22:42:37 GMT
EXPOSE 80
# Fri, 28 Feb 2020 22:42:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Feb 2020 22:42:39 GMT
CMD ["traefik"]
# Fri, 28 Feb 2020 22:42:39 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:52b1f3e98b82f1ca594ec918a75407d1920e426975edfd8289cd7eb9a2acaa8f`  
		Last Modified: Fri, 28 Feb 2020 22:43:10 GMT  
		Size: 18.0 MB (18028744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006197e30cad84f3d1a363029848ac4fa0782b89916b3db4fcc9b5c97bbedea9`  
		Last Modified: Fri, 28 Feb 2020 22:43:04 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.1.6-windowsservercore-1809`

```console
$ docker pull traefik@sha256:d197841c98f70a5cfcc3aae372d7843eff10045fe38cdadcc5acdf2fd084fc7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1040; amd64

### `traefik:v2.1.6-windowsservercore-1809` - windows version 10.0.17763.1040; amd64

```console
$ docker pull traefik@sha256:6ef62e89404c45ea849cd51a5dcfac5732a225572b7fd1679f9345ab21577a7e
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2254677851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f8b8df80a5f009f8eeeba97b27d2069784c291ae48289a714a113adbb942941`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 17 Feb 2020 06:57:13 GMT
RUN Install update 1809-amd64
# Thu, 20 Feb 2020 01:13:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 28 Feb 2020 23:24:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.6/traefik_v2.1.6_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Fri, 28 Feb 2020 23:24:15 GMT
EXPOSE 80
# Fri, 28 Feb 2020 23:24:16 GMT
ENTRYPOINT ["/traefik"]
# Fri, 28 Feb 2020 23:24:18 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b76f678ce4ee0ac830ca2fbfbe9bb25345f876cbb007fe9683043f3cfc54411d`  
		Last Modified: Fri, 28 Feb 2020 23:24:59 GMT  
		Size: 24.2 MB (24169151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48efb386c689e1ece2ee5afa2b9c2a40d015e2bd1fe8166fd5e785b2402b4d7b`  
		Last Modified: Fri, 28 Feb 2020 23:24:53 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b37b2b9555ab0edb0fc149d4c974e6bf124c14c385605002d75cc7521955b00`  
		Last Modified: Fri, 28 Feb 2020 23:24:53 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06a84dcfb78e0a621d3addfd89ebdffd9763f973134ef5433195c6b49c6f33d`  
		Last Modified: Fri, 28 Feb 2020 23:24:53 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:d197841c98f70a5cfcc3aae372d7843eff10045fe38cdadcc5acdf2fd084fc7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1040; amd64

### `traefik:v2.1-windowsservercore-1809` - windows version 10.0.17763.1040; amd64

```console
$ docker pull traefik@sha256:6ef62e89404c45ea849cd51a5dcfac5732a225572b7fd1679f9345ab21577a7e
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2254677851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f8b8df80a5f009f8eeeba97b27d2069784c291ae48289a714a113adbb942941`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 17 Feb 2020 06:57:13 GMT
RUN Install update 1809-amd64
# Thu, 20 Feb 2020 01:13:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 28 Feb 2020 23:24:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.6/traefik_v2.1.6_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Fri, 28 Feb 2020 23:24:15 GMT
EXPOSE 80
# Fri, 28 Feb 2020 23:24:16 GMT
ENTRYPOINT ["/traefik"]
# Fri, 28 Feb 2020 23:24:18 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b76f678ce4ee0ac830ca2fbfbe9bb25345f876cbb007fe9683043f3cfc54411d`  
		Last Modified: Fri, 28 Feb 2020 23:24:59 GMT  
		Size: 24.2 MB (24169151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48efb386c689e1ece2ee5afa2b9c2a40d015e2bd1fe8166fd5e785b2402b4d7b`  
		Last Modified: Fri, 28 Feb 2020 23:24:53 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b37b2b9555ab0edb0fc149d4c974e6bf124c14c385605002d75cc7521955b00`  
		Last Modified: Fri, 28 Feb 2020 23:24:53 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06a84dcfb78e0a621d3addfd89ebdffd9763f973134ef5433195c6b49c6f33d`  
		Last Modified: Fri, 28 Feb 2020 23:24:53 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:d197841c98f70a5cfcc3aae372d7843eff10045fe38cdadcc5acdf2fd084fc7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1040; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.1040; amd64

```console
$ docker pull traefik@sha256:6ef62e89404c45ea849cd51a5dcfac5732a225572b7fd1679f9345ab21577a7e
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2254677851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f8b8df80a5f009f8eeeba97b27d2069784c291ae48289a714a113adbb942941`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 17 Feb 2020 06:57:13 GMT
RUN Install update 1809-amd64
# Thu, 20 Feb 2020 01:13:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 28 Feb 2020 23:24:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.6/traefik_v2.1.6_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Fri, 28 Feb 2020 23:24:15 GMT
EXPOSE 80
# Fri, 28 Feb 2020 23:24:16 GMT
ENTRYPOINT ["/traefik"]
# Fri, 28 Feb 2020 23:24:18 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b76f678ce4ee0ac830ca2fbfbe9bb25345f876cbb007fe9683043f3cfc54411d`  
		Last Modified: Fri, 28 Feb 2020 23:24:59 GMT  
		Size: 24.2 MB (24169151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48efb386c689e1ece2ee5afa2b9c2a40d015e2bd1fe8166fd5e785b2402b4d7b`  
		Last Modified: Fri, 28 Feb 2020 23:24:53 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b37b2b9555ab0edb0fc149d4c974e6bf124c14c385605002d75cc7521955b00`  
		Last Modified: Fri, 28 Feb 2020 23:24:53 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06a84dcfb78e0a621d3addfd89ebdffd9763f973134ef5433195c6b49c6f33d`  
		Last Modified: Fri, 28 Feb 2020 23:24:53 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
