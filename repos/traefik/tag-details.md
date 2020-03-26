<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:1.7`](#traefik17)
-	[`traefik:1.7.24`](#traefik1724)
-	[`traefik:1.7.24-alpine`](#traefik1724-alpine)
-	[`traefik:1.7.24-windowsservercore-1809`](#traefik1724-windowsservercore-1809)
-	[`traefik:1.7-alpine`](#traefik17-alpine)
-	[`traefik:1.7-windowsservercore-1809`](#traefik17-windowsservercore-1809)
-	[`traefik:2.2`](#traefik22)
-	[`traefik:2.2.0`](#traefik220)
-	[`traefik:2.2.0-windowsservercore-1809`](#traefik220-windowsservercore-1809)
-	[`traefik:2.2-windowsservercore-1809`](#traefik22-windowsservercore-1809)
-	[`traefik:chevrotin`](#traefikchevrotin)
-	[`traefik:chevrotin-windowsservercore-1809`](#traefikchevrotin-windowsservercore-1809)
-	[`traefik:latest`](#traefiklatest)
-	[`traefik:maroilles`](#traefikmaroilles)
-	[`traefik:maroilles-alpine`](#traefikmaroilles-alpine)
-	[`traefik:maroilles-windowsservercore-1809`](#traefikmaroilles-windowsservercore-1809)
-	[`traefik:v1.7`](#traefikv17)
-	[`traefik:v1.7.24`](#traefikv1724)
-	[`traefik:v1.7.24-alpine`](#traefikv1724-alpine)
-	[`traefik:v1.7.24-windowsservercore-1809`](#traefikv1724-windowsservercore-1809)
-	[`traefik:v1.7-alpine`](#traefikv17-alpine)
-	[`traefik:v1.7-windowsservercore-1809`](#traefikv17-windowsservercore-1809)
-	[`traefik:v2.2`](#traefikv22)
-	[`traefik:v2.2.0`](#traefikv220)
-	[`traefik:v2.2.0-windowsservercore-1809`](#traefikv220-windowsservercore-1809)
-	[`traefik:v2.2-windowsservercore-1809`](#traefikv22-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:1.7`

```console
$ docker pull traefik@sha256:47bec236a121a07703e27fc3e18c201ae0241cff1038ea2faf5d05bf5ea82286
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7` - linux; amd64

```console
$ docker pull traefik@sha256:bec5a86cd327d82a50fe89aae5c57d49a13bb9c7fe82fcdd7c886adf09645801
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21578312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:100389fa48aa58f1587f27467ac7f319ca8724b7bbad55ee09ada0de310a3bf4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 02:50:22 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 02:50:24 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 25 Mar 2020 22:24:07 GMT
COPY file:1f3cec74af68ac254dc1c90001edd0f7a71f8e42168f4523b5b170d518e50e2a in / 
# Wed, 25 Mar 2020 22:24:07 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:24:07 GMT
VOLUME [/tmp]
# Wed, 25 Mar 2020 22:24:07 GMT
ENTRYPOINT ["/traefik"]
# Wed, 25 Mar 2020 22:24:08 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6f9aa7cec283ff91d23b1d8e88e428fd21f67593d121f450a42173fe6443f190`  
		Last Modified: Wed, 25 Mar 2020 22:24:49 GMT  
		Size: 21.1 MB (21119254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:1733e40d59ca54506c6b3859245878b29270da0d17eaa5b10322bc83cf5749bc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20230146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6df2ff4474d538ce68e1599c24ef3227b9087dbfa625a1049a3172fe56a021b9`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 03:46:16 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 03:46:17 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 25 Mar 2020 21:50:06 GMT
COPY file:5fc84f7de0956e9c09bc8249cedc256b1ebfbbdf7a970a1b03cbc35342bc98d8 in / 
# Wed, 25 Mar 2020 21:50:07 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:50:07 GMT
VOLUME [/tmp]
# Wed, 25 Mar 2020 21:50:08 GMT
ENTRYPOINT ["/traefik"]
# Wed, 25 Mar 2020 21:50:08 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:cc2e8d91f8cdcad6fef81a6606a958dc4fa4ffe856944124f101909ef0e2a6de`  
		Last Modified: Wed, 25 Mar 2020 21:51:04 GMT  
		Size: 19.8 MB (19771060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7f26aa867bbfa1637f66f2faee17fd66549e441185789b64aa07f0326e75f321
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.0 MB (19950262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7b0a67ae19f09c258a8a530bf8f7315c03f0157c72a093a495d017a4d8032a`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 05:55:25 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 05:55:26 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 25 Mar 2020 21:44:21 GMT
COPY file:0347658f660b1b9c0951c6a64bfc0f8a407487940ca58f7d6da08472f61358db in / 
# Wed, 25 Mar 2020 21:44:21 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:44:22 GMT
VOLUME [/tmp]
# Wed, 25 Mar 2020 21:44:23 GMT
ENTRYPOINT ["/traefik"]
# Wed, 25 Mar 2020 21:44:23 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:e41d3d1eaac6c67b9dab999e93238a86c8df48b874e4225dd36534ce81905c58`  
		Last Modified: Wed, 25 Mar 2020 21:45:23 GMT  
		Size: 19.5 MB (19491184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.24`

```console
$ docker pull traefik@sha256:47bec236a121a07703e27fc3e18c201ae0241cff1038ea2faf5d05bf5ea82286
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.24` - linux; amd64

```console
$ docker pull traefik@sha256:bec5a86cd327d82a50fe89aae5c57d49a13bb9c7fe82fcdd7c886adf09645801
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21578312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:100389fa48aa58f1587f27467ac7f319ca8724b7bbad55ee09ada0de310a3bf4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 02:50:22 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 02:50:24 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 25 Mar 2020 22:24:07 GMT
COPY file:1f3cec74af68ac254dc1c90001edd0f7a71f8e42168f4523b5b170d518e50e2a in / 
# Wed, 25 Mar 2020 22:24:07 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:24:07 GMT
VOLUME [/tmp]
# Wed, 25 Mar 2020 22:24:07 GMT
ENTRYPOINT ["/traefik"]
# Wed, 25 Mar 2020 22:24:08 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6f9aa7cec283ff91d23b1d8e88e428fd21f67593d121f450a42173fe6443f190`  
		Last Modified: Wed, 25 Mar 2020 22:24:49 GMT  
		Size: 21.1 MB (21119254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.24` - linux; arm variant v6

```console
$ docker pull traefik@sha256:1733e40d59ca54506c6b3859245878b29270da0d17eaa5b10322bc83cf5749bc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20230146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6df2ff4474d538ce68e1599c24ef3227b9087dbfa625a1049a3172fe56a021b9`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 03:46:16 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 03:46:17 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 25 Mar 2020 21:50:06 GMT
COPY file:5fc84f7de0956e9c09bc8249cedc256b1ebfbbdf7a970a1b03cbc35342bc98d8 in / 
# Wed, 25 Mar 2020 21:50:07 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:50:07 GMT
VOLUME [/tmp]
# Wed, 25 Mar 2020 21:50:08 GMT
ENTRYPOINT ["/traefik"]
# Wed, 25 Mar 2020 21:50:08 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:cc2e8d91f8cdcad6fef81a6606a958dc4fa4ffe856944124f101909ef0e2a6de`  
		Last Modified: Wed, 25 Mar 2020 21:51:04 GMT  
		Size: 19.8 MB (19771060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.24` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7f26aa867bbfa1637f66f2faee17fd66549e441185789b64aa07f0326e75f321
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.0 MB (19950262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7b0a67ae19f09c258a8a530bf8f7315c03f0157c72a093a495d017a4d8032a`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 05:55:25 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 05:55:26 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 25 Mar 2020 21:44:21 GMT
COPY file:0347658f660b1b9c0951c6a64bfc0f8a407487940ca58f7d6da08472f61358db in / 
# Wed, 25 Mar 2020 21:44:21 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:44:22 GMT
VOLUME [/tmp]
# Wed, 25 Mar 2020 21:44:23 GMT
ENTRYPOINT ["/traefik"]
# Wed, 25 Mar 2020 21:44:23 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:e41d3d1eaac6c67b9dab999e93238a86c8df48b874e4225dd36534ce81905c58`  
		Last Modified: Wed, 25 Mar 2020 21:45:23 GMT  
		Size: 19.5 MB (19491184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.24-alpine`

```console
$ docker pull traefik@sha256:a5be418acbd9a1a3011242c27feadd440ca56afbec22a7763150202de397cb6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.24-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:178c67d6e375ce45264f1a47eef709bca9928ac85badaa8f0d877059d5f37b6a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24617292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa4204cec7f48d0cc16d69e25ac8a29074a4782bc92622e55ec94c3b11f5b479`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:45:50 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 22:23:44 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.24/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 22:23:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 22:23:45 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:23:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 22:23:45 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 22:23:45 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f365f1b91ebb32c62c3856cd602b14702103c16ede6873855d0c5a5faa874810`  
		Last Modified: Mon, 23 Mar 2020 23:47:03 GMT  
		Size: 694.1 KB (694143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9cb6e408627ad0a100994d33c802c10828d8373fb7234572e0235fca9d7294c`  
		Last Modified: Wed, 25 Mar 2020 22:24:39 GMT  
		Size: 21.1 MB (21119525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5c0f262e2748518c0df991fbe02ea98c1eb9fc9a355c8eb8ca0c4cd4b43b55`  
		Last Modified: Wed, 25 Mar 2020 22:24:34 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.24-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:4f2a0e53c458ad8c389a40413c074135270a7bd2f82b1eb51a7dd0a5f093ec2b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23088245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd24e8f81b3e69a7b6eee14be566e2fd65f042b52389beb520915838d86f15e3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 03:43:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 21:49:52 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.24/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 21:49:53 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 21:49:54 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:49:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 21:49:55 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 21:49:55 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b73c299e24e9aa32bbbec493b7588c3a6592d11b52ccb01c156037b819aef46`  
		Last Modified: Tue, 24 Mar 2020 03:47:03 GMT  
		Size: 698.1 KB (698067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65b61609c3447263dc8c67420226770998aab72683c8da887882dda9a04761d`  
		Last Modified: Wed, 25 Mar 2020 21:50:48 GMT  
		Size: 19.8 MB (19771230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf34024959fde388d8f122f98686c98d2f26a6ee616fac255e9d24a7684480d`  
		Last Modified: Wed, 25 Mar 2020 21:50:40 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.24-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:2960a1bff52c4e20800f297ac9491661804f276e4c167c5f477cae56e45bf482
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22911054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10cc83f1529223ab41bc828bcbd1d0b3937e49b4786ab5851376c284cac448b1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 05:52:48 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 21:44:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.24/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 21:44:06 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 21:44:07 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:44:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 21:44:08 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 21:44:08 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc893b889cb9ecb596775296ec01901b5ffcd52efc8691a608afb27fc5be6e6`  
		Last Modified: Tue, 24 Mar 2020 05:55:52 GMT  
		Size: 696.2 KB (696184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46883925a5415d0997e2373210f823fdb48428220d78047fe8ff251f7fc6810`  
		Last Modified: Wed, 25 Mar 2020 21:45:06 GMT  
		Size: 19.5 MB (19491362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09800e005e5decf1b215e0d6adfd8871dafad512432f8e624b6e59c927639d73`  
		Last Modified: Wed, 25 Mar 2020 21:44:59 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.24-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b426bd3967d042be18586fe7adb6c566dcb6fcfd17c1e7d8fdc99d672481d747
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:1.7.24-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:cdd49fc23c498159f787d89d707a0472892b98a7475f733e0066be54ec585c4f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2291142795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32019c1c23bff7833c4766fe4d51a8efb2a3ea4c9512dcbd4a4c04a0b2d90d51`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Mar 2020 22:16:11 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.24/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 25 Mar 2020 22:16:14 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:16:16 GMT
ENTRYPOINT ["/traefik"]
# Wed, 25 Mar 2020 22:16:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:af9dafbf4071c5188d0bacf25804474510f4ed2632d998299e90d50759d1c345`  
		Last Modified: Wed, 25 Mar 2020 22:17:08 GMT  
		Size: 25.8 MB (25801842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912d37b34307d1c69659cb03f9fc4935e7fc4b6f77f739d272ed6b19a0998081`  
		Last Modified: Wed, 25 Mar 2020 22:17:02 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f437a5e5ec2a4c30cac218fed1c9d68c25a39998424ca2ee0b70bfdc37d815c1`  
		Last Modified: Wed, 25 Mar 2020 22:17:02 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736087e6923330749a7eb4dc3fc0d6ef3787429db038a584539e1a5d3e35bd23`  
		Last Modified: Wed, 25 Mar 2020 22:17:02 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-alpine`

```console
$ docker pull traefik@sha256:a5be418acbd9a1a3011242c27feadd440ca56afbec22a7763150202de397cb6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:178c67d6e375ce45264f1a47eef709bca9928ac85badaa8f0d877059d5f37b6a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24617292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa4204cec7f48d0cc16d69e25ac8a29074a4782bc92622e55ec94c3b11f5b479`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:45:50 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 22:23:44 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.24/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 22:23:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 22:23:45 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:23:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 22:23:45 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 22:23:45 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f365f1b91ebb32c62c3856cd602b14702103c16ede6873855d0c5a5faa874810`  
		Last Modified: Mon, 23 Mar 2020 23:47:03 GMT  
		Size: 694.1 KB (694143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9cb6e408627ad0a100994d33c802c10828d8373fb7234572e0235fca9d7294c`  
		Last Modified: Wed, 25 Mar 2020 22:24:39 GMT  
		Size: 21.1 MB (21119525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5c0f262e2748518c0df991fbe02ea98c1eb9fc9a355c8eb8ca0c4cd4b43b55`  
		Last Modified: Wed, 25 Mar 2020 22:24:34 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:4f2a0e53c458ad8c389a40413c074135270a7bd2f82b1eb51a7dd0a5f093ec2b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23088245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd24e8f81b3e69a7b6eee14be566e2fd65f042b52389beb520915838d86f15e3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 03:43:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 21:49:52 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.24/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 21:49:53 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 21:49:54 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:49:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 21:49:55 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 21:49:55 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b73c299e24e9aa32bbbec493b7588c3a6592d11b52ccb01c156037b819aef46`  
		Last Modified: Tue, 24 Mar 2020 03:47:03 GMT  
		Size: 698.1 KB (698067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65b61609c3447263dc8c67420226770998aab72683c8da887882dda9a04761d`  
		Last Modified: Wed, 25 Mar 2020 21:50:48 GMT  
		Size: 19.8 MB (19771230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf34024959fde388d8f122f98686c98d2f26a6ee616fac255e9d24a7684480d`  
		Last Modified: Wed, 25 Mar 2020 21:50:40 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:2960a1bff52c4e20800f297ac9491661804f276e4c167c5f477cae56e45bf482
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22911054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10cc83f1529223ab41bc828bcbd1d0b3937e49b4786ab5851376c284cac448b1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 05:52:48 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 21:44:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.24/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 21:44:06 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 21:44:07 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:44:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 21:44:08 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 21:44:08 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc893b889cb9ecb596775296ec01901b5ffcd52efc8691a608afb27fc5be6e6`  
		Last Modified: Tue, 24 Mar 2020 05:55:52 GMT  
		Size: 696.2 KB (696184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46883925a5415d0997e2373210f823fdb48428220d78047fe8ff251f7fc6810`  
		Last Modified: Wed, 25 Mar 2020 21:45:06 GMT  
		Size: 19.5 MB (19491362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09800e005e5decf1b215e0d6adfd8871dafad512432f8e624b6e59c927639d73`  
		Last Modified: Wed, 25 Mar 2020 21:44:59 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b426bd3967d042be18586fe7adb6c566dcb6fcfd17c1e7d8fdc99d672481d747
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:1.7-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:cdd49fc23c498159f787d89d707a0472892b98a7475f733e0066be54ec585c4f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2291142795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32019c1c23bff7833c4766fe4d51a8efb2a3ea4c9512dcbd4a4c04a0b2d90d51`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Mar 2020 22:16:11 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.24/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 25 Mar 2020 22:16:14 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:16:16 GMT
ENTRYPOINT ["/traefik"]
# Wed, 25 Mar 2020 22:16:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:af9dafbf4071c5188d0bacf25804474510f4ed2632d998299e90d50759d1c345`  
		Last Modified: Wed, 25 Mar 2020 22:17:08 GMT  
		Size: 25.8 MB (25801842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912d37b34307d1c69659cb03f9fc4935e7fc4b6f77f739d272ed6b19a0998081`  
		Last Modified: Wed, 25 Mar 2020 22:17:02 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f437a5e5ec2a4c30cac218fed1c9d68c25a39998424ca2ee0b70bfdc37d815c1`  
		Last Modified: Wed, 25 Mar 2020 22:17:02 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736087e6923330749a7eb4dc3fc0d6ef3787429db038a584539e1a5d3e35bd23`  
		Last Modified: Wed, 25 Mar 2020 22:17:02 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.2`

```console
$ docker pull traefik@sha256:615483752426932469aa2229ef3f0825b33b3ad7e1326dcd388205cb3a74352e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.2` - linux; amd64

```console
$ docker pull traefik@sha256:14591144dc8a5dc71dea7ac160683f5578bfbc9cf97aeb042270f843c68e0b17
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.8 MB (24783196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:085ead62a4d4b06c34090d14b0f0b516d44777c7b9d71d36f09410f0aef9e5f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:45:50 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 22:23:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0/traefik_v2.2.0_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 22:23:37 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 22:23:38 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:23:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 22:23:38 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 22:23:38 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f365f1b91ebb32c62c3856cd602b14702103c16ede6873855d0c5a5faa874810`  
		Last Modified: Mon, 23 Mar 2020 23:47:03 GMT  
		Size: 694.1 KB (694143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc367a6045f5900ec7708f21ef9df2d7ad7483e36d85979057667e0b3866bdb6`  
		Last Modified: Wed, 25 Mar 2020 22:24:27 GMT  
		Size: 21.3 MB (21285429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff697159d0030e6aa732f628239bba97a20cfba5cc1c0de77e822a794efedd5c`  
		Last Modified: Wed, 25 Mar 2020 22:24:22 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.2` - linux; arm variant v6

```console
$ docker pull traefik@sha256:270be8c81ce1f3fd9e507ee5650b1fd1436524b824191d7a3c544a4cf8a6691c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.3 MB (23305889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:736f4bc7eb2b854949899ad08e8a9780abc4b29446eef07ef7dc700186b7dd14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 03:43:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 21:49:39 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0/traefik_v2.2.0_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 21:49:40 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 21:49:41 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:49:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 21:49:42 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 21:49:42 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b73c299e24e9aa32bbbec493b7588c3a6592d11b52ccb01c156037b819aef46`  
		Last Modified: Tue, 24 Mar 2020 03:47:03 GMT  
		Size: 698.1 KB (698067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc381da900f5d2e94abf26cfc9f11efbec2599125dbc8181d4b32942e0a69f56`  
		Last Modified: Wed, 25 Mar 2020 21:50:30 GMT  
		Size: 20.0 MB (19988874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99b8e78c75f49ffc9e249e66cfcecd68bc3b77d2d85735efaab87ffb5203677`  
		Last Modified: Wed, 25 Mar 2020 21:50:23 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.2` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:6d0a99e202bc3f732000a78b696281369b771234893fff22106471f3d65daffb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23053503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20d0e36d477b886f5ede8ae4753d1cef2acd7570659836ba0f4ab2e743d55bcd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 05:52:48 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 21:43:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0/traefik_v2.2.0_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 21:43:54 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 21:43:55 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:43:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 21:43:56 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 21:43:57 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc893b889cb9ecb596775296ec01901b5ffcd52efc8691a608afb27fc5be6e6`  
		Last Modified: Tue, 24 Mar 2020 05:55:52 GMT  
		Size: 696.2 KB (696184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b612f6b713c999a6de7f98b8c222af24cf379ecb710e67b5c5c51d55510f28`  
		Last Modified: Wed, 25 Mar 2020 21:44:44 GMT  
		Size: 19.6 MB (19633812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687ff5f94664c57720083b9b43ff6fe9b9d232b33ea28f07dfc57140fac200f6`  
		Last Modified: Wed, 25 Mar 2020 21:44:38 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.2.0`

```console
$ docker pull traefik@sha256:615483752426932469aa2229ef3f0825b33b3ad7e1326dcd388205cb3a74352e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.2.0` - linux; amd64

```console
$ docker pull traefik@sha256:14591144dc8a5dc71dea7ac160683f5578bfbc9cf97aeb042270f843c68e0b17
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.8 MB (24783196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:085ead62a4d4b06c34090d14b0f0b516d44777c7b9d71d36f09410f0aef9e5f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:45:50 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 22:23:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0/traefik_v2.2.0_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 22:23:37 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 22:23:38 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:23:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 22:23:38 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 22:23:38 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f365f1b91ebb32c62c3856cd602b14702103c16ede6873855d0c5a5faa874810`  
		Last Modified: Mon, 23 Mar 2020 23:47:03 GMT  
		Size: 694.1 KB (694143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc367a6045f5900ec7708f21ef9df2d7ad7483e36d85979057667e0b3866bdb6`  
		Last Modified: Wed, 25 Mar 2020 22:24:27 GMT  
		Size: 21.3 MB (21285429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff697159d0030e6aa732f628239bba97a20cfba5cc1c0de77e822a794efedd5c`  
		Last Modified: Wed, 25 Mar 2020 22:24:22 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.2.0` - linux; arm variant v6

```console
$ docker pull traefik@sha256:270be8c81ce1f3fd9e507ee5650b1fd1436524b824191d7a3c544a4cf8a6691c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.3 MB (23305889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:736f4bc7eb2b854949899ad08e8a9780abc4b29446eef07ef7dc700186b7dd14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 03:43:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 21:49:39 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0/traefik_v2.2.0_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 21:49:40 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 21:49:41 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:49:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 21:49:42 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 21:49:42 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b73c299e24e9aa32bbbec493b7588c3a6592d11b52ccb01c156037b819aef46`  
		Last Modified: Tue, 24 Mar 2020 03:47:03 GMT  
		Size: 698.1 KB (698067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc381da900f5d2e94abf26cfc9f11efbec2599125dbc8181d4b32942e0a69f56`  
		Last Modified: Wed, 25 Mar 2020 21:50:30 GMT  
		Size: 20.0 MB (19988874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99b8e78c75f49ffc9e249e66cfcecd68bc3b77d2d85735efaab87ffb5203677`  
		Last Modified: Wed, 25 Mar 2020 21:50:23 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.2.0` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:6d0a99e202bc3f732000a78b696281369b771234893fff22106471f3d65daffb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23053503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20d0e36d477b886f5ede8ae4753d1cef2acd7570659836ba0f4ab2e743d55bcd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 05:52:48 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 21:43:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0/traefik_v2.2.0_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 21:43:54 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 21:43:55 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:43:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 21:43:56 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 21:43:57 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc893b889cb9ecb596775296ec01901b5ffcd52efc8691a608afb27fc5be6e6`  
		Last Modified: Tue, 24 Mar 2020 05:55:52 GMT  
		Size: 696.2 KB (696184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b612f6b713c999a6de7f98b8c222af24cf379ecb710e67b5c5c51d55510f28`  
		Last Modified: Wed, 25 Mar 2020 21:44:44 GMT  
		Size: 19.6 MB (19633812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687ff5f94664c57720083b9b43ff6fe9b9d232b33ea28f07dfc57140fac200f6`  
		Last Modified: Wed, 25 Mar 2020 21:44:38 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.2.0-windowsservercore-1809`

```console
$ docker pull traefik@sha256:fe6e0415135464e6f7f8071af475cea23b6e2c2cd1b62b84730d47aa5adb4597
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:2.2.0-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:44af67ec4d7ee639d6981625961cef63ea5cb78b2ef9edbfc18a3ad445cd6e64
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2291277474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73d76399547b88a3d964fb7eaa5733d4fb87e72d74b20f1f82a54ddb540cb50c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Mar 2020 22:15:07 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.2.0/traefik_v2.2.0_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 25 Mar 2020 22:15:12 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:15:13 GMT
ENTRYPOINT ["/traefik"]
# Wed, 25 Mar 2020 22:15:14 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:35030e579ef70c21318512a160fd079dd8f970997106efcf78786e9ab1000b27`  
		Last Modified: Wed, 25 Mar 2020 22:16:46 GMT  
		Size: 25.9 MB (25936523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6146f53de7073bee8aaf32ea1f114a598bc979d2c95d7aea012a43b37b7b2509`  
		Last Modified: Wed, 25 Mar 2020 22:16:39 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5200557f5e26f8ba1a7321f87fe4402ef5c3fbf86abf1b086f3519b348dd6cba`  
		Last Modified: Wed, 25 Mar 2020 22:16:39 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b358f870169f5b072e7bfe113d68bbb8d94386b00413c1bcbd9706efcaaed6bb`  
		Last Modified: Wed, 25 Mar 2020 22:16:40 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:fe6e0415135464e6f7f8071af475cea23b6e2c2cd1b62b84730d47aa5adb4597
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:2.2-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:44af67ec4d7ee639d6981625961cef63ea5cb78b2ef9edbfc18a3ad445cd6e64
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2291277474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73d76399547b88a3d964fb7eaa5733d4fb87e72d74b20f1f82a54ddb540cb50c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Mar 2020 22:15:07 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.2.0/traefik_v2.2.0_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 25 Mar 2020 22:15:12 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:15:13 GMT
ENTRYPOINT ["/traefik"]
# Wed, 25 Mar 2020 22:15:14 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:35030e579ef70c21318512a160fd079dd8f970997106efcf78786e9ab1000b27`  
		Last Modified: Wed, 25 Mar 2020 22:16:46 GMT  
		Size: 25.9 MB (25936523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6146f53de7073bee8aaf32ea1f114a598bc979d2c95d7aea012a43b37b7b2509`  
		Last Modified: Wed, 25 Mar 2020 22:16:39 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5200557f5e26f8ba1a7321f87fe4402ef5c3fbf86abf1b086f3519b348dd6cba`  
		Last Modified: Wed, 25 Mar 2020 22:16:39 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b358f870169f5b072e7bfe113d68bbb8d94386b00413c1bcbd9706efcaaed6bb`  
		Last Modified: Wed, 25 Mar 2020 22:16:40 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:chevrotin`

```console
$ docker pull traefik@sha256:615483752426932469aa2229ef3f0825b33b3ad7e1326dcd388205cb3a74352e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:chevrotin` - linux; amd64

```console
$ docker pull traefik@sha256:14591144dc8a5dc71dea7ac160683f5578bfbc9cf97aeb042270f843c68e0b17
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.8 MB (24783196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:085ead62a4d4b06c34090d14b0f0b516d44777c7b9d71d36f09410f0aef9e5f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:45:50 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 22:23:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0/traefik_v2.2.0_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 22:23:37 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 22:23:38 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:23:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 22:23:38 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 22:23:38 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f365f1b91ebb32c62c3856cd602b14702103c16ede6873855d0c5a5faa874810`  
		Last Modified: Mon, 23 Mar 2020 23:47:03 GMT  
		Size: 694.1 KB (694143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc367a6045f5900ec7708f21ef9df2d7ad7483e36d85979057667e0b3866bdb6`  
		Last Modified: Wed, 25 Mar 2020 22:24:27 GMT  
		Size: 21.3 MB (21285429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff697159d0030e6aa732f628239bba97a20cfba5cc1c0de77e822a794efedd5c`  
		Last Modified: Wed, 25 Mar 2020 22:24:22 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:chevrotin` - linux; arm variant v6

```console
$ docker pull traefik@sha256:270be8c81ce1f3fd9e507ee5650b1fd1436524b824191d7a3c544a4cf8a6691c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.3 MB (23305889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:736f4bc7eb2b854949899ad08e8a9780abc4b29446eef07ef7dc700186b7dd14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 03:43:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 21:49:39 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0/traefik_v2.2.0_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 21:49:40 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 21:49:41 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:49:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 21:49:42 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 21:49:42 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b73c299e24e9aa32bbbec493b7588c3a6592d11b52ccb01c156037b819aef46`  
		Last Modified: Tue, 24 Mar 2020 03:47:03 GMT  
		Size: 698.1 KB (698067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc381da900f5d2e94abf26cfc9f11efbec2599125dbc8181d4b32942e0a69f56`  
		Last Modified: Wed, 25 Mar 2020 21:50:30 GMT  
		Size: 20.0 MB (19988874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99b8e78c75f49ffc9e249e66cfcecd68bc3b77d2d85735efaab87ffb5203677`  
		Last Modified: Wed, 25 Mar 2020 21:50:23 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:chevrotin` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:6d0a99e202bc3f732000a78b696281369b771234893fff22106471f3d65daffb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23053503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20d0e36d477b886f5ede8ae4753d1cef2acd7570659836ba0f4ab2e743d55bcd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 05:52:48 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 21:43:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0/traefik_v2.2.0_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 21:43:54 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 21:43:55 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:43:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 21:43:56 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 21:43:57 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc893b889cb9ecb596775296ec01901b5ffcd52efc8691a608afb27fc5be6e6`  
		Last Modified: Tue, 24 Mar 2020 05:55:52 GMT  
		Size: 696.2 KB (696184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b612f6b713c999a6de7f98b8c222af24cf379ecb710e67b5c5c51d55510f28`  
		Last Modified: Wed, 25 Mar 2020 21:44:44 GMT  
		Size: 19.6 MB (19633812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687ff5f94664c57720083b9b43ff6fe9b9d232b33ea28f07dfc57140fac200f6`  
		Last Modified: Wed, 25 Mar 2020 21:44:38 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:chevrotin-windowsservercore-1809`

```console
$ docker pull traefik@sha256:fe6e0415135464e6f7f8071af475cea23b6e2c2cd1b62b84730d47aa5adb4597
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:chevrotin-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:44af67ec4d7ee639d6981625961cef63ea5cb78b2ef9edbfc18a3ad445cd6e64
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2291277474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73d76399547b88a3d964fb7eaa5733d4fb87e72d74b20f1f82a54ddb540cb50c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Mar 2020 22:15:07 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.2.0/traefik_v2.2.0_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 25 Mar 2020 22:15:12 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:15:13 GMT
ENTRYPOINT ["/traefik"]
# Wed, 25 Mar 2020 22:15:14 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:35030e579ef70c21318512a160fd079dd8f970997106efcf78786e9ab1000b27`  
		Last Modified: Wed, 25 Mar 2020 22:16:46 GMT  
		Size: 25.9 MB (25936523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6146f53de7073bee8aaf32ea1f114a598bc979d2c95d7aea012a43b37b7b2509`  
		Last Modified: Wed, 25 Mar 2020 22:16:39 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5200557f5e26f8ba1a7321f87fe4402ef5c3fbf86abf1b086f3519b348dd6cba`  
		Last Modified: Wed, 25 Mar 2020 22:16:39 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b358f870169f5b072e7bfe113d68bbb8d94386b00413c1bcbd9706efcaaed6bb`  
		Last Modified: Wed, 25 Mar 2020 22:16:40 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:615483752426932469aa2229ef3f0825b33b3ad7e1326dcd388205cb3a74352e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:14591144dc8a5dc71dea7ac160683f5578bfbc9cf97aeb042270f843c68e0b17
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.8 MB (24783196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:085ead62a4d4b06c34090d14b0f0b516d44777c7b9d71d36f09410f0aef9e5f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:45:50 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 22:23:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0/traefik_v2.2.0_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 22:23:37 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 22:23:38 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:23:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 22:23:38 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 22:23:38 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f365f1b91ebb32c62c3856cd602b14702103c16ede6873855d0c5a5faa874810`  
		Last Modified: Mon, 23 Mar 2020 23:47:03 GMT  
		Size: 694.1 KB (694143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc367a6045f5900ec7708f21ef9df2d7ad7483e36d85979057667e0b3866bdb6`  
		Last Modified: Wed, 25 Mar 2020 22:24:27 GMT  
		Size: 21.3 MB (21285429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff697159d0030e6aa732f628239bba97a20cfba5cc1c0de77e822a794efedd5c`  
		Last Modified: Wed, 25 Mar 2020 22:24:22 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:270be8c81ce1f3fd9e507ee5650b1fd1436524b824191d7a3c544a4cf8a6691c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.3 MB (23305889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:736f4bc7eb2b854949899ad08e8a9780abc4b29446eef07ef7dc700186b7dd14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 03:43:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 21:49:39 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0/traefik_v2.2.0_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 21:49:40 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 21:49:41 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:49:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 21:49:42 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 21:49:42 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b73c299e24e9aa32bbbec493b7588c3a6592d11b52ccb01c156037b819aef46`  
		Last Modified: Tue, 24 Mar 2020 03:47:03 GMT  
		Size: 698.1 KB (698067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc381da900f5d2e94abf26cfc9f11efbec2599125dbc8181d4b32942e0a69f56`  
		Last Modified: Wed, 25 Mar 2020 21:50:30 GMT  
		Size: 20.0 MB (19988874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99b8e78c75f49ffc9e249e66cfcecd68bc3b77d2d85735efaab87ffb5203677`  
		Last Modified: Wed, 25 Mar 2020 21:50:23 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:6d0a99e202bc3f732000a78b696281369b771234893fff22106471f3d65daffb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23053503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20d0e36d477b886f5ede8ae4753d1cef2acd7570659836ba0f4ab2e743d55bcd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 05:52:48 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 21:43:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0/traefik_v2.2.0_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 21:43:54 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 21:43:55 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:43:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 21:43:56 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 21:43:57 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc893b889cb9ecb596775296ec01901b5ffcd52efc8691a608afb27fc5be6e6`  
		Last Modified: Tue, 24 Mar 2020 05:55:52 GMT  
		Size: 696.2 KB (696184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b612f6b713c999a6de7f98b8c222af24cf379ecb710e67b5c5c51d55510f28`  
		Last Modified: Wed, 25 Mar 2020 21:44:44 GMT  
		Size: 19.6 MB (19633812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687ff5f94664c57720083b9b43ff6fe9b9d232b33ea28f07dfc57140fac200f6`  
		Last Modified: Wed, 25 Mar 2020 21:44:38 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles`

```console
$ docker pull traefik@sha256:47bec236a121a07703e27fc3e18c201ae0241cff1038ea2faf5d05bf5ea82286
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles` - linux; amd64

```console
$ docker pull traefik@sha256:bec5a86cd327d82a50fe89aae5c57d49a13bb9c7fe82fcdd7c886adf09645801
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21578312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:100389fa48aa58f1587f27467ac7f319ca8724b7bbad55ee09ada0de310a3bf4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 02:50:22 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 02:50:24 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 25 Mar 2020 22:24:07 GMT
COPY file:1f3cec74af68ac254dc1c90001edd0f7a71f8e42168f4523b5b170d518e50e2a in / 
# Wed, 25 Mar 2020 22:24:07 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:24:07 GMT
VOLUME [/tmp]
# Wed, 25 Mar 2020 22:24:07 GMT
ENTRYPOINT ["/traefik"]
# Wed, 25 Mar 2020 22:24:08 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6f9aa7cec283ff91d23b1d8e88e428fd21f67593d121f450a42173fe6443f190`  
		Last Modified: Wed, 25 Mar 2020 22:24:49 GMT  
		Size: 21.1 MB (21119254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm variant v6

```console
$ docker pull traefik@sha256:1733e40d59ca54506c6b3859245878b29270da0d17eaa5b10322bc83cf5749bc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20230146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6df2ff4474d538ce68e1599c24ef3227b9087dbfa625a1049a3172fe56a021b9`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 03:46:16 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 03:46:17 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 25 Mar 2020 21:50:06 GMT
COPY file:5fc84f7de0956e9c09bc8249cedc256b1ebfbbdf7a970a1b03cbc35342bc98d8 in / 
# Wed, 25 Mar 2020 21:50:07 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:50:07 GMT
VOLUME [/tmp]
# Wed, 25 Mar 2020 21:50:08 GMT
ENTRYPOINT ["/traefik"]
# Wed, 25 Mar 2020 21:50:08 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:cc2e8d91f8cdcad6fef81a6606a958dc4fa4ffe856944124f101909ef0e2a6de`  
		Last Modified: Wed, 25 Mar 2020 21:51:04 GMT  
		Size: 19.8 MB (19771060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7f26aa867bbfa1637f66f2faee17fd66549e441185789b64aa07f0326e75f321
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.0 MB (19950262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7b0a67ae19f09c258a8a530bf8f7315c03f0157c72a093a495d017a4d8032a`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 05:55:25 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 05:55:26 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 25 Mar 2020 21:44:21 GMT
COPY file:0347658f660b1b9c0951c6a64bfc0f8a407487940ca58f7d6da08472f61358db in / 
# Wed, 25 Mar 2020 21:44:21 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:44:22 GMT
VOLUME [/tmp]
# Wed, 25 Mar 2020 21:44:23 GMT
ENTRYPOINT ["/traefik"]
# Wed, 25 Mar 2020 21:44:23 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:e41d3d1eaac6c67b9dab999e93238a86c8df48b874e4225dd36534ce81905c58`  
		Last Modified: Wed, 25 Mar 2020 21:45:23 GMT  
		Size: 19.5 MB (19491184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-alpine`

```console
$ docker pull traefik@sha256:a5be418acbd9a1a3011242c27feadd440ca56afbec22a7763150202de397cb6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:178c67d6e375ce45264f1a47eef709bca9928ac85badaa8f0d877059d5f37b6a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24617292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa4204cec7f48d0cc16d69e25ac8a29074a4782bc92622e55ec94c3b11f5b479`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:45:50 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 22:23:44 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.24/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 22:23:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 22:23:45 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:23:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 22:23:45 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 22:23:45 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f365f1b91ebb32c62c3856cd602b14702103c16ede6873855d0c5a5faa874810`  
		Last Modified: Mon, 23 Mar 2020 23:47:03 GMT  
		Size: 694.1 KB (694143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9cb6e408627ad0a100994d33c802c10828d8373fb7234572e0235fca9d7294c`  
		Last Modified: Wed, 25 Mar 2020 22:24:39 GMT  
		Size: 21.1 MB (21119525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5c0f262e2748518c0df991fbe02ea98c1eb9fc9a355c8eb8ca0c4cd4b43b55`  
		Last Modified: Wed, 25 Mar 2020 22:24:34 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:4f2a0e53c458ad8c389a40413c074135270a7bd2f82b1eb51a7dd0a5f093ec2b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23088245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd24e8f81b3e69a7b6eee14be566e2fd65f042b52389beb520915838d86f15e3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 03:43:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 21:49:52 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.24/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 21:49:53 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 21:49:54 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:49:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 21:49:55 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 21:49:55 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b73c299e24e9aa32bbbec493b7588c3a6592d11b52ccb01c156037b819aef46`  
		Last Modified: Tue, 24 Mar 2020 03:47:03 GMT  
		Size: 698.1 KB (698067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65b61609c3447263dc8c67420226770998aab72683c8da887882dda9a04761d`  
		Last Modified: Wed, 25 Mar 2020 21:50:48 GMT  
		Size: 19.8 MB (19771230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf34024959fde388d8f122f98686c98d2f26a6ee616fac255e9d24a7684480d`  
		Last Modified: Wed, 25 Mar 2020 21:50:40 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:2960a1bff52c4e20800f297ac9491661804f276e4c167c5f477cae56e45bf482
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22911054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10cc83f1529223ab41bc828bcbd1d0b3937e49b4786ab5851376c284cac448b1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 05:52:48 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 21:44:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.24/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 21:44:06 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 21:44:07 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:44:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 21:44:08 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 21:44:08 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc893b889cb9ecb596775296ec01901b5ffcd52efc8691a608afb27fc5be6e6`  
		Last Modified: Tue, 24 Mar 2020 05:55:52 GMT  
		Size: 696.2 KB (696184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46883925a5415d0997e2373210f823fdb48428220d78047fe8ff251f7fc6810`  
		Last Modified: Wed, 25 Mar 2020 21:45:06 GMT  
		Size: 19.5 MB (19491362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09800e005e5decf1b215e0d6adfd8871dafad512432f8e624b6e59c927639d73`  
		Last Modified: Wed, 25 Mar 2020 21:44:59 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b426bd3967d042be18586fe7adb6c566dcb6fcfd17c1e7d8fdc99d672481d747
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:cdd49fc23c498159f787d89d707a0472892b98a7475f733e0066be54ec585c4f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2291142795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32019c1c23bff7833c4766fe4d51a8efb2a3ea4c9512dcbd4a4c04a0b2d90d51`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Mar 2020 22:16:11 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.24/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 25 Mar 2020 22:16:14 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:16:16 GMT
ENTRYPOINT ["/traefik"]
# Wed, 25 Mar 2020 22:16:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:af9dafbf4071c5188d0bacf25804474510f4ed2632d998299e90d50759d1c345`  
		Last Modified: Wed, 25 Mar 2020 22:17:08 GMT  
		Size: 25.8 MB (25801842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912d37b34307d1c69659cb03f9fc4935e7fc4b6f77f739d272ed6b19a0998081`  
		Last Modified: Wed, 25 Mar 2020 22:17:02 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f437a5e5ec2a4c30cac218fed1c9d68c25a39998424ca2ee0b70bfdc37d815c1`  
		Last Modified: Wed, 25 Mar 2020 22:17:02 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736087e6923330749a7eb4dc3fc0d6ef3787429db038a584539e1a5d3e35bd23`  
		Last Modified: Wed, 25 Mar 2020 22:17:02 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7`

```console
$ docker pull traefik@sha256:47bec236a121a07703e27fc3e18c201ae0241cff1038ea2faf5d05bf5ea82286
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7` - linux; amd64

```console
$ docker pull traefik@sha256:bec5a86cd327d82a50fe89aae5c57d49a13bb9c7fe82fcdd7c886adf09645801
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21578312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:100389fa48aa58f1587f27467ac7f319ca8724b7bbad55ee09ada0de310a3bf4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 02:50:22 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 02:50:24 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 25 Mar 2020 22:24:07 GMT
COPY file:1f3cec74af68ac254dc1c90001edd0f7a71f8e42168f4523b5b170d518e50e2a in / 
# Wed, 25 Mar 2020 22:24:07 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:24:07 GMT
VOLUME [/tmp]
# Wed, 25 Mar 2020 22:24:07 GMT
ENTRYPOINT ["/traefik"]
# Wed, 25 Mar 2020 22:24:08 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6f9aa7cec283ff91d23b1d8e88e428fd21f67593d121f450a42173fe6443f190`  
		Last Modified: Wed, 25 Mar 2020 22:24:49 GMT  
		Size: 21.1 MB (21119254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:1733e40d59ca54506c6b3859245878b29270da0d17eaa5b10322bc83cf5749bc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20230146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6df2ff4474d538ce68e1599c24ef3227b9087dbfa625a1049a3172fe56a021b9`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 03:46:16 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 03:46:17 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 25 Mar 2020 21:50:06 GMT
COPY file:5fc84f7de0956e9c09bc8249cedc256b1ebfbbdf7a970a1b03cbc35342bc98d8 in / 
# Wed, 25 Mar 2020 21:50:07 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:50:07 GMT
VOLUME [/tmp]
# Wed, 25 Mar 2020 21:50:08 GMT
ENTRYPOINT ["/traefik"]
# Wed, 25 Mar 2020 21:50:08 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:cc2e8d91f8cdcad6fef81a6606a958dc4fa4ffe856944124f101909ef0e2a6de`  
		Last Modified: Wed, 25 Mar 2020 21:51:04 GMT  
		Size: 19.8 MB (19771060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7f26aa867bbfa1637f66f2faee17fd66549e441185789b64aa07f0326e75f321
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.0 MB (19950262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7b0a67ae19f09c258a8a530bf8f7315c03f0157c72a093a495d017a4d8032a`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 05:55:25 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 05:55:26 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 25 Mar 2020 21:44:21 GMT
COPY file:0347658f660b1b9c0951c6a64bfc0f8a407487940ca58f7d6da08472f61358db in / 
# Wed, 25 Mar 2020 21:44:21 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:44:22 GMT
VOLUME [/tmp]
# Wed, 25 Mar 2020 21:44:23 GMT
ENTRYPOINT ["/traefik"]
# Wed, 25 Mar 2020 21:44:23 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:e41d3d1eaac6c67b9dab999e93238a86c8df48b874e4225dd36534ce81905c58`  
		Last Modified: Wed, 25 Mar 2020 21:45:23 GMT  
		Size: 19.5 MB (19491184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.24`

```console
$ docker pull traefik@sha256:47bec236a121a07703e27fc3e18c201ae0241cff1038ea2faf5d05bf5ea82286
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.24` - linux; amd64

```console
$ docker pull traefik@sha256:bec5a86cd327d82a50fe89aae5c57d49a13bb9c7fe82fcdd7c886adf09645801
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21578312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:100389fa48aa58f1587f27467ac7f319ca8724b7bbad55ee09ada0de310a3bf4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 21 Feb 2020 02:50:22 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Fri, 21 Feb 2020 02:50:24 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 25 Mar 2020 22:24:07 GMT
COPY file:1f3cec74af68ac254dc1c90001edd0f7a71f8e42168f4523b5b170d518e50e2a in / 
# Wed, 25 Mar 2020 22:24:07 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:24:07 GMT
VOLUME [/tmp]
# Wed, 25 Mar 2020 22:24:07 GMT
ENTRYPOINT ["/traefik"]
# Wed, 25 Mar 2020 22:24:08 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6f9aa7cec283ff91d23b1d8e88e428fd21f67593d121f450a42173fe6443f190`  
		Last Modified: Wed, 25 Mar 2020 22:24:49 GMT  
		Size: 21.1 MB (21119254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.24` - linux; arm variant v6

```console
$ docker pull traefik@sha256:1733e40d59ca54506c6b3859245878b29270da0d17eaa5b10322bc83cf5749bc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20230146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6df2ff4474d538ce68e1599c24ef3227b9087dbfa625a1049a3172fe56a021b9`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 03:46:16 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 03:46:17 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 25 Mar 2020 21:50:06 GMT
COPY file:5fc84f7de0956e9c09bc8249cedc256b1ebfbbdf7a970a1b03cbc35342bc98d8 in / 
# Wed, 25 Mar 2020 21:50:07 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:50:07 GMT
VOLUME [/tmp]
# Wed, 25 Mar 2020 21:50:08 GMT
ENTRYPOINT ["/traefik"]
# Wed, 25 Mar 2020 21:50:08 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:cc2e8d91f8cdcad6fef81a6606a958dc4fa4ffe856944124f101909ef0e2a6de`  
		Last Modified: Wed, 25 Mar 2020 21:51:04 GMT  
		Size: 19.8 MB (19771060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.24` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7f26aa867bbfa1637f66f2faee17fd66549e441185789b64aa07f0326e75f321
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.0 MB (19950262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7b0a67ae19f09c258a8a530bf8f7315c03f0157c72a093a495d017a4d8032a`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 24 Mar 2020 05:55:25 GMT
COPY file:c1f4ee36c6a15bdd9f8e9d8fd7b3c37c57af612bce8638eaf7a83e7873de24cb in /etc/ssl/certs/ 
# Tue, 24 Mar 2020 05:55:26 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Wed, 25 Mar 2020 21:44:21 GMT
COPY file:0347658f660b1b9c0951c6a64bfc0f8a407487940ca58f7d6da08472f61358db in / 
# Wed, 25 Mar 2020 21:44:21 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:44:22 GMT
VOLUME [/tmp]
# Wed, 25 Mar 2020 21:44:23 GMT
ENTRYPOINT ["/traefik"]
# Wed, 25 Mar 2020 21:44:23 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:e41d3d1eaac6c67b9dab999e93238a86c8df48b874e4225dd36534ce81905c58`  
		Last Modified: Wed, 25 Mar 2020 21:45:23 GMT  
		Size: 19.5 MB (19491184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.24-alpine`

```console
$ docker pull traefik@sha256:a5be418acbd9a1a3011242c27feadd440ca56afbec22a7763150202de397cb6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.24-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:178c67d6e375ce45264f1a47eef709bca9928ac85badaa8f0d877059d5f37b6a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24617292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa4204cec7f48d0cc16d69e25ac8a29074a4782bc92622e55ec94c3b11f5b479`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:45:50 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 22:23:44 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.24/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 22:23:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 22:23:45 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:23:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 22:23:45 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 22:23:45 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f365f1b91ebb32c62c3856cd602b14702103c16ede6873855d0c5a5faa874810`  
		Last Modified: Mon, 23 Mar 2020 23:47:03 GMT  
		Size: 694.1 KB (694143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9cb6e408627ad0a100994d33c802c10828d8373fb7234572e0235fca9d7294c`  
		Last Modified: Wed, 25 Mar 2020 22:24:39 GMT  
		Size: 21.1 MB (21119525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5c0f262e2748518c0df991fbe02ea98c1eb9fc9a355c8eb8ca0c4cd4b43b55`  
		Last Modified: Wed, 25 Mar 2020 22:24:34 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.24-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:4f2a0e53c458ad8c389a40413c074135270a7bd2f82b1eb51a7dd0a5f093ec2b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23088245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd24e8f81b3e69a7b6eee14be566e2fd65f042b52389beb520915838d86f15e3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 03:43:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 21:49:52 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.24/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 21:49:53 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 21:49:54 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:49:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 21:49:55 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 21:49:55 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b73c299e24e9aa32bbbec493b7588c3a6592d11b52ccb01c156037b819aef46`  
		Last Modified: Tue, 24 Mar 2020 03:47:03 GMT  
		Size: 698.1 KB (698067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65b61609c3447263dc8c67420226770998aab72683c8da887882dda9a04761d`  
		Last Modified: Wed, 25 Mar 2020 21:50:48 GMT  
		Size: 19.8 MB (19771230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf34024959fde388d8f122f98686c98d2f26a6ee616fac255e9d24a7684480d`  
		Last Modified: Wed, 25 Mar 2020 21:50:40 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.24-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:2960a1bff52c4e20800f297ac9491661804f276e4c167c5f477cae56e45bf482
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22911054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10cc83f1529223ab41bc828bcbd1d0b3937e49b4786ab5851376c284cac448b1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 05:52:48 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 21:44:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.24/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 21:44:06 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 21:44:07 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:44:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 21:44:08 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 21:44:08 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc893b889cb9ecb596775296ec01901b5ffcd52efc8691a608afb27fc5be6e6`  
		Last Modified: Tue, 24 Mar 2020 05:55:52 GMT  
		Size: 696.2 KB (696184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46883925a5415d0997e2373210f823fdb48428220d78047fe8ff251f7fc6810`  
		Last Modified: Wed, 25 Mar 2020 21:45:06 GMT  
		Size: 19.5 MB (19491362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09800e005e5decf1b215e0d6adfd8871dafad512432f8e624b6e59c927639d73`  
		Last Modified: Wed, 25 Mar 2020 21:44:59 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.24-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b426bd3967d042be18586fe7adb6c566dcb6fcfd17c1e7d8fdc99d672481d747
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:v1.7.24-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:cdd49fc23c498159f787d89d707a0472892b98a7475f733e0066be54ec585c4f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2291142795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32019c1c23bff7833c4766fe4d51a8efb2a3ea4c9512dcbd4a4c04a0b2d90d51`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Mar 2020 22:16:11 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.24/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 25 Mar 2020 22:16:14 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:16:16 GMT
ENTRYPOINT ["/traefik"]
# Wed, 25 Mar 2020 22:16:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:af9dafbf4071c5188d0bacf25804474510f4ed2632d998299e90d50759d1c345`  
		Last Modified: Wed, 25 Mar 2020 22:17:08 GMT  
		Size: 25.8 MB (25801842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912d37b34307d1c69659cb03f9fc4935e7fc4b6f77f739d272ed6b19a0998081`  
		Last Modified: Wed, 25 Mar 2020 22:17:02 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f437a5e5ec2a4c30cac218fed1c9d68c25a39998424ca2ee0b70bfdc37d815c1`  
		Last Modified: Wed, 25 Mar 2020 22:17:02 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736087e6923330749a7eb4dc3fc0d6ef3787429db038a584539e1a5d3e35bd23`  
		Last Modified: Wed, 25 Mar 2020 22:17:02 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-alpine`

```console
$ docker pull traefik@sha256:a5be418acbd9a1a3011242c27feadd440ca56afbec22a7763150202de397cb6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:178c67d6e375ce45264f1a47eef709bca9928ac85badaa8f0d877059d5f37b6a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24617292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa4204cec7f48d0cc16d69e25ac8a29074a4782bc92622e55ec94c3b11f5b479`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:45:50 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 22:23:44 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.24/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 22:23:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 22:23:45 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:23:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 22:23:45 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 22:23:45 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f365f1b91ebb32c62c3856cd602b14702103c16ede6873855d0c5a5faa874810`  
		Last Modified: Mon, 23 Mar 2020 23:47:03 GMT  
		Size: 694.1 KB (694143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9cb6e408627ad0a100994d33c802c10828d8373fb7234572e0235fca9d7294c`  
		Last Modified: Wed, 25 Mar 2020 22:24:39 GMT  
		Size: 21.1 MB (21119525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5c0f262e2748518c0df991fbe02ea98c1eb9fc9a355c8eb8ca0c4cd4b43b55`  
		Last Modified: Wed, 25 Mar 2020 22:24:34 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:4f2a0e53c458ad8c389a40413c074135270a7bd2f82b1eb51a7dd0a5f093ec2b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23088245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd24e8f81b3e69a7b6eee14be566e2fd65f042b52389beb520915838d86f15e3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 03:43:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 21:49:52 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.24/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 21:49:53 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 21:49:54 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:49:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 21:49:55 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 21:49:55 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b73c299e24e9aa32bbbec493b7588c3a6592d11b52ccb01c156037b819aef46`  
		Last Modified: Tue, 24 Mar 2020 03:47:03 GMT  
		Size: 698.1 KB (698067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65b61609c3447263dc8c67420226770998aab72683c8da887882dda9a04761d`  
		Last Modified: Wed, 25 Mar 2020 21:50:48 GMT  
		Size: 19.8 MB (19771230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf34024959fde388d8f122f98686c98d2f26a6ee616fac255e9d24a7684480d`  
		Last Modified: Wed, 25 Mar 2020 21:50:40 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:2960a1bff52c4e20800f297ac9491661804f276e4c167c5f477cae56e45bf482
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22911054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10cc83f1529223ab41bc828bcbd1d0b3937e49b4786ab5851376c284cac448b1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 05:52:48 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 21:44:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.24/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 21:44:06 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 21:44:07 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:44:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 21:44:08 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 21:44:08 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc893b889cb9ecb596775296ec01901b5ffcd52efc8691a608afb27fc5be6e6`  
		Last Modified: Tue, 24 Mar 2020 05:55:52 GMT  
		Size: 696.2 KB (696184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46883925a5415d0997e2373210f823fdb48428220d78047fe8ff251f7fc6810`  
		Last Modified: Wed, 25 Mar 2020 21:45:06 GMT  
		Size: 19.5 MB (19491362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09800e005e5decf1b215e0d6adfd8871dafad512432f8e624b6e59c927639d73`  
		Last Modified: Wed, 25 Mar 2020 21:44:59 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b426bd3967d042be18586fe7adb6c566dcb6fcfd17c1e7d8fdc99d672481d747
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:v1.7-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:cdd49fc23c498159f787d89d707a0472892b98a7475f733e0066be54ec585c4f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2291142795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32019c1c23bff7833c4766fe4d51a8efb2a3ea4c9512dcbd4a4c04a0b2d90d51`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Mar 2020 22:16:11 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.24/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 25 Mar 2020 22:16:14 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:16:16 GMT
ENTRYPOINT ["/traefik"]
# Wed, 25 Mar 2020 22:16:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.24 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:af9dafbf4071c5188d0bacf25804474510f4ed2632d998299e90d50759d1c345`  
		Last Modified: Wed, 25 Mar 2020 22:17:08 GMT  
		Size: 25.8 MB (25801842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912d37b34307d1c69659cb03f9fc4935e7fc4b6f77f739d272ed6b19a0998081`  
		Last Modified: Wed, 25 Mar 2020 22:17:02 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f437a5e5ec2a4c30cac218fed1c9d68c25a39998424ca2ee0b70bfdc37d815c1`  
		Last Modified: Wed, 25 Mar 2020 22:17:02 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736087e6923330749a7eb4dc3fc0d6ef3787429db038a584539e1a5d3e35bd23`  
		Last Modified: Wed, 25 Mar 2020 22:17:02 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.2`

```console
$ docker pull traefik@sha256:615483752426932469aa2229ef3f0825b33b3ad7e1326dcd388205cb3a74352e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.2` - linux; amd64

```console
$ docker pull traefik@sha256:14591144dc8a5dc71dea7ac160683f5578bfbc9cf97aeb042270f843c68e0b17
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.8 MB (24783196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:085ead62a4d4b06c34090d14b0f0b516d44777c7b9d71d36f09410f0aef9e5f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:45:50 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 22:23:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0/traefik_v2.2.0_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 22:23:37 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 22:23:38 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:23:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 22:23:38 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 22:23:38 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f365f1b91ebb32c62c3856cd602b14702103c16ede6873855d0c5a5faa874810`  
		Last Modified: Mon, 23 Mar 2020 23:47:03 GMT  
		Size: 694.1 KB (694143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc367a6045f5900ec7708f21ef9df2d7ad7483e36d85979057667e0b3866bdb6`  
		Last Modified: Wed, 25 Mar 2020 22:24:27 GMT  
		Size: 21.3 MB (21285429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff697159d0030e6aa732f628239bba97a20cfba5cc1c0de77e822a794efedd5c`  
		Last Modified: Wed, 25 Mar 2020 22:24:22 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.2` - linux; arm variant v6

```console
$ docker pull traefik@sha256:270be8c81ce1f3fd9e507ee5650b1fd1436524b824191d7a3c544a4cf8a6691c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.3 MB (23305889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:736f4bc7eb2b854949899ad08e8a9780abc4b29446eef07ef7dc700186b7dd14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 03:43:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 21:49:39 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0/traefik_v2.2.0_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 21:49:40 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 21:49:41 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:49:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 21:49:42 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 21:49:42 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b73c299e24e9aa32bbbec493b7588c3a6592d11b52ccb01c156037b819aef46`  
		Last Modified: Tue, 24 Mar 2020 03:47:03 GMT  
		Size: 698.1 KB (698067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc381da900f5d2e94abf26cfc9f11efbec2599125dbc8181d4b32942e0a69f56`  
		Last Modified: Wed, 25 Mar 2020 21:50:30 GMT  
		Size: 20.0 MB (19988874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99b8e78c75f49ffc9e249e66cfcecd68bc3b77d2d85735efaab87ffb5203677`  
		Last Modified: Wed, 25 Mar 2020 21:50:23 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.2` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:6d0a99e202bc3f732000a78b696281369b771234893fff22106471f3d65daffb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23053503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20d0e36d477b886f5ede8ae4753d1cef2acd7570659836ba0f4ab2e743d55bcd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 05:52:48 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 21:43:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0/traefik_v2.2.0_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 21:43:54 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 21:43:55 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:43:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 21:43:56 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 21:43:57 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc893b889cb9ecb596775296ec01901b5ffcd52efc8691a608afb27fc5be6e6`  
		Last Modified: Tue, 24 Mar 2020 05:55:52 GMT  
		Size: 696.2 KB (696184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b612f6b713c999a6de7f98b8c222af24cf379ecb710e67b5c5c51d55510f28`  
		Last Modified: Wed, 25 Mar 2020 21:44:44 GMT  
		Size: 19.6 MB (19633812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687ff5f94664c57720083b9b43ff6fe9b9d232b33ea28f07dfc57140fac200f6`  
		Last Modified: Wed, 25 Mar 2020 21:44:38 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.2.0`

```console
$ docker pull traefik@sha256:615483752426932469aa2229ef3f0825b33b3ad7e1326dcd388205cb3a74352e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.2.0` - linux; amd64

```console
$ docker pull traefik@sha256:14591144dc8a5dc71dea7ac160683f5578bfbc9cf97aeb042270f843c68e0b17
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.8 MB (24783196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:085ead62a4d4b06c34090d14b0f0b516d44777c7b9d71d36f09410f0aef9e5f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:45:50 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 22:23:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0/traefik_v2.2.0_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 22:23:37 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 22:23:38 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:23:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 22:23:38 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 22:23:38 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f365f1b91ebb32c62c3856cd602b14702103c16ede6873855d0c5a5faa874810`  
		Last Modified: Mon, 23 Mar 2020 23:47:03 GMT  
		Size: 694.1 KB (694143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc367a6045f5900ec7708f21ef9df2d7ad7483e36d85979057667e0b3866bdb6`  
		Last Modified: Wed, 25 Mar 2020 22:24:27 GMT  
		Size: 21.3 MB (21285429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff697159d0030e6aa732f628239bba97a20cfba5cc1c0de77e822a794efedd5c`  
		Last Modified: Wed, 25 Mar 2020 22:24:22 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.2.0` - linux; arm variant v6

```console
$ docker pull traefik@sha256:270be8c81ce1f3fd9e507ee5650b1fd1436524b824191d7a3c544a4cf8a6691c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.3 MB (23305889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:736f4bc7eb2b854949899ad08e8a9780abc4b29446eef07ef7dc700186b7dd14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 03:43:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 21:49:39 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0/traefik_v2.2.0_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 21:49:40 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 21:49:41 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:49:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 21:49:42 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 21:49:42 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b73c299e24e9aa32bbbec493b7588c3a6592d11b52ccb01c156037b819aef46`  
		Last Modified: Tue, 24 Mar 2020 03:47:03 GMT  
		Size: 698.1 KB (698067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc381da900f5d2e94abf26cfc9f11efbec2599125dbc8181d4b32942e0a69f56`  
		Last Modified: Wed, 25 Mar 2020 21:50:30 GMT  
		Size: 20.0 MB (19988874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99b8e78c75f49ffc9e249e66cfcecd68bc3b77d2d85735efaab87ffb5203677`  
		Last Modified: Wed, 25 Mar 2020 21:50:23 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.2.0` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:6d0a99e202bc3f732000a78b696281369b771234893fff22106471f3d65daffb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23053503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20d0e36d477b886f5ede8ae4753d1cef2acd7570659836ba0f4ab2e743d55bcd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 05:52:48 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 25 Mar 2020 21:43:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.2.0/traefik_v2.2.0_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 25 Mar 2020 21:43:54 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 25 Mar 2020 21:43:55 GMT
EXPOSE 80
# Wed, 25 Mar 2020 21:43:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 25 Mar 2020 21:43:56 GMT
CMD ["traefik"]
# Wed, 25 Mar 2020 21:43:57 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc893b889cb9ecb596775296ec01901b5ffcd52efc8691a608afb27fc5be6e6`  
		Last Modified: Tue, 24 Mar 2020 05:55:52 GMT  
		Size: 696.2 KB (696184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b612f6b713c999a6de7f98b8c222af24cf379ecb710e67b5c5c51d55510f28`  
		Last Modified: Wed, 25 Mar 2020 21:44:44 GMT  
		Size: 19.6 MB (19633812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687ff5f94664c57720083b9b43ff6fe9b9d232b33ea28f07dfc57140fac200f6`  
		Last Modified: Wed, 25 Mar 2020 21:44:38 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.2.0-windowsservercore-1809`

```console
$ docker pull traefik@sha256:fe6e0415135464e6f7f8071af475cea23b6e2c2cd1b62b84730d47aa5adb4597
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:v2.2.0-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:44af67ec4d7ee639d6981625961cef63ea5cb78b2ef9edbfc18a3ad445cd6e64
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2291277474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73d76399547b88a3d964fb7eaa5733d4fb87e72d74b20f1f82a54ddb540cb50c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Mar 2020 22:15:07 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.2.0/traefik_v2.2.0_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 25 Mar 2020 22:15:12 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:15:13 GMT
ENTRYPOINT ["/traefik"]
# Wed, 25 Mar 2020 22:15:14 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:35030e579ef70c21318512a160fd079dd8f970997106efcf78786e9ab1000b27`  
		Last Modified: Wed, 25 Mar 2020 22:16:46 GMT  
		Size: 25.9 MB (25936523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6146f53de7073bee8aaf32ea1f114a598bc979d2c95d7aea012a43b37b7b2509`  
		Last Modified: Wed, 25 Mar 2020 22:16:39 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5200557f5e26f8ba1a7321f87fe4402ef5c3fbf86abf1b086f3519b348dd6cba`  
		Last Modified: Wed, 25 Mar 2020 22:16:39 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b358f870169f5b072e7bfe113d68bbb8d94386b00413c1bcbd9706efcaaed6bb`  
		Last Modified: Wed, 25 Mar 2020 22:16:40 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:fe6e0415135464e6f7f8071af475cea23b6e2c2cd1b62b84730d47aa5adb4597
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:v2.2-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:44af67ec4d7ee639d6981625961cef63ea5cb78b2ef9edbfc18a3ad445cd6e64
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2291277474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73d76399547b88a3d964fb7eaa5733d4fb87e72d74b20f1f82a54ddb540cb50c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Mar 2020 22:15:07 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.2.0/traefik_v2.2.0_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 25 Mar 2020 22:15:12 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:15:13 GMT
ENTRYPOINT ["/traefik"]
# Wed, 25 Mar 2020 22:15:14 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:35030e579ef70c21318512a160fd079dd8f970997106efcf78786e9ab1000b27`  
		Last Modified: Wed, 25 Mar 2020 22:16:46 GMT  
		Size: 25.9 MB (25936523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6146f53de7073bee8aaf32ea1f114a598bc979d2c95d7aea012a43b37b7b2509`  
		Last Modified: Wed, 25 Mar 2020 22:16:39 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5200557f5e26f8ba1a7321f87fe4402ef5c3fbf86abf1b086f3519b348dd6cba`  
		Last Modified: Wed, 25 Mar 2020 22:16:39 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b358f870169f5b072e7bfe113d68bbb8d94386b00413c1bcbd9706efcaaed6bb`  
		Last Modified: Wed, 25 Mar 2020 22:16:40 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:fe6e0415135464e6f7f8071af475cea23b6e2c2cd1b62b84730d47aa5adb4597
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:44af67ec4d7ee639d6981625961cef63ea5cb78b2ef9edbfc18a3ad445cd6e64
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2291277474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73d76399547b88a3d964fb7eaa5733d4fb87e72d74b20f1f82a54ddb540cb50c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Mar 2020 22:15:07 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.2.0/traefik_v2.2.0_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 25 Mar 2020 22:15:12 GMT
EXPOSE 80
# Wed, 25 Mar 2020 22:15:13 GMT
ENTRYPOINT ["/traefik"]
# Wed, 25 Mar 2020 22:15:14 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.2.0 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:35030e579ef70c21318512a160fd079dd8f970997106efcf78786e9ab1000b27`  
		Last Modified: Wed, 25 Mar 2020 22:16:46 GMT  
		Size: 25.9 MB (25936523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6146f53de7073bee8aaf32ea1f114a598bc979d2c95d7aea012a43b37b7b2509`  
		Last Modified: Wed, 25 Mar 2020 22:16:39 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5200557f5e26f8ba1a7321f87fe4402ef5c3fbf86abf1b086f3519b348dd6cba`  
		Last Modified: Wed, 25 Mar 2020 22:16:39 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b358f870169f5b072e7bfe113d68bbb8d94386b00413c1bcbd9706efcaaed6bb`  
		Last Modified: Wed, 25 Mar 2020 22:16:40 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
