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
$ docker pull traefik@sha256:49f6541232fa1cd1d1877d91d35d9276efa5ada1c1e4ea6e6342de1df5942a32
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
$ docker pull traefik@sha256:deae6848bac45d48e36cea3e48aa8d289f8f284c421d58736a88825a8db66edd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 MB (21654471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eb0348674b0db0f6a054d59f91ec2f8f51baed4369ad0de60f592ac813e38e7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:50:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.7/traefik_v2.1.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:50:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:50:01 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:50:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:50:02 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:50:03 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.7 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:68cf8a85b83356b3dd3e9b38b2326515167376b106c35040c06953768b87ec2b`  
		Last Modified: Wed, 18 Mar 2020 21:52:13 GMT  
		Size: 18.3 MB (18338528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8015aaedc4e75c3133ebb3ff448c2f672131101ca4c1560af4cf9d1f210d9e3`  
		Last Modified: Wed, 18 Mar 2020 21:52:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:70b8405bfc502596f69b4e2b0472c23a7b7fdcda7550ca90dfc512ee9efd345f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 MB (21453352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22a1f8fae66ab6068e3e6b3d494778ae7527124e43a4753a186f0ddd4ddc7aa0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:40:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.7/traefik_v2.1.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:40:54 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:40:54 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:40:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:40:55 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:40:56 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.7 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:0118bf0ba897b75b854225037df623dc0ba66fde7fd013f6978553097a18a6fa`  
		Last Modified: Wed, 18 Mar 2020 21:45:06 GMT  
		Size: 18.0 MB (18033866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292de31b72d125dcaa1c0b28235dfb28871c2fb2d3ea26f022a9dc543816e5c3`  
		Last Modified: Wed, 18 Mar 2020 21:44:58 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.1.8`

**does not exist** (yet?)

## `traefik:2.1.8-windowsservercore-1809`

**does not exist** (yet?)

## `traefik:2.1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:924895fe18d5e276bd784bb1453de6e64802a7bd1d36c8995db8c63b4daf9e89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:2.1-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:6ce87750417b85819c39ba50b0ac140ead81c63533980fccad4fc5784ae221bc
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2289603103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b5df0dbddf8d272cfa2060ea91765334084f996347f54642d665aed86436d9f`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 18 Mar 2020 21:16:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.7/traefik_v2.1.7_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 18 Mar 2020 21:16:26 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:16:27 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:16:28 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.7 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:06f895641955abb2113ba9240580f2939d45b9894b338288688fd40f2ce00a7b`  
		Last Modified: Wed, 18 Mar 2020 21:18:25 GMT  
		Size: 24.3 MB (24262121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05eb28b67cb9e14124f26d200b48383b0e0a60e98231985b600293edeb82fecd`  
		Last Modified: Wed, 18 Mar 2020 21:18:20 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d69bf59e2ab83f1d466d9da6922c2e4706ccef4e4f28f42161ce68fd8c80879`  
		Last Modified: Wed, 18 Mar 2020 21:18:20 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c75bfdfeed7d42f654d13958eeb8364ab195ac927c2e9f5f904968179ab151f`  
		Last Modified: Wed, 18 Mar 2020 21:18:42 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.2`

```console
$ docker pull traefik@sha256:c5218f66e8e41c9d5388c9443ba9f88cfb5c28c4d2f3a3e14dab4fdfa2478a71
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
$ docker pull traefik@sha256:7343ec86cee5b8875dd3b0c8071dd1b4fc683c6a536a2f3f9d3c40053d56476e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.3 MB (23303483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a2346b154cd91daccbc831a27bfb664c31cd40c60e8cc0d6fff964b4ae0ee10`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:49:48 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0-rc3/traefik_v2.2.0-rc3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:49:49 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:49:49 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:49:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:49:50 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:49:51 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:e333e2bf0f9313ead0c0a88bac6df2ede1c5637d79dbc2865a126509a0f6cb69`  
		Last Modified: Wed, 18 Mar 2020 21:51:57 GMT  
		Size: 20.0 MB (19987540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d1c766dbe760a08e7a18cfe490dc4eaf16ed1342083c6c15e7c659321076e0`  
		Last Modified: Wed, 18 Mar 2020 21:51:49 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.2` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:c2d5761b1fd800e187c3dbfb3467b91a874280218158abe5de98d4c58c556e8c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23052125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b841b1ba74ace676d602e9044272d28f43fa1f4e481d3899dbf391b5827a9ec4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:40:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0-rc3/traefik_v2.2.0-rc3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:40:42 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:40:43 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:40:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:40:44 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:40:45 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:4a3867e748ecfa0dd55b07ed8ca560b6e0a28b80a3d17c9cf2378320c2c39a7f`  
		Last Modified: Wed, 18 Mar 2020 21:44:49 GMT  
		Size: 19.6 MB (19632638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d09084103f1ea0bf4671712f5b695db09d0d41cc823b73b3f10772cd214ac7`  
		Last Modified: Wed, 18 Mar 2020 21:44:43 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.2.0-rc4`

**does not exist** (yet?)

## `traefik:2.2.0-rc4-windowsservercore-1809`

**does not exist** (yet?)

## `traefik:2.2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:ae15650b71958b08f028991f4b38791ecca77f853d6dc7b419deb1ca4502819d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:2.2-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:155db1e5f3a7990698b182425ce606137bf6f1c3bb174e3a19bd5a665ed2dae4
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2291276244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c1bf119d6abe6823dc4724851c9f94adbc53020db79ad0f79b5e844c850ef86`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 18 Mar 2020 21:15:22 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.2.0-rc3/traefik_v2.2.0-rc3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 18 Mar 2020 21:15:25 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:15:26 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:15:27 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:2ff4d97ecd69f43057409220e5d59c27e58d08cc771f11f32e2529b483765559`  
		Last Modified: Wed, 18 Mar 2020 21:18:04 GMT  
		Size: 25.9 MB (25935303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc5d7d61d7ec4d6025f91b964e672d8364cb29fb8ad7db35b20d237f1482f9e`  
		Last Modified: Wed, 18 Mar 2020 21:17:58 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8a22bf54991e83d941fcc58687c032e136df72dc28458e12b834a051fe0d01`  
		Last Modified: Wed, 18 Mar 2020 21:17:58 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a17d523ea7cc71927e7c1c07163c592e6e262c4c0e193b371f63817dfbe7c0`  
		Last Modified: Wed, 18 Mar 2020 21:17:58 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:cantal`

```console
$ docker pull traefik@sha256:49f6541232fa1cd1d1877d91d35d9276efa5ada1c1e4ea6e6342de1df5942a32
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
$ docker pull traefik@sha256:deae6848bac45d48e36cea3e48aa8d289f8f284c421d58736a88825a8db66edd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 MB (21654471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eb0348674b0db0f6a054d59f91ec2f8f51baed4369ad0de60f592ac813e38e7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:50:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.7/traefik_v2.1.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:50:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:50:01 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:50:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:50:02 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:50:03 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.7 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:68cf8a85b83356b3dd3e9b38b2326515167376b106c35040c06953768b87ec2b`  
		Last Modified: Wed, 18 Mar 2020 21:52:13 GMT  
		Size: 18.3 MB (18338528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8015aaedc4e75c3133ebb3ff448c2f672131101ca4c1560af4cf9d1f210d9e3`  
		Last Modified: Wed, 18 Mar 2020 21:52:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:cantal` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:70b8405bfc502596f69b4e2b0472c23a7b7fdcda7550ca90dfc512ee9efd345f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 MB (21453352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22a1f8fae66ab6068e3e6b3d494778ae7527124e43a4753a186f0ddd4ddc7aa0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:40:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.7/traefik_v2.1.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:40:54 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:40:54 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:40:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:40:55 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:40:56 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.7 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:0118bf0ba897b75b854225037df623dc0ba66fde7fd013f6978553097a18a6fa`  
		Last Modified: Wed, 18 Mar 2020 21:45:06 GMT  
		Size: 18.0 MB (18033866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292de31b72d125dcaa1c0b28235dfb28871c2fb2d3ea26f022a9dc543816e5c3`  
		Last Modified: Wed, 18 Mar 2020 21:44:58 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:cantal-windowsservercore-1809`

```console
$ docker pull traefik@sha256:924895fe18d5e276bd784bb1453de6e64802a7bd1d36c8995db8c63b4daf9e89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:cantal-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:6ce87750417b85819c39ba50b0ac140ead81c63533980fccad4fc5784ae221bc
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2289603103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b5df0dbddf8d272cfa2060ea91765334084f996347f54642d665aed86436d9f`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 18 Mar 2020 21:16:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.7/traefik_v2.1.7_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 18 Mar 2020 21:16:26 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:16:27 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:16:28 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.7 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:06f895641955abb2113ba9240580f2939d45b9894b338288688fd40f2ce00a7b`  
		Last Modified: Wed, 18 Mar 2020 21:18:25 GMT  
		Size: 24.3 MB (24262121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05eb28b67cb9e14124f26d200b48383b0e0a60e98231985b600293edeb82fecd`  
		Last Modified: Wed, 18 Mar 2020 21:18:20 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d69bf59e2ab83f1d466d9da6922c2e4706ccef4e4f28f42161ce68fd8c80879`  
		Last Modified: Wed, 18 Mar 2020 21:18:20 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c75bfdfeed7d42f654d13958eeb8364ab195ac927c2e9f5f904968179ab151f`  
		Last Modified: Wed, 18 Mar 2020 21:18:42 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:chevrotin`

```console
$ docker pull traefik@sha256:c5218f66e8e41c9d5388c9443ba9f88cfb5c28c4d2f3a3e14dab4fdfa2478a71
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
$ docker pull traefik@sha256:7343ec86cee5b8875dd3b0c8071dd1b4fc683c6a536a2f3f9d3c40053d56476e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.3 MB (23303483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a2346b154cd91daccbc831a27bfb664c31cd40c60e8cc0d6fff964b4ae0ee10`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:49:48 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0-rc3/traefik_v2.2.0-rc3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:49:49 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:49:49 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:49:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:49:50 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:49:51 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:e333e2bf0f9313ead0c0a88bac6df2ede1c5637d79dbc2865a126509a0f6cb69`  
		Last Modified: Wed, 18 Mar 2020 21:51:57 GMT  
		Size: 20.0 MB (19987540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d1c766dbe760a08e7a18cfe490dc4eaf16ed1342083c6c15e7c659321076e0`  
		Last Modified: Wed, 18 Mar 2020 21:51:49 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:chevrotin` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:c2d5761b1fd800e187c3dbfb3467b91a874280218158abe5de98d4c58c556e8c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23052125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b841b1ba74ace676d602e9044272d28f43fa1f4e481d3899dbf391b5827a9ec4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:40:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0-rc3/traefik_v2.2.0-rc3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:40:42 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:40:43 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:40:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:40:44 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:40:45 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:4a3867e748ecfa0dd55b07ed8ca560b6e0a28b80a3d17c9cf2378320c2c39a7f`  
		Last Modified: Wed, 18 Mar 2020 21:44:49 GMT  
		Size: 19.6 MB (19632638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d09084103f1ea0bf4671712f5b695db09d0d41cc823b73b3f10772cd214ac7`  
		Last Modified: Wed, 18 Mar 2020 21:44:43 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:chevrotin-windowsservercore-1809`

```console
$ docker pull traefik@sha256:ae15650b71958b08f028991f4b38791ecca77f853d6dc7b419deb1ca4502819d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:chevrotin-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:155db1e5f3a7990698b182425ce606137bf6f1c3bb174e3a19bd5a665ed2dae4
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2291276244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c1bf119d6abe6823dc4724851c9f94adbc53020db79ad0f79b5e844c850ef86`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 18 Mar 2020 21:15:22 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.2.0-rc3/traefik_v2.2.0-rc3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 18 Mar 2020 21:15:25 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:15:26 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:15:27 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:2ff4d97ecd69f43057409220e5d59c27e58d08cc771f11f32e2529b483765559`  
		Last Modified: Wed, 18 Mar 2020 21:18:04 GMT  
		Size: 25.9 MB (25935303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc5d7d61d7ec4d6025f91b964e672d8364cb29fb8ad7db35b20d237f1482f9e`  
		Last Modified: Wed, 18 Mar 2020 21:17:58 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8a22bf54991e83d941fcc58687c032e136df72dc28458e12b834a051fe0d01`  
		Last Modified: Wed, 18 Mar 2020 21:17:58 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a17d523ea7cc71927e7c1c07163c592e6e262c4c0e193b371f63817dfbe7c0`  
		Last Modified: Wed, 18 Mar 2020 21:17:58 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:49f6541232fa1cd1d1877d91d35d9276efa5ada1c1e4ea6e6342de1df5942a32
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
$ docker pull traefik@sha256:deae6848bac45d48e36cea3e48aa8d289f8f284c421d58736a88825a8db66edd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 MB (21654471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eb0348674b0db0f6a054d59f91ec2f8f51baed4369ad0de60f592ac813e38e7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:50:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.7/traefik_v2.1.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:50:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:50:01 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:50:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:50:02 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:50:03 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.7 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:68cf8a85b83356b3dd3e9b38b2326515167376b106c35040c06953768b87ec2b`  
		Last Modified: Wed, 18 Mar 2020 21:52:13 GMT  
		Size: 18.3 MB (18338528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8015aaedc4e75c3133ebb3ff448c2f672131101ca4c1560af4cf9d1f210d9e3`  
		Last Modified: Wed, 18 Mar 2020 21:52:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:70b8405bfc502596f69b4e2b0472c23a7b7fdcda7550ca90dfc512ee9efd345f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 MB (21453352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22a1f8fae66ab6068e3e6b3d494778ae7527124e43a4753a186f0ddd4ddc7aa0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:40:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.7/traefik_v2.1.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:40:54 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:40:54 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:40:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:40:55 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:40:56 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.7 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:0118bf0ba897b75b854225037df623dc0ba66fde7fd013f6978553097a18a6fa`  
		Last Modified: Wed, 18 Mar 2020 21:45:06 GMT  
		Size: 18.0 MB (18033866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292de31b72d125dcaa1c0b28235dfb28871c2fb2d3ea26f022a9dc543816e5c3`  
		Last Modified: Wed, 18 Mar 2020 21:44:58 GMT  
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
$ docker pull traefik@sha256:49f6541232fa1cd1d1877d91d35d9276efa5ada1c1e4ea6e6342de1df5942a32
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
$ docker pull traefik@sha256:deae6848bac45d48e36cea3e48aa8d289f8f284c421d58736a88825a8db66edd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 MB (21654471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eb0348674b0db0f6a054d59f91ec2f8f51baed4369ad0de60f592ac813e38e7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:50:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.7/traefik_v2.1.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:50:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:50:01 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:50:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:50:02 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:50:03 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.7 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:68cf8a85b83356b3dd3e9b38b2326515167376b106c35040c06953768b87ec2b`  
		Last Modified: Wed, 18 Mar 2020 21:52:13 GMT  
		Size: 18.3 MB (18338528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8015aaedc4e75c3133ebb3ff448c2f672131101ca4c1560af4cf9d1f210d9e3`  
		Last Modified: Wed, 18 Mar 2020 21:52:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:70b8405bfc502596f69b4e2b0472c23a7b7fdcda7550ca90dfc512ee9efd345f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 MB (21453352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22a1f8fae66ab6068e3e6b3d494778ae7527124e43a4753a186f0ddd4ddc7aa0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:40:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.7/traefik_v2.1.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:40:54 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:40:54 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:40:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:40:55 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:40:56 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.7 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:0118bf0ba897b75b854225037df623dc0ba66fde7fd013f6978553097a18a6fa`  
		Last Modified: Wed, 18 Mar 2020 21:45:06 GMT  
		Size: 18.0 MB (18033866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292de31b72d125dcaa1c0b28235dfb28871c2fb2d3ea26f022a9dc543816e5c3`  
		Last Modified: Wed, 18 Mar 2020 21:44:58 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.1.8`

**does not exist** (yet?)

## `traefik:v2.1.8-windowsservercore-1809`

**does not exist** (yet?)

## `traefik:v2.1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:924895fe18d5e276bd784bb1453de6e64802a7bd1d36c8995db8c63b4daf9e89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:v2.1-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:6ce87750417b85819c39ba50b0ac140ead81c63533980fccad4fc5784ae221bc
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2289603103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b5df0dbddf8d272cfa2060ea91765334084f996347f54642d665aed86436d9f`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 18 Mar 2020 21:16:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.7/traefik_v2.1.7_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 18 Mar 2020 21:16:26 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:16:27 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:16:28 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.7 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:06f895641955abb2113ba9240580f2939d45b9894b338288688fd40f2ce00a7b`  
		Last Modified: Wed, 18 Mar 2020 21:18:25 GMT  
		Size: 24.3 MB (24262121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05eb28b67cb9e14124f26d200b48383b0e0a60e98231985b600293edeb82fecd`  
		Last Modified: Wed, 18 Mar 2020 21:18:20 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d69bf59e2ab83f1d466d9da6922c2e4706ccef4e4f28f42161ce68fd8c80879`  
		Last Modified: Wed, 18 Mar 2020 21:18:20 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c75bfdfeed7d42f654d13958eeb8364ab195ac927c2e9f5f904968179ab151f`  
		Last Modified: Wed, 18 Mar 2020 21:18:42 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.2`

```console
$ docker pull traefik@sha256:c5218f66e8e41c9d5388c9443ba9f88cfb5c28c4d2f3a3e14dab4fdfa2478a71
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
$ docker pull traefik@sha256:7343ec86cee5b8875dd3b0c8071dd1b4fc683c6a536a2f3f9d3c40053d56476e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.3 MB (23303483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a2346b154cd91daccbc831a27bfb664c31cd40c60e8cc0d6fff964b4ae0ee10`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:49:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:49:48 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0-rc3/traefik_v2.2.0-rc3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:49:49 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:49:49 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:49:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:49:50 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:49:51 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:e333e2bf0f9313ead0c0a88bac6df2ede1c5637d79dbc2865a126509a0f6cb69`  
		Last Modified: Wed, 18 Mar 2020 21:51:57 GMT  
		Size: 20.0 MB (19987540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d1c766dbe760a08e7a18cfe490dc4eaf16ed1342083c6c15e7c659321076e0`  
		Last Modified: Wed, 18 Mar 2020 21:51:49 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.2` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:c2d5761b1fd800e187c3dbfb3467b91a874280218158abe5de98d4c58c556e8c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23052125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b841b1ba74ace676d602e9044272d28f43fa1f4e481d3899dbf391b5827a9ec4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 06 Feb 2020 22:44:26 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Mar 2020 21:40:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0-rc3/traefik_v2.2.0-rc3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Mar 2020 21:40:42 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Mar 2020 21:40:43 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:40:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Mar 2020 21:40:44 GMT
CMD ["traefik"]
# Wed, 18 Mar 2020 21:40:45 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:4a3867e748ecfa0dd55b07ed8ca560b6e0a28b80a3d17c9cf2378320c2c39a7f`  
		Last Modified: Wed, 18 Mar 2020 21:44:49 GMT  
		Size: 19.6 MB (19632638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d09084103f1ea0bf4671712f5b695db09d0d41cc823b73b3f10772cd214ac7`  
		Last Modified: Wed, 18 Mar 2020 21:44:43 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.2.0-rc4`

**does not exist** (yet?)

## `traefik:v2.2.0-rc4-windowsservercore-1809`

**does not exist** (yet?)

## `traefik:v2.2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:ae15650b71958b08f028991f4b38791ecca77f853d6dc7b419deb1ca4502819d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:v2.2-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:155db1e5f3a7990698b182425ce606137bf6f1c3bb174e3a19bd5a665ed2dae4
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2291276244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c1bf119d6abe6823dc4724851c9f94adbc53020db79ad0f79b5e844c850ef86`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 18 Mar 2020 21:15:22 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.2.0-rc3/traefik_v2.2.0-rc3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 18 Mar 2020 21:15:25 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:15:26 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:15:27 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0-rc3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:2ff4d97ecd69f43057409220e5d59c27e58d08cc771f11f32e2529b483765559`  
		Last Modified: Wed, 18 Mar 2020 21:18:04 GMT  
		Size: 25.9 MB (25935303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc5d7d61d7ec4d6025f91b964e672d8364cb29fb8ad7db35b20d237f1482f9e`  
		Last Modified: Wed, 18 Mar 2020 21:17:58 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8a22bf54991e83d941fcc58687c032e136df72dc28458e12b834a051fe0d01`  
		Last Modified: Wed, 18 Mar 2020 21:17:58 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a17d523ea7cc71927e7c1c07163c592e6e262c4c0e193b371f63817dfbe7c0`  
		Last Modified: Wed, 18 Mar 2020 21:17:58 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:924895fe18d5e276bd784bb1453de6e64802a7bd1d36c8995db8c63b4daf9e89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:6ce87750417b85819c39ba50b0ac140ead81c63533980fccad4fc5784ae221bc
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2289603103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b5df0dbddf8d272cfa2060ea91765334084f996347f54642d665aed86436d9f`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 18 Mar 2020 21:16:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.7/traefik_v2.1.7_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 18 Mar 2020 21:16:26 GMT
EXPOSE 80
# Wed, 18 Mar 2020 21:16:27 GMT
ENTRYPOINT ["/traefik"]
# Wed, 18 Mar 2020 21:16:28 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.7 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:06f895641955abb2113ba9240580f2939d45b9894b338288688fd40f2ce00a7b`  
		Last Modified: Wed, 18 Mar 2020 21:18:25 GMT  
		Size: 24.3 MB (24262121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05eb28b67cb9e14124f26d200b48383b0e0a60e98231985b600293edeb82fecd`  
		Last Modified: Wed, 18 Mar 2020 21:18:20 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d69bf59e2ab83f1d466d9da6922c2e4706ccef4e4f28f42161ce68fd8c80879`  
		Last Modified: Wed, 18 Mar 2020 21:18:20 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c75bfdfeed7d42f654d13958eeb8364ab195ac927c2e9f5f904968179ab151f`  
		Last Modified: Wed, 18 Mar 2020 21:18:42 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
