<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:1.7`](#traefik17)
-	[`traefik:1.7.22`](#traefik1722)
-	[`traefik:1.7.22-alpine`](#traefik1722-alpine)
-	[`traefik:1.7.22-windowsservercore-1809`](#traefik1722-windowsservercore-1809)
-	[`traefik:1.7-alpine`](#traefik17-alpine)
-	[`traefik:1.7-windowsservercore-1809`](#traefik17-windowsservercore-1809)
-	[`traefik:2.1`](#traefik21)
-	[`traefik:2.1.8`](#traefik218)
-	[`traefik:2.1.8-windowsservercore-1809`](#traefik218-windowsservercore-1809)
-	[`traefik:2.1-windowsservercore-1809`](#traefik21-windowsservercore-1809)
-	[`traefik:2.2`](#traefik22)
-	[`traefik:2.2.0-rc4`](#traefik220-rc4)
-	[`traefik:2.2.0-rc4-windowsservercore-1809`](#traefik220-rc4-windowsservercore-1809)
-	[`traefik:2.2-windowsservercore-1809`](#traefik22-windowsservercore-1809)
-	[`traefik:cantal`](#traefikcantal)
-	[`traefik:cantal-windowsservercore-1809`](#traefikcantal-windowsservercore-1809)
-	[`traefik:chevrotin`](#traefikchevrotin)
-	[`traefik:chevrotin-windowsservercore-1809`](#traefikchevrotin-windowsservercore-1809)
-	[`traefik:latest`](#traefiklatest)
-	[`traefik:maroilles`](#traefikmaroilles)
-	[`traefik:maroilles-alpine`](#traefikmaroilles-alpine)
-	[`traefik:maroilles-windowsservercore-1809`](#traefikmaroilles-windowsservercore-1809)
-	[`traefik:v1.7`](#traefikv17)
-	[`traefik:v1.7.22`](#traefikv1722)
-	[`traefik:v1.7.22-alpine`](#traefikv1722-alpine)
-	[`traefik:v1.7.22-windowsservercore-1809`](#traefikv1722-windowsservercore-1809)
-	[`traefik:v1.7-alpine`](#traefikv17-alpine)
-	[`traefik:v1.7-windowsservercore-1809`](#traefikv17-windowsservercore-1809)
-	[`traefik:v2.1`](#traefikv21)
-	[`traefik:v2.1.8`](#traefikv218)
-	[`traefik:v2.1.8-windowsservercore-1809`](#traefikv218-windowsservercore-1809)
-	[`traefik:v2.1-windowsservercore-1809`](#traefikv21-windowsservercore-1809)
-	[`traefik:v2.2`](#traefikv22)
-	[`traefik:v2.2.0-rc4`](#traefikv220-rc4)
-	[`traefik:v2.2.0-rc4-windowsservercore-1809`](#traefikv220-rc4-windowsservercore-1809)
-	[`traefik:v2.2-windowsservercore-1809`](#traefikv22-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:1.7`

```console
$ docker pull traefik@sha256:15edd6d0ea71a9707b8a04990d092e3991bb59e4c38a169fe560eb209fe68d62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7` - linux; amd64

```console
$ docker pull traefik@sha256:6c1049970de79b7703d38773b1634cb9565be5ce2659807108ca08228946b948
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21571319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbf38cb8e98bdb21ebd03bca02621dbdc7dd76d41034db8662757fd1fd142dbc`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 02:50:22 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 02:50:24 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 18 Mar 2020 21:23:49 GMT
COPY file:611156692287f4137768d904cdfca3c57dd2b840528ed03d2b27fbf4a618c79a in / 
# Wed, 18 Mar 2020 21:23:49 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:23:50 GMT
VOLUME [/tmp]
# Wed, 18 Mar 2020 21:23:50 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:23:50 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:f203ccc96c789e6f70d1f0458f88c831c48596578b8dae2c7fe4fd569c9ec0c7`  
		Last Modified: Wed, 18 Mar 2020 21:24:36 GMT  
		Size: 21.1 MB (21112261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:ba73a04b251fd94c0f40da302d18772d0bd6dfd88363d383869da0779187c920
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20227768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73829bbe4d35461654cfdd0078b7e0c390f97454819bc8035f9d9389949cc0f7`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 20 Feb 2020 23:23:27 GMT
COPY file:f457e8adb6c53dc9a59d4eb315e663a1b1eda09623526a54957ad04390140125 in /etc/ssl/certs/ 
# Thu, 20 Feb 2020 23:23:31 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 18 Mar 2020 21:51:25 GMT
COPY file:46207763c5061776ce0c8cc2ede9efbcf14bc283d70e53f63843ebe0e87b2e0c in / 
# Wed, 18 Mar 2020 21:51:25 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:51:26 GMT
VOLUME [/tmp]
# Wed, 18 Mar 2020 21:51:27 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:51:27 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:356b7dc4a9e195c092ad13a4c030815858f9f167d12d16c6a9d8582e2b17ccb6`  
		Last Modified: Wed, 18 Mar 2020 21:52:46 GMT  
		Size: 19.8 MB (19768704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:ad07c1f6ee27f16f698d6ccf409c141e54d5284cf4573a022022e559a3d1587b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19945496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb0471ca83912aa3360a706722088202117b9d4e2c581521db2319aedb51c35`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 01:08:43 GMT
COPY file:f457e8adb6c53dc9a59d4eb315e663a1b1eda09623526a54957ad04390140125 in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 01:08:48 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 18 Mar 2020 21:44:23 GMT
COPY file:4740636fd61ff936bab2e643c72c42f288056018cf20251b49a50374f56a5182 in / 
# Wed, 18 Mar 2020 21:44:24 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:44:25 GMT
VOLUME [/tmp]
# Wed, 18 Mar 2020 21:44:25 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:44:26 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:4c88ce9cc194a14a9a9c0f1b9763af861528373a7c41e0209acc56901b44d872`  
		Last Modified: Wed, 18 Mar 2020 21:45:40 GMT  
		Size: 19.5 MB (19486404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.22`

```console
$ docker pull traefik@sha256:15edd6d0ea71a9707b8a04990d092e3991bb59e4c38a169fe560eb209fe68d62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.22` - linux; amd64

```console
$ docker pull traefik@sha256:6c1049970de79b7703d38773b1634cb9565be5ce2659807108ca08228946b948
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21571319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbf38cb8e98bdb21ebd03bca02621dbdc7dd76d41034db8662757fd1fd142dbc`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 02:50:22 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 02:50:24 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 18 Mar 2020 21:23:49 GMT
COPY file:611156692287f4137768d904cdfca3c57dd2b840528ed03d2b27fbf4a618c79a in / 
# Wed, 18 Mar 2020 21:23:49 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:23:50 GMT
VOLUME [/tmp]
# Wed, 18 Mar 2020 21:23:50 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:23:50 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:f203ccc96c789e6f70d1f0458f88c831c48596578b8dae2c7fe4fd569c9ec0c7`  
		Last Modified: Wed, 18 Mar 2020 21:24:36 GMT  
		Size: 21.1 MB (21112261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.22` - linux; arm variant v6

```console
$ docker pull traefik@sha256:ba73a04b251fd94c0f40da302d18772d0bd6dfd88363d383869da0779187c920
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20227768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73829bbe4d35461654cfdd0078b7e0c390f97454819bc8035f9d9389949cc0f7`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 20 Feb 2020 23:23:27 GMT
COPY file:f457e8adb6c53dc9a59d4eb315e663a1b1eda09623526a54957ad04390140125 in /etc/ssl/certs/ 
# Thu, 20 Feb 2020 23:23:31 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 18 Mar 2020 21:51:25 GMT
COPY file:46207763c5061776ce0c8cc2ede9efbcf14bc283d70e53f63843ebe0e87b2e0c in / 
# Wed, 18 Mar 2020 21:51:25 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:51:26 GMT
VOLUME [/tmp]
# Wed, 18 Mar 2020 21:51:27 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:51:27 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:356b7dc4a9e195c092ad13a4c030815858f9f167d12d16c6a9d8582e2b17ccb6`  
		Last Modified: Wed, 18 Mar 2020 21:52:46 GMT  
		Size: 19.8 MB (19768704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.22` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:ad07c1f6ee27f16f698d6ccf409c141e54d5284cf4573a022022e559a3d1587b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19945496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb0471ca83912aa3360a706722088202117b9d4e2c581521db2319aedb51c35`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 01:08:43 GMT
COPY file:f457e8adb6c53dc9a59d4eb315e663a1b1eda09623526a54957ad04390140125 in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 01:08:48 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 18 Mar 2020 21:44:23 GMT
COPY file:4740636fd61ff936bab2e643c72c42f288056018cf20251b49a50374f56a5182 in / 
# Wed, 18 Mar 2020 21:44:24 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:44:25 GMT
VOLUME [/tmp]
# Wed, 18 Mar 2020 21:44:25 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:44:26 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:4c88ce9cc194a14a9a9c0f1b9763af861528373a7c41e0209acc56901b44d872`  
		Last Modified: Wed, 18 Mar 2020 21:45:40 GMT  
		Size: 19.5 MB (19486404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.22-alpine`

```console
$ docker pull traefik@sha256:0e8a8ced58f5e622a0ce2c74cef71ddee1e451fc28b160c1b84a1a3db8330bbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.22-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:b962d3ac91a9e11c88cf528a618c3679199dbfb42e3287f5bcb6112834636d3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24610153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01698f5f3d38aab7009255cb0128e3d1b64fb9d786deff3b8c8551ca34ba13c9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:23:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.22/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:23:32 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:23:32 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:23:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:23:32 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:23:32 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9821e36a40099dff67072fe099ac945c1ac3714751b0e2cbf22ba73e60b87c2b`  
		Last Modified: Wed, 18 Mar 2020 21:24:25 GMT  
		Size: 21.1 MB (21112646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64290e4840c8dda64c296a123aae5d34803c1807590f1e8d066053467c9cbcd1`  
		Last Modified: Wed, 18 Mar 2020 21:24:21 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.22-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:2924672d57ea80afe7b2fa9f18d2c071ef2b549b919e4706a7432d6ef08bce47
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23084518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fe48847efbf9f8af4e6b5355ba48508038248300193205adb5dc6dbc597335`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:50:14 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.22/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:50:15 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:50:16 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:50:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:50:17 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:50:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:5dde6016f49e2a1d3e9dcd060b23e4c5f0f12235888fcc06a8bd8878efe4cc84`  
		Last Modified: Wed, 18 Mar 2020 21:52:30 GMT  
		Size: 19.8 MB (19768575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e156d270acb91d9191a38c899aaa13302805048ab7487c1cdeeb756768a5b65`  
		Last Modified: Wed, 18 Mar 2020 21:52:24 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.22-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7c4b7a1347754ac471278b488697807abda18b2a1ffbcff3dc49a11cadb2a47c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22906084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2295dec92f083d7445e1910d8cb41e36edae8e7f8c617bb036c4069786538e6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:41:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.22/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:41:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:41:06 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:41:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:41:07 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:41:07 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:4b6fac89a32ef648fc441f3f66feee802e0f63ca2b6461793a9b570667dccedc`  
		Last Modified: Wed, 18 Mar 2020 21:45:23 GMT  
		Size: 19.5 MB (19486597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca4069149f37bbb859c9011c637e6e96f315c0624202c1b9f9e64c0f90da99d`  
		Last Modified: Wed, 18 Mar 2020 21:45:16 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.22-windowsservercore-1809`

```console
$ docker pull traefik@sha256:c45e49ece6fc26eb95c95f320e00d46758767fa2c146440741bd5369d259de5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:1.7.22-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:bd88226dd52059213f633dc9a3bdf0aed30826180a4b179e3ad0ee627d81eb99
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2291136525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d9a993def2d50ea7861006eeae29e3c17544402639ae01c64d56076d13f6dd4`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 18 Mar 2020 21:17:24 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.22/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 18 Mar 2020 21:17:27 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:17:29 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:17:30 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a7fab05ac5ad4b2f665ad71b5c08a81e82bff7ea2fdcbb66c14193d2dd268875`  
		Last Modified: Wed, 11 Mar 2020 01:16:21 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f23cddbd996747d71298787af1bd8bf6d4e4eda66e8bbf74d436d63f37325d`  
		Last Modified: Wed, 18 Mar 2020 21:19:05 GMT  
		Size: 25.8 MB (25795602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2612aaca4eba01ffd479ecfc14152f152c76201b7e0291ac46c22d3997f6a98`  
		Last Modified: Wed, 18 Mar 2020 21:18:59 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2112913d41c0c7ffd73f6f8673cadb8a67731e2e3125c2e91a3d8797f1b400`  
		Last Modified: Wed, 18 Mar 2020 21:18:59 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed1ef7067f20aa0022342f8d741e6cba951ccc3e04a529b05d51bf3021b3b0f`  
		Last Modified: Wed, 18 Mar 2020 21:18:59 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-alpine`

```console
$ docker pull traefik@sha256:0e8a8ced58f5e622a0ce2c74cef71ddee1e451fc28b160c1b84a1a3db8330bbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:b962d3ac91a9e11c88cf528a618c3679199dbfb42e3287f5bcb6112834636d3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24610153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01698f5f3d38aab7009255cb0128e3d1b64fb9d786deff3b8c8551ca34ba13c9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:23:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.22/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:23:32 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:23:32 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:23:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:23:32 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:23:32 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9821e36a40099dff67072fe099ac945c1ac3714751b0e2cbf22ba73e60b87c2b`  
		Last Modified: Wed, 18 Mar 2020 21:24:25 GMT  
		Size: 21.1 MB (21112646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64290e4840c8dda64c296a123aae5d34803c1807590f1e8d066053467c9cbcd1`  
		Last Modified: Wed, 18 Mar 2020 21:24:21 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:2924672d57ea80afe7b2fa9f18d2c071ef2b549b919e4706a7432d6ef08bce47
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23084518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fe48847efbf9f8af4e6b5355ba48508038248300193205adb5dc6dbc597335`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:50:14 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.22/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:50:15 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:50:16 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:50:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:50:17 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:50:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:5dde6016f49e2a1d3e9dcd060b23e4c5f0f12235888fcc06a8bd8878efe4cc84`  
		Last Modified: Wed, 18 Mar 2020 21:52:30 GMT  
		Size: 19.8 MB (19768575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e156d270acb91d9191a38c899aaa13302805048ab7487c1cdeeb756768a5b65`  
		Last Modified: Wed, 18 Mar 2020 21:52:24 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7c4b7a1347754ac471278b488697807abda18b2a1ffbcff3dc49a11cadb2a47c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22906084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2295dec92f083d7445e1910d8cb41e36edae8e7f8c617bb036c4069786538e6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:41:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.22/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:41:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:41:06 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:41:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:41:07 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:41:07 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:4b6fac89a32ef648fc441f3f66feee802e0f63ca2b6461793a9b570667dccedc`  
		Last Modified: Wed, 18 Mar 2020 21:45:23 GMT  
		Size: 19.5 MB (19486597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca4069149f37bbb859c9011c637e6e96f315c0624202c1b9f9e64c0f90da99d`  
		Last Modified: Wed, 18 Mar 2020 21:45:16 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:c45e49ece6fc26eb95c95f320e00d46758767fa2c146440741bd5369d259de5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:1.7-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:bd88226dd52059213f633dc9a3bdf0aed30826180a4b179e3ad0ee627d81eb99
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2291136525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d9a993def2d50ea7861006eeae29e3c17544402639ae01c64d56076d13f6dd4`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 18 Mar 2020 21:17:24 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.22/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 18 Mar 2020 21:17:27 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:17:29 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:17:30 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a7fab05ac5ad4b2f665ad71b5c08a81e82bff7ea2fdcbb66c14193d2dd268875`  
		Last Modified: Wed, 11 Mar 2020 01:16:21 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f23cddbd996747d71298787af1bd8bf6d4e4eda66e8bbf74d436d63f37325d`  
		Last Modified: Wed, 18 Mar 2020 21:19:05 GMT  
		Size: 25.8 MB (25795602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2612aaca4eba01ffd479ecfc14152f152c76201b7e0291ac46c22d3997f6a98`  
		Last Modified: Wed, 18 Mar 2020 21:18:59 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2112913d41c0c7ffd73f6f8673cadb8a67731e2e3125c2e91a3d8797f1b400`  
		Last Modified: Wed, 18 Mar 2020 21:18:59 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed1ef7067f20aa0022342f8d741e6cba951ccc3e04a529b05d51bf3021b3b0f`  
		Last Modified: Wed, 18 Mar 2020 21:18:59 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.1`

```console
$ docker pull traefik@sha256:825521d793f572a3944787c134468017fdd719340fba06be53c33382e33b5ed1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.1` - linux; amd64

```console
$ docker pull traefik@sha256:b648fb36b8b7a16c29b17098ab0d4e3d6b690f3743113d5715b476a86c0c6eb6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23078678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc73dafdaf77f021af5d6e11d26485ef404c9c448041d04e2ab64c02085b45fb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:23:25 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.7/traefik_v2.1.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:23:25 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:23:25 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:23:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:23:26 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:23:26 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.7 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:d23d352c6a6b6e399956a83e278cfbf4a6ee13202799f970464fb64a83191572`  
		Last Modified: Wed, 18 Mar 2020 21:24:15 GMT  
		Size: 19.6 MB (19581171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36778517a2cb14855119773806f3a6beab6c4e85b1dcf74981e652d0079561a9`  
		Last Modified: Wed, 18 Mar 2020 21:24:10 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.1` - linux; arm variant v6

```console
$ docker pull traefik@sha256:d4a0b779bb40f2148d63a9431422cdd9a641c74ef1fcea23de774e454d0aa433
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 MB (21652564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48ee9f0382c3f27923bbd3252f34486b585e3294b5b5825cf10dd3a21bd41d9c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 19 Mar 2020 23:23:46 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.8/traefik_v2.1.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 19 Mar 2020 23:23:49 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 19 Mar 2020 23:23:51 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:23:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Mar 2020 23:23:55 GMT
CMD ["traefik"]
# Thu, 19 Mar 2020 23:23:57 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:53885d3a3b2b3c65397006830e2537614bdb892855376d49405c3d3f57b156f3`  
		Last Modified: Thu, 19 Mar 2020 23:24:51 GMT  
		Size: 18.3 MB (18336621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcd6f2d908241954732cb48c247880bdeaeb4c9941514c06bb5e01a406312c7`  
		Last Modified: Thu, 19 Mar 2020 23:24:45 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:064fbe4896c26fce414a7df2df0a3b0571ccefb73366b2739112b52612ebbf14
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 MB (21453551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eaee0200df033a74b1986f9d77ef02c0efbe5323827d25b39c8481656d1a114`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 20 Mar 2020 01:08:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.8/traefik_v2.1.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 20 Mar 2020 01:08:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 20 Mar 2020 01:08:51 GMT
EXPOSE 80
# Fri, 20 Mar 2020 01:09:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 20 Mar 2020 01:09:09 GMT
CMD ["traefik"]
# Fri, 20 Mar 2020 01:09:13 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:f90c65e62bd1d8a41d60336854858745d85736586b37abe6790a7a6d6f5181ad`  
		Last Modified: Fri, 20 Mar 2020 01:10:09 GMT  
		Size: 18.0 MB (18034065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9bae08bcb1e759e95d0a6764537920273d6cb4815345c68f8682589d015a87`  
		Last Modified: Fri, 20 Mar 2020 01:10:06 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.1.8`

```console
$ docker pull traefik@sha256:c154b732efbc133dd9fb2f75cb997b0078a9acd606c073aecd48bba192d1c9b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.1.8` - linux; arm variant v6

```console
$ docker pull traefik@sha256:d4a0b779bb40f2148d63a9431422cdd9a641c74ef1fcea23de774e454d0aa433
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 MB (21652564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48ee9f0382c3f27923bbd3252f34486b585e3294b5b5825cf10dd3a21bd41d9c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 19 Mar 2020 23:23:46 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.8/traefik_v2.1.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 19 Mar 2020 23:23:49 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 19 Mar 2020 23:23:51 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:23:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Mar 2020 23:23:55 GMT
CMD ["traefik"]
# Thu, 19 Mar 2020 23:23:57 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:53885d3a3b2b3c65397006830e2537614bdb892855376d49405c3d3f57b156f3`  
		Last Modified: Thu, 19 Mar 2020 23:24:51 GMT  
		Size: 18.3 MB (18336621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcd6f2d908241954732cb48c247880bdeaeb4c9941514c06bb5e01a406312c7`  
		Last Modified: Thu, 19 Mar 2020 23:24:45 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.1.8` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:064fbe4896c26fce414a7df2df0a3b0571ccefb73366b2739112b52612ebbf14
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 MB (21453551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eaee0200df033a74b1986f9d77ef02c0efbe5323827d25b39c8481656d1a114`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 20 Mar 2020 01:08:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.8/traefik_v2.1.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 20 Mar 2020 01:08:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 20 Mar 2020 01:08:51 GMT
EXPOSE 80
# Fri, 20 Mar 2020 01:09:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 20 Mar 2020 01:09:09 GMT
CMD ["traefik"]
# Fri, 20 Mar 2020 01:09:13 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:f90c65e62bd1d8a41d60336854858745d85736586b37abe6790a7a6d6f5181ad`  
		Last Modified: Fri, 20 Mar 2020 01:10:09 GMT  
		Size: 18.0 MB (18034065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9bae08bcb1e759e95d0a6764537920273d6cb4815345c68f8682589d015a87`  
		Last Modified: Fri, 20 Mar 2020 01:10:06 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.1.8-windowsservercore-1809`

```console
$ docker pull traefik@sha256:4aee458ca67f38c594327c15417266a1de3c2c0b7da10adfc52a9d3281e71226
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:2.1.8-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:3b931df7ee834cd3981b0feed94aa43c270f61cd9b77fe55a521f2b752f53f51
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2289603149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02b29a74a7f7c2b1610fac17b8e9a47ce49630ce32c1470e065db828d23d08f1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 19 Mar 2020 23:41:52 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.8/traefik_v2.1.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 19 Mar 2020 23:41:56 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:41:58 GMT
ENTRYPOINT ["/traefik"]
# Thu, 19 Mar 2020 23:41:59 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a7fab05ac5ad4b2f665ad71b5c08a81e82bff7ea2fdcbb66c14193d2dd268875`  
		Last Modified: Wed, 11 Mar 2020 01:16:21 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa08490fed3660037a1b158752b8fe631ad840b0f2907c5fc2485a9e14e43ea3`  
		Last Modified: Thu, 19 Mar 2020 23:42:51 GMT  
		Size: 24.3 MB (24262030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97399e32101679e0af4842e21af256551e26a9ee7a8d9eca1324c30fbf93a627`  
		Last Modified: Thu, 19 Mar 2020 23:42:45 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142ff7dfc7b934a74d26c9bf367751fab4187d03eb3a4d53a682baf74371f93d`  
		Last Modified: Thu, 19 Mar 2020 23:42:45 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2695d512369d35885c9793f1d4824dae683f03a4f251b460b87c4c52790df131`  
		Last Modified: Thu, 19 Mar 2020 23:42:45 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:4aee458ca67f38c594327c15417266a1de3c2c0b7da10adfc52a9d3281e71226
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:2.1-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:3b931df7ee834cd3981b0feed94aa43c270f61cd9b77fe55a521f2b752f53f51
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2289603149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02b29a74a7f7c2b1610fac17b8e9a47ce49630ce32c1470e065db828d23d08f1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 19 Mar 2020 23:41:52 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.8/traefik_v2.1.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 19 Mar 2020 23:41:56 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:41:58 GMT
ENTRYPOINT ["/traefik"]
# Thu, 19 Mar 2020 23:41:59 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a7fab05ac5ad4b2f665ad71b5c08a81e82bff7ea2fdcbb66c14193d2dd268875`  
		Last Modified: Wed, 11 Mar 2020 01:16:21 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa08490fed3660037a1b158752b8fe631ad840b0f2907c5fc2485a9e14e43ea3`  
		Last Modified: Thu, 19 Mar 2020 23:42:51 GMT  
		Size: 24.3 MB (24262030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97399e32101679e0af4842e21af256551e26a9ee7a8d9eca1324c30fbf93a627`  
		Last Modified: Thu, 19 Mar 2020 23:42:45 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142ff7dfc7b934a74d26c9bf367751fab4187d03eb3a4d53a682baf74371f93d`  
		Last Modified: Thu, 19 Mar 2020 23:42:45 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2695d512369d35885c9793f1d4824dae683f03a4f251b460b87c4c52790df131`  
		Last Modified: Thu, 19 Mar 2020 23:42:45 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.2`

```console
$ docker pull traefik@sha256:c00ad870b0a5a508a76723c5fd7dba74ee7d243823d20c1dae3a976de6e0a936
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.2` - linux; amd64

```console
$ docker pull traefik@sha256:a638691e542297b5e9c0e418aac95b3cf73d45177e9682d6bca73149c3c69bab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.8 MB (24780272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d1e6db5348027b0b036e274331d64662f34d66206a1ceaef0b17851c7f6885`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:23:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0-rc3/traefik_v2.2.0-rc3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:23:19 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:23:19 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:23:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:23:19 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:23:19 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:463bdeb7d88cb685b1d681a3d5c74d95efea6e0977efbe675e5171f92fd80322`  
		Last Modified: Wed, 18 Mar 2020 21:24:05 GMT  
		Size: 21.3 MB (21282765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3468d963bd074dbab9c5b9541fef31413dec4bd0eeb723b9cae6b305eb5033`  
		Last Modified: Wed, 18 Mar 2020 21:24:01 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.2` - linux; arm variant v6

```console
$ docker pull traefik@sha256:3f9230e23558384ec74667d3bb267a300a0620a5f6e405cada6dd5041c6dbaaf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.3 MB (23304555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a133c917280780e2eb70f42f1223f6652a4c727c1b412a3cc0294e83e252503a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 19 Mar 2020 23:23:28 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0-rc4/traefik_v2.2.0-rc4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 19 Mar 2020 23:23:30 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 19 Mar 2020 23:23:30 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:23:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Mar 2020 23:23:32 GMT
CMD ["traefik"]
# Thu, 19 Mar 2020 23:23:33 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:10a7ce7075e3cb97febbff60365fb86b17a86c0294b17c66364899585f12e1c4`  
		Last Modified: Thu, 19 Mar 2020 23:24:36 GMT  
		Size: 20.0 MB (19988611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688ec71b4885f6ba4c9d6f9c1ca43724c7dbc4609ba9d6f566fbfa8f604ad9c0`  
		Last Modified: Thu, 19 Mar 2020 23:24:29 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.2` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:b8e90b0dfa530d3ccfe3571f7b4fa950820de68c5856468a2e1096c11289683b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23052008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad21ca0460e4eb9c7f51c7bacdda2c7ab8eac9146c62e43216e7196d8d35e56f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 20 Mar 2020 01:07:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0-rc4/traefik_v2.2.0-rc4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 20 Mar 2020 01:07:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 20 Mar 2020 01:07:53 GMT
EXPOSE 80
# Fri, 20 Mar 2020 01:08:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 20 Mar 2020 01:08:05 GMT
CMD ["traefik"]
# Fri, 20 Mar 2020 01:08:08 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:45222051a4be92d7d44b388d03292f59f1af91178dedc7bf90a9a597cc018d1d`  
		Last Modified: Fri, 20 Mar 2020 01:09:54 GMT  
		Size: 19.6 MB (19632522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb2aaf6eb4c73fcc17336c4f6603672d042551a0a0763019d9c93882805906ab`  
		Last Modified: Fri, 20 Mar 2020 01:09:47 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.2.0-rc4`

```console
$ docker pull traefik@sha256:b2acf6d39f118c4a57152ae1292fb17af09eb0178bc9a3a0212a4dd43a9f76be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.2.0-rc4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:3f9230e23558384ec74667d3bb267a300a0620a5f6e405cada6dd5041c6dbaaf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.3 MB (23304555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a133c917280780e2eb70f42f1223f6652a4c727c1b412a3cc0294e83e252503a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 19 Mar 2020 23:23:28 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0-rc4/traefik_v2.2.0-rc4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 19 Mar 2020 23:23:30 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 19 Mar 2020 23:23:30 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:23:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Mar 2020 23:23:32 GMT
CMD ["traefik"]
# Thu, 19 Mar 2020 23:23:33 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:10a7ce7075e3cb97febbff60365fb86b17a86c0294b17c66364899585f12e1c4`  
		Last Modified: Thu, 19 Mar 2020 23:24:36 GMT  
		Size: 20.0 MB (19988611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688ec71b4885f6ba4c9d6f9c1ca43724c7dbc4609ba9d6f566fbfa8f604ad9c0`  
		Last Modified: Thu, 19 Mar 2020 23:24:29 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.2.0-rc4` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:b8e90b0dfa530d3ccfe3571f7b4fa950820de68c5856468a2e1096c11289683b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23052008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad21ca0460e4eb9c7f51c7bacdda2c7ab8eac9146c62e43216e7196d8d35e56f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 20 Mar 2020 01:07:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0-rc4/traefik_v2.2.0-rc4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 20 Mar 2020 01:07:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 20 Mar 2020 01:07:53 GMT
EXPOSE 80
# Fri, 20 Mar 2020 01:08:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 20 Mar 2020 01:08:05 GMT
CMD ["traefik"]
# Fri, 20 Mar 2020 01:08:08 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:45222051a4be92d7d44b388d03292f59f1af91178dedc7bf90a9a597cc018d1d`  
		Last Modified: Fri, 20 Mar 2020 01:09:54 GMT  
		Size: 19.6 MB (19632522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb2aaf6eb4c73fcc17336c4f6603672d042551a0a0763019d9c93882805906ab`  
		Last Modified: Fri, 20 Mar 2020 01:09:47 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.2.0-rc4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:10b613c0d809a2f32e3f1f05a4d1bf8948740b300edc48c0db647d89ded615a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:2.2.0-rc4-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:be5249e8a1f004bc3b704f5f678a716baeb1e02cbabf159eb439b82457d3cadf
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2291275576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e276e79ace0d8ef3779cc569768475cf7763dcb4753b2da424149790667851c1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 19 Mar 2020 23:40:57 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.2.0-rc4/traefik_v2.2.0-rc4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 19 Mar 2020 23:41:01 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:41:02 GMT
ENTRYPOINT ["/traefik"]
# Thu, 19 Mar 2020 23:41:03 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a7fab05ac5ad4b2f665ad71b5c08a81e82bff7ea2fdcbb66c14193d2dd268875`  
		Last Modified: Wed, 11 Mar 2020 01:16:21 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:549f06fe79c6ff9fe97ad90025e8fa1f62dc9cc3b2d1a223c2be32e8e944ff9e`  
		Last Modified: Thu, 19 Mar 2020 23:42:30 GMT  
		Size: 25.9 MB (25934473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465d2f7acd904d7ca8da43eb4cdd73475b80ccce5ba79a88d9968266c4bad07f`  
		Last Modified: Thu, 19 Mar 2020 23:42:24 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809f97326d00cd242ff10557bd548b8db16c340fd5d7fc274f3282623f542bbb`  
		Last Modified: Thu, 19 Mar 2020 23:42:24 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e27a6ecc6db484f65e2587cb61e379ddb398f17469e292905230bc60e36fc04`  
		Last Modified: Thu, 19 Mar 2020 23:42:24 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:10b613c0d809a2f32e3f1f05a4d1bf8948740b300edc48c0db647d89ded615a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:2.2-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:be5249e8a1f004bc3b704f5f678a716baeb1e02cbabf159eb439b82457d3cadf
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2291275576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e276e79ace0d8ef3779cc569768475cf7763dcb4753b2da424149790667851c1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 19 Mar 2020 23:40:57 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.2.0-rc4/traefik_v2.2.0-rc4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 19 Mar 2020 23:41:01 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:41:02 GMT
ENTRYPOINT ["/traefik"]
# Thu, 19 Mar 2020 23:41:03 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a7fab05ac5ad4b2f665ad71b5c08a81e82bff7ea2fdcbb66c14193d2dd268875`  
		Last Modified: Wed, 11 Mar 2020 01:16:21 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:549f06fe79c6ff9fe97ad90025e8fa1f62dc9cc3b2d1a223c2be32e8e944ff9e`  
		Last Modified: Thu, 19 Mar 2020 23:42:30 GMT  
		Size: 25.9 MB (25934473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465d2f7acd904d7ca8da43eb4cdd73475b80ccce5ba79a88d9968266c4bad07f`  
		Last Modified: Thu, 19 Mar 2020 23:42:24 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809f97326d00cd242ff10557bd548b8db16c340fd5d7fc274f3282623f542bbb`  
		Last Modified: Thu, 19 Mar 2020 23:42:24 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e27a6ecc6db484f65e2587cb61e379ddb398f17469e292905230bc60e36fc04`  
		Last Modified: Thu, 19 Mar 2020 23:42:24 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:cantal`

```console
$ docker pull traefik@sha256:825521d793f572a3944787c134468017fdd719340fba06be53c33382e33b5ed1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:cantal` - linux; amd64

```console
$ docker pull traefik@sha256:b648fb36b8b7a16c29b17098ab0d4e3d6b690f3743113d5715b476a86c0c6eb6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23078678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc73dafdaf77f021af5d6e11d26485ef404c9c448041d04e2ab64c02085b45fb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:23:25 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.7/traefik_v2.1.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:23:25 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:23:25 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:23:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:23:26 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:23:26 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.7 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:d23d352c6a6b6e399956a83e278cfbf4a6ee13202799f970464fb64a83191572`  
		Last Modified: Wed, 18 Mar 2020 21:24:15 GMT  
		Size: 19.6 MB (19581171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36778517a2cb14855119773806f3a6beab6c4e85b1dcf74981e652d0079561a9`  
		Last Modified: Wed, 18 Mar 2020 21:24:10 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:cantal` - linux; arm variant v6

```console
$ docker pull traefik@sha256:d4a0b779bb40f2148d63a9431422cdd9a641c74ef1fcea23de774e454d0aa433
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 MB (21652564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48ee9f0382c3f27923bbd3252f34486b585e3294b5b5825cf10dd3a21bd41d9c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 19 Mar 2020 23:23:46 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.8/traefik_v2.1.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 19 Mar 2020 23:23:49 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 19 Mar 2020 23:23:51 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:23:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Mar 2020 23:23:55 GMT
CMD ["traefik"]
# Thu, 19 Mar 2020 23:23:57 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:53885d3a3b2b3c65397006830e2537614bdb892855376d49405c3d3f57b156f3`  
		Last Modified: Thu, 19 Mar 2020 23:24:51 GMT  
		Size: 18.3 MB (18336621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcd6f2d908241954732cb48c247880bdeaeb4c9941514c06bb5e01a406312c7`  
		Last Modified: Thu, 19 Mar 2020 23:24:45 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:cantal` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:064fbe4896c26fce414a7df2df0a3b0571ccefb73366b2739112b52612ebbf14
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 MB (21453551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eaee0200df033a74b1986f9d77ef02c0efbe5323827d25b39c8481656d1a114`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 20 Mar 2020 01:08:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.8/traefik_v2.1.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 20 Mar 2020 01:08:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 20 Mar 2020 01:08:51 GMT
EXPOSE 80
# Fri, 20 Mar 2020 01:09:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 20 Mar 2020 01:09:09 GMT
CMD ["traefik"]
# Fri, 20 Mar 2020 01:09:13 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:f90c65e62bd1d8a41d60336854858745d85736586b37abe6790a7a6d6f5181ad`  
		Last Modified: Fri, 20 Mar 2020 01:10:09 GMT  
		Size: 18.0 MB (18034065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9bae08bcb1e759e95d0a6764537920273d6cb4815345c68f8682589d015a87`  
		Last Modified: Fri, 20 Mar 2020 01:10:06 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:cantal-windowsservercore-1809`

```console
$ docker pull traefik@sha256:4aee458ca67f38c594327c15417266a1de3c2c0b7da10adfc52a9d3281e71226
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:cantal-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:3b931df7ee834cd3981b0feed94aa43c270f61cd9b77fe55a521f2b752f53f51
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2289603149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02b29a74a7f7c2b1610fac17b8e9a47ce49630ce32c1470e065db828d23d08f1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 19 Mar 2020 23:41:52 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.8/traefik_v2.1.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 19 Mar 2020 23:41:56 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:41:58 GMT
ENTRYPOINT ["/traefik"]
# Thu, 19 Mar 2020 23:41:59 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a7fab05ac5ad4b2f665ad71b5c08a81e82bff7ea2fdcbb66c14193d2dd268875`  
		Last Modified: Wed, 11 Mar 2020 01:16:21 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa08490fed3660037a1b158752b8fe631ad840b0f2907c5fc2485a9e14e43ea3`  
		Last Modified: Thu, 19 Mar 2020 23:42:51 GMT  
		Size: 24.3 MB (24262030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97399e32101679e0af4842e21af256551e26a9ee7a8d9eca1324c30fbf93a627`  
		Last Modified: Thu, 19 Mar 2020 23:42:45 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142ff7dfc7b934a74d26c9bf367751fab4187d03eb3a4d53a682baf74371f93d`  
		Last Modified: Thu, 19 Mar 2020 23:42:45 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2695d512369d35885c9793f1d4824dae683f03a4f251b460b87c4c52790df131`  
		Last Modified: Thu, 19 Mar 2020 23:42:45 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:chevrotin`

```console
$ docker pull traefik@sha256:c00ad870b0a5a508a76723c5fd7dba74ee7d243823d20c1dae3a976de6e0a936
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:chevrotin` - linux; amd64

```console
$ docker pull traefik@sha256:a638691e542297b5e9c0e418aac95b3cf73d45177e9682d6bca73149c3c69bab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.8 MB (24780272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d1e6db5348027b0b036e274331d64662f34d66206a1ceaef0b17851c7f6885`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:23:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0-rc3/traefik_v2.2.0-rc3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:23:19 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:23:19 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:23:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:23:19 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:23:19 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:463bdeb7d88cb685b1d681a3d5c74d95efea6e0977efbe675e5171f92fd80322`  
		Last Modified: Wed, 18 Mar 2020 21:24:05 GMT  
		Size: 21.3 MB (21282765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3468d963bd074dbab9c5b9541fef31413dec4bd0eeb723b9cae6b305eb5033`  
		Last Modified: Wed, 18 Mar 2020 21:24:01 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:chevrotin` - linux; arm variant v6

```console
$ docker pull traefik@sha256:3f9230e23558384ec74667d3bb267a300a0620a5f6e405cada6dd5041c6dbaaf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.3 MB (23304555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a133c917280780e2eb70f42f1223f6652a4c727c1b412a3cc0294e83e252503a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 19 Mar 2020 23:23:28 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0-rc4/traefik_v2.2.0-rc4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 19 Mar 2020 23:23:30 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 19 Mar 2020 23:23:30 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:23:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Mar 2020 23:23:32 GMT
CMD ["traefik"]
# Thu, 19 Mar 2020 23:23:33 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:10a7ce7075e3cb97febbff60365fb86b17a86c0294b17c66364899585f12e1c4`  
		Last Modified: Thu, 19 Mar 2020 23:24:36 GMT  
		Size: 20.0 MB (19988611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688ec71b4885f6ba4c9d6f9c1ca43724c7dbc4609ba9d6f566fbfa8f604ad9c0`  
		Last Modified: Thu, 19 Mar 2020 23:24:29 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:chevrotin` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:b8e90b0dfa530d3ccfe3571f7b4fa950820de68c5856468a2e1096c11289683b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23052008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad21ca0460e4eb9c7f51c7bacdda2c7ab8eac9146c62e43216e7196d8d35e56f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 20 Mar 2020 01:07:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0-rc4/traefik_v2.2.0-rc4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 20 Mar 2020 01:07:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 20 Mar 2020 01:07:53 GMT
EXPOSE 80
# Fri, 20 Mar 2020 01:08:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 20 Mar 2020 01:08:05 GMT
CMD ["traefik"]
# Fri, 20 Mar 2020 01:08:08 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:45222051a4be92d7d44b388d03292f59f1af91178dedc7bf90a9a597cc018d1d`  
		Last Modified: Fri, 20 Mar 2020 01:09:54 GMT  
		Size: 19.6 MB (19632522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb2aaf6eb4c73fcc17336c4f6603672d042551a0a0763019d9c93882805906ab`  
		Last Modified: Fri, 20 Mar 2020 01:09:47 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:chevrotin-windowsservercore-1809`

```console
$ docker pull traefik@sha256:10b613c0d809a2f32e3f1f05a4d1bf8948740b300edc48c0db647d89ded615a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:chevrotin-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:be5249e8a1f004bc3b704f5f678a716baeb1e02cbabf159eb439b82457d3cadf
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2291275576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e276e79ace0d8ef3779cc569768475cf7763dcb4753b2da424149790667851c1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 19 Mar 2020 23:40:57 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.2.0-rc4/traefik_v2.2.0-rc4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 19 Mar 2020 23:41:01 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:41:02 GMT
ENTRYPOINT ["/traefik"]
# Thu, 19 Mar 2020 23:41:03 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a7fab05ac5ad4b2f665ad71b5c08a81e82bff7ea2fdcbb66c14193d2dd268875`  
		Last Modified: Wed, 11 Mar 2020 01:16:21 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:549f06fe79c6ff9fe97ad90025e8fa1f62dc9cc3b2d1a223c2be32e8e944ff9e`  
		Last Modified: Thu, 19 Mar 2020 23:42:30 GMT  
		Size: 25.9 MB (25934473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465d2f7acd904d7ca8da43eb4cdd73475b80ccce5ba79a88d9968266c4bad07f`  
		Last Modified: Thu, 19 Mar 2020 23:42:24 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809f97326d00cd242ff10557bd548b8db16c340fd5d7fc274f3282623f542bbb`  
		Last Modified: Thu, 19 Mar 2020 23:42:24 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e27a6ecc6db484f65e2587cb61e379ddb398f17469e292905230bc60e36fc04`  
		Last Modified: Thu, 19 Mar 2020 23:42:24 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:825521d793f572a3944787c134468017fdd719340fba06be53c33382e33b5ed1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:b648fb36b8b7a16c29b17098ab0d4e3d6b690f3743113d5715b476a86c0c6eb6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23078678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc73dafdaf77f021af5d6e11d26485ef404c9c448041d04e2ab64c02085b45fb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:23:25 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.7/traefik_v2.1.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:23:25 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:23:25 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:23:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:23:26 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:23:26 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.7 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:d23d352c6a6b6e399956a83e278cfbf4a6ee13202799f970464fb64a83191572`  
		Last Modified: Wed, 18 Mar 2020 21:24:15 GMT  
		Size: 19.6 MB (19581171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36778517a2cb14855119773806f3a6beab6c4e85b1dcf74981e652d0079561a9`  
		Last Modified: Wed, 18 Mar 2020 21:24:10 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:d4a0b779bb40f2148d63a9431422cdd9a641c74ef1fcea23de774e454d0aa433
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 MB (21652564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48ee9f0382c3f27923bbd3252f34486b585e3294b5b5825cf10dd3a21bd41d9c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 19 Mar 2020 23:23:46 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.8/traefik_v2.1.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 19 Mar 2020 23:23:49 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 19 Mar 2020 23:23:51 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:23:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Mar 2020 23:23:55 GMT
CMD ["traefik"]
# Thu, 19 Mar 2020 23:23:57 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:53885d3a3b2b3c65397006830e2537614bdb892855376d49405c3d3f57b156f3`  
		Last Modified: Thu, 19 Mar 2020 23:24:51 GMT  
		Size: 18.3 MB (18336621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcd6f2d908241954732cb48c247880bdeaeb4c9941514c06bb5e01a406312c7`  
		Last Modified: Thu, 19 Mar 2020 23:24:45 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:064fbe4896c26fce414a7df2df0a3b0571ccefb73366b2739112b52612ebbf14
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 MB (21453551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eaee0200df033a74b1986f9d77ef02c0efbe5323827d25b39c8481656d1a114`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 20 Mar 2020 01:08:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.8/traefik_v2.1.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 20 Mar 2020 01:08:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 20 Mar 2020 01:08:51 GMT
EXPOSE 80
# Fri, 20 Mar 2020 01:09:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 20 Mar 2020 01:09:09 GMT
CMD ["traefik"]
# Fri, 20 Mar 2020 01:09:13 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:f90c65e62bd1d8a41d60336854858745d85736586b37abe6790a7a6d6f5181ad`  
		Last Modified: Fri, 20 Mar 2020 01:10:09 GMT  
		Size: 18.0 MB (18034065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9bae08bcb1e759e95d0a6764537920273d6cb4815345c68f8682589d015a87`  
		Last Modified: Fri, 20 Mar 2020 01:10:06 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles`

```console
$ docker pull traefik@sha256:15edd6d0ea71a9707b8a04990d092e3991bb59e4c38a169fe560eb209fe68d62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles` - linux; amd64

```console
$ docker pull traefik@sha256:6c1049970de79b7703d38773b1634cb9565be5ce2659807108ca08228946b948
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21571319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbf38cb8e98bdb21ebd03bca02621dbdc7dd76d41034db8662757fd1fd142dbc`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 02:50:22 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 02:50:24 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 18 Mar 2020 21:23:49 GMT
COPY file:611156692287f4137768d904cdfca3c57dd2b840528ed03d2b27fbf4a618c79a in / 
# Wed, 18 Mar 2020 21:23:49 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:23:50 GMT
VOLUME [/tmp]
# Wed, 18 Mar 2020 21:23:50 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:23:50 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:f203ccc96c789e6f70d1f0458f88c831c48596578b8dae2c7fe4fd569c9ec0c7`  
		Last Modified: Wed, 18 Mar 2020 21:24:36 GMT  
		Size: 21.1 MB (21112261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm variant v6

```console
$ docker pull traefik@sha256:ba73a04b251fd94c0f40da302d18772d0bd6dfd88363d383869da0779187c920
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20227768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73829bbe4d35461654cfdd0078b7e0c390f97454819bc8035f9d9389949cc0f7`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 20 Feb 2020 23:23:27 GMT
COPY file:f457e8adb6c53dc9a59d4eb315e663a1b1eda09623526a54957ad04390140125 in /etc/ssl/certs/ 
# Thu, 20 Feb 2020 23:23:31 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 18 Mar 2020 21:51:25 GMT
COPY file:46207763c5061776ce0c8cc2ede9efbcf14bc283d70e53f63843ebe0e87b2e0c in / 
# Wed, 18 Mar 2020 21:51:25 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:51:26 GMT
VOLUME [/tmp]
# Wed, 18 Mar 2020 21:51:27 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:51:27 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:356b7dc4a9e195c092ad13a4c030815858f9f167d12d16c6a9d8582e2b17ccb6`  
		Last Modified: Wed, 18 Mar 2020 21:52:46 GMT  
		Size: 19.8 MB (19768704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:ad07c1f6ee27f16f698d6ccf409c141e54d5284cf4573a022022e559a3d1587b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19945496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb0471ca83912aa3360a706722088202117b9d4e2c581521db2319aedb51c35`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 01:08:43 GMT
COPY file:f457e8adb6c53dc9a59d4eb315e663a1b1eda09623526a54957ad04390140125 in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 01:08:48 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 18 Mar 2020 21:44:23 GMT
COPY file:4740636fd61ff936bab2e643c72c42f288056018cf20251b49a50374f56a5182 in / 
# Wed, 18 Mar 2020 21:44:24 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:44:25 GMT
VOLUME [/tmp]
# Wed, 18 Mar 2020 21:44:25 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:44:26 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:4c88ce9cc194a14a9a9c0f1b9763af861528373a7c41e0209acc56901b44d872`  
		Last Modified: Wed, 18 Mar 2020 21:45:40 GMT  
		Size: 19.5 MB (19486404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-alpine`

```console
$ docker pull traefik@sha256:0e8a8ced58f5e622a0ce2c74cef71ddee1e451fc28b160c1b84a1a3db8330bbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:b962d3ac91a9e11c88cf528a618c3679199dbfb42e3287f5bcb6112834636d3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24610153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01698f5f3d38aab7009255cb0128e3d1b64fb9d786deff3b8c8551ca34ba13c9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:23:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.22/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:23:32 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:23:32 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:23:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:23:32 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:23:32 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9821e36a40099dff67072fe099ac945c1ac3714751b0e2cbf22ba73e60b87c2b`  
		Last Modified: Wed, 18 Mar 2020 21:24:25 GMT  
		Size: 21.1 MB (21112646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64290e4840c8dda64c296a123aae5d34803c1807590f1e8d066053467c9cbcd1`  
		Last Modified: Wed, 18 Mar 2020 21:24:21 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:2924672d57ea80afe7b2fa9f18d2c071ef2b549b919e4706a7432d6ef08bce47
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23084518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fe48847efbf9f8af4e6b5355ba48508038248300193205adb5dc6dbc597335`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:50:14 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.22/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:50:15 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:50:16 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:50:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:50:17 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:50:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:5dde6016f49e2a1d3e9dcd060b23e4c5f0f12235888fcc06a8bd8878efe4cc84`  
		Last Modified: Wed, 18 Mar 2020 21:52:30 GMT  
		Size: 19.8 MB (19768575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e156d270acb91d9191a38c899aaa13302805048ab7487c1cdeeb756768a5b65`  
		Last Modified: Wed, 18 Mar 2020 21:52:24 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7c4b7a1347754ac471278b488697807abda18b2a1ffbcff3dc49a11cadb2a47c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22906084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2295dec92f083d7445e1910d8cb41e36edae8e7f8c617bb036c4069786538e6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:41:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.22/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:41:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:41:06 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:41:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:41:07 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:41:07 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:4b6fac89a32ef648fc441f3f66feee802e0f63ca2b6461793a9b570667dccedc`  
		Last Modified: Wed, 18 Mar 2020 21:45:23 GMT  
		Size: 19.5 MB (19486597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca4069149f37bbb859c9011c637e6e96f315c0624202c1b9f9e64c0f90da99d`  
		Last Modified: Wed, 18 Mar 2020 21:45:16 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-windowsservercore-1809`

```console
$ docker pull traefik@sha256:c45e49ece6fc26eb95c95f320e00d46758767fa2c146440741bd5369d259de5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:bd88226dd52059213f633dc9a3bdf0aed30826180a4b179e3ad0ee627d81eb99
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2291136525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d9a993def2d50ea7861006eeae29e3c17544402639ae01c64d56076d13f6dd4`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 18 Mar 2020 21:17:24 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.22/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 18 Mar 2020 21:17:27 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:17:29 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:17:30 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a7fab05ac5ad4b2f665ad71b5c08a81e82bff7ea2fdcbb66c14193d2dd268875`  
		Last Modified: Wed, 11 Mar 2020 01:16:21 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f23cddbd996747d71298787af1bd8bf6d4e4eda66e8bbf74d436d63f37325d`  
		Last Modified: Wed, 18 Mar 2020 21:19:05 GMT  
		Size: 25.8 MB (25795602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2612aaca4eba01ffd479ecfc14152f152c76201b7e0291ac46c22d3997f6a98`  
		Last Modified: Wed, 18 Mar 2020 21:18:59 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2112913d41c0c7ffd73f6f8673cadb8a67731e2e3125c2e91a3d8797f1b400`  
		Last Modified: Wed, 18 Mar 2020 21:18:59 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed1ef7067f20aa0022342f8d741e6cba951ccc3e04a529b05d51bf3021b3b0f`  
		Last Modified: Wed, 18 Mar 2020 21:18:59 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7`

```console
$ docker pull traefik@sha256:15edd6d0ea71a9707b8a04990d092e3991bb59e4c38a169fe560eb209fe68d62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7` - linux; amd64

```console
$ docker pull traefik@sha256:6c1049970de79b7703d38773b1634cb9565be5ce2659807108ca08228946b948
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21571319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbf38cb8e98bdb21ebd03bca02621dbdc7dd76d41034db8662757fd1fd142dbc`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 02:50:22 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 02:50:24 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 18 Mar 2020 21:23:49 GMT
COPY file:611156692287f4137768d904cdfca3c57dd2b840528ed03d2b27fbf4a618c79a in / 
# Wed, 18 Mar 2020 21:23:49 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:23:50 GMT
VOLUME [/tmp]
# Wed, 18 Mar 2020 21:23:50 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:23:50 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:f203ccc96c789e6f70d1f0458f88c831c48596578b8dae2c7fe4fd569c9ec0c7`  
		Last Modified: Wed, 18 Mar 2020 21:24:36 GMT  
		Size: 21.1 MB (21112261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:ba73a04b251fd94c0f40da302d18772d0bd6dfd88363d383869da0779187c920
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20227768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73829bbe4d35461654cfdd0078b7e0c390f97454819bc8035f9d9389949cc0f7`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 20 Feb 2020 23:23:27 GMT
COPY file:f457e8adb6c53dc9a59d4eb315e663a1b1eda09623526a54957ad04390140125 in /etc/ssl/certs/ 
# Thu, 20 Feb 2020 23:23:31 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 18 Mar 2020 21:51:25 GMT
COPY file:46207763c5061776ce0c8cc2ede9efbcf14bc283d70e53f63843ebe0e87b2e0c in / 
# Wed, 18 Mar 2020 21:51:25 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:51:26 GMT
VOLUME [/tmp]
# Wed, 18 Mar 2020 21:51:27 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:51:27 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:356b7dc4a9e195c092ad13a4c030815858f9f167d12d16c6a9d8582e2b17ccb6`  
		Last Modified: Wed, 18 Mar 2020 21:52:46 GMT  
		Size: 19.8 MB (19768704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:ad07c1f6ee27f16f698d6ccf409c141e54d5284cf4573a022022e559a3d1587b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19945496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb0471ca83912aa3360a706722088202117b9d4e2c581521db2319aedb51c35`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 01:08:43 GMT
COPY file:f457e8adb6c53dc9a59d4eb315e663a1b1eda09623526a54957ad04390140125 in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 01:08:48 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 18 Mar 2020 21:44:23 GMT
COPY file:4740636fd61ff936bab2e643c72c42f288056018cf20251b49a50374f56a5182 in / 
# Wed, 18 Mar 2020 21:44:24 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:44:25 GMT
VOLUME [/tmp]
# Wed, 18 Mar 2020 21:44:25 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:44:26 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:4c88ce9cc194a14a9a9c0f1b9763af861528373a7c41e0209acc56901b44d872`  
		Last Modified: Wed, 18 Mar 2020 21:45:40 GMT  
		Size: 19.5 MB (19486404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.22`

```console
$ docker pull traefik@sha256:15edd6d0ea71a9707b8a04990d092e3991bb59e4c38a169fe560eb209fe68d62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.22` - linux; amd64

```console
$ docker pull traefik@sha256:6c1049970de79b7703d38773b1634cb9565be5ce2659807108ca08228946b948
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21571319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbf38cb8e98bdb21ebd03bca02621dbdc7dd76d41034db8662757fd1fd142dbc`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 02:50:22 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 02:50:24 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 18 Mar 2020 21:23:49 GMT
COPY file:611156692287f4137768d904cdfca3c57dd2b840528ed03d2b27fbf4a618c79a in / 
# Wed, 18 Mar 2020 21:23:49 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:23:50 GMT
VOLUME [/tmp]
# Wed, 18 Mar 2020 21:23:50 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:23:50 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:f203ccc96c789e6f70d1f0458f88c831c48596578b8dae2c7fe4fd569c9ec0c7`  
		Last Modified: Wed, 18 Mar 2020 21:24:36 GMT  
		Size: 21.1 MB (21112261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.22` - linux; arm variant v6

```console
$ docker pull traefik@sha256:ba73a04b251fd94c0f40da302d18772d0bd6dfd88363d383869da0779187c920
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20227768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73829bbe4d35461654cfdd0078b7e0c390f97454819bc8035f9d9389949cc0f7`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 20 Feb 2020 23:23:27 GMT
COPY file:f457e8adb6c53dc9a59d4eb315e663a1b1eda09623526a54957ad04390140125 in /etc/ssl/certs/ 
# Thu, 20 Feb 2020 23:23:31 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 18 Mar 2020 21:51:25 GMT
COPY file:46207763c5061776ce0c8cc2ede9efbcf14bc283d70e53f63843ebe0e87b2e0c in / 
# Wed, 18 Mar 2020 21:51:25 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:51:26 GMT
VOLUME [/tmp]
# Wed, 18 Mar 2020 21:51:27 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:51:27 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:356b7dc4a9e195c092ad13a4c030815858f9f167d12d16c6a9d8582e2b17ccb6`  
		Last Modified: Wed, 18 Mar 2020 21:52:46 GMT  
		Size: 19.8 MB (19768704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.22` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:ad07c1f6ee27f16f698d6ccf409c141e54d5284cf4573a022022e559a3d1587b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19945496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb0471ca83912aa3360a706722088202117b9d4e2c581521db2319aedb51c35`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 01:08:43 GMT
COPY file:f457e8adb6c53dc9a59d4eb315e663a1b1eda09623526a54957ad04390140125 in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 01:08:48 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 18 Mar 2020 21:44:23 GMT
COPY file:4740636fd61ff936bab2e643c72c42f288056018cf20251b49a50374f56a5182 in / 
# Wed, 18 Mar 2020 21:44:24 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:44:25 GMT
VOLUME [/tmp]
# Wed, 18 Mar 2020 21:44:25 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:44:26 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:4c88ce9cc194a14a9a9c0f1b9763af861528373a7c41e0209acc56901b44d872`  
		Last Modified: Wed, 18 Mar 2020 21:45:40 GMT  
		Size: 19.5 MB (19486404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.22-alpine`

```console
$ docker pull traefik@sha256:0e8a8ced58f5e622a0ce2c74cef71ddee1e451fc28b160c1b84a1a3db8330bbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.22-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:b962d3ac91a9e11c88cf528a618c3679199dbfb42e3287f5bcb6112834636d3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24610153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01698f5f3d38aab7009255cb0128e3d1b64fb9d786deff3b8c8551ca34ba13c9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:23:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.22/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:23:32 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:23:32 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:23:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:23:32 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:23:32 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9821e36a40099dff67072fe099ac945c1ac3714751b0e2cbf22ba73e60b87c2b`  
		Last Modified: Wed, 18 Mar 2020 21:24:25 GMT  
		Size: 21.1 MB (21112646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64290e4840c8dda64c296a123aae5d34803c1807590f1e8d066053467c9cbcd1`  
		Last Modified: Wed, 18 Mar 2020 21:24:21 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.22-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:2924672d57ea80afe7b2fa9f18d2c071ef2b549b919e4706a7432d6ef08bce47
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23084518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fe48847efbf9f8af4e6b5355ba48508038248300193205adb5dc6dbc597335`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:50:14 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.22/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:50:15 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:50:16 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:50:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:50:17 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:50:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:5dde6016f49e2a1d3e9dcd060b23e4c5f0f12235888fcc06a8bd8878efe4cc84`  
		Last Modified: Wed, 18 Mar 2020 21:52:30 GMT  
		Size: 19.8 MB (19768575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e156d270acb91d9191a38c899aaa13302805048ab7487c1cdeeb756768a5b65`  
		Last Modified: Wed, 18 Mar 2020 21:52:24 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.22-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7c4b7a1347754ac471278b488697807abda18b2a1ffbcff3dc49a11cadb2a47c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22906084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2295dec92f083d7445e1910d8cb41e36edae8e7f8c617bb036c4069786538e6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:41:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.22/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:41:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:41:06 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:41:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:41:07 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:41:07 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:4b6fac89a32ef648fc441f3f66feee802e0f63ca2b6461793a9b570667dccedc`  
		Last Modified: Wed, 18 Mar 2020 21:45:23 GMT  
		Size: 19.5 MB (19486597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca4069149f37bbb859c9011c637e6e96f315c0624202c1b9f9e64c0f90da99d`  
		Last Modified: Wed, 18 Mar 2020 21:45:16 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.22-windowsservercore-1809`

```console
$ docker pull traefik@sha256:c45e49ece6fc26eb95c95f320e00d46758767fa2c146440741bd5369d259de5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:v1.7.22-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:bd88226dd52059213f633dc9a3bdf0aed30826180a4b179e3ad0ee627d81eb99
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2291136525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d9a993def2d50ea7861006eeae29e3c17544402639ae01c64d56076d13f6dd4`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 18 Mar 2020 21:17:24 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.22/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 18 Mar 2020 21:17:27 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:17:29 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:17:30 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a7fab05ac5ad4b2f665ad71b5c08a81e82bff7ea2fdcbb66c14193d2dd268875`  
		Last Modified: Wed, 11 Mar 2020 01:16:21 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f23cddbd996747d71298787af1bd8bf6d4e4eda66e8bbf74d436d63f37325d`  
		Last Modified: Wed, 18 Mar 2020 21:19:05 GMT  
		Size: 25.8 MB (25795602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2612aaca4eba01ffd479ecfc14152f152c76201b7e0291ac46c22d3997f6a98`  
		Last Modified: Wed, 18 Mar 2020 21:18:59 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2112913d41c0c7ffd73f6f8673cadb8a67731e2e3125c2e91a3d8797f1b400`  
		Last Modified: Wed, 18 Mar 2020 21:18:59 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed1ef7067f20aa0022342f8d741e6cba951ccc3e04a529b05d51bf3021b3b0f`  
		Last Modified: Wed, 18 Mar 2020 21:18:59 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-alpine`

```console
$ docker pull traefik@sha256:0e8a8ced58f5e622a0ce2c74cef71ddee1e451fc28b160c1b84a1a3db8330bbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:b962d3ac91a9e11c88cf528a618c3679199dbfb42e3287f5bcb6112834636d3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24610153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01698f5f3d38aab7009255cb0128e3d1b64fb9d786deff3b8c8551ca34ba13c9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:23:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.22/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:23:32 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:23:32 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:23:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:23:32 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:23:32 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9821e36a40099dff67072fe099ac945c1ac3714751b0e2cbf22ba73e60b87c2b`  
		Last Modified: Wed, 18 Mar 2020 21:24:25 GMT  
		Size: 21.1 MB (21112646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64290e4840c8dda64c296a123aae5d34803c1807590f1e8d066053467c9cbcd1`  
		Last Modified: Wed, 18 Mar 2020 21:24:21 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:2924672d57ea80afe7b2fa9f18d2c071ef2b549b919e4706a7432d6ef08bce47
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23084518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fe48847efbf9f8af4e6b5355ba48508038248300193205adb5dc6dbc597335`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:50:14 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.22/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:50:15 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:50:16 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:50:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:50:17 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:50:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:5dde6016f49e2a1d3e9dcd060b23e4c5f0f12235888fcc06a8bd8878efe4cc84`  
		Last Modified: Wed, 18 Mar 2020 21:52:30 GMT  
		Size: 19.8 MB (19768575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e156d270acb91d9191a38c899aaa13302805048ab7487c1cdeeb756768a5b65`  
		Last Modified: Wed, 18 Mar 2020 21:52:24 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7c4b7a1347754ac471278b488697807abda18b2a1ffbcff3dc49a11cadb2a47c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22906084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2295dec92f083d7445e1910d8cb41e36edae8e7f8c617bb036c4069786538e6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:41:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.22/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:41:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:41:06 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:41:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:41:07 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:41:07 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:4b6fac89a32ef648fc441f3f66feee802e0f63ca2b6461793a9b570667dccedc`  
		Last Modified: Wed, 18 Mar 2020 21:45:23 GMT  
		Size: 19.5 MB (19486597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca4069149f37bbb859c9011c637e6e96f315c0624202c1b9f9e64c0f90da99d`  
		Last Modified: Wed, 18 Mar 2020 21:45:16 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:c45e49ece6fc26eb95c95f320e00d46758767fa2c146440741bd5369d259de5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:v1.7-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:bd88226dd52059213f633dc9a3bdf0aed30826180a4b179e3ad0ee627d81eb99
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2291136525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d9a993def2d50ea7861006eeae29e3c17544402639ae01c64d56076d13f6dd4`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 18 Mar 2020 21:17:24 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.22/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 18 Mar 2020 21:17:27 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:17:29 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:17:30 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.22 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a7fab05ac5ad4b2f665ad71b5c08a81e82bff7ea2fdcbb66c14193d2dd268875`  
		Last Modified: Wed, 11 Mar 2020 01:16:21 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f23cddbd996747d71298787af1bd8bf6d4e4eda66e8bbf74d436d63f37325d`  
		Last Modified: Wed, 18 Mar 2020 21:19:05 GMT  
		Size: 25.8 MB (25795602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2612aaca4eba01ffd479ecfc14152f152c76201b7e0291ac46c22d3997f6a98`  
		Last Modified: Wed, 18 Mar 2020 21:18:59 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2112913d41c0c7ffd73f6f8673cadb8a67731e2e3125c2e91a3d8797f1b400`  
		Last Modified: Wed, 18 Mar 2020 21:18:59 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed1ef7067f20aa0022342f8d741e6cba951ccc3e04a529b05d51bf3021b3b0f`  
		Last Modified: Wed, 18 Mar 2020 21:18:59 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.1`

```console
$ docker pull traefik@sha256:825521d793f572a3944787c134468017fdd719340fba06be53c33382e33b5ed1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.1` - linux; amd64

```console
$ docker pull traefik@sha256:b648fb36b8b7a16c29b17098ab0d4e3d6b690f3743113d5715b476a86c0c6eb6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23078678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc73dafdaf77f021af5d6e11d26485ef404c9c448041d04e2ab64c02085b45fb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:23:25 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.7/traefik_v2.1.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:23:25 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:23:25 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:23:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:23:26 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:23:26 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.7 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:d23d352c6a6b6e399956a83e278cfbf4a6ee13202799f970464fb64a83191572`  
		Last Modified: Wed, 18 Mar 2020 21:24:15 GMT  
		Size: 19.6 MB (19581171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36778517a2cb14855119773806f3a6beab6c4e85b1dcf74981e652d0079561a9`  
		Last Modified: Wed, 18 Mar 2020 21:24:10 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.1` - linux; arm variant v6

```console
$ docker pull traefik@sha256:d4a0b779bb40f2148d63a9431422cdd9a641c74ef1fcea23de774e454d0aa433
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 MB (21652564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48ee9f0382c3f27923bbd3252f34486b585e3294b5b5825cf10dd3a21bd41d9c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 19 Mar 2020 23:23:46 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.8/traefik_v2.1.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 19 Mar 2020 23:23:49 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 19 Mar 2020 23:23:51 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:23:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Mar 2020 23:23:55 GMT
CMD ["traefik"]
# Thu, 19 Mar 2020 23:23:57 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:53885d3a3b2b3c65397006830e2537614bdb892855376d49405c3d3f57b156f3`  
		Last Modified: Thu, 19 Mar 2020 23:24:51 GMT  
		Size: 18.3 MB (18336621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcd6f2d908241954732cb48c247880bdeaeb4c9941514c06bb5e01a406312c7`  
		Last Modified: Thu, 19 Mar 2020 23:24:45 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:064fbe4896c26fce414a7df2df0a3b0571ccefb73366b2739112b52612ebbf14
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 MB (21453551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eaee0200df033a74b1986f9d77ef02c0efbe5323827d25b39c8481656d1a114`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 20 Mar 2020 01:08:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.8/traefik_v2.1.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 20 Mar 2020 01:08:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 20 Mar 2020 01:08:51 GMT
EXPOSE 80
# Fri, 20 Mar 2020 01:09:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 20 Mar 2020 01:09:09 GMT
CMD ["traefik"]
# Fri, 20 Mar 2020 01:09:13 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:f90c65e62bd1d8a41d60336854858745d85736586b37abe6790a7a6d6f5181ad`  
		Last Modified: Fri, 20 Mar 2020 01:10:09 GMT  
		Size: 18.0 MB (18034065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9bae08bcb1e759e95d0a6764537920273d6cb4815345c68f8682589d015a87`  
		Last Modified: Fri, 20 Mar 2020 01:10:06 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.1.8`

```console
$ docker pull traefik@sha256:c154b732efbc133dd9fb2f75cb997b0078a9acd606c073aecd48bba192d1c9b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.1.8` - linux; arm variant v6

```console
$ docker pull traefik@sha256:d4a0b779bb40f2148d63a9431422cdd9a641c74ef1fcea23de774e454d0aa433
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 MB (21652564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48ee9f0382c3f27923bbd3252f34486b585e3294b5b5825cf10dd3a21bd41d9c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 19 Mar 2020 23:23:46 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.8/traefik_v2.1.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 19 Mar 2020 23:23:49 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 19 Mar 2020 23:23:51 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:23:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Mar 2020 23:23:55 GMT
CMD ["traefik"]
# Thu, 19 Mar 2020 23:23:57 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:53885d3a3b2b3c65397006830e2537614bdb892855376d49405c3d3f57b156f3`  
		Last Modified: Thu, 19 Mar 2020 23:24:51 GMT  
		Size: 18.3 MB (18336621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcd6f2d908241954732cb48c247880bdeaeb4c9941514c06bb5e01a406312c7`  
		Last Modified: Thu, 19 Mar 2020 23:24:45 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.1.8` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:064fbe4896c26fce414a7df2df0a3b0571ccefb73366b2739112b52612ebbf14
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 MB (21453551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eaee0200df033a74b1986f9d77ef02c0efbe5323827d25b39c8481656d1a114`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 20 Mar 2020 01:08:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.8/traefik_v2.1.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 20 Mar 2020 01:08:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 20 Mar 2020 01:08:51 GMT
EXPOSE 80
# Fri, 20 Mar 2020 01:09:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 20 Mar 2020 01:09:09 GMT
CMD ["traefik"]
# Fri, 20 Mar 2020 01:09:13 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:f90c65e62bd1d8a41d60336854858745d85736586b37abe6790a7a6d6f5181ad`  
		Last Modified: Fri, 20 Mar 2020 01:10:09 GMT  
		Size: 18.0 MB (18034065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9bae08bcb1e759e95d0a6764537920273d6cb4815345c68f8682589d015a87`  
		Last Modified: Fri, 20 Mar 2020 01:10:06 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.1.8-windowsservercore-1809`

```console
$ docker pull traefik@sha256:4aee458ca67f38c594327c15417266a1de3c2c0b7da10adfc52a9d3281e71226
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:v2.1.8-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:3b931df7ee834cd3981b0feed94aa43c270f61cd9b77fe55a521f2b752f53f51
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2289603149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02b29a74a7f7c2b1610fac17b8e9a47ce49630ce32c1470e065db828d23d08f1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 19 Mar 2020 23:41:52 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.8/traefik_v2.1.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 19 Mar 2020 23:41:56 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:41:58 GMT
ENTRYPOINT ["/traefik"]
# Thu, 19 Mar 2020 23:41:59 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a7fab05ac5ad4b2f665ad71b5c08a81e82bff7ea2fdcbb66c14193d2dd268875`  
		Last Modified: Wed, 11 Mar 2020 01:16:21 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa08490fed3660037a1b158752b8fe631ad840b0f2907c5fc2485a9e14e43ea3`  
		Last Modified: Thu, 19 Mar 2020 23:42:51 GMT  
		Size: 24.3 MB (24262030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97399e32101679e0af4842e21af256551e26a9ee7a8d9eca1324c30fbf93a627`  
		Last Modified: Thu, 19 Mar 2020 23:42:45 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142ff7dfc7b934a74d26c9bf367751fab4187d03eb3a4d53a682baf74371f93d`  
		Last Modified: Thu, 19 Mar 2020 23:42:45 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2695d512369d35885c9793f1d4824dae683f03a4f251b460b87c4c52790df131`  
		Last Modified: Thu, 19 Mar 2020 23:42:45 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:4aee458ca67f38c594327c15417266a1de3c2c0b7da10adfc52a9d3281e71226
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:v2.1-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:3b931df7ee834cd3981b0feed94aa43c270f61cd9b77fe55a521f2b752f53f51
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2289603149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02b29a74a7f7c2b1610fac17b8e9a47ce49630ce32c1470e065db828d23d08f1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 19 Mar 2020 23:41:52 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.8/traefik_v2.1.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 19 Mar 2020 23:41:56 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:41:58 GMT
ENTRYPOINT ["/traefik"]
# Thu, 19 Mar 2020 23:41:59 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a7fab05ac5ad4b2f665ad71b5c08a81e82bff7ea2fdcbb66c14193d2dd268875`  
		Last Modified: Wed, 11 Mar 2020 01:16:21 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa08490fed3660037a1b158752b8fe631ad840b0f2907c5fc2485a9e14e43ea3`  
		Last Modified: Thu, 19 Mar 2020 23:42:51 GMT  
		Size: 24.3 MB (24262030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97399e32101679e0af4842e21af256551e26a9ee7a8d9eca1324c30fbf93a627`  
		Last Modified: Thu, 19 Mar 2020 23:42:45 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142ff7dfc7b934a74d26c9bf367751fab4187d03eb3a4d53a682baf74371f93d`  
		Last Modified: Thu, 19 Mar 2020 23:42:45 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2695d512369d35885c9793f1d4824dae683f03a4f251b460b87c4c52790df131`  
		Last Modified: Thu, 19 Mar 2020 23:42:45 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.2`

```console
$ docker pull traefik@sha256:c00ad870b0a5a508a76723c5fd7dba74ee7d243823d20c1dae3a976de6e0a936
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.2` - linux; amd64

```console
$ docker pull traefik@sha256:a638691e542297b5e9c0e418aac95b3cf73d45177e9682d6bca73149c3c69bab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.8 MB (24780272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d1e6db5348027b0b036e274331d64662f34d66206a1ceaef0b17851c7f6885`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 23:42:56 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:23:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0-rc3/traefik_v2.2.0-rc3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:23:19 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:23:19 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:23:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:23:19 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:23:19 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:463bdeb7d88cb685b1d681a3d5c74d95efea6e0977efbe675e5171f92fd80322`  
		Last Modified: Wed, 18 Mar 2020 21:24:05 GMT  
		Size: 21.3 MB (21282765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3468d963bd074dbab9c5b9541fef31413dec4bd0eeb723b9cae6b305eb5033`  
		Last Modified: Wed, 18 Mar 2020 21:24:01 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.2` - linux; arm variant v6

```console
$ docker pull traefik@sha256:3f9230e23558384ec74667d3bb267a300a0620a5f6e405cada6dd5041c6dbaaf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.3 MB (23304555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a133c917280780e2eb70f42f1223f6652a4c727c1b412a3cc0294e83e252503a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 19 Mar 2020 23:23:28 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0-rc4/traefik_v2.2.0-rc4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 19 Mar 2020 23:23:30 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 19 Mar 2020 23:23:30 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:23:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Mar 2020 23:23:32 GMT
CMD ["traefik"]
# Thu, 19 Mar 2020 23:23:33 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:10a7ce7075e3cb97febbff60365fb86b17a86c0294b17c66364899585f12e1c4`  
		Last Modified: Thu, 19 Mar 2020 23:24:36 GMT  
		Size: 20.0 MB (19988611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688ec71b4885f6ba4c9d6f9c1ca43724c7dbc4609ba9d6f566fbfa8f604ad9c0`  
		Last Modified: Thu, 19 Mar 2020 23:24:29 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.2` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:b8e90b0dfa530d3ccfe3571f7b4fa950820de68c5856468a2e1096c11289683b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23052008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad21ca0460e4eb9c7f51c7bacdda2c7ab8eac9146c62e43216e7196d8d35e56f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 20 Mar 2020 01:07:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0-rc4/traefik_v2.2.0-rc4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 20 Mar 2020 01:07:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 20 Mar 2020 01:07:53 GMT
EXPOSE 80
# Fri, 20 Mar 2020 01:08:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 20 Mar 2020 01:08:05 GMT
CMD ["traefik"]
# Fri, 20 Mar 2020 01:08:08 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:45222051a4be92d7d44b388d03292f59f1af91178dedc7bf90a9a597cc018d1d`  
		Last Modified: Fri, 20 Mar 2020 01:09:54 GMT  
		Size: 19.6 MB (19632522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb2aaf6eb4c73fcc17336c4f6603672d042551a0a0763019d9c93882805906ab`  
		Last Modified: Fri, 20 Mar 2020 01:09:47 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.2.0-rc4`

```console
$ docker pull traefik@sha256:b2acf6d39f118c4a57152ae1292fb17af09eb0178bc9a3a0212a4dd43a9f76be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.2.0-rc4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:3f9230e23558384ec74667d3bb267a300a0620a5f6e405cada6dd5041c6dbaaf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.3 MB (23304555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a133c917280780e2eb70f42f1223f6652a4c727c1b412a3cc0294e83e252503a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 19 Mar 2020 23:23:28 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0-rc4/traefik_v2.2.0-rc4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 19 Mar 2020 23:23:30 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 19 Mar 2020 23:23:30 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:23:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Mar 2020 23:23:32 GMT
CMD ["traefik"]
# Thu, 19 Mar 2020 23:23:33 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:10a7ce7075e3cb97febbff60365fb86b17a86c0294b17c66364899585f12e1c4`  
		Last Modified: Thu, 19 Mar 2020 23:24:36 GMT  
		Size: 20.0 MB (19988611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688ec71b4885f6ba4c9d6f9c1ca43724c7dbc4609ba9d6f566fbfa8f604ad9c0`  
		Last Modified: Thu, 19 Mar 2020 23:24:29 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.2.0-rc4` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:b8e90b0dfa530d3ccfe3571f7b4fa950820de68c5856468a2e1096c11289683b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23052008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad21ca0460e4eb9c7f51c7bacdda2c7ab8eac9146c62e43216e7196d8d35e56f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 20 Mar 2020 01:07:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0-rc4/traefik_v2.2.0-rc4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 20 Mar 2020 01:07:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 20 Mar 2020 01:07:53 GMT
EXPOSE 80
# Fri, 20 Mar 2020 01:08:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 20 Mar 2020 01:08:05 GMT
CMD ["traefik"]
# Fri, 20 Mar 2020 01:08:08 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:45222051a4be92d7d44b388d03292f59f1af91178dedc7bf90a9a597cc018d1d`  
		Last Modified: Fri, 20 Mar 2020 01:09:54 GMT  
		Size: 19.6 MB (19632522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb2aaf6eb4c73fcc17336c4f6603672d042551a0a0763019d9c93882805906ab`  
		Last Modified: Fri, 20 Mar 2020 01:09:47 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.2.0-rc4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:10b613c0d809a2f32e3f1f05a4d1bf8948740b300edc48c0db647d89ded615a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:v2.2.0-rc4-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:be5249e8a1f004bc3b704f5f678a716baeb1e02cbabf159eb439b82457d3cadf
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2291275576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e276e79ace0d8ef3779cc569768475cf7763dcb4753b2da424149790667851c1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 19 Mar 2020 23:40:57 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.2.0-rc4/traefik_v2.2.0-rc4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 19 Mar 2020 23:41:01 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:41:02 GMT
ENTRYPOINT ["/traefik"]
# Thu, 19 Mar 2020 23:41:03 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a7fab05ac5ad4b2f665ad71b5c08a81e82bff7ea2fdcbb66c14193d2dd268875`  
		Last Modified: Wed, 11 Mar 2020 01:16:21 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:549f06fe79c6ff9fe97ad90025e8fa1f62dc9cc3b2d1a223c2be32e8e944ff9e`  
		Last Modified: Thu, 19 Mar 2020 23:42:30 GMT  
		Size: 25.9 MB (25934473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465d2f7acd904d7ca8da43eb4cdd73475b80ccce5ba79a88d9968266c4bad07f`  
		Last Modified: Thu, 19 Mar 2020 23:42:24 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809f97326d00cd242ff10557bd548b8db16c340fd5d7fc274f3282623f542bbb`  
		Last Modified: Thu, 19 Mar 2020 23:42:24 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e27a6ecc6db484f65e2587cb61e379ddb398f17469e292905230bc60e36fc04`  
		Last Modified: Thu, 19 Mar 2020 23:42:24 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:10b613c0d809a2f32e3f1f05a4d1bf8948740b300edc48c0db647d89ded615a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:v2.2-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:be5249e8a1f004bc3b704f5f678a716baeb1e02cbabf159eb439b82457d3cadf
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2291275576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e276e79ace0d8ef3779cc569768475cf7763dcb4753b2da424149790667851c1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 19 Mar 2020 23:40:57 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.2.0-rc4/traefik_v2.2.0-rc4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 19 Mar 2020 23:41:01 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:41:02 GMT
ENTRYPOINT ["/traefik"]
# Thu, 19 Mar 2020 23:41:03 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a7fab05ac5ad4b2f665ad71b5c08a81e82bff7ea2fdcbb66c14193d2dd268875`  
		Last Modified: Wed, 11 Mar 2020 01:16:21 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:549f06fe79c6ff9fe97ad90025e8fa1f62dc9cc3b2d1a223c2be32e8e944ff9e`  
		Last Modified: Thu, 19 Mar 2020 23:42:30 GMT  
		Size: 25.9 MB (25934473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465d2f7acd904d7ca8da43eb4cdd73475b80ccce5ba79a88d9968266c4bad07f`  
		Last Modified: Thu, 19 Mar 2020 23:42:24 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809f97326d00cd242ff10557bd548b8db16c340fd5d7fc274f3282623f542bbb`  
		Last Modified: Thu, 19 Mar 2020 23:42:24 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e27a6ecc6db484f65e2587cb61e379ddb398f17469e292905230bc60e36fc04`  
		Last Modified: Thu, 19 Mar 2020 23:42:24 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:4aee458ca67f38c594327c15417266a1de3c2c0b7da10adfc52a9d3281e71226
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:3b931df7ee834cd3981b0feed94aa43c270f61cd9b77fe55a521f2b752f53f51
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2289603149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02b29a74a7f7c2b1610fac17b8e9a47ce49630ce32c1470e065db828d23d08f1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 19 Mar 2020 23:41:52 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.8/traefik_v2.1.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 19 Mar 2020 23:41:56 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:41:58 GMT
ENTRYPOINT ["/traefik"]
# Thu, 19 Mar 2020 23:41:59 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a7fab05ac5ad4b2f665ad71b5c08a81e82bff7ea2fdcbb66c14193d2dd268875`  
		Last Modified: Wed, 11 Mar 2020 01:16:21 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa08490fed3660037a1b158752b8fe631ad840b0f2907c5fc2485a9e14e43ea3`  
		Last Modified: Thu, 19 Mar 2020 23:42:51 GMT  
		Size: 24.3 MB (24262030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97399e32101679e0af4842e21af256551e26a9ee7a8d9eca1324c30fbf93a627`  
		Last Modified: Thu, 19 Mar 2020 23:42:45 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142ff7dfc7b934a74d26c9bf367751fab4187d03eb3a4d53a682baf74371f93d`  
		Last Modified: Thu, 19 Mar 2020 23:42:45 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2695d512369d35885c9793f1d4824dae683f03a4f251b460b87c4c52790df131`  
		Last Modified: Thu, 19 Mar 2020 23:42:45 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
