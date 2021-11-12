## `traefik:brie`

```console
$ docker pull traefik@sha256:7be61d1f7a089ceed8f8bb8697be30453e7cd98f568fce2c7677266e3da97bd2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:brie` - linux; amd64

```console
$ docker pull traefik@sha256:212aee66cc6eecbd6a04ef0af0b8616fbc4f716d4c9a52dfa9808b4a8dea5d8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29845535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3bb9550d562ded287f2fc5f71056c652d49cd1ae0ddde3a39acefb3b10dc1ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 17:28:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 08 Nov 2021 20:51:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 08 Nov 2021 20:51:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 08 Nov 2021 20:51:20 GMT
EXPOSE 80
# Mon, 08 Nov 2021 20:51:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 08 Nov 2021 20:51:21 GMT
CMD ["traefik"]
# Mon, 08 Nov 2021 20:51:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:c117e813430bc0788d2b53069f51b9f1387ffaf32a071b5b966237a4e8be398c`  
		Last Modified: Mon, 08 Nov 2021 20:51:51 GMT  
		Size: 26.4 MB (26374365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aedf838ed1f44594dd320fce1909f9563036b91ae4efdbc35f75a5a73473b2d`  
		Last Modified: Mon, 08 Nov 2021 20:51:46 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:brie` - linux; arm variant v6

```console
$ docker pull traefik@sha256:47c3bf77a86d3f12c448c710877a4cd9fbf7775884a426684c20e7a250b2671f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28053789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2674cfd4de72e6257efeb153c7ffcd248fb5cdd348ebd52d4524d8d476b00bb8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 02 Sep 2021 18:16:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 08 Nov 2021 19:50:17 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 08 Nov 2021 19:50:18 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 08 Nov 2021 19:50:18 GMT
EXPOSE 80
# Mon, 08 Nov 2021 19:50:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 08 Nov 2021 19:50:19 GMT
CMD ["traefik"]
# Mon, 08 Nov 2021 19:50:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:26b9fa73a27b6241465393f381be172fc0be70f4efd5a14ba17c88443ef3cb5c`  
		Last Modified: Mon, 08 Nov 2021 19:52:36 GMT  
		Size: 24.8 MB (24763982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a45d7c981057236b7ce62e75fe4c05de960f65a54e62478e05d6e030080c72d6`  
		Last Modified: Mon, 08 Nov 2021 19:52:18 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:brie` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:317dbd98705ff9a2719bb8357e83c496ea70f7caff8aca06b123e1d0862dbee0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27461064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bd5494cab630ed31508338889d5d02c98d6113f9d818584913b8ddd68dd1121`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:16:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 12 Nov 2021 18:16:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.4/traefik_v2.5.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 12 Nov 2021 18:16:37 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 12 Nov 2021 18:16:37 GMT
EXPOSE 80
# Fri, 12 Nov 2021 18:16:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 18:16:39 GMT
CMD ["traefik"]
# Fri, 12 Nov 2021 18:16:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cc5a4b7f102f236064e4712164f29c52d256612820409cc28c41a7f5def4a5`  
		Last Modified: Fri, 12 Nov 2021 18:17:40 GMT  
		Size: 680.0 KB (680008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd938bc8aa751ad66221cfd63d8acc173d3ceed14728f87fdac32ed0598cd3af`  
		Last Modified: Fri, 12 Nov 2021 18:17:44 GMT  
		Size: 24.1 MB (24062987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ef3656e6ddb41988a45143ead13d5199714713ea7eee816d82ed9d85f35b5c`  
		Last Modified: Fri, 12 Nov 2021 18:17:40 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
