<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `caddy`

-	[`caddy:2`](#caddy2)
-	[`caddy:2-alpine`](#caddy2-alpine)
-	[`caddy:2-builder`](#caddy2-builder)
-	[`caddy:2-builder-alpine`](#caddy2-builder-alpine)
-	[`caddy:2-builder-windowsservercore-1809`](#caddy2-builder-windowsservercore-1809)
-	[`caddy:2-builder-windowsservercore-ltsc2022`](#caddy2-builder-windowsservercore-ltsc2022)
-	[`caddy:2-windowsservercore`](#caddy2-windowsservercore)
-	[`caddy:2-windowsservercore-1809`](#caddy2-windowsservercore-1809)
-	[`caddy:2-windowsservercore-ltsc2022`](#caddy2-windowsservercore-ltsc2022)
-	[`caddy:2.5.1`](#caddy251)
-	[`caddy:2.5.1-alpine`](#caddy251-alpine)
-	[`caddy:2.5.1-builder`](#caddy251-builder)
-	[`caddy:2.5.1-builder-alpine`](#caddy251-builder-alpine)
-	[`caddy:2.5.1-builder-windowsservercore-1809`](#caddy251-builder-windowsservercore-1809)
-	[`caddy:2.5.1-builder-windowsservercore-ltsc2022`](#caddy251-builder-windowsservercore-ltsc2022)
-	[`caddy:2.5.1-windowsservercore`](#caddy251-windowsservercore)
-	[`caddy:2.5.1-windowsservercore-1809`](#caddy251-windowsservercore-1809)
-	[`caddy:2.5.1-windowsservercore-ltsc2022`](#caddy251-windowsservercore-ltsc2022)
-	[`caddy:alpine`](#caddyalpine)
-	[`caddy:builder`](#caddybuilder)
-	[`caddy:builder-alpine`](#caddybuilder-alpine)
-	[`caddy:builder-windowsservercore-1809`](#caddybuilder-windowsservercore-1809)
-	[`caddy:builder-windowsservercore-ltsc2022`](#caddybuilder-windowsservercore-ltsc2022)
-	[`caddy:latest`](#caddylatest)
-	[`caddy:windowsservercore`](#caddywindowsservercore)
-	[`caddy:windowsservercore-1809`](#caddywindowsservercore-1809)
-	[`caddy:windowsservercore-ltsc2022`](#caddywindowsservercore-ltsc2022)

## `caddy:2`

```console
$ docker pull caddy@sha256:eb2cce28a50cb1f20f1e4a13181f3e453e58d20999cffa7750222d9907023b6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2928; amd64
	-	windows version 10.0.20348.707; amd64

### `caddy:2` - linux; amd64

```console
$ docker pull caddy@sha256:6e62b63d4d7a4826f9e93c904a0e5b886a8bea2234b6569e300924282a2e8e6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16788470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e63f36e9049faf60b3a47c774237eddacb8916cacb003e418f2591de1a3bee29`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:25:00 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:19:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:19:24 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:19:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:19:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:19:26 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:19:26 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:19:27 GMT
EXPOSE 80
# Fri, 06 May 2022 19:19:27 GMT
EXPOSE 443
# Fri, 06 May 2022 19:19:28 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:19:28 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:19:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87ed6b8c4412bcd2bb1f40611012b40444b12071baf4884d0e75044fc1f32c1`  
		Last Modified: Tue, 05 Apr 2022 04:25:48 GMT  
		Size: 291.5 KB (291522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4c78357cc2da49b060ec4367d3d35d9837faf50e873e07ab40822e9fa57d00`  
		Last Modified: Fri, 06 May 2022 19:19:49 GMT  
		Size: 5.8 KB (5836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3edd190820fd86aaeb4fc1b7a28d7ff52e776414d3830f1a14d103967b455965`  
		Last Modified: Fri, 06 May 2022 19:19:51 GMT  
		Size: 13.7 MB (13676400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b96fea00470fa7356d42265c310e3940426e4c5572f288e8f7111a03b2fdddc`  
		Last Modified: Fri, 06 May 2022 19:19:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:813c33aa7f94275843088c57b0e44ea6c190d5296b664d7795f66bf3c3804392
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16056332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ee6ea861df7cd9fff1d948de8590f2bac9f2b90ebea7bc71ef7c7654f2d8d40`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:15:01 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:49:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:49:35 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:49:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:49:42 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:49:42 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:49:42 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:49:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:49:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:49:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:49:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:49:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:49:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:49:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:49:46 GMT
EXPOSE 80
# Fri, 06 May 2022 19:49:46 GMT
EXPOSE 443
# Fri, 06 May 2022 19:49:46 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:49:47 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:49:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b230dd773e10769a2eb3e507260d2470a646efd48a639739ba8852b2915302`  
		Last Modified: Tue, 05 Apr 2022 03:18:10 GMT  
		Size: 291.7 KB (291685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd82040b030d75398d6d6fb1c3d12cc9e25a954a92227895e1e5f7ea54736c20`  
		Last Modified: Fri, 06 May 2022 19:51:07 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583abcfacbc800cc0863a5117f1911222bec7ea3fcaed7c36ce4b94b489c3b3e`  
		Last Modified: Fri, 06 May 2022 19:51:16 GMT  
		Size: 13.1 MB (13136691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6903af22655a77183d11fb6d870f6ebc4776e6d9222e9de261b0a377cb81bbcf`  
		Last Modified: Fri, 06 May 2022 19:51:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:2e61a3ed70ad9a4784ff95cf49efa7ec58255c5263c3faba6a5270a847542a41
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.8 MB (15835582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93c6db987e0721fcd4f557ec160b55012a73d2f69de7198fac316514b27ed58f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:33:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:57:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:57:32 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:57:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:57:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:57:39 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:57:39 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:57:40 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:57:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:57:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:57:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:57:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:57:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:57:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:57:42 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:57:43 GMT
EXPOSE 80
# Fri, 06 May 2022 19:57:43 GMT
EXPOSE 443
# Fri, 06 May 2022 19:57:44 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:57:44 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:57:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03203881a2568530a735b6e0e7a40ebb79adedc5193a675807b04eeb92cc6ed1`  
		Last Modified: Tue, 05 Apr 2022 06:35:07 GMT  
		Size: 290.7 KB (290668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507adf96fcab6911303d2b3d14aeb43223c106ee9901b3e31f30668a4dbd5ffb`  
		Last Modified: Fri, 06 May 2022 19:59:02 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23435dc592c99e66d2e9f715136b809e73116ee6725847ed8fd158135e3283be`  
		Last Modified: Fri, 06 May 2022 19:59:11 GMT  
		Size: 13.1 MB (13114610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e55b7a8b43f4fdfecf61cea01ddddc80930ed485d9aafc41c26f84380f858f3`  
		Last Modified: Fri, 06 May 2022 19:59:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:cda45585c425161575996ee5d954166745d44d39928846423ecdce6b61a9fb4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.5 MB (15523770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:890cdb4fef0cc66aabb117ff1b3e11fb86de5117d28a5b0e64a743efb92c4269`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:12:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:39:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:39:32 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:39:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:39:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:39:37 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:39:38 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:39:39 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:39:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:39:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:39:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:39:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:39:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:39:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:39:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:39:47 GMT
EXPOSE 80
# Fri, 06 May 2022 19:39:48 GMT
EXPOSE 443
# Fri, 06 May 2022 19:39:49 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:39:50 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:39:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83aa37f2341b1e6d98420668c9bc849a47f2c471d159b2303885040bd8d0a92f`  
		Last Modified: Tue, 05 Apr 2022 03:13:38 GMT  
		Size: 291.3 KB (291301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc050d3d6ffb91c2f68db47e3d5f056afad26e465a03ae7e43383df0fc8ad89`  
		Last Modified: Fri, 06 May 2022 19:40:32 GMT  
		Size: 5.8 KB (5753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8adaff0bd78d0b115843dd841c83d1690484b25369e804b1133b838b7ad5ce8f`  
		Last Modified: Fri, 06 May 2022 19:40:35 GMT  
		Size: 12.5 MB (12510086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f703c61da5ec8e48b081aceac2cb64fb25162c2f0ba1ad16a104610b676f50f6`  
		Last Modified: Fri, 06 May 2022 19:40:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:d1ab9f3165d5b23b9ff5bd4fcb74b3f8bbf834ba34c42c58e496b3d33017ca59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15203958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfbb2004b1ba3aace5176af38455ef6b8328a074388b16b35358d61330ad2658`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:08:34 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:16:53 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:16:58 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:17:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:17:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:17:25 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:17:32 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:17:36 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:17:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:17:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:17:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:17:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:17:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:18:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:18:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:18:13 GMT
EXPOSE 80
# Fri, 06 May 2022 19:18:17 GMT
EXPOSE 443
# Fri, 06 May 2022 19:18:19 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:18:22 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:18:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743509d6ced044a369685ebb068417e8757981a39d1b397c7b0182ab89f83528`  
		Last Modified: Tue, 05 Apr 2022 07:11:24 GMT  
		Size: 293.7 KB (293721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b659dd8890d066269209696348c58ed19351199266936a5e81f1991a52333d1`  
		Last Modified: Fri, 06 May 2022 19:19:31 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86272ae554176010d052c51dcc5540948b8e59082743b04ac5bb67d05c3fdcd`  
		Last Modified: Fri, 06 May 2022 19:19:33 GMT  
		Size: 12.1 MB (12093067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff57ff409904cc43937df14c68e6d97e1269adde095e91671fb5438dc58a1808`  
		Last Modified: Fri, 06 May 2022 19:19:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:fbee089e769bc54babbe3ac3217c0e5b60c4a5157b76b0f37aa73cc71486c8fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16129299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f94fa793c943e1cb1c5bda77b0e7077b344648635da2222a1061307e3e61ca96`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:19:41 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:41:25 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:41:25 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:41:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:41:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:41:28 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:41:28 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:41:28 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:41:29 GMT
EXPOSE 80
# Fri, 06 May 2022 19:41:29 GMT
EXPOSE 443
# Fri, 06 May 2022 19:41:30 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:41:30 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:41:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8cc7c7c7ffd67f5740add448d341753330a2abdc6ed06e995cb7d28de381ab`  
		Last Modified: Tue, 05 Apr 2022 06:20:44 GMT  
		Size: 291.8 KB (291821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3d2fae470dbad90c4c4c1262110f14447a47b6e81edc4e0e80ceb50538fe57`  
		Last Modified: Fri, 06 May 2022 19:42:10 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a8f9dbbf38ad9456666a4e6a3eda871b385d4ef76ab6dc25e31030d1daf71c`  
		Last Modified: Fri, 06 May 2022 19:42:12 GMT  
		Size: 13.2 MB (13231118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf07e991258bc58c5e8a5785f741bc746e75848423d2c27d26448015c5887f1`  
		Last Modified: Fri, 06 May 2022 19:42:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.2928; amd64

```console
$ docker pull caddy@sha256:8ad6979cdadd3d080deeb3a2f13d37c23789748ea80b29ac44624cf39bd589ff
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2518898800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8393d2b14b909a4ce523ae0d4999f2a492deb9e76ac12cc8dc111b5f0e3bd74d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:28:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 10 May 2022 23:28:55 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:29:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('4294796c4bd4bed0c593d83606a5413de30f35f88d624e1b1e5b6cd8672ffbcc7a689d7ce4ef30c1abea0e95eda62220faac15d2a6aca0c3e2b418abe7a74118')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 10 May 2022 23:29:54 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 10 May 2022 23:29:56 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 10 May 2022 23:29:57 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Tue, 10 May 2022 23:29:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 10 May 2022 23:29:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 10 May 2022 23:29:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 10 May 2022 23:30:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 10 May 2022 23:30:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 10 May 2022 23:30:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 10 May 2022 23:30:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 10 May 2022 23:30:04 GMT
EXPOSE 80
# Tue, 10 May 2022 23:30:05 GMT
EXPOSE 443
# Tue, 10 May 2022 23:30:06 GMT
EXPOSE 2019
# Tue, 10 May 2022 23:30:47 GMT
RUN caddy version
# Tue, 10 May 2022 23:30:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d722bd7a5ed597b5a9ed7c5144caa608e784120c4442579352b7c2325ce47ffc`  
		Last Modified: Tue, 10 May 2022 23:35:41 GMT  
		Size: 498.2 KB (498231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0dfede5e37c630a175a1c987d90aaf1ec1db8cd7d43e3d63648743c6ace743`  
		Last Modified: Tue, 10 May 2022 23:35:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef201446c9bd5610f78b8e5a1680047ff45fadb77727762c323d5e48d77f9f2`  
		Last Modified: Tue, 10 May 2022 23:35:44 GMT  
		Size: 14.0 MB (14007489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b824e8abcb45a47ada825f0b722a588cbc9d1f68f5536a76b7afed2c5eb15a0c`  
		Last Modified: Tue, 10 May 2022 23:35:39 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b01057f474e19bdcaebab2c156622642945d2c7074276c82de663baeb418143`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520fb9c4921f60cfaea07cfa8d5733cf7f4f0810e56106911d7b25f59e86e997`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74d9e7abc08a32b35b26f8bba23c597b1e19d604766b326f61e77da0b494285`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595304462c9d3aa03aa9e164a98a38be5e1f5307c2981b65aa228101c73ce91b`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e307ee1571a8185932bbd90267a8b8d367f784859d99a2742d44e89e19e8b6c0`  
		Last Modified: Tue, 10 May 2022 23:35:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b335f1fddf0ed6abcc0e715ff827614cc2f0f4bbe8a0e1565145951d841c96`  
		Last Modified: Tue, 10 May 2022 23:35:36 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0974b9a20e0fa84c8a353a7c04992bec9e06825ed808054a358b84409744ba`  
		Last Modified: Tue, 10 May 2022 23:35:35 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d5086c691961c9f1a18b9d161cf8cb3dbd7b581c68ab75760b8c5e62647928`  
		Last Modified: Tue, 10 May 2022 23:35:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9194a8cf5ac8d920d218d9100152393ac6cce9142b15904894374694ae2d2fc`  
		Last Modified: Tue, 10 May 2022 23:35:36 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd07be490606caadc3893d219aee0682d6f8b71b2a4a8f2fb2ca826cdffb74`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b19beef4c4a6634592447260a670c8ee571e59cb775833787d39b815e9ba511`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2dab7fd2beddb5439029e7d8a75fc7c7fe2d3a534a63f51a04f85dd371cd1c`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e195aa5e2a95379397baf57f681e2c39a7c673d3c06d0ff3e4eeed3d8cecee1`  
		Last Modified: Tue, 10 May 2022 23:35:34 GMT  
		Size: 314.6 KB (314586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87827ca78b495430e19218a9e3f7f2837078a77df34bb929124ea20614287d5`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.20348.707; amd64

```console
$ docker pull caddy@sha256:a3894222673d46b3e350553c6b7d4f92ab27b85a87fa1f773e9b090d5774ca9e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2252723203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:063f1879bd2783934ad3ac23aa37bf45f19be756f6b018f4c3a67d2d4a759c7c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:31:41 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 10 May 2022 23:31:42 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:32:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('4294796c4bd4bed0c593d83606a5413de30f35f88d624e1b1e5b6cd8672ffbcc7a689d7ce4ef30c1abea0e95eda62220faac15d2a6aca0c3e2b418abe7a74118')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 10 May 2022 23:32:11 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 10 May 2022 23:32:12 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 10 May 2022 23:32:13 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Tue, 10 May 2022 23:32:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 10 May 2022 23:32:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 10 May 2022 23:32:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 10 May 2022 23:32:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 10 May 2022 23:32:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 10 May 2022 23:32:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 10 May 2022 23:32:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 10 May 2022 23:32:21 GMT
EXPOSE 80
# Tue, 10 May 2022 23:32:22 GMT
EXPOSE 443
# Tue, 10 May 2022 23:32:23 GMT
EXPOSE 2019
# Tue, 10 May 2022 23:32:42 GMT
RUN caddy version
# Tue, 10 May 2022 23:32:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9baa8a196af04dc55746ee82c0774537bce72a589b75d9efce1a4680f03e35`  
		Last Modified: Tue, 10 May 2022 23:36:04 GMT  
		Size: 616.1 KB (616130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe60c7e90fdaeffa9bce60d9a7c7b340dedc357bfb70a2ce8c6d7b8bd0e74a11`  
		Last Modified: Tue, 10 May 2022 23:36:04 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f955bea173999b55d2087a27b9cc80e92bf168918c6e892175c2a75bdbfac933`  
		Last Modified: Tue, 10 May 2022 23:36:07 GMT  
		Size: 14.2 MB (14224642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e1ab4508d5347b929d5a33f71e0f24f653e61c147260200d32e3bd7cdd2340`  
		Last Modified: Tue, 10 May 2022 23:36:02 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8044ca4427c5edfee653001205397a2cc33f8fb4416c16c4a4936317c572ed`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f144416d38a1aa75558e0b93b88fcb3de122ee88349826ee99d596e1b00d9cc0`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32edbcceba80e7a70e44725926012bb70624bb0ae91c85db2766ca2e4c5a5d7c`  
		Last Modified: Tue, 10 May 2022 23:36:02 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd90105a2a3136e4d25d0add2b6fbe5798d51588215367128f1566d66b255289`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e448ed08c6c6ca9f854cb7014ea2e79c04e83f1905f78f578b67303b709fa3`  
		Last Modified: Tue, 10 May 2022 23:36:00 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d49b1b3778cd2ebf32521f530e29275a9a473afa997654b32338ff4349bf5c`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2112945425b7d069bc5705be1345e5ad6e27206e1531b10d0bc92d9c69ea9c3`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7243327255edd82b277f456085138a672f5a43d616e80f73156c8eb31139121d`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1a14330360d7ab3af40d4fb6f2de975e42e05f8e4cb064cc49fe1d9446e6b1`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808ce6a15ca3e6ad031229bcad8a3ed69171a7005c05ef4e77ffcfd777e9d1f7`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdfcf611e614d42a256d103775233f59ab7bb6ad0b00ca2f915bf739600f8d6`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3811622d464d497ce363eed806c75f9b994cd1d04b3009b2d0671af2863ebd0`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b006092864e6cfdfedd054a2635236c62958e97de81c720d9e38772276ee11`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 325.9 KB (325870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2afb0ece27a359f16126f263176baa74c3d3f2f2733cce186e4e31ad0eca4f8`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:0033b34d2df3fe0bf94088c36e7d722ceca1b38cbdd49c08b2c10b9f9aa58912
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:6e62b63d4d7a4826f9e93c904a0e5b886a8bea2234b6569e300924282a2e8e6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16788470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e63f36e9049faf60b3a47c774237eddacb8916cacb003e418f2591de1a3bee29`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:25:00 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:19:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:19:24 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:19:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:19:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:19:26 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:19:26 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:19:27 GMT
EXPOSE 80
# Fri, 06 May 2022 19:19:27 GMT
EXPOSE 443
# Fri, 06 May 2022 19:19:28 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:19:28 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:19:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87ed6b8c4412bcd2bb1f40611012b40444b12071baf4884d0e75044fc1f32c1`  
		Last Modified: Tue, 05 Apr 2022 04:25:48 GMT  
		Size: 291.5 KB (291522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4c78357cc2da49b060ec4367d3d35d9837faf50e873e07ab40822e9fa57d00`  
		Last Modified: Fri, 06 May 2022 19:19:49 GMT  
		Size: 5.8 KB (5836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3edd190820fd86aaeb4fc1b7a28d7ff52e776414d3830f1a14d103967b455965`  
		Last Modified: Fri, 06 May 2022 19:19:51 GMT  
		Size: 13.7 MB (13676400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b96fea00470fa7356d42265c310e3940426e4c5572f288e8f7111a03b2fdddc`  
		Last Modified: Fri, 06 May 2022 19:19:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:813c33aa7f94275843088c57b0e44ea6c190d5296b664d7795f66bf3c3804392
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16056332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ee6ea861df7cd9fff1d948de8590f2bac9f2b90ebea7bc71ef7c7654f2d8d40`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:15:01 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:49:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:49:35 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:49:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:49:42 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:49:42 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:49:42 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:49:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:49:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:49:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:49:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:49:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:49:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:49:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:49:46 GMT
EXPOSE 80
# Fri, 06 May 2022 19:49:46 GMT
EXPOSE 443
# Fri, 06 May 2022 19:49:46 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:49:47 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:49:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b230dd773e10769a2eb3e507260d2470a646efd48a639739ba8852b2915302`  
		Last Modified: Tue, 05 Apr 2022 03:18:10 GMT  
		Size: 291.7 KB (291685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd82040b030d75398d6d6fb1c3d12cc9e25a954a92227895e1e5f7ea54736c20`  
		Last Modified: Fri, 06 May 2022 19:51:07 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583abcfacbc800cc0863a5117f1911222bec7ea3fcaed7c36ce4b94b489c3b3e`  
		Last Modified: Fri, 06 May 2022 19:51:16 GMT  
		Size: 13.1 MB (13136691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6903af22655a77183d11fb6d870f6ebc4776e6d9222e9de261b0a377cb81bbcf`  
		Last Modified: Fri, 06 May 2022 19:51:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:2e61a3ed70ad9a4784ff95cf49efa7ec58255c5263c3faba6a5270a847542a41
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.8 MB (15835582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93c6db987e0721fcd4f557ec160b55012a73d2f69de7198fac316514b27ed58f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:33:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:57:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:57:32 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:57:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:57:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:57:39 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:57:39 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:57:40 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:57:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:57:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:57:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:57:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:57:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:57:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:57:42 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:57:43 GMT
EXPOSE 80
# Fri, 06 May 2022 19:57:43 GMT
EXPOSE 443
# Fri, 06 May 2022 19:57:44 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:57:44 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:57:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03203881a2568530a735b6e0e7a40ebb79adedc5193a675807b04eeb92cc6ed1`  
		Last Modified: Tue, 05 Apr 2022 06:35:07 GMT  
		Size: 290.7 KB (290668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507adf96fcab6911303d2b3d14aeb43223c106ee9901b3e31f30668a4dbd5ffb`  
		Last Modified: Fri, 06 May 2022 19:59:02 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23435dc592c99e66d2e9f715136b809e73116ee6725847ed8fd158135e3283be`  
		Last Modified: Fri, 06 May 2022 19:59:11 GMT  
		Size: 13.1 MB (13114610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e55b7a8b43f4fdfecf61cea01ddddc80930ed485d9aafc41c26f84380f858f3`  
		Last Modified: Fri, 06 May 2022 19:59:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:cda45585c425161575996ee5d954166745d44d39928846423ecdce6b61a9fb4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.5 MB (15523770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:890cdb4fef0cc66aabb117ff1b3e11fb86de5117d28a5b0e64a743efb92c4269`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:12:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:39:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:39:32 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:39:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:39:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:39:37 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:39:38 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:39:39 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:39:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:39:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:39:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:39:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:39:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:39:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:39:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:39:47 GMT
EXPOSE 80
# Fri, 06 May 2022 19:39:48 GMT
EXPOSE 443
# Fri, 06 May 2022 19:39:49 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:39:50 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:39:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83aa37f2341b1e6d98420668c9bc849a47f2c471d159b2303885040bd8d0a92f`  
		Last Modified: Tue, 05 Apr 2022 03:13:38 GMT  
		Size: 291.3 KB (291301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc050d3d6ffb91c2f68db47e3d5f056afad26e465a03ae7e43383df0fc8ad89`  
		Last Modified: Fri, 06 May 2022 19:40:32 GMT  
		Size: 5.8 KB (5753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8adaff0bd78d0b115843dd841c83d1690484b25369e804b1133b838b7ad5ce8f`  
		Last Modified: Fri, 06 May 2022 19:40:35 GMT  
		Size: 12.5 MB (12510086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f703c61da5ec8e48b081aceac2cb64fb25162c2f0ba1ad16a104610b676f50f6`  
		Last Modified: Fri, 06 May 2022 19:40:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:d1ab9f3165d5b23b9ff5bd4fcb74b3f8bbf834ba34c42c58e496b3d33017ca59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15203958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfbb2004b1ba3aace5176af38455ef6b8328a074388b16b35358d61330ad2658`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:08:34 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:16:53 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:16:58 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:17:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:17:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:17:25 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:17:32 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:17:36 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:17:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:17:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:17:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:17:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:17:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:18:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:18:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:18:13 GMT
EXPOSE 80
# Fri, 06 May 2022 19:18:17 GMT
EXPOSE 443
# Fri, 06 May 2022 19:18:19 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:18:22 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:18:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743509d6ced044a369685ebb068417e8757981a39d1b397c7b0182ab89f83528`  
		Last Modified: Tue, 05 Apr 2022 07:11:24 GMT  
		Size: 293.7 KB (293721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b659dd8890d066269209696348c58ed19351199266936a5e81f1991a52333d1`  
		Last Modified: Fri, 06 May 2022 19:19:31 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86272ae554176010d052c51dcc5540948b8e59082743b04ac5bb67d05c3fdcd`  
		Last Modified: Fri, 06 May 2022 19:19:33 GMT  
		Size: 12.1 MB (12093067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff57ff409904cc43937df14c68e6d97e1269adde095e91671fb5438dc58a1808`  
		Last Modified: Fri, 06 May 2022 19:19:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:fbee089e769bc54babbe3ac3217c0e5b60c4a5157b76b0f37aa73cc71486c8fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16129299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f94fa793c943e1cb1c5bda77b0e7077b344648635da2222a1061307e3e61ca96`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:19:41 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:41:25 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:41:25 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:41:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:41:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:41:28 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:41:28 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:41:28 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:41:29 GMT
EXPOSE 80
# Fri, 06 May 2022 19:41:29 GMT
EXPOSE 443
# Fri, 06 May 2022 19:41:30 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:41:30 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:41:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8cc7c7c7ffd67f5740add448d341753330a2abdc6ed06e995cb7d28de381ab`  
		Last Modified: Tue, 05 Apr 2022 06:20:44 GMT  
		Size: 291.8 KB (291821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3d2fae470dbad90c4c4c1262110f14447a47b6e81edc4e0e80ceb50538fe57`  
		Last Modified: Fri, 06 May 2022 19:42:10 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a8f9dbbf38ad9456666a4e6a3eda871b385d4ef76ab6dc25e31030d1daf71c`  
		Last Modified: Fri, 06 May 2022 19:42:12 GMT  
		Size: 13.2 MB (13231118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf07e991258bc58c5e8a5785f741bc746e75848423d2c27d26448015c5887f1`  
		Last Modified: Fri, 06 May 2022 19:42:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:81fcae6c8754b60a6694fa9de78ad16f624bf2746f50e224dbd447d197597ae5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2928; amd64
	-	windows version 10.0.20348.707; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:1e292f2e17935f1d904222aa4291d4b4f0a3f48ddd2c73af04039226c812d84b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126492209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c80070b3eb6003cffb12fd895325316a7ad91a7f7116a69ce3970897ef0742d3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:19:44 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:19:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:19:45 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:20:38 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:22:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 22:22:12 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:22:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:22:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:22:13 GMT
WORKDIR /go
# Wed, 01 Jun 2022 22:49:16 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 22:49:16 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 22:49:16 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 22:49:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 22:49:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 22:49:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 22:49:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea60b727a1ce729d031ec1e4f2521a246e71bdb72d3fd9c9c04711cce80e1722`  
		Last Modified: Wed, 25 May 2022 00:24:05 GMT  
		Size: 271.8 KB (271822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c4a77219572e69864cd3069b7b47e55202681be151bd7394f9cb6645b5687b`  
		Last Modified: Wed, 25 May 2022 00:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370296b7ddb629fff1cc98d8d390acf0782fdb8f55cf4054637f6127bbcfe2a9`  
		Last Modified: Wed, 01 Jun 2022 22:30:44 GMT  
		Size: 115.2 MB (115199527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6cee850709034cc7b53152e226caba834fdeb704dab0621f1813bc9081173c`  
		Last Modified: Wed, 01 Jun 2022 22:30:29 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1136d32ff848474c9a359e03d2fcc678a7b8f0dc7e73222ae72e60f7fd4d74`  
		Last Modified: Wed, 01 Jun 2022 22:49:37 GMT  
		Size: 6.9 MB (6931847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c29192c5c8d89201d847a27e2e77e0c4e47f3cef0219cb077dcd8b5bdd9fe1`  
		Last Modified: Wed, 01 Jun 2022 22:49:36 GMT  
		Size: 1.3 MB (1289410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865185451556d5e92a06e01ff04ae2d479a7ff41a4cef4d7f3e27cdb3d0a559e`  
		Last Modified: Wed, 01 Jun 2022 22:49:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:7de3187171d024e8352c7d65d8c0f7264ecba7b1a0f704295fd611019cb3570f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.5 MB (122503603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d3ac773c95b35b7b4dbac45428257530fdef319e97ee68be2648997c9e4bcd5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:49:39 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:49:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:51:15 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:55:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 22:55:14 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:55:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:55:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:55:16 GMT
WORKDIR /go
# Wed, 01 Jun 2022 23:30:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 23:30:47 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 23:30:48 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 23:30:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 23:30:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 23:30:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 23:30:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6c67ddc305b7f97a531083e369316343b3d19da2352e4e3274db751bba38e2`  
		Last Modified: Wed, 25 May 2022 00:59:27 GMT  
		Size: 272.0 KB (272047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8a37c8e9266706ee6b9ca75c42931dfe1320723ad6a20f0ad4c97554998348`  
		Last Modified: Wed, 25 May 2022 00:59:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d540be111b8c098590378841899d81bec5b744ccbd9ab573bc9b5101566901c`  
		Last Modified: Wed, 01 Jun 2022 23:09:53 GMT  
		Size: 111.6 MB (111598618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cafdd66ccebe1705fc4faa98039c9de106fbcbe091c52f158673fe04e82f802e`  
		Last Modified: Wed, 01 Jun 2022 23:08:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96872e0a675044607ec984baa827068687c978aa91bb47e3f49960519818427`  
		Last Modified: Wed, 01 Jun 2022 23:31:59 GMT  
		Size: 6.8 MB (6796920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3293e1352a64f4c075b505e4c5b86af54f57290c7d7f30c7881824677027cc2`  
		Last Modified: Wed, 01 Jun 2022 23:31:56 GMT  
		Size: 1.2 MB (1229160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4753da45404db22fc7c2a859da39a898b3708ecbfc5cfea606ee7431d28666e4`  
		Last Modified: Wed, 01 Jun 2022 23:31:55 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:011ac9678dff1b4c8b7b55ed5e314c4cff6da6b30703063ebd229e6b72d63cd6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121343857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48dd50101a28b86b1db7401d9cb0cf460f9f9e9a5543d3b3abe69cf3a4290028`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 03:51:19 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 03:51:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 03:51:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 23:01:24 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 23:05:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 23:05:24 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 23:05:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 23:05:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 23:05:28 GMT
WORKDIR /go
# Wed, 01 Jun 2022 23:54:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 23:54:05 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 23:54:05 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 23:54:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 23:54:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 23:54:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 23:54:09 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e4e5a89e8a0366f9710ba7cb04de284f11234b8cb3dba3e69e35a76dd1c62`  
		Last Modified: Wed, 25 May 2022 04:03:05 GMT  
		Size: 271.0 KB (270972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3b879ada9b059c6167f45b720f44118516dfc73e29b727218447700619fbc5`  
		Last Modified: Wed, 25 May 2022 04:03:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fc48eab20f513149fdf3afa2d29409fae14ca579ba77b44d39b1c7d30bd160`  
		Last Modified: Wed, 01 Jun 2022 23:29:17 GMT  
		Size: 111.4 MB (111376293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4611066e57bc80a36e6249e8637f907272e5888e39790c2360619a7e0cba4833`  
		Last Modified: Wed, 01 Jun 2022 23:28:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65e673e15769cdf43d8d431796fdce20817845053df123db32c4d1ebb097dda`  
		Last Modified: Wed, 01 Jun 2022 23:55:15 GMT  
		Size: 6.1 MB (6056216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f57b87d4f5a15b224a843782ea88621460db848ce77a22ea9556319c9e5c0c`  
		Last Modified: Wed, 01 Jun 2022 23:55:13 GMT  
		Size: 1.2 MB (1228015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a540258c6d4d9ec99d0f270d7f398f2a784a811119862c84d641faf27d9d52f`  
		Last Modified: Wed, 01 Jun 2022 23:55:12 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:499ea69b717472a063a52ae5197f6deb99d1b2bf52f6ffe632ae6ee4b151e8d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121425869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8397cebecc3630e1971e7a6391326e81bf1f7987dad0cd00d290554058a8e96`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:40:10 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:40:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:40:12 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:41:13 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:43:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 22:43:14 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:43:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:43:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:43:16 GMT
WORKDIR /go
# Wed, 01 Jun 2022 23:12:50 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 23:12:51 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 23:12:51 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 23:12:52 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 23:12:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 23:12:56 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 23:12:56 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a3192eca97ce26527d2bdbb26d1130abcc1c9dd7b800ce2fd14619fa422640`  
		Last Modified: Wed, 25 May 2022 00:45:29 GMT  
		Size: 271.7 KB (271711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a050256f5b6fc0800b8ae0d96e136745091c36ce8e53ba74d8ab3eed65966a59`  
		Last Modified: Wed, 25 May 2022 00:45:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656be50a0ddc84123afb23ccbb17811b43648fa17b4c8664716e9e07553c8b35`  
		Last Modified: Wed, 01 Jun 2022 22:54:01 GMT  
		Size: 110.2 MB (110233232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbca73fdf42200f09770a4826a8cc1004903cd4e9005eff055c63246812a376`  
		Last Modified: Wed, 01 Jun 2022 22:53:46 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab89aed908fe45f53da57dfae1a8b8c6cd86095ae16ff74114042f8a979f1932`  
		Last Modified: Wed, 01 Jun 2022 23:13:30 GMT  
		Size: 7.0 MB (7036774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb64d47dd3ed3c1225ae6e128fbf6d24fcc3c845ef16f462a471531f409af29`  
		Last Modified: Wed, 01 Jun 2022 23:13:29 GMT  
		Size: 1.2 MB (1189006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9128167bb5002c5f6502cafb32b7004c893d437d65d07a486683d6a4827295`  
		Last Modified: Wed, 01 Jun 2022 23:13:28 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:51489e35e697983a57f901922b0dabd40e875688ab29307b905d29ce55fbaab9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121929763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ab8036b8f55aab1eb0d1627d8569e7b7b92390a17e595ffaf9dfe82da24529`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:17:40 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:17:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:17:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 May 2022 00:18:07 GMT
ENV GOLANG_VERSION=1.18.2
# Wed, 25 May 2022 00:21:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 25 May 2022 00:21:40 GMT
ENV GOPATH=/go
# Wed, 25 May 2022 00:21:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 May 2022 00:21:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 25 May 2022 00:21:58 GMT
WORKDIR /go
# Wed, 25 May 2022 00:45:35 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 25 May 2022 00:45:39 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 25 May 2022 00:45:43 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 25 May 2022 00:45:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 25 May 2022 00:45:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 25 May 2022 00:45:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 25 May 2022 00:46:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211c1f83aeafafff903bb460e7e24594fe138ebceeb1b56e898cf0158ea3daaf`  
		Last Modified: Wed, 25 May 2022 00:27:59 GMT  
		Size: 274.2 KB (274180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8365966bf1e6bd302f9e7c3d8e027aef3cfab1652ed22b8bd53311ef9517f0d3`  
		Last Modified: Wed, 25 May 2022 00:27:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6a047513e9ca46258b5a80c34d0bb9eef5b7e2c8004c5ddd1ca930e7c33659`  
		Last Modified: Wed, 25 May 2022 00:28:25 GMT  
		Size: 110.2 MB (110219016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4216cfe6259a3cf57000a58c453b0ffda2da2dd8b841017c33f4f9e33c8fa5da`  
		Last Modified: Wed, 25 May 2022 00:27:58 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2f4bee20e80c6473651d3ce23e74677476c7b12c9aa9bb880a3b819b0137d9`  
		Last Modified: Wed, 25 May 2022 00:46:38 GMT  
		Size: 7.5 MB (7469747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e99268d0161e857b0995380335a9c16bad6eaad709fc33fe99363301fc93c28`  
		Last Modified: Wed, 25 May 2022 00:46:38 GMT  
		Size: 1.2 MB (1176359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fa65f829c67a09aeb16d10c849ef12dcac7f86668154a677c8caa2bcc02c49`  
		Last Modified: Wed, 25 May 2022 00:46:37 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:2999d8fa276be8936078596794d15be8b708720ee296803ac88d976675f8b84a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124255828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc7070a321e5a4b1b7616b221cf9a73591e4fc00c310bfaad9825483eb4eb0d8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:41:57 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:41:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:41:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:43:25 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:45:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 22:46:11 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:46:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:46:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:46:13 GMT
WORKDIR /go
# Wed, 01 Jun 2022 23:16:35 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 23:16:36 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 23:16:37 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 23:16:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 23:16:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 23:16:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 23:16:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e497ff1a375465e6a6ba78259a6f2e9f7986cf27789ba79ddfd1cca023a160`  
		Last Modified: Wed, 25 May 2022 00:50:39 GMT  
		Size: 272.2 KB (272155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e413365aa9b9c967651e3a27f41641db43d81f24ff58ea4de0ce2c662c5d5f`  
		Last Modified: Wed, 25 May 2022 00:50:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e76ee5124cc2e0e213f5fc781375c53acc53fda6cb50eb09ce717d9ce4626ce`  
		Last Modified: Wed, 01 Jun 2022 22:58:35 GMT  
		Size: 113.1 MB (113111409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43db1e7eb380ed189bd16b98ad5afb071c88b789a987c6d8c2dd65dc4bfbf16d`  
		Last Modified: Wed, 01 Jun 2022 22:58:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0ade8df88187af31cea8632059bf709714e41aa1f2cf4a4bd3cee7562d3291`  
		Last Modified: Wed, 01 Jun 2022 23:17:26 GMT  
		Size: 7.0 MB (7047929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634c737128f1d3d767c417a20c9a5faaab86feb02d4e7a179046b7da981707f7`  
		Last Modified: Wed, 01 Jun 2022 23:17:25 GMT  
		Size: 1.2 MB (1243129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d94f95e9c108ec4db470dfbacda85ff19601a76bcfb7c7328b26c4fa4b09b9`  
		Last Modified: Wed, 01 Jun 2022 23:17:25 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.2928; amd64

```console
$ docker pull caddy@sha256:9ccfa9fc4fc4236cf295417a18c7d16b0a79495b916cd1b95c231e18daed3423
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2674256754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e7531282f56b1596b6475bd16a7058aaa9dc1e6884e7902f556e23b3eccf951`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 22:21:43 GMT
ENV GIT_VERSION=2.23.0
# Tue, 10 May 2022 22:21:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 10 May 2022 22:21:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 10 May 2022 22:21:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 10 May 2022 22:23:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:23:36 GMT
ENV GOPATH=C:\go
# Tue, 10 May 2022 22:24:28 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 10 May 2022 22:40:47 GMT
ENV GOLANG_VERSION=1.17.10
# Tue, 10 May 2022 22:44:40 GMT
RUN $url = 'https://dl.google.com/go/go1.17.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ba9198a29fa5c4f322212d21569e8507165c3b34e1ed1f1f9cf6dfb71ddcdeb2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:44:47 GMT
WORKDIR C:\go
# Tue, 10 May 2022 23:33:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:33:03 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 10 May 2022 23:33:04 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:33:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 10 May 2022 23:34:01 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 10 May 2022 23:34:02 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01012ab52f3f9693dd4b85e6e19a0b2659b4f869d6b5b5d2ea62afe84c9037c`  
		Last Modified: Tue, 10 May 2022 22:55:50 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988abb6e02c6ab2eb0330641b6378c4e110c132c761de086dfc1629462491e90`  
		Last Modified: Tue, 10 May 2022 22:55:48 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b62ac07a4cd6e0fd762f7f6e904be7b001affa78e8fbfeb8ca017a6f643d62c`  
		Last Modified: Tue, 10 May 2022 22:55:47 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e235721feec6368d5a652fd467681dffe74326d42da4bed8e43f777bc39c47`  
		Last Modified: Tue, 10 May 2022 22:55:47 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8195b6f87245387233358bc8fcc2679a23d9aa46cd4bfef94ac49284694c5c42`  
		Last Modified: Tue, 10 May 2022 22:56:13 GMT  
		Size: 25.6 MB (25580295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cfe0249f2fac54d31ea467ce63bdc69e4504b726a87d969fb1b42ab2ab3853`  
		Last Modified: Tue, 10 May 2022 22:55:45 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c97dcc9056ac36ad6120d94049a937f5366e71fda7c478ff3462d542cc0645`  
		Last Modified: Tue, 10 May 2022 22:55:45 GMT  
		Size: 322.0 KB (321981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4753086b1ed8db6655e0993e3f676d7f71455415cce16cd5593b330f9a89b3a`  
		Last Modified: Tue, 10 May 2022 23:05:04 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66134c7f83737bd3064ea2c3dce37ea0157cde99b46bbf80744100fd7f18a0aa`  
		Last Modified: Tue, 10 May 2022 23:07:31 GMT  
		Size: 142.6 MB (142588622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0697a4af489e787e5def466bbf9614e20bf5b1cea211f3a8f8ce2f0b5a10a3f`  
		Last Modified: Tue, 10 May 2022 23:05:04 GMT  
		Size: 1.6 KB (1566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c242b44aab0e82a2f6bf16213c350b73347e55ad15ecafa05877414e1327e96b`  
		Last Modified: Tue, 10 May 2022 23:36:29 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223dbf32ed9ac3b13af8e1196395df286392aa610ec5ba0bf809061dbf84a5cb`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a255b634df668adc897872554f8b720fdd5e6f4a9c47db0bbc489d25a0aaa66e`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe18292f9995b50f39e6e8ef4cfa31d2913132bef8804b56e260a907b205cd18`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168a524248b6a67f943614b53e6a0825bd107c0b90796733fccfe1184d013a45`  
		Last Modified: Tue, 10 May 2022 23:36:28 GMT  
		Size: 1.7 MB (1691907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4398dd61eb69a257d8e25ec572462f611d347efd5e30a944117a652f47314944`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.20348.707; amd64

```console
$ docker pull caddy@sha256:5577ab08abcc0385dd65f73089851d37eb4cd88a29a3cd1d511c6c526221fc42
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2415395050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8e125146193f9e2329bf6ce618db8d09adc336b804bec5cd23b54463959d504`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 22:16:59 GMT
ENV GIT_VERSION=2.23.0
# Tue, 10 May 2022 22:17:00 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 10 May 2022 22:17:01 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 10 May 2022 22:17:02 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 10 May 2022 22:17:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:17:52 GMT
ENV GOPATH=C:\go
# Tue, 10 May 2022 22:18:24 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 10 May 2022 22:18:25 GMT
ENV GOLANG_VERSION=1.18.2
# Tue, 10 May 2022 22:21:20 GMT
RUN $url = 'https://dl.google.com/go/go1.18.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '41fc44109c39a98e0c3672989ac5ad205cbb5768067e099dc4fb2b75cba922cf'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:21:26 GMT
WORKDIR C:\go
# Tue, 10 May 2022 23:34:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:34:18 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 10 May 2022 23:34:19 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:34:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 10 May 2022 23:34:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 10 May 2022 23:34:53 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb2ee3c21cb72c263da0dc4c6080f1d34c7ce3c7f24dcce76815784ec99440f`  
		Last Modified: Tue, 10 May 2022 22:52:57 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db422a46fd25683fe2e5990dc5db827b96c7b135679867ac162c2a318803463`  
		Last Modified: Tue, 10 May 2022 22:52:56 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4110a58975fa9bc64fa3a7d64804d47aa9ba813231538466dfedf4c35658cae7`  
		Last Modified: Tue, 10 May 2022 22:52:55 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e110f1696433dc412066aa30ea4222e641d7d377d593568f539b471b865a664`  
		Last Modified: Tue, 10 May 2022 22:52:55 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aca2a7cb069b5fd7ea06af17cd99249cae08f77d945258e72108af23fb4570a`  
		Last Modified: Tue, 10 May 2022 22:53:21 GMT  
		Size: 25.7 MB (25692112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc78480e80903590627dacfc79a3c978709b8c787cc193391852c4f8bf2ffca`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f488db75670938176d831a4bc8ddd4bb629e7a61e9ce5101882db134c0d162`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 541.2 KB (541163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7e0fbd217082bd92c424bbe5de58f546b38e43068d1f7b3a1121e42ffcbac6`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d268be7c91150b1073b85f55a434b87a1602a325ad6af8f2c2896f34f83388`  
		Last Modified: Tue, 10 May 2022 22:55:29 GMT  
		Size: 149.7 MB (149697865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3786f32f80e906fe1e08346c7294bfcfaa5d640b7c8cd920c91fb3b33f8bb6e4`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 1.5 KB (1536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd4f585b833fb8fb9f417326d46999e8726e1aa94e3796e9005a10daf16e12d`  
		Last Modified: Tue, 10 May 2022 23:36:48 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707272d91e9f672f1fe7a0de3ecaeefc72c1d00ee1025438e7cfb0dc74a77ee2`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a90464121b8d7fd8edb1f37124b634fe69680d1b4af3a6b853417ab05e9243a0`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20695dc76bb11cb698c1e429bbcb5e3011dfd00666a09a81c2cbd4f4607b1da`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884b6dd02ff92d7127e63601c97c036dee9230f73ecfe1d2d382466b705e9836`  
		Last Modified: Tue, 10 May 2022 23:36:46 GMT  
		Size: 1.9 MB (1910625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f0345f50b887c52e7c023a68e29e1332dac19143806fc334ea4d6e9a2cb0d5`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:ffbabc549906ee81026a50566ab1b254cafdafcc6e43c09abcc61fde1d323146
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:1e292f2e17935f1d904222aa4291d4b4f0a3f48ddd2c73af04039226c812d84b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126492209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c80070b3eb6003cffb12fd895325316a7ad91a7f7116a69ce3970897ef0742d3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:19:44 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:19:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:19:45 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:20:38 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:22:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 22:22:12 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:22:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:22:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:22:13 GMT
WORKDIR /go
# Wed, 01 Jun 2022 22:49:16 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 22:49:16 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 22:49:16 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 22:49:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 22:49:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 22:49:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 22:49:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea60b727a1ce729d031ec1e4f2521a246e71bdb72d3fd9c9c04711cce80e1722`  
		Last Modified: Wed, 25 May 2022 00:24:05 GMT  
		Size: 271.8 KB (271822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c4a77219572e69864cd3069b7b47e55202681be151bd7394f9cb6645b5687b`  
		Last Modified: Wed, 25 May 2022 00:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370296b7ddb629fff1cc98d8d390acf0782fdb8f55cf4054637f6127bbcfe2a9`  
		Last Modified: Wed, 01 Jun 2022 22:30:44 GMT  
		Size: 115.2 MB (115199527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6cee850709034cc7b53152e226caba834fdeb704dab0621f1813bc9081173c`  
		Last Modified: Wed, 01 Jun 2022 22:30:29 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1136d32ff848474c9a359e03d2fcc678a7b8f0dc7e73222ae72e60f7fd4d74`  
		Last Modified: Wed, 01 Jun 2022 22:49:37 GMT  
		Size: 6.9 MB (6931847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c29192c5c8d89201d847a27e2e77e0c4e47f3cef0219cb077dcd8b5bdd9fe1`  
		Last Modified: Wed, 01 Jun 2022 22:49:36 GMT  
		Size: 1.3 MB (1289410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865185451556d5e92a06e01ff04ae2d479a7ff41a4cef4d7f3e27cdb3d0a559e`  
		Last Modified: Wed, 01 Jun 2022 22:49:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:7de3187171d024e8352c7d65d8c0f7264ecba7b1a0f704295fd611019cb3570f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.5 MB (122503603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d3ac773c95b35b7b4dbac45428257530fdef319e97ee68be2648997c9e4bcd5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:49:39 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:49:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:51:15 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:55:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 22:55:14 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:55:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:55:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:55:16 GMT
WORKDIR /go
# Wed, 01 Jun 2022 23:30:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 23:30:47 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 23:30:48 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 23:30:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 23:30:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 23:30:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 23:30:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6c67ddc305b7f97a531083e369316343b3d19da2352e4e3274db751bba38e2`  
		Last Modified: Wed, 25 May 2022 00:59:27 GMT  
		Size: 272.0 KB (272047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8a37c8e9266706ee6b9ca75c42931dfe1320723ad6a20f0ad4c97554998348`  
		Last Modified: Wed, 25 May 2022 00:59:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d540be111b8c098590378841899d81bec5b744ccbd9ab573bc9b5101566901c`  
		Last Modified: Wed, 01 Jun 2022 23:09:53 GMT  
		Size: 111.6 MB (111598618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cafdd66ccebe1705fc4faa98039c9de106fbcbe091c52f158673fe04e82f802e`  
		Last Modified: Wed, 01 Jun 2022 23:08:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96872e0a675044607ec984baa827068687c978aa91bb47e3f49960519818427`  
		Last Modified: Wed, 01 Jun 2022 23:31:59 GMT  
		Size: 6.8 MB (6796920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3293e1352a64f4c075b505e4c5b86af54f57290c7d7f30c7881824677027cc2`  
		Last Modified: Wed, 01 Jun 2022 23:31:56 GMT  
		Size: 1.2 MB (1229160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4753da45404db22fc7c2a859da39a898b3708ecbfc5cfea606ee7431d28666e4`  
		Last Modified: Wed, 01 Jun 2022 23:31:55 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:011ac9678dff1b4c8b7b55ed5e314c4cff6da6b30703063ebd229e6b72d63cd6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121343857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48dd50101a28b86b1db7401d9cb0cf460f9f9e9a5543d3b3abe69cf3a4290028`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 03:51:19 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 03:51:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 03:51:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 23:01:24 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 23:05:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 23:05:24 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 23:05:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 23:05:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 23:05:28 GMT
WORKDIR /go
# Wed, 01 Jun 2022 23:54:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 23:54:05 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 23:54:05 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 23:54:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 23:54:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 23:54:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 23:54:09 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e4e5a89e8a0366f9710ba7cb04de284f11234b8cb3dba3e69e35a76dd1c62`  
		Last Modified: Wed, 25 May 2022 04:03:05 GMT  
		Size: 271.0 KB (270972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3b879ada9b059c6167f45b720f44118516dfc73e29b727218447700619fbc5`  
		Last Modified: Wed, 25 May 2022 04:03:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fc48eab20f513149fdf3afa2d29409fae14ca579ba77b44d39b1c7d30bd160`  
		Last Modified: Wed, 01 Jun 2022 23:29:17 GMT  
		Size: 111.4 MB (111376293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4611066e57bc80a36e6249e8637f907272e5888e39790c2360619a7e0cba4833`  
		Last Modified: Wed, 01 Jun 2022 23:28:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65e673e15769cdf43d8d431796fdce20817845053df123db32c4d1ebb097dda`  
		Last Modified: Wed, 01 Jun 2022 23:55:15 GMT  
		Size: 6.1 MB (6056216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f57b87d4f5a15b224a843782ea88621460db848ce77a22ea9556319c9e5c0c`  
		Last Modified: Wed, 01 Jun 2022 23:55:13 GMT  
		Size: 1.2 MB (1228015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a540258c6d4d9ec99d0f270d7f398f2a784a811119862c84d641faf27d9d52f`  
		Last Modified: Wed, 01 Jun 2022 23:55:12 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:499ea69b717472a063a52ae5197f6deb99d1b2bf52f6ffe632ae6ee4b151e8d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121425869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8397cebecc3630e1971e7a6391326e81bf1f7987dad0cd00d290554058a8e96`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:40:10 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:40:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:40:12 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:41:13 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:43:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 22:43:14 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:43:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:43:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:43:16 GMT
WORKDIR /go
# Wed, 01 Jun 2022 23:12:50 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 23:12:51 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 23:12:51 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 23:12:52 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 23:12:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 23:12:56 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 23:12:56 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a3192eca97ce26527d2bdbb26d1130abcc1c9dd7b800ce2fd14619fa422640`  
		Last Modified: Wed, 25 May 2022 00:45:29 GMT  
		Size: 271.7 KB (271711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a050256f5b6fc0800b8ae0d96e136745091c36ce8e53ba74d8ab3eed65966a59`  
		Last Modified: Wed, 25 May 2022 00:45:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656be50a0ddc84123afb23ccbb17811b43648fa17b4c8664716e9e07553c8b35`  
		Last Modified: Wed, 01 Jun 2022 22:54:01 GMT  
		Size: 110.2 MB (110233232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbca73fdf42200f09770a4826a8cc1004903cd4e9005eff055c63246812a376`  
		Last Modified: Wed, 01 Jun 2022 22:53:46 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab89aed908fe45f53da57dfae1a8b8c6cd86095ae16ff74114042f8a979f1932`  
		Last Modified: Wed, 01 Jun 2022 23:13:30 GMT  
		Size: 7.0 MB (7036774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb64d47dd3ed3c1225ae6e128fbf6d24fcc3c845ef16f462a471531f409af29`  
		Last Modified: Wed, 01 Jun 2022 23:13:29 GMT  
		Size: 1.2 MB (1189006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9128167bb5002c5f6502cafb32b7004c893d437d65d07a486683d6a4827295`  
		Last Modified: Wed, 01 Jun 2022 23:13:28 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:51489e35e697983a57f901922b0dabd40e875688ab29307b905d29ce55fbaab9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121929763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ab8036b8f55aab1eb0d1627d8569e7b7b92390a17e595ffaf9dfe82da24529`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:17:40 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:17:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:17:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 May 2022 00:18:07 GMT
ENV GOLANG_VERSION=1.18.2
# Wed, 25 May 2022 00:21:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 25 May 2022 00:21:40 GMT
ENV GOPATH=/go
# Wed, 25 May 2022 00:21:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 May 2022 00:21:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 25 May 2022 00:21:58 GMT
WORKDIR /go
# Wed, 25 May 2022 00:45:35 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 25 May 2022 00:45:39 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 25 May 2022 00:45:43 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 25 May 2022 00:45:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 25 May 2022 00:45:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 25 May 2022 00:45:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 25 May 2022 00:46:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211c1f83aeafafff903bb460e7e24594fe138ebceeb1b56e898cf0158ea3daaf`  
		Last Modified: Wed, 25 May 2022 00:27:59 GMT  
		Size: 274.2 KB (274180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8365966bf1e6bd302f9e7c3d8e027aef3cfab1652ed22b8bd53311ef9517f0d3`  
		Last Modified: Wed, 25 May 2022 00:27:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6a047513e9ca46258b5a80c34d0bb9eef5b7e2c8004c5ddd1ca930e7c33659`  
		Last Modified: Wed, 25 May 2022 00:28:25 GMT  
		Size: 110.2 MB (110219016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4216cfe6259a3cf57000a58c453b0ffda2da2dd8b841017c33f4f9e33c8fa5da`  
		Last Modified: Wed, 25 May 2022 00:27:58 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2f4bee20e80c6473651d3ce23e74677476c7b12c9aa9bb880a3b819b0137d9`  
		Last Modified: Wed, 25 May 2022 00:46:38 GMT  
		Size: 7.5 MB (7469747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e99268d0161e857b0995380335a9c16bad6eaad709fc33fe99363301fc93c28`  
		Last Modified: Wed, 25 May 2022 00:46:38 GMT  
		Size: 1.2 MB (1176359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fa65f829c67a09aeb16d10c849ef12dcac7f86668154a677c8caa2bcc02c49`  
		Last Modified: Wed, 25 May 2022 00:46:37 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:2999d8fa276be8936078596794d15be8b708720ee296803ac88d976675f8b84a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124255828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc7070a321e5a4b1b7616b221cf9a73591e4fc00c310bfaad9825483eb4eb0d8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:41:57 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:41:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:41:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:43:25 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:45:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 22:46:11 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:46:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:46:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:46:13 GMT
WORKDIR /go
# Wed, 01 Jun 2022 23:16:35 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 23:16:36 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 23:16:37 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 23:16:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 23:16:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 23:16:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 23:16:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e497ff1a375465e6a6ba78259a6f2e9f7986cf27789ba79ddfd1cca023a160`  
		Last Modified: Wed, 25 May 2022 00:50:39 GMT  
		Size: 272.2 KB (272155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e413365aa9b9c967651e3a27f41641db43d81f24ff58ea4de0ce2c662c5d5f`  
		Last Modified: Wed, 25 May 2022 00:50:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e76ee5124cc2e0e213f5fc781375c53acc53fda6cb50eb09ce717d9ce4626ce`  
		Last Modified: Wed, 01 Jun 2022 22:58:35 GMT  
		Size: 113.1 MB (113111409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43db1e7eb380ed189bd16b98ad5afb071c88b789a987c6d8c2dd65dc4bfbf16d`  
		Last Modified: Wed, 01 Jun 2022 22:58:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0ade8df88187af31cea8632059bf709714e41aa1f2cf4a4bd3cee7562d3291`  
		Last Modified: Wed, 01 Jun 2022 23:17:26 GMT  
		Size: 7.0 MB (7047929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634c737128f1d3d767c417a20c9a5faaab86feb02d4e7a179046b7da981707f7`  
		Last Modified: Wed, 01 Jun 2022 23:17:25 GMT  
		Size: 1.2 MB (1243129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d94f95e9c108ec4db470dfbacda85ff19601a76bcfb7c7328b26c4fa4b09b9`  
		Last Modified: Wed, 01 Jun 2022 23:17:25 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:80ca8f74f642d7218cc111d5ea59115a305c4cd6030325cb4c4a7fad93d4c5a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull caddy@sha256:9ccfa9fc4fc4236cf295417a18c7d16b0a79495b916cd1b95c231e18daed3423
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2674256754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e7531282f56b1596b6475bd16a7058aaa9dc1e6884e7902f556e23b3eccf951`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 22:21:43 GMT
ENV GIT_VERSION=2.23.0
# Tue, 10 May 2022 22:21:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 10 May 2022 22:21:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 10 May 2022 22:21:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 10 May 2022 22:23:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:23:36 GMT
ENV GOPATH=C:\go
# Tue, 10 May 2022 22:24:28 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 10 May 2022 22:40:47 GMT
ENV GOLANG_VERSION=1.17.10
# Tue, 10 May 2022 22:44:40 GMT
RUN $url = 'https://dl.google.com/go/go1.17.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ba9198a29fa5c4f322212d21569e8507165c3b34e1ed1f1f9cf6dfb71ddcdeb2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:44:47 GMT
WORKDIR C:\go
# Tue, 10 May 2022 23:33:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:33:03 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 10 May 2022 23:33:04 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:33:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 10 May 2022 23:34:01 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 10 May 2022 23:34:02 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01012ab52f3f9693dd4b85e6e19a0b2659b4f869d6b5b5d2ea62afe84c9037c`  
		Last Modified: Tue, 10 May 2022 22:55:50 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988abb6e02c6ab2eb0330641b6378c4e110c132c761de086dfc1629462491e90`  
		Last Modified: Tue, 10 May 2022 22:55:48 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b62ac07a4cd6e0fd762f7f6e904be7b001affa78e8fbfeb8ca017a6f643d62c`  
		Last Modified: Tue, 10 May 2022 22:55:47 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e235721feec6368d5a652fd467681dffe74326d42da4bed8e43f777bc39c47`  
		Last Modified: Tue, 10 May 2022 22:55:47 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8195b6f87245387233358bc8fcc2679a23d9aa46cd4bfef94ac49284694c5c42`  
		Last Modified: Tue, 10 May 2022 22:56:13 GMT  
		Size: 25.6 MB (25580295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cfe0249f2fac54d31ea467ce63bdc69e4504b726a87d969fb1b42ab2ab3853`  
		Last Modified: Tue, 10 May 2022 22:55:45 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c97dcc9056ac36ad6120d94049a937f5366e71fda7c478ff3462d542cc0645`  
		Last Modified: Tue, 10 May 2022 22:55:45 GMT  
		Size: 322.0 KB (321981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4753086b1ed8db6655e0993e3f676d7f71455415cce16cd5593b330f9a89b3a`  
		Last Modified: Tue, 10 May 2022 23:05:04 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66134c7f83737bd3064ea2c3dce37ea0157cde99b46bbf80744100fd7f18a0aa`  
		Last Modified: Tue, 10 May 2022 23:07:31 GMT  
		Size: 142.6 MB (142588622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0697a4af489e787e5def466bbf9614e20bf5b1cea211f3a8f8ce2f0b5a10a3f`  
		Last Modified: Tue, 10 May 2022 23:05:04 GMT  
		Size: 1.6 KB (1566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c242b44aab0e82a2f6bf16213c350b73347e55ad15ecafa05877414e1327e96b`  
		Last Modified: Tue, 10 May 2022 23:36:29 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223dbf32ed9ac3b13af8e1196395df286392aa610ec5ba0bf809061dbf84a5cb`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a255b634df668adc897872554f8b720fdd5e6f4a9c47db0bbc489d25a0aaa66e`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe18292f9995b50f39e6e8ef4cfa31d2913132bef8804b56e260a907b205cd18`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168a524248b6a67f943614b53e6a0825bd107c0b90796733fccfe1184d013a45`  
		Last Modified: Tue, 10 May 2022 23:36:28 GMT  
		Size: 1.7 MB (1691907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4398dd61eb69a257d8e25ec572462f611d347efd5e30a944117a652f47314944`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:f5f71b248dea482aed03fe1e9ffdbd84e3e337044b6e4263956c9e8069ff8da2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `caddy:2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.707; amd64

```console
$ docker pull caddy@sha256:5577ab08abcc0385dd65f73089851d37eb4cd88a29a3cd1d511c6c526221fc42
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2415395050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8e125146193f9e2329bf6ce618db8d09adc336b804bec5cd23b54463959d504`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 22:16:59 GMT
ENV GIT_VERSION=2.23.0
# Tue, 10 May 2022 22:17:00 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 10 May 2022 22:17:01 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 10 May 2022 22:17:02 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 10 May 2022 22:17:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:17:52 GMT
ENV GOPATH=C:\go
# Tue, 10 May 2022 22:18:24 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 10 May 2022 22:18:25 GMT
ENV GOLANG_VERSION=1.18.2
# Tue, 10 May 2022 22:21:20 GMT
RUN $url = 'https://dl.google.com/go/go1.18.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '41fc44109c39a98e0c3672989ac5ad205cbb5768067e099dc4fb2b75cba922cf'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:21:26 GMT
WORKDIR C:\go
# Tue, 10 May 2022 23:34:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:34:18 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 10 May 2022 23:34:19 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:34:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 10 May 2022 23:34:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 10 May 2022 23:34:53 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb2ee3c21cb72c263da0dc4c6080f1d34c7ce3c7f24dcce76815784ec99440f`  
		Last Modified: Tue, 10 May 2022 22:52:57 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db422a46fd25683fe2e5990dc5db827b96c7b135679867ac162c2a318803463`  
		Last Modified: Tue, 10 May 2022 22:52:56 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4110a58975fa9bc64fa3a7d64804d47aa9ba813231538466dfedf4c35658cae7`  
		Last Modified: Tue, 10 May 2022 22:52:55 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e110f1696433dc412066aa30ea4222e641d7d377d593568f539b471b865a664`  
		Last Modified: Tue, 10 May 2022 22:52:55 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aca2a7cb069b5fd7ea06af17cd99249cae08f77d945258e72108af23fb4570a`  
		Last Modified: Tue, 10 May 2022 22:53:21 GMT  
		Size: 25.7 MB (25692112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc78480e80903590627dacfc79a3c978709b8c787cc193391852c4f8bf2ffca`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f488db75670938176d831a4bc8ddd4bb629e7a61e9ce5101882db134c0d162`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 541.2 KB (541163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7e0fbd217082bd92c424bbe5de58f546b38e43068d1f7b3a1121e42ffcbac6`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d268be7c91150b1073b85f55a434b87a1602a325ad6af8f2c2896f34f83388`  
		Last Modified: Tue, 10 May 2022 22:55:29 GMT  
		Size: 149.7 MB (149697865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3786f32f80e906fe1e08346c7294bfcfaa5d640b7c8cd920c91fb3b33f8bb6e4`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 1.5 KB (1536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd4f585b833fb8fb9f417326d46999e8726e1aa94e3796e9005a10daf16e12d`  
		Last Modified: Tue, 10 May 2022 23:36:48 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707272d91e9f672f1fe7a0de3ecaeefc72c1d00ee1025438e7cfb0dc74a77ee2`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a90464121b8d7fd8edb1f37124b634fe69680d1b4af3a6b853417ab05e9243a0`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20695dc76bb11cb698c1e429bbcb5e3011dfd00666a09a81c2cbd4f4607b1da`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884b6dd02ff92d7127e63601c97c036dee9230f73ecfe1d2d382466b705e9836`  
		Last Modified: Tue, 10 May 2022 23:36:46 GMT  
		Size: 1.9 MB (1910625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f0345f50b887c52e7c023a68e29e1332dac19143806fc334ea4d6e9a2cb0d5`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:285398d41e72fa7778b741796f7a0892454ea9bdc4ed67b25cec85cd7494f9cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2928; amd64
	-	windows version 10.0.20348.707; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.2928; amd64

```console
$ docker pull caddy@sha256:8ad6979cdadd3d080deeb3a2f13d37c23789748ea80b29ac44624cf39bd589ff
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2518898800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8393d2b14b909a4ce523ae0d4999f2a492deb9e76ac12cc8dc111b5f0e3bd74d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:28:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 10 May 2022 23:28:55 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:29:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('4294796c4bd4bed0c593d83606a5413de30f35f88d624e1b1e5b6cd8672ffbcc7a689d7ce4ef30c1abea0e95eda62220faac15d2a6aca0c3e2b418abe7a74118')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 10 May 2022 23:29:54 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 10 May 2022 23:29:56 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 10 May 2022 23:29:57 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Tue, 10 May 2022 23:29:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 10 May 2022 23:29:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 10 May 2022 23:29:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 10 May 2022 23:30:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 10 May 2022 23:30:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 10 May 2022 23:30:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 10 May 2022 23:30:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 10 May 2022 23:30:04 GMT
EXPOSE 80
# Tue, 10 May 2022 23:30:05 GMT
EXPOSE 443
# Tue, 10 May 2022 23:30:06 GMT
EXPOSE 2019
# Tue, 10 May 2022 23:30:47 GMT
RUN caddy version
# Tue, 10 May 2022 23:30:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d722bd7a5ed597b5a9ed7c5144caa608e784120c4442579352b7c2325ce47ffc`  
		Last Modified: Tue, 10 May 2022 23:35:41 GMT  
		Size: 498.2 KB (498231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0dfede5e37c630a175a1c987d90aaf1ec1db8cd7d43e3d63648743c6ace743`  
		Last Modified: Tue, 10 May 2022 23:35:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef201446c9bd5610f78b8e5a1680047ff45fadb77727762c323d5e48d77f9f2`  
		Last Modified: Tue, 10 May 2022 23:35:44 GMT  
		Size: 14.0 MB (14007489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b824e8abcb45a47ada825f0b722a588cbc9d1f68f5536a76b7afed2c5eb15a0c`  
		Last Modified: Tue, 10 May 2022 23:35:39 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b01057f474e19bdcaebab2c156622642945d2c7074276c82de663baeb418143`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520fb9c4921f60cfaea07cfa8d5733cf7f4f0810e56106911d7b25f59e86e997`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74d9e7abc08a32b35b26f8bba23c597b1e19d604766b326f61e77da0b494285`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595304462c9d3aa03aa9e164a98a38be5e1f5307c2981b65aa228101c73ce91b`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e307ee1571a8185932bbd90267a8b8d367f784859d99a2742d44e89e19e8b6c0`  
		Last Modified: Tue, 10 May 2022 23:35:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b335f1fddf0ed6abcc0e715ff827614cc2f0f4bbe8a0e1565145951d841c96`  
		Last Modified: Tue, 10 May 2022 23:35:36 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0974b9a20e0fa84c8a353a7c04992bec9e06825ed808054a358b84409744ba`  
		Last Modified: Tue, 10 May 2022 23:35:35 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d5086c691961c9f1a18b9d161cf8cb3dbd7b581c68ab75760b8c5e62647928`  
		Last Modified: Tue, 10 May 2022 23:35:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9194a8cf5ac8d920d218d9100152393ac6cce9142b15904894374694ae2d2fc`  
		Last Modified: Tue, 10 May 2022 23:35:36 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd07be490606caadc3893d219aee0682d6f8b71b2a4a8f2fb2ca826cdffb74`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b19beef4c4a6634592447260a670c8ee571e59cb775833787d39b815e9ba511`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2dab7fd2beddb5439029e7d8a75fc7c7fe2d3a534a63f51a04f85dd371cd1c`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e195aa5e2a95379397baf57f681e2c39a7c673d3c06d0ff3e4eeed3d8cecee1`  
		Last Modified: Tue, 10 May 2022 23:35:34 GMT  
		Size: 314.6 KB (314586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87827ca78b495430e19218a9e3f7f2837078a77df34bb929124ea20614287d5`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.20348.707; amd64

```console
$ docker pull caddy@sha256:a3894222673d46b3e350553c6b7d4f92ab27b85a87fa1f773e9b090d5774ca9e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2252723203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:063f1879bd2783934ad3ac23aa37bf45f19be756f6b018f4c3a67d2d4a759c7c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:31:41 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 10 May 2022 23:31:42 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:32:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('4294796c4bd4bed0c593d83606a5413de30f35f88d624e1b1e5b6cd8672ffbcc7a689d7ce4ef30c1abea0e95eda62220faac15d2a6aca0c3e2b418abe7a74118')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 10 May 2022 23:32:11 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 10 May 2022 23:32:12 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 10 May 2022 23:32:13 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Tue, 10 May 2022 23:32:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 10 May 2022 23:32:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 10 May 2022 23:32:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 10 May 2022 23:32:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 10 May 2022 23:32:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 10 May 2022 23:32:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 10 May 2022 23:32:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 10 May 2022 23:32:21 GMT
EXPOSE 80
# Tue, 10 May 2022 23:32:22 GMT
EXPOSE 443
# Tue, 10 May 2022 23:32:23 GMT
EXPOSE 2019
# Tue, 10 May 2022 23:32:42 GMT
RUN caddy version
# Tue, 10 May 2022 23:32:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9baa8a196af04dc55746ee82c0774537bce72a589b75d9efce1a4680f03e35`  
		Last Modified: Tue, 10 May 2022 23:36:04 GMT  
		Size: 616.1 KB (616130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe60c7e90fdaeffa9bce60d9a7c7b340dedc357bfb70a2ce8c6d7b8bd0e74a11`  
		Last Modified: Tue, 10 May 2022 23:36:04 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f955bea173999b55d2087a27b9cc80e92bf168918c6e892175c2a75bdbfac933`  
		Last Modified: Tue, 10 May 2022 23:36:07 GMT  
		Size: 14.2 MB (14224642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e1ab4508d5347b929d5a33f71e0f24f653e61c147260200d32e3bd7cdd2340`  
		Last Modified: Tue, 10 May 2022 23:36:02 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8044ca4427c5edfee653001205397a2cc33f8fb4416c16c4a4936317c572ed`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f144416d38a1aa75558e0b93b88fcb3de122ee88349826ee99d596e1b00d9cc0`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32edbcceba80e7a70e44725926012bb70624bb0ae91c85db2766ca2e4c5a5d7c`  
		Last Modified: Tue, 10 May 2022 23:36:02 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd90105a2a3136e4d25d0add2b6fbe5798d51588215367128f1566d66b255289`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e448ed08c6c6ca9f854cb7014ea2e79c04e83f1905f78f578b67303b709fa3`  
		Last Modified: Tue, 10 May 2022 23:36:00 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d49b1b3778cd2ebf32521f530e29275a9a473afa997654b32338ff4349bf5c`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2112945425b7d069bc5705be1345e5ad6e27206e1531b10d0bc92d9c69ea9c3`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7243327255edd82b277f456085138a672f5a43d616e80f73156c8eb31139121d`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1a14330360d7ab3af40d4fb6f2de975e42e05f8e4cb064cc49fe1d9446e6b1`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808ce6a15ca3e6ad031229bcad8a3ed69171a7005c05ef4e77ffcfd777e9d1f7`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdfcf611e614d42a256d103775233f59ab7bb6ad0b00ca2f915bf739600f8d6`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3811622d464d497ce363eed806c75f9b994cd1d04b3009b2d0671af2863ebd0`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b006092864e6cfdfedd054a2635236c62958e97de81c720d9e38772276ee11`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 325.9 KB (325870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2afb0ece27a359f16126f263176baa74c3d3f2f2733cce186e4e31ad0eca4f8`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:61aa7b1019d479a8c0c21f043ffbec427336684486cad3858e71de43f3962e7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull caddy@sha256:8ad6979cdadd3d080deeb3a2f13d37c23789748ea80b29ac44624cf39bd589ff
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2518898800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8393d2b14b909a4ce523ae0d4999f2a492deb9e76ac12cc8dc111b5f0e3bd74d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:28:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 10 May 2022 23:28:55 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:29:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('4294796c4bd4bed0c593d83606a5413de30f35f88d624e1b1e5b6cd8672ffbcc7a689d7ce4ef30c1abea0e95eda62220faac15d2a6aca0c3e2b418abe7a74118')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 10 May 2022 23:29:54 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 10 May 2022 23:29:56 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 10 May 2022 23:29:57 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Tue, 10 May 2022 23:29:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 10 May 2022 23:29:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 10 May 2022 23:29:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 10 May 2022 23:30:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 10 May 2022 23:30:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 10 May 2022 23:30:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 10 May 2022 23:30:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 10 May 2022 23:30:04 GMT
EXPOSE 80
# Tue, 10 May 2022 23:30:05 GMT
EXPOSE 443
# Tue, 10 May 2022 23:30:06 GMT
EXPOSE 2019
# Tue, 10 May 2022 23:30:47 GMT
RUN caddy version
# Tue, 10 May 2022 23:30:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d722bd7a5ed597b5a9ed7c5144caa608e784120c4442579352b7c2325ce47ffc`  
		Last Modified: Tue, 10 May 2022 23:35:41 GMT  
		Size: 498.2 KB (498231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0dfede5e37c630a175a1c987d90aaf1ec1db8cd7d43e3d63648743c6ace743`  
		Last Modified: Tue, 10 May 2022 23:35:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef201446c9bd5610f78b8e5a1680047ff45fadb77727762c323d5e48d77f9f2`  
		Last Modified: Tue, 10 May 2022 23:35:44 GMT  
		Size: 14.0 MB (14007489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b824e8abcb45a47ada825f0b722a588cbc9d1f68f5536a76b7afed2c5eb15a0c`  
		Last Modified: Tue, 10 May 2022 23:35:39 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b01057f474e19bdcaebab2c156622642945d2c7074276c82de663baeb418143`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520fb9c4921f60cfaea07cfa8d5733cf7f4f0810e56106911d7b25f59e86e997`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74d9e7abc08a32b35b26f8bba23c597b1e19d604766b326f61e77da0b494285`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595304462c9d3aa03aa9e164a98a38be5e1f5307c2981b65aa228101c73ce91b`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e307ee1571a8185932bbd90267a8b8d367f784859d99a2742d44e89e19e8b6c0`  
		Last Modified: Tue, 10 May 2022 23:35:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b335f1fddf0ed6abcc0e715ff827614cc2f0f4bbe8a0e1565145951d841c96`  
		Last Modified: Tue, 10 May 2022 23:35:36 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0974b9a20e0fa84c8a353a7c04992bec9e06825ed808054a358b84409744ba`  
		Last Modified: Tue, 10 May 2022 23:35:35 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d5086c691961c9f1a18b9d161cf8cb3dbd7b581c68ab75760b8c5e62647928`  
		Last Modified: Tue, 10 May 2022 23:35:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9194a8cf5ac8d920d218d9100152393ac6cce9142b15904894374694ae2d2fc`  
		Last Modified: Tue, 10 May 2022 23:35:36 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd07be490606caadc3893d219aee0682d6f8b71b2a4a8f2fb2ca826cdffb74`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b19beef4c4a6634592447260a670c8ee571e59cb775833787d39b815e9ba511`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2dab7fd2beddb5439029e7d8a75fc7c7fe2d3a534a63f51a04f85dd371cd1c`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e195aa5e2a95379397baf57f681e2c39a7c673d3c06d0ff3e4eeed3d8cecee1`  
		Last Modified: Tue, 10 May 2022 23:35:34 GMT  
		Size: 314.6 KB (314586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87827ca78b495430e19218a9e3f7f2837078a77df34bb929124ea20614287d5`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:88a75e54141f2e7531d3262b5a00a17002af383f24e29dab09212e4cbbfa2fdd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `caddy:2-windowsservercore-ltsc2022` - windows version 10.0.20348.707; amd64

```console
$ docker pull caddy@sha256:a3894222673d46b3e350553c6b7d4f92ab27b85a87fa1f773e9b090d5774ca9e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2252723203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:063f1879bd2783934ad3ac23aa37bf45f19be756f6b018f4c3a67d2d4a759c7c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:31:41 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 10 May 2022 23:31:42 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:32:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('4294796c4bd4bed0c593d83606a5413de30f35f88d624e1b1e5b6cd8672ffbcc7a689d7ce4ef30c1abea0e95eda62220faac15d2a6aca0c3e2b418abe7a74118')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 10 May 2022 23:32:11 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 10 May 2022 23:32:12 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 10 May 2022 23:32:13 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Tue, 10 May 2022 23:32:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 10 May 2022 23:32:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 10 May 2022 23:32:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 10 May 2022 23:32:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 10 May 2022 23:32:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 10 May 2022 23:32:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 10 May 2022 23:32:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 10 May 2022 23:32:21 GMT
EXPOSE 80
# Tue, 10 May 2022 23:32:22 GMT
EXPOSE 443
# Tue, 10 May 2022 23:32:23 GMT
EXPOSE 2019
# Tue, 10 May 2022 23:32:42 GMT
RUN caddy version
# Tue, 10 May 2022 23:32:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9baa8a196af04dc55746ee82c0774537bce72a589b75d9efce1a4680f03e35`  
		Last Modified: Tue, 10 May 2022 23:36:04 GMT  
		Size: 616.1 KB (616130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe60c7e90fdaeffa9bce60d9a7c7b340dedc357bfb70a2ce8c6d7b8bd0e74a11`  
		Last Modified: Tue, 10 May 2022 23:36:04 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f955bea173999b55d2087a27b9cc80e92bf168918c6e892175c2a75bdbfac933`  
		Last Modified: Tue, 10 May 2022 23:36:07 GMT  
		Size: 14.2 MB (14224642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e1ab4508d5347b929d5a33f71e0f24f653e61c147260200d32e3bd7cdd2340`  
		Last Modified: Tue, 10 May 2022 23:36:02 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8044ca4427c5edfee653001205397a2cc33f8fb4416c16c4a4936317c572ed`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f144416d38a1aa75558e0b93b88fcb3de122ee88349826ee99d596e1b00d9cc0`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32edbcceba80e7a70e44725926012bb70624bb0ae91c85db2766ca2e4c5a5d7c`  
		Last Modified: Tue, 10 May 2022 23:36:02 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd90105a2a3136e4d25d0add2b6fbe5798d51588215367128f1566d66b255289`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e448ed08c6c6ca9f854cb7014ea2e79c04e83f1905f78f578b67303b709fa3`  
		Last Modified: Tue, 10 May 2022 23:36:00 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d49b1b3778cd2ebf32521f530e29275a9a473afa997654b32338ff4349bf5c`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2112945425b7d069bc5705be1345e5ad6e27206e1531b10d0bc92d9c69ea9c3`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7243327255edd82b277f456085138a672f5a43d616e80f73156c8eb31139121d`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1a14330360d7ab3af40d4fb6f2de975e42e05f8e4cb064cc49fe1d9446e6b1`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808ce6a15ca3e6ad031229bcad8a3ed69171a7005c05ef4e77ffcfd777e9d1f7`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdfcf611e614d42a256d103775233f59ab7bb6ad0b00ca2f915bf739600f8d6`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3811622d464d497ce363eed806c75f9b994cd1d04b3009b2d0671af2863ebd0`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b006092864e6cfdfedd054a2635236c62958e97de81c720d9e38772276ee11`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 325.9 KB (325870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2afb0ece27a359f16126f263176baa74c3d3f2f2733cce186e4e31ad0eca4f8`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.1`

```console
$ docker pull caddy@sha256:eb2cce28a50cb1f20f1e4a13181f3e453e58d20999cffa7750222d9907023b6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2928; amd64
	-	windows version 10.0.20348.707; amd64

### `caddy:2.5.1` - linux; amd64

```console
$ docker pull caddy@sha256:6e62b63d4d7a4826f9e93c904a0e5b886a8bea2234b6569e300924282a2e8e6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16788470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e63f36e9049faf60b3a47c774237eddacb8916cacb003e418f2591de1a3bee29`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:25:00 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:19:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:19:24 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:19:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:19:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:19:26 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:19:26 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:19:27 GMT
EXPOSE 80
# Fri, 06 May 2022 19:19:27 GMT
EXPOSE 443
# Fri, 06 May 2022 19:19:28 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:19:28 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:19:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87ed6b8c4412bcd2bb1f40611012b40444b12071baf4884d0e75044fc1f32c1`  
		Last Modified: Tue, 05 Apr 2022 04:25:48 GMT  
		Size: 291.5 KB (291522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4c78357cc2da49b060ec4367d3d35d9837faf50e873e07ab40822e9fa57d00`  
		Last Modified: Fri, 06 May 2022 19:19:49 GMT  
		Size: 5.8 KB (5836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3edd190820fd86aaeb4fc1b7a28d7ff52e776414d3830f1a14d103967b455965`  
		Last Modified: Fri, 06 May 2022 19:19:51 GMT  
		Size: 13.7 MB (13676400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b96fea00470fa7356d42265c310e3940426e4c5572f288e8f7111a03b2fdddc`  
		Last Modified: Fri, 06 May 2022 19:19:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.1` - linux; arm variant v6

```console
$ docker pull caddy@sha256:813c33aa7f94275843088c57b0e44ea6c190d5296b664d7795f66bf3c3804392
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16056332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ee6ea861df7cd9fff1d948de8590f2bac9f2b90ebea7bc71ef7c7654f2d8d40`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:15:01 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:49:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:49:35 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:49:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:49:42 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:49:42 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:49:42 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:49:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:49:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:49:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:49:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:49:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:49:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:49:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:49:46 GMT
EXPOSE 80
# Fri, 06 May 2022 19:49:46 GMT
EXPOSE 443
# Fri, 06 May 2022 19:49:46 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:49:47 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:49:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b230dd773e10769a2eb3e507260d2470a646efd48a639739ba8852b2915302`  
		Last Modified: Tue, 05 Apr 2022 03:18:10 GMT  
		Size: 291.7 KB (291685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd82040b030d75398d6d6fb1c3d12cc9e25a954a92227895e1e5f7ea54736c20`  
		Last Modified: Fri, 06 May 2022 19:51:07 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583abcfacbc800cc0863a5117f1911222bec7ea3fcaed7c36ce4b94b489c3b3e`  
		Last Modified: Fri, 06 May 2022 19:51:16 GMT  
		Size: 13.1 MB (13136691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6903af22655a77183d11fb6d870f6ebc4776e6d9222e9de261b0a377cb81bbcf`  
		Last Modified: Fri, 06 May 2022 19:51:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.1` - linux; arm variant v7

```console
$ docker pull caddy@sha256:2e61a3ed70ad9a4784ff95cf49efa7ec58255c5263c3faba6a5270a847542a41
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.8 MB (15835582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93c6db987e0721fcd4f557ec160b55012a73d2f69de7198fac316514b27ed58f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:33:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:57:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:57:32 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:57:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:57:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:57:39 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:57:39 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:57:40 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:57:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:57:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:57:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:57:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:57:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:57:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:57:42 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:57:43 GMT
EXPOSE 80
# Fri, 06 May 2022 19:57:43 GMT
EXPOSE 443
# Fri, 06 May 2022 19:57:44 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:57:44 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:57:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03203881a2568530a735b6e0e7a40ebb79adedc5193a675807b04eeb92cc6ed1`  
		Last Modified: Tue, 05 Apr 2022 06:35:07 GMT  
		Size: 290.7 KB (290668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507adf96fcab6911303d2b3d14aeb43223c106ee9901b3e31f30668a4dbd5ffb`  
		Last Modified: Fri, 06 May 2022 19:59:02 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23435dc592c99e66d2e9f715136b809e73116ee6725847ed8fd158135e3283be`  
		Last Modified: Fri, 06 May 2022 19:59:11 GMT  
		Size: 13.1 MB (13114610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e55b7a8b43f4fdfecf61cea01ddddc80930ed485d9aafc41c26f84380f858f3`  
		Last Modified: Fri, 06 May 2022 19:59:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.1` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:cda45585c425161575996ee5d954166745d44d39928846423ecdce6b61a9fb4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.5 MB (15523770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:890cdb4fef0cc66aabb117ff1b3e11fb86de5117d28a5b0e64a743efb92c4269`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:12:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:39:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:39:32 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:39:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:39:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:39:37 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:39:38 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:39:39 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:39:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:39:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:39:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:39:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:39:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:39:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:39:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:39:47 GMT
EXPOSE 80
# Fri, 06 May 2022 19:39:48 GMT
EXPOSE 443
# Fri, 06 May 2022 19:39:49 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:39:50 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:39:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83aa37f2341b1e6d98420668c9bc849a47f2c471d159b2303885040bd8d0a92f`  
		Last Modified: Tue, 05 Apr 2022 03:13:38 GMT  
		Size: 291.3 KB (291301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc050d3d6ffb91c2f68db47e3d5f056afad26e465a03ae7e43383df0fc8ad89`  
		Last Modified: Fri, 06 May 2022 19:40:32 GMT  
		Size: 5.8 KB (5753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8adaff0bd78d0b115843dd841c83d1690484b25369e804b1133b838b7ad5ce8f`  
		Last Modified: Fri, 06 May 2022 19:40:35 GMT  
		Size: 12.5 MB (12510086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f703c61da5ec8e48b081aceac2cb64fb25162c2f0ba1ad16a104610b676f50f6`  
		Last Modified: Fri, 06 May 2022 19:40:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.1` - linux; ppc64le

```console
$ docker pull caddy@sha256:d1ab9f3165d5b23b9ff5bd4fcb74b3f8bbf834ba34c42c58e496b3d33017ca59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15203958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfbb2004b1ba3aace5176af38455ef6b8328a074388b16b35358d61330ad2658`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:08:34 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:16:53 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:16:58 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:17:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:17:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:17:25 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:17:32 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:17:36 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:17:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:17:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:17:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:17:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:17:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:18:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:18:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:18:13 GMT
EXPOSE 80
# Fri, 06 May 2022 19:18:17 GMT
EXPOSE 443
# Fri, 06 May 2022 19:18:19 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:18:22 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:18:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743509d6ced044a369685ebb068417e8757981a39d1b397c7b0182ab89f83528`  
		Last Modified: Tue, 05 Apr 2022 07:11:24 GMT  
		Size: 293.7 KB (293721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b659dd8890d066269209696348c58ed19351199266936a5e81f1991a52333d1`  
		Last Modified: Fri, 06 May 2022 19:19:31 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86272ae554176010d052c51dcc5540948b8e59082743b04ac5bb67d05c3fdcd`  
		Last Modified: Fri, 06 May 2022 19:19:33 GMT  
		Size: 12.1 MB (12093067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff57ff409904cc43937df14c68e6d97e1269adde095e91671fb5438dc58a1808`  
		Last Modified: Fri, 06 May 2022 19:19:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.1` - linux; s390x

```console
$ docker pull caddy@sha256:fbee089e769bc54babbe3ac3217c0e5b60c4a5157b76b0f37aa73cc71486c8fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16129299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f94fa793c943e1cb1c5bda77b0e7077b344648635da2222a1061307e3e61ca96`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:19:41 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:41:25 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:41:25 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:41:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:41:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:41:28 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:41:28 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:41:28 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:41:29 GMT
EXPOSE 80
# Fri, 06 May 2022 19:41:29 GMT
EXPOSE 443
# Fri, 06 May 2022 19:41:30 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:41:30 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:41:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8cc7c7c7ffd67f5740add448d341753330a2abdc6ed06e995cb7d28de381ab`  
		Last Modified: Tue, 05 Apr 2022 06:20:44 GMT  
		Size: 291.8 KB (291821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3d2fae470dbad90c4c4c1262110f14447a47b6e81edc4e0e80ceb50538fe57`  
		Last Modified: Fri, 06 May 2022 19:42:10 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a8f9dbbf38ad9456666a4e6a3eda871b385d4ef76ab6dc25e31030d1daf71c`  
		Last Modified: Fri, 06 May 2022 19:42:12 GMT  
		Size: 13.2 MB (13231118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf07e991258bc58c5e8a5785f741bc746e75848423d2c27d26448015c5887f1`  
		Last Modified: Fri, 06 May 2022 19:42:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.1` - windows version 10.0.17763.2928; amd64

```console
$ docker pull caddy@sha256:8ad6979cdadd3d080deeb3a2f13d37c23789748ea80b29ac44624cf39bd589ff
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2518898800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8393d2b14b909a4ce523ae0d4999f2a492deb9e76ac12cc8dc111b5f0e3bd74d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:28:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 10 May 2022 23:28:55 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:29:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('4294796c4bd4bed0c593d83606a5413de30f35f88d624e1b1e5b6cd8672ffbcc7a689d7ce4ef30c1abea0e95eda62220faac15d2a6aca0c3e2b418abe7a74118')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 10 May 2022 23:29:54 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 10 May 2022 23:29:56 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 10 May 2022 23:29:57 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Tue, 10 May 2022 23:29:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 10 May 2022 23:29:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 10 May 2022 23:29:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 10 May 2022 23:30:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 10 May 2022 23:30:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 10 May 2022 23:30:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 10 May 2022 23:30:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 10 May 2022 23:30:04 GMT
EXPOSE 80
# Tue, 10 May 2022 23:30:05 GMT
EXPOSE 443
# Tue, 10 May 2022 23:30:06 GMT
EXPOSE 2019
# Tue, 10 May 2022 23:30:47 GMT
RUN caddy version
# Tue, 10 May 2022 23:30:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d722bd7a5ed597b5a9ed7c5144caa608e784120c4442579352b7c2325ce47ffc`  
		Last Modified: Tue, 10 May 2022 23:35:41 GMT  
		Size: 498.2 KB (498231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0dfede5e37c630a175a1c987d90aaf1ec1db8cd7d43e3d63648743c6ace743`  
		Last Modified: Tue, 10 May 2022 23:35:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef201446c9bd5610f78b8e5a1680047ff45fadb77727762c323d5e48d77f9f2`  
		Last Modified: Tue, 10 May 2022 23:35:44 GMT  
		Size: 14.0 MB (14007489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b824e8abcb45a47ada825f0b722a588cbc9d1f68f5536a76b7afed2c5eb15a0c`  
		Last Modified: Tue, 10 May 2022 23:35:39 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b01057f474e19bdcaebab2c156622642945d2c7074276c82de663baeb418143`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520fb9c4921f60cfaea07cfa8d5733cf7f4f0810e56106911d7b25f59e86e997`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74d9e7abc08a32b35b26f8bba23c597b1e19d604766b326f61e77da0b494285`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595304462c9d3aa03aa9e164a98a38be5e1f5307c2981b65aa228101c73ce91b`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e307ee1571a8185932bbd90267a8b8d367f784859d99a2742d44e89e19e8b6c0`  
		Last Modified: Tue, 10 May 2022 23:35:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b335f1fddf0ed6abcc0e715ff827614cc2f0f4bbe8a0e1565145951d841c96`  
		Last Modified: Tue, 10 May 2022 23:35:36 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0974b9a20e0fa84c8a353a7c04992bec9e06825ed808054a358b84409744ba`  
		Last Modified: Tue, 10 May 2022 23:35:35 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d5086c691961c9f1a18b9d161cf8cb3dbd7b581c68ab75760b8c5e62647928`  
		Last Modified: Tue, 10 May 2022 23:35:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9194a8cf5ac8d920d218d9100152393ac6cce9142b15904894374694ae2d2fc`  
		Last Modified: Tue, 10 May 2022 23:35:36 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd07be490606caadc3893d219aee0682d6f8b71b2a4a8f2fb2ca826cdffb74`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b19beef4c4a6634592447260a670c8ee571e59cb775833787d39b815e9ba511`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2dab7fd2beddb5439029e7d8a75fc7c7fe2d3a534a63f51a04f85dd371cd1c`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e195aa5e2a95379397baf57f681e2c39a7c673d3c06d0ff3e4eeed3d8cecee1`  
		Last Modified: Tue, 10 May 2022 23:35:34 GMT  
		Size: 314.6 KB (314586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87827ca78b495430e19218a9e3f7f2837078a77df34bb929124ea20614287d5`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.1` - windows version 10.0.20348.707; amd64

```console
$ docker pull caddy@sha256:a3894222673d46b3e350553c6b7d4f92ab27b85a87fa1f773e9b090d5774ca9e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2252723203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:063f1879bd2783934ad3ac23aa37bf45f19be756f6b018f4c3a67d2d4a759c7c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:31:41 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 10 May 2022 23:31:42 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:32:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('4294796c4bd4bed0c593d83606a5413de30f35f88d624e1b1e5b6cd8672ffbcc7a689d7ce4ef30c1abea0e95eda62220faac15d2a6aca0c3e2b418abe7a74118')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 10 May 2022 23:32:11 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 10 May 2022 23:32:12 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 10 May 2022 23:32:13 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Tue, 10 May 2022 23:32:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 10 May 2022 23:32:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 10 May 2022 23:32:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 10 May 2022 23:32:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 10 May 2022 23:32:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 10 May 2022 23:32:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 10 May 2022 23:32:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 10 May 2022 23:32:21 GMT
EXPOSE 80
# Tue, 10 May 2022 23:32:22 GMT
EXPOSE 443
# Tue, 10 May 2022 23:32:23 GMT
EXPOSE 2019
# Tue, 10 May 2022 23:32:42 GMT
RUN caddy version
# Tue, 10 May 2022 23:32:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9baa8a196af04dc55746ee82c0774537bce72a589b75d9efce1a4680f03e35`  
		Last Modified: Tue, 10 May 2022 23:36:04 GMT  
		Size: 616.1 KB (616130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe60c7e90fdaeffa9bce60d9a7c7b340dedc357bfb70a2ce8c6d7b8bd0e74a11`  
		Last Modified: Tue, 10 May 2022 23:36:04 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f955bea173999b55d2087a27b9cc80e92bf168918c6e892175c2a75bdbfac933`  
		Last Modified: Tue, 10 May 2022 23:36:07 GMT  
		Size: 14.2 MB (14224642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e1ab4508d5347b929d5a33f71e0f24f653e61c147260200d32e3bd7cdd2340`  
		Last Modified: Tue, 10 May 2022 23:36:02 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8044ca4427c5edfee653001205397a2cc33f8fb4416c16c4a4936317c572ed`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f144416d38a1aa75558e0b93b88fcb3de122ee88349826ee99d596e1b00d9cc0`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32edbcceba80e7a70e44725926012bb70624bb0ae91c85db2766ca2e4c5a5d7c`  
		Last Modified: Tue, 10 May 2022 23:36:02 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd90105a2a3136e4d25d0add2b6fbe5798d51588215367128f1566d66b255289`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e448ed08c6c6ca9f854cb7014ea2e79c04e83f1905f78f578b67303b709fa3`  
		Last Modified: Tue, 10 May 2022 23:36:00 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d49b1b3778cd2ebf32521f530e29275a9a473afa997654b32338ff4349bf5c`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2112945425b7d069bc5705be1345e5ad6e27206e1531b10d0bc92d9c69ea9c3`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7243327255edd82b277f456085138a672f5a43d616e80f73156c8eb31139121d`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1a14330360d7ab3af40d4fb6f2de975e42e05f8e4cb064cc49fe1d9446e6b1`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808ce6a15ca3e6ad031229bcad8a3ed69171a7005c05ef4e77ffcfd777e9d1f7`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdfcf611e614d42a256d103775233f59ab7bb6ad0b00ca2f915bf739600f8d6`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3811622d464d497ce363eed806c75f9b994cd1d04b3009b2d0671af2863ebd0`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b006092864e6cfdfedd054a2635236c62958e97de81c720d9e38772276ee11`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 325.9 KB (325870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2afb0ece27a359f16126f263176baa74c3d3f2f2733cce186e4e31ad0eca4f8`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.1-alpine`

```console
$ docker pull caddy@sha256:0033b34d2df3fe0bf94088c36e7d722ceca1b38cbdd49c08b2c10b9f9aa58912
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.5.1-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:6e62b63d4d7a4826f9e93c904a0e5b886a8bea2234b6569e300924282a2e8e6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16788470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e63f36e9049faf60b3a47c774237eddacb8916cacb003e418f2591de1a3bee29`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:25:00 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:19:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:19:24 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:19:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:19:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:19:26 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:19:26 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:19:27 GMT
EXPOSE 80
# Fri, 06 May 2022 19:19:27 GMT
EXPOSE 443
# Fri, 06 May 2022 19:19:28 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:19:28 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:19:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87ed6b8c4412bcd2bb1f40611012b40444b12071baf4884d0e75044fc1f32c1`  
		Last Modified: Tue, 05 Apr 2022 04:25:48 GMT  
		Size: 291.5 KB (291522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4c78357cc2da49b060ec4367d3d35d9837faf50e873e07ab40822e9fa57d00`  
		Last Modified: Fri, 06 May 2022 19:19:49 GMT  
		Size: 5.8 KB (5836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3edd190820fd86aaeb4fc1b7a28d7ff52e776414d3830f1a14d103967b455965`  
		Last Modified: Fri, 06 May 2022 19:19:51 GMT  
		Size: 13.7 MB (13676400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b96fea00470fa7356d42265c310e3940426e4c5572f288e8f7111a03b2fdddc`  
		Last Modified: Fri, 06 May 2022 19:19:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.1-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:813c33aa7f94275843088c57b0e44ea6c190d5296b664d7795f66bf3c3804392
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16056332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ee6ea861df7cd9fff1d948de8590f2bac9f2b90ebea7bc71ef7c7654f2d8d40`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:15:01 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:49:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:49:35 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:49:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:49:42 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:49:42 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:49:42 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:49:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:49:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:49:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:49:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:49:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:49:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:49:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:49:46 GMT
EXPOSE 80
# Fri, 06 May 2022 19:49:46 GMT
EXPOSE 443
# Fri, 06 May 2022 19:49:46 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:49:47 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:49:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b230dd773e10769a2eb3e507260d2470a646efd48a639739ba8852b2915302`  
		Last Modified: Tue, 05 Apr 2022 03:18:10 GMT  
		Size: 291.7 KB (291685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd82040b030d75398d6d6fb1c3d12cc9e25a954a92227895e1e5f7ea54736c20`  
		Last Modified: Fri, 06 May 2022 19:51:07 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583abcfacbc800cc0863a5117f1911222bec7ea3fcaed7c36ce4b94b489c3b3e`  
		Last Modified: Fri, 06 May 2022 19:51:16 GMT  
		Size: 13.1 MB (13136691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6903af22655a77183d11fb6d870f6ebc4776e6d9222e9de261b0a377cb81bbcf`  
		Last Modified: Fri, 06 May 2022 19:51:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.1-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:2e61a3ed70ad9a4784ff95cf49efa7ec58255c5263c3faba6a5270a847542a41
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.8 MB (15835582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93c6db987e0721fcd4f557ec160b55012a73d2f69de7198fac316514b27ed58f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:33:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:57:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:57:32 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:57:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:57:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:57:39 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:57:39 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:57:40 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:57:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:57:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:57:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:57:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:57:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:57:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:57:42 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:57:43 GMT
EXPOSE 80
# Fri, 06 May 2022 19:57:43 GMT
EXPOSE 443
# Fri, 06 May 2022 19:57:44 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:57:44 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:57:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03203881a2568530a735b6e0e7a40ebb79adedc5193a675807b04eeb92cc6ed1`  
		Last Modified: Tue, 05 Apr 2022 06:35:07 GMT  
		Size: 290.7 KB (290668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507adf96fcab6911303d2b3d14aeb43223c106ee9901b3e31f30668a4dbd5ffb`  
		Last Modified: Fri, 06 May 2022 19:59:02 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23435dc592c99e66d2e9f715136b809e73116ee6725847ed8fd158135e3283be`  
		Last Modified: Fri, 06 May 2022 19:59:11 GMT  
		Size: 13.1 MB (13114610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e55b7a8b43f4fdfecf61cea01ddddc80930ed485d9aafc41c26f84380f858f3`  
		Last Modified: Fri, 06 May 2022 19:59:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.1-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:cda45585c425161575996ee5d954166745d44d39928846423ecdce6b61a9fb4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.5 MB (15523770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:890cdb4fef0cc66aabb117ff1b3e11fb86de5117d28a5b0e64a743efb92c4269`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:12:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:39:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:39:32 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:39:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:39:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:39:37 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:39:38 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:39:39 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:39:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:39:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:39:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:39:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:39:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:39:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:39:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:39:47 GMT
EXPOSE 80
# Fri, 06 May 2022 19:39:48 GMT
EXPOSE 443
# Fri, 06 May 2022 19:39:49 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:39:50 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:39:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83aa37f2341b1e6d98420668c9bc849a47f2c471d159b2303885040bd8d0a92f`  
		Last Modified: Tue, 05 Apr 2022 03:13:38 GMT  
		Size: 291.3 KB (291301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc050d3d6ffb91c2f68db47e3d5f056afad26e465a03ae7e43383df0fc8ad89`  
		Last Modified: Fri, 06 May 2022 19:40:32 GMT  
		Size: 5.8 KB (5753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8adaff0bd78d0b115843dd841c83d1690484b25369e804b1133b838b7ad5ce8f`  
		Last Modified: Fri, 06 May 2022 19:40:35 GMT  
		Size: 12.5 MB (12510086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f703c61da5ec8e48b081aceac2cb64fb25162c2f0ba1ad16a104610b676f50f6`  
		Last Modified: Fri, 06 May 2022 19:40:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.1-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:d1ab9f3165d5b23b9ff5bd4fcb74b3f8bbf834ba34c42c58e496b3d33017ca59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15203958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfbb2004b1ba3aace5176af38455ef6b8328a074388b16b35358d61330ad2658`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:08:34 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:16:53 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:16:58 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:17:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:17:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:17:25 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:17:32 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:17:36 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:17:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:17:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:17:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:17:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:17:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:18:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:18:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:18:13 GMT
EXPOSE 80
# Fri, 06 May 2022 19:18:17 GMT
EXPOSE 443
# Fri, 06 May 2022 19:18:19 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:18:22 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:18:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743509d6ced044a369685ebb068417e8757981a39d1b397c7b0182ab89f83528`  
		Last Modified: Tue, 05 Apr 2022 07:11:24 GMT  
		Size: 293.7 KB (293721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b659dd8890d066269209696348c58ed19351199266936a5e81f1991a52333d1`  
		Last Modified: Fri, 06 May 2022 19:19:31 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86272ae554176010d052c51dcc5540948b8e59082743b04ac5bb67d05c3fdcd`  
		Last Modified: Fri, 06 May 2022 19:19:33 GMT  
		Size: 12.1 MB (12093067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff57ff409904cc43937df14c68e6d97e1269adde095e91671fb5438dc58a1808`  
		Last Modified: Fri, 06 May 2022 19:19:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.1-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:fbee089e769bc54babbe3ac3217c0e5b60c4a5157b76b0f37aa73cc71486c8fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16129299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f94fa793c943e1cb1c5bda77b0e7077b344648635da2222a1061307e3e61ca96`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:19:41 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:41:25 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:41:25 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:41:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:41:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:41:28 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:41:28 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:41:28 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:41:29 GMT
EXPOSE 80
# Fri, 06 May 2022 19:41:29 GMT
EXPOSE 443
# Fri, 06 May 2022 19:41:30 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:41:30 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:41:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8cc7c7c7ffd67f5740add448d341753330a2abdc6ed06e995cb7d28de381ab`  
		Last Modified: Tue, 05 Apr 2022 06:20:44 GMT  
		Size: 291.8 KB (291821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3d2fae470dbad90c4c4c1262110f14447a47b6e81edc4e0e80ceb50538fe57`  
		Last Modified: Fri, 06 May 2022 19:42:10 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a8f9dbbf38ad9456666a4e6a3eda871b385d4ef76ab6dc25e31030d1daf71c`  
		Last Modified: Fri, 06 May 2022 19:42:12 GMT  
		Size: 13.2 MB (13231118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf07e991258bc58c5e8a5785f741bc746e75848423d2c27d26448015c5887f1`  
		Last Modified: Fri, 06 May 2022 19:42:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.1-builder`

```console
$ docker pull caddy@sha256:81fcae6c8754b60a6694fa9de78ad16f624bf2746f50e224dbd447d197597ae5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2928; amd64
	-	windows version 10.0.20348.707; amd64

### `caddy:2.5.1-builder` - linux; amd64

```console
$ docker pull caddy@sha256:1e292f2e17935f1d904222aa4291d4b4f0a3f48ddd2c73af04039226c812d84b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126492209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c80070b3eb6003cffb12fd895325316a7ad91a7f7116a69ce3970897ef0742d3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:19:44 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:19:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:19:45 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:20:38 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:22:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 22:22:12 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:22:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:22:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:22:13 GMT
WORKDIR /go
# Wed, 01 Jun 2022 22:49:16 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 22:49:16 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 22:49:16 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 22:49:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 22:49:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 22:49:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 22:49:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea60b727a1ce729d031ec1e4f2521a246e71bdb72d3fd9c9c04711cce80e1722`  
		Last Modified: Wed, 25 May 2022 00:24:05 GMT  
		Size: 271.8 KB (271822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c4a77219572e69864cd3069b7b47e55202681be151bd7394f9cb6645b5687b`  
		Last Modified: Wed, 25 May 2022 00:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370296b7ddb629fff1cc98d8d390acf0782fdb8f55cf4054637f6127bbcfe2a9`  
		Last Modified: Wed, 01 Jun 2022 22:30:44 GMT  
		Size: 115.2 MB (115199527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6cee850709034cc7b53152e226caba834fdeb704dab0621f1813bc9081173c`  
		Last Modified: Wed, 01 Jun 2022 22:30:29 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1136d32ff848474c9a359e03d2fcc678a7b8f0dc7e73222ae72e60f7fd4d74`  
		Last Modified: Wed, 01 Jun 2022 22:49:37 GMT  
		Size: 6.9 MB (6931847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c29192c5c8d89201d847a27e2e77e0c4e47f3cef0219cb077dcd8b5bdd9fe1`  
		Last Modified: Wed, 01 Jun 2022 22:49:36 GMT  
		Size: 1.3 MB (1289410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865185451556d5e92a06e01ff04ae2d479a7ff41a4cef4d7f3e27cdb3d0a559e`  
		Last Modified: Wed, 01 Jun 2022 22:49:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.1-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:7de3187171d024e8352c7d65d8c0f7264ecba7b1a0f704295fd611019cb3570f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.5 MB (122503603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d3ac773c95b35b7b4dbac45428257530fdef319e97ee68be2648997c9e4bcd5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:49:39 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:49:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:51:15 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:55:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 22:55:14 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:55:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:55:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:55:16 GMT
WORKDIR /go
# Wed, 01 Jun 2022 23:30:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 23:30:47 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 23:30:48 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 23:30:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 23:30:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 23:30:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 23:30:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6c67ddc305b7f97a531083e369316343b3d19da2352e4e3274db751bba38e2`  
		Last Modified: Wed, 25 May 2022 00:59:27 GMT  
		Size: 272.0 KB (272047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8a37c8e9266706ee6b9ca75c42931dfe1320723ad6a20f0ad4c97554998348`  
		Last Modified: Wed, 25 May 2022 00:59:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d540be111b8c098590378841899d81bec5b744ccbd9ab573bc9b5101566901c`  
		Last Modified: Wed, 01 Jun 2022 23:09:53 GMT  
		Size: 111.6 MB (111598618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cafdd66ccebe1705fc4faa98039c9de106fbcbe091c52f158673fe04e82f802e`  
		Last Modified: Wed, 01 Jun 2022 23:08:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96872e0a675044607ec984baa827068687c978aa91bb47e3f49960519818427`  
		Last Modified: Wed, 01 Jun 2022 23:31:59 GMT  
		Size: 6.8 MB (6796920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3293e1352a64f4c075b505e4c5b86af54f57290c7d7f30c7881824677027cc2`  
		Last Modified: Wed, 01 Jun 2022 23:31:56 GMT  
		Size: 1.2 MB (1229160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4753da45404db22fc7c2a859da39a898b3708ecbfc5cfea606ee7431d28666e4`  
		Last Modified: Wed, 01 Jun 2022 23:31:55 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.1-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:011ac9678dff1b4c8b7b55ed5e314c4cff6da6b30703063ebd229e6b72d63cd6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121343857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48dd50101a28b86b1db7401d9cb0cf460f9f9e9a5543d3b3abe69cf3a4290028`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 03:51:19 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 03:51:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 03:51:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 23:01:24 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 23:05:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 23:05:24 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 23:05:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 23:05:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 23:05:28 GMT
WORKDIR /go
# Wed, 01 Jun 2022 23:54:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 23:54:05 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 23:54:05 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 23:54:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 23:54:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 23:54:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 23:54:09 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e4e5a89e8a0366f9710ba7cb04de284f11234b8cb3dba3e69e35a76dd1c62`  
		Last Modified: Wed, 25 May 2022 04:03:05 GMT  
		Size: 271.0 KB (270972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3b879ada9b059c6167f45b720f44118516dfc73e29b727218447700619fbc5`  
		Last Modified: Wed, 25 May 2022 04:03:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fc48eab20f513149fdf3afa2d29409fae14ca579ba77b44d39b1c7d30bd160`  
		Last Modified: Wed, 01 Jun 2022 23:29:17 GMT  
		Size: 111.4 MB (111376293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4611066e57bc80a36e6249e8637f907272e5888e39790c2360619a7e0cba4833`  
		Last Modified: Wed, 01 Jun 2022 23:28:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65e673e15769cdf43d8d431796fdce20817845053df123db32c4d1ebb097dda`  
		Last Modified: Wed, 01 Jun 2022 23:55:15 GMT  
		Size: 6.1 MB (6056216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f57b87d4f5a15b224a843782ea88621460db848ce77a22ea9556319c9e5c0c`  
		Last Modified: Wed, 01 Jun 2022 23:55:13 GMT  
		Size: 1.2 MB (1228015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a540258c6d4d9ec99d0f270d7f398f2a784a811119862c84d641faf27d9d52f`  
		Last Modified: Wed, 01 Jun 2022 23:55:12 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.1-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:499ea69b717472a063a52ae5197f6deb99d1b2bf52f6ffe632ae6ee4b151e8d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121425869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8397cebecc3630e1971e7a6391326e81bf1f7987dad0cd00d290554058a8e96`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:40:10 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:40:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:40:12 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:41:13 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:43:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 22:43:14 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:43:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:43:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:43:16 GMT
WORKDIR /go
# Wed, 01 Jun 2022 23:12:50 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 23:12:51 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 23:12:51 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 23:12:52 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 23:12:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 23:12:56 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 23:12:56 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a3192eca97ce26527d2bdbb26d1130abcc1c9dd7b800ce2fd14619fa422640`  
		Last Modified: Wed, 25 May 2022 00:45:29 GMT  
		Size: 271.7 KB (271711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a050256f5b6fc0800b8ae0d96e136745091c36ce8e53ba74d8ab3eed65966a59`  
		Last Modified: Wed, 25 May 2022 00:45:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656be50a0ddc84123afb23ccbb17811b43648fa17b4c8664716e9e07553c8b35`  
		Last Modified: Wed, 01 Jun 2022 22:54:01 GMT  
		Size: 110.2 MB (110233232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbca73fdf42200f09770a4826a8cc1004903cd4e9005eff055c63246812a376`  
		Last Modified: Wed, 01 Jun 2022 22:53:46 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab89aed908fe45f53da57dfae1a8b8c6cd86095ae16ff74114042f8a979f1932`  
		Last Modified: Wed, 01 Jun 2022 23:13:30 GMT  
		Size: 7.0 MB (7036774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb64d47dd3ed3c1225ae6e128fbf6d24fcc3c845ef16f462a471531f409af29`  
		Last Modified: Wed, 01 Jun 2022 23:13:29 GMT  
		Size: 1.2 MB (1189006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9128167bb5002c5f6502cafb32b7004c893d437d65d07a486683d6a4827295`  
		Last Modified: Wed, 01 Jun 2022 23:13:28 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.1-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:51489e35e697983a57f901922b0dabd40e875688ab29307b905d29ce55fbaab9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121929763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ab8036b8f55aab1eb0d1627d8569e7b7b92390a17e595ffaf9dfe82da24529`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:17:40 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:17:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:17:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 May 2022 00:18:07 GMT
ENV GOLANG_VERSION=1.18.2
# Wed, 25 May 2022 00:21:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 25 May 2022 00:21:40 GMT
ENV GOPATH=/go
# Wed, 25 May 2022 00:21:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 May 2022 00:21:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 25 May 2022 00:21:58 GMT
WORKDIR /go
# Wed, 25 May 2022 00:45:35 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 25 May 2022 00:45:39 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 25 May 2022 00:45:43 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 25 May 2022 00:45:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 25 May 2022 00:45:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 25 May 2022 00:45:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 25 May 2022 00:46:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211c1f83aeafafff903bb460e7e24594fe138ebceeb1b56e898cf0158ea3daaf`  
		Last Modified: Wed, 25 May 2022 00:27:59 GMT  
		Size: 274.2 KB (274180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8365966bf1e6bd302f9e7c3d8e027aef3cfab1652ed22b8bd53311ef9517f0d3`  
		Last Modified: Wed, 25 May 2022 00:27:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6a047513e9ca46258b5a80c34d0bb9eef5b7e2c8004c5ddd1ca930e7c33659`  
		Last Modified: Wed, 25 May 2022 00:28:25 GMT  
		Size: 110.2 MB (110219016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4216cfe6259a3cf57000a58c453b0ffda2da2dd8b841017c33f4f9e33c8fa5da`  
		Last Modified: Wed, 25 May 2022 00:27:58 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2f4bee20e80c6473651d3ce23e74677476c7b12c9aa9bb880a3b819b0137d9`  
		Last Modified: Wed, 25 May 2022 00:46:38 GMT  
		Size: 7.5 MB (7469747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e99268d0161e857b0995380335a9c16bad6eaad709fc33fe99363301fc93c28`  
		Last Modified: Wed, 25 May 2022 00:46:38 GMT  
		Size: 1.2 MB (1176359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fa65f829c67a09aeb16d10c849ef12dcac7f86668154a677c8caa2bcc02c49`  
		Last Modified: Wed, 25 May 2022 00:46:37 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.1-builder` - linux; s390x

```console
$ docker pull caddy@sha256:2999d8fa276be8936078596794d15be8b708720ee296803ac88d976675f8b84a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124255828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc7070a321e5a4b1b7616b221cf9a73591e4fc00c310bfaad9825483eb4eb0d8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:41:57 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:41:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:41:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:43:25 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:45:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 22:46:11 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:46:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:46:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:46:13 GMT
WORKDIR /go
# Wed, 01 Jun 2022 23:16:35 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 23:16:36 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 23:16:37 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 23:16:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 23:16:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 23:16:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 23:16:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e497ff1a375465e6a6ba78259a6f2e9f7986cf27789ba79ddfd1cca023a160`  
		Last Modified: Wed, 25 May 2022 00:50:39 GMT  
		Size: 272.2 KB (272155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e413365aa9b9c967651e3a27f41641db43d81f24ff58ea4de0ce2c662c5d5f`  
		Last Modified: Wed, 25 May 2022 00:50:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e76ee5124cc2e0e213f5fc781375c53acc53fda6cb50eb09ce717d9ce4626ce`  
		Last Modified: Wed, 01 Jun 2022 22:58:35 GMT  
		Size: 113.1 MB (113111409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43db1e7eb380ed189bd16b98ad5afb071c88b789a987c6d8c2dd65dc4bfbf16d`  
		Last Modified: Wed, 01 Jun 2022 22:58:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0ade8df88187af31cea8632059bf709714e41aa1f2cf4a4bd3cee7562d3291`  
		Last Modified: Wed, 01 Jun 2022 23:17:26 GMT  
		Size: 7.0 MB (7047929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634c737128f1d3d767c417a20c9a5faaab86feb02d4e7a179046b7da981707f7`  
		Last Modified: Wed, 01 Jun 2022 23:17:25 GMT  
		Size: 1.2 MB (1243129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d94f95e9c108ec4db470dfbacda85ff19601a76bcfb7c7328b26c4fa4b09b9`  
		Last Modified: Wed, 01 Jun 2022 23:17:25 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.1-builder` - windows version 10.0.17763.2928; amd64

```console
$ docker pull caddy@sha256:9ccfa9fc4fc4236cf295417a18c7d16b0a79495b916cd1b95c231e18daed3423
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2674256754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e7531282f56b1596b6475bd16a7058aaa9dc1e6884e7902f556e23b3eccf951`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 22:21:43 GMT
ENV GIT_VERSION=2.23.0
# Tue, 10 May 2022 22:21:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 10 May 2022 22:21:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 10 May 2022 22:21:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 10 May 2022 22:23:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:23:36 GMT
ENV GOPATH=C:\go
# Tue, 10 May 2022 22:24:28 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 10 May 2022 22:40:47 GMT
ENV GOLANG_VERSION=1.17.10
# Tue, 10 May 2022 22:44:40 GMT
RUN $url = 'https://dl.google.com/go/go1.17.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ba9198a29fa5c4f322212d21569e8507165c3b34e1ed1f1f9cf6dfb71ddcdeb2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:44:47 GMT
WORKDIR C:\go
# Tue, 10 May 2022 23:33:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:33:03 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 10 May 2022 23:33:04 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:33:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 10 May 2022 23:34:01 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 10 May 2022 23:34:02 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01012ab52f3f9693dd4b85e6e19a0b2659b4f869d6b5b5d2ea62afe84c9037c`  
		Last Modified: Tue, 10 May 2022 22:55:50 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988abb6e02c6ab2eb0330641b6378c4e110c132c761de086dfc1629462491e90`  
		Last Modified: Tue, 10 May 2022 22:55:48 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b62ac07a4cd6e0fd762f7f6e904be7b001affa78e8fbfeb8ca017a6f643d62c`  
		Last Modified: Tue, 10 May 2022 22:55:47 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e235721feec6368d5a652fd467681dffe74326d42da4bed8e43f777bc39c47`  
		Last Modified: Tue, 10 May 2022 22:55:47 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8195b6f87245387233358bc8fcc2679a23d9aa46cd4bfef94ac49284694c5c42`  
		Last Modified: Tue, 10 May 2022 22:56:13 GMT  
		Size: 25.6 MB (25580295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cfe0249f2fac54d31ea467ce63bdc69e4504b726a87d969fb1b42ab2ab3853`  
		Last Modified: Tue, 10 May 2022 22:55:45 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c97dcc9056ac36ad6120d94049a937f5366e71fda7c478ff3462d542cc0645`  
		Last Modified: Tue, 10 May 2022 22:55:45 GMT  
		Size: 322.0 KB (321981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4753086b1ed8db6655e0993e3f676d7f71455415cce16cd5593b330f9a89b3a`  
		Last Modified: Tue, 10 May 2022 23:05:04 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66134c7f83737bd3064ea2c3dce37ea0157cde99b46bbf80744100fd7f18a0aa`  
		Last Modified: Tue, 10 May 2022 23:07:31 GMT  
		Size: 142.6 MB (142588622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0697a4af489e787e5def466bbf9614e20bf5b1cea211f3a8f8ce2f0b5a10a3f`  
		Last Modified: Tue, 10 May 2022 23:05:04 GMT  
		Size: 1.6 KB (1566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c242b44aab0e82a2f6bf16213c350b73347e55ad15ecafa05877414e1327e96b`  
		Last Modified: Tue, 10 May 2022 23:36:29 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223dbf32ed9ac3b13af8e1196395df286392aa610ec5ba0bf809061dbf84a5cb`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a255b634df668adc897872554f8b720fdd5e6f4a9c47db0bbc489d25a0aaa66e`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe18292f9995b50f39e6e8ef4cfa31d2913132bef8804b56e260a907b205cd18`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168a524248b6a67f943614b53e6a0825bd107c0b90796733fccfe1184d013a45`  
		Last Modified: Tue, 10 May 2022 23:36:28 GMT  
		Size: 1.7 MB (1691907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4398dd61eb69a257d8e25ec572462f611d347efd5e30a944117a652f47314944`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.1-builder` - windows version 10.0.20348.707; amd64

```console
$ docker pull caddy@sha256:5577ab08abcc0385dd65f73089851d37eb4cd88a29a3cd1d511c6c526221fc42
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2415395050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8e125146193f9e2329bf6ce618db8d09adc336b804bec5cd23b54463959d504`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 22:16:59 GMT
ENV GIT_VERSION=2.23.0
# Tue, 10 May 2022 22:17:00 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 10 May 2022 22:17:01 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 10 May 2022 22:17:02 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 10 May 2022 22:17:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:17:52 GMT
ENV GOPATH=C:\go
# Tue, 10 May 2022 22:18:24 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 10 May 2022 22:18:25 GMT
ENV GOLANG_VERSION=1.18.2
# Tue, 10 May 2022 22:21:20 GMT
RUN $url = 'https://dl.google.com/go/go1.18.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '41fc44109c39a98e0c3672989ac5ad205cbb5768067e099dc4fb2b75cba922cf'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:21:26 GMT
WORKDIR C:\go
# Tue, 10 May 2022 23:34:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:34:18 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 10 May 2022 23:34:19 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:34:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 10 May 2022 23:34:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 10 May 2022 23:34:53 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb2ee3c21cb72c263da0dc4c6080f1d34c7ce3c7f24dcce76815784ec99440f`  
		Last Modified: Tue, 10 May 2022 22:52:57 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db422a46fd25683fe2e5990dc5db827b96c7b135679867ac162c2a318803463`  
		Last Modified: Tue, 10 May 2022 22:52:56 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4110a58975fa9bc64fa3a7d64804d47aa9ba813231538466dfedf4c35658cae7`  
		Last Modified: Tue, 10 May 2022 22:52:55 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e110f1696433dc412066aa30ea4222e641d7d377d593568f539b471b865a664`  
		Last Modified: Tue, 10 May 2022 22:52:55 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aca2a7cb069b5fd7ea06af17cd99249cae08f77d945258e72108af23fb4570a`  
		Last Modified: Tue, 10 May 2022 22:53:21 GMT  
		Size: 25.7 MB (25692112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc78480e80903590627dacfc79a3c978709b8c787cc193391852c4f8bf2ffca`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f488db75670938176d831a4bc8ddd4bb629e7a61e9ce5101882db134c0d162`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 541.2 KB (541163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7e0fbd217082bd92c424bbe5de58f546b38e43068d1f7b3a1121e42ffcbac6`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d268be7c91150b1073b85f55a434b87a1602a325ad6af8f2c2896f34f83388`  
		Last Modified: Tue, 10 May 2022 22:55:29 GMT  
		Size: 149.7 MB (149697865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3786f32f80e906fe1e08346c7294bfcfaa5d640b7c8cd920c91fb3b33f8bb6e4`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 1.5 KB (1536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd4f585b833fb8fb9f417326d46999e8726e1aa94e3796e9005a10daf16e12d`  
		Last Modified: Tue, 10 May 2022 23:36:48 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707272d91e9f672f1fe7a0de3ecaeefc72c1d00ee1025438e7cfb0dc74a77ee2`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a90464121b8d7fd8edb1f37124b634fe69680d1b4af3a6b853417ab05e9243a0`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20695dc76bb11cb698c1e429bbcb5e3011dfd00666a09a81c2cbd4f4607b1da`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884b6dd02ff92d7127e63601c97c036dee9230f73ecfe1d2d382466b705e9836`  
		Last Modified: Tue, 10 May 2022 23:36:46 GMT  
		Size: 1.9 MB (1910625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f0345f50b887c52e7c023a68e29e1332dac19143806fc334ea4d6e9a2cb0d5`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.1-builder-alpine`

```console
$ docker pull caddy@sha256:ffbabc549906ee81026a50566ab1b254cafdafcc6e43c09abcc61fde1d323146
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.5.1-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:1e292f2e17935f1d904222aa4291d4b4f0a3f48ddd2c73af04039226c812d84b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126492209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c80070b3eb6003cffb12fd895325316a7ad91a7f7116a69ce3970897ef0742d3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:19:44 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:19:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:19:45 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:20:38 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:22:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 22:22:12 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:22:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:22:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:22:13 GMT
WORKDIR /go
# Wed, 01 Jun 2022 22:49:16 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 22:49:16 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 22:49:16 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 22:49:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 22:49:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 22:49:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 22:49:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea60b727a1ce729d031ec1e4f2521a246e71bdb72d3fd9c9c04711cce80e1722`  
		Last Modified: Wed, 25 May 2022 00:24:05 GMT  
		Size: 271.8 KB (271822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c4a77219572e69864cd3069b7b47e55202681be151bd7394f9cb6645b5687b`  
		Last Modified: Wed, 25 May 2022 00:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370296b7ddb629fff1cc98d8d390acf0782fdb8f55cf4054637f6127bbcfe2a9`  
		Last Modified: Wed, 01 Jun 2022 22:30:44 GMT  
		Size: 115.2 MB (115199527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6cee850709034cc7b53152e226caba834fdeb704dab0621f1813bc9081173c`  
		Last Modified: Wed, 01 Jun 2022 22:30:29 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1136d32ff848474c9a359e03d2fcc678a7b8f0dc7e73222ae72e60f7fd4d74`  
		Last Modified: Wed, 01 Jun 2022 22:49:37 GMT  
		Size: 6.9 MB (6931847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c29192c5c8d89201d847a27e2e77e0c4e47f3cef0219cb077dcd8b5bdd9fe1`  
		Last Modified: Wed, 01 Jun 2022 22:49:36 GMT  
		Size: 1.3 MB (1289410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865185451556d5e92a06e01ff04ae2d479a7ff41a4cef4d7f3e27cdb3d0a559e`  
		Last Modified: Wed, 01 Jun 2022 22:49:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.1-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:7de3187171d024e8352c7d65d8c0f7264ecba7b1a0f704295fd611019cb3570f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.5 MB (122503603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d3ac773c95b35b7b4dbac45428257530fdef319e97ee68be2648997c9e4bcd5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:49:39 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:49:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:51:15 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:55:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 22:55:14 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:55:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:55:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:55:16 GMT
WORKDIR /go
# Wed, 01 Jun 2022 23:30:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 23:30:47 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 23:30:48 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 23:30:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 23:30:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 23:30:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 23:30:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6c67ddc305b7f97a531083e369316343b3d19da2352e4e3274db751bba38e2`  
		Last Modified: Wed, 25 May 2022 00:59:27 GMT  
		Size: 272.0 KB (272047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8a37c8e9266706ee6b9ca75c42931dfe1320723ad6a20f0ad4c97554998348`  
		Last Modified: Wed, 25 May 2022 00:59:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d540be111b8c098590378841899d81bec5b744ccbd9ab573bc9b5101566901c`  
		Last Modified: Wed, 01 Jun 2022 23:09:53 GMT  
		Size: 111.6 MB (111598618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cafdd66ccebe1705fc4faa98039c9de106fbcbe091c52f158673fe04e82f802e`  
		Last Modified: Wed, 01 Jun 2022 23:08:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96872e0a675044607ec984baa827068687c978aa91bb47e3f49960519818427`  
		Last Modified: Wed, 01 Jun 2022 23:31:59 GMT  
		Size: 6.8 MB (6796920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3293e1352a64f4c075b505e4c5b86af54f57290c7d7f30c7881824677027cc2`  
		Last Modified: Wed, 01 Jun 2022 23:31:56 GMT  
		Size: 1.2 MB (1229160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4753da45404db22fc7c2a859da39a898b3708ecbfc5cfea606ee7431d28666e4`  
		Last Modified: Wed, 01 Jun 2022 23:31:55 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.1-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:011ac9678dff1b4c8b7b55ed5e314c4cff6da6b30703063ebd229e6b72d63cd6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121343857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48dd50101a28b86b1db7401d9cb0cf460f9f9e9a5543d3b3abe69cf3a4290028`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 03:51:19 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 03:51:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 03:51:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 23:01:24 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 23:05:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 23:05:24 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 23:05:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 23:05:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 23:05:28 GMT
WORKDIR /go
# Wed, 01 Jun 2022 23:54:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 23:54:05 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 23:54:05 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 23:54:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 23:54:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 23:54:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 23:54:09 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e4e5a89e8a0366f9710ba7cb04de284f11234b8cb3dba3e69e35a76dd1c62`  
		Last Modified: Wed, 25 May 2022 04:03:05 GMT  
		Size: 271.0 KB (270972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3b879ada9b059c6167f45b720f44118516dfc73e29b727218447700619fbc5`  
		Last Modified: Wed, 25 May 2022 04:03:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fc48eab20f513149fdf3afa2d29409fae14ca579ba77b44d39b1c7d30bd160`  
		Last Modified: Wed, 01 Jun 2022 23:29:17 GMT  
		Size: 111.4 MB (111376293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4611066e57bc80a36e6249e8637f907272e5888e39790c2360619a7e0cba4833`  
		Last Modified: Wed, 01 Jun 2022 23:28:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65e673e15769cdf43d8d431796fdce20817845053df123db32c4d1ebb097dda`  
		Last Modified: Wed, 01 Jun 2022 23:55:15 GMT  
		Size: 6.1 MB (6056216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f57b87d4f5a15b224a843782ea88621460db848ce77a22ea9556319c9e5c0c`  
		Last Modified: Wed, 01 Jun 2022 23:55:13 GMT  
		Size: 1.2 MB (1228015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a540258c6d4d9ec99d0f270d7f398f2a784a811119862c84d641faf27d9d52f`  
		Last Modified: Wed, 01 Jun 2022 23:55:12 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.1-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:499ea69b717472a063a52ae5197f6deb99d1b2bf52f6ffe632ae6ee4b151e8d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121425869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8397cebecc3630e1971e7a6391326e81bf1f7987dad0cd00d290554058a8e96`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:40:10 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:40:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:40:12 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:41:13 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:43:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 22:43:14 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:43:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:43:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:43:16 GMT
WORKDIR /go
# Wed, 01 Jun 2022 23:12:50 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 23:12:51 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 23:12:51 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 23:12:52 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 23:12:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 23:12:56 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 23:12:56 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a3192eca97ce26527d2bdbb26d1130abcc1c9dd7b800ce2fd14619fa422640`  
		Last Modified: Wed, 25 May 2022 00:45:29 GMT  
		Size: 271.7 KB (271711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a050256f5b6fc0800b8ae0d96e136745091c36ce8e53ba74d8ab3eed65966a59`  
		Last Modified: Wed, 25 May 2022 00:45:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656be50a0ddc84123afb23ccbb17811b43648fa17b4c8664716e9e07553c8b35`  
		Last Modified: Wed, 01 Jun 2022 22:54:01 GMT  
		Size: 110.2 MB (110233232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbca73fdf42200f09770a4826a8cc1004903cd4e9005eff055c63246812a376`  
		Last Modified: Wed, 01 Jun 2022 22:53:46 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab89aed908fe45f53da57dfae1a8b8c6cd86095ae16ff74114042f8a979f1932`  
		Last Modified: Wed, 01 Jun 2022 23:13:30 GMT  
		Size: 7.0 MB (7036774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb64d47dd3ed3c1225ae6e128fbf6d24fcc3c845ef16f462a471531f409af29`  
		Last Modified: Wed, 01 Jun 2022 23:13:29 GMT  
		Size: 1.2 MB (1189006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9128167bb5002c5f6502cafb32b7004c893d437d65d07a486683d6a4827295`  
		Last Modified: Wed, 01 Jun 2022 23:13:28 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.1-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:51489e35e697983a57f901922b0dabd40e875688ab29307b905d29ce55fbaab9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121929763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ab8036b8f55aab1eb0d1627d8569e7b7b92390a17e595ffaf9dfe82da24529`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:17:40 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:17:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:17:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 May 2022 00:18:07 GMT
ENV GOLANG_VERSION=1.18.2
# Wed, 25 May 2022 00:21:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 25 May 2022 00:21:40 GMT
ENV GOPATH=/go
# Wed, 25 May 2022 00:21:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 May 2022 00:21:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 25 May 2022 00:21:58 GMT
WORKDIR /go
# Wed, 25 May 2022 00:45:35 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 25 May 2022 00:45:39 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 25 May 2022 00:45:43 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 25 May 2022 00:45:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 25 May 2022 00:45:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 25 May 2022 00:45:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 25 May 2022 00:46:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211c1f83aeafafff903bb460e7e24594fe138ebceeb1b56e898cf0158ea3daaf`  
		Last Modified: Wed, 25 May 2022 00:27:59 GMT  
		Size: 274.2 KB (274180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8365966bf1e6bd302f9e7c3d8e027aef3cfab1652ed22b8bd53311ef9517f0d3`  
		Last Modified: Wed, 25 May 2022 00:27:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6a047513e9ca46258b5a80c34d0bb9eef5b7e2c8004c5ddd1ca930e7c33659`  
		Last Modified: Wed, 25 May 2022 00:28:25 GMT  
		Size: 110.2 MB (110219016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4216cfe6259a3cf57000a58c453b0ffda2da2dd8b841017c33f4f9e33c8fa5da`  
		Last Modified: Wed, 25 May 2022 00:27:58 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2f4bee20e80c6473651d3ce23e74677476c7b12c9aa9bb880a3b819b0137d9`  
		Last Modified: Wed, 25 May 2022 00:46:38 GMT  
		Size: 7.5 MB (7469747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e99268d0161e857b0995380335a9c16bad6eaad709fc33fe99363301fc93c28`  
		Last Modified: Wed, 25 May 2022 00:46:38 GMT  
		Size: 1.2 MB (1176359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fa65f829c67a09aeb16d10c849ef12dcac7f86668154a677c8caa2bcc02c49`  
		Last Modified: Wed, 25 May 2022 00:46:37 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.1-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:2999d8fa276be8936078596794d15be8b708720ee296803ac88d976675f8b84a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124255828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc7070a321e5a4b1b7616b221cf9a73591e4fc00c310bfaad9825483eb4eb0d8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:41:57 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:41:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:41:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:43:25 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:45:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 22:46:11 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:46:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:46:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:46:13 GMT
WORKDIR /go
# Wed, 01 Jun 2022 23:16:35 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 23:16:36 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 23:16:37 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 23:16:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 23:16:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 23:16:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 23:16:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e497ff1a375465e6a6ba78259a6f2e9f7986cf27789ba79ddfd1cca023a160`  
		Last Modified: Wed, 25 May 2022 00:50:39 GMT  
		Size: 272.2 KB (272155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e413365aa9b9c967651e3a27f41641db43d81f24ff58ea4de0ce2c662c5d5f`  
		Last Modified: Wed, 25 May 2022 00:50:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e76ee5124cc2e0e213f5fc781375c53acc53fda6cb50eb09ce717d9ce4626ce`  
		Last Modified: Wed, 01 Jun 2022 22:58:35 GMT  
		Size: 113.1 MB (113111409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43db1e7eb380ed189bd16b98ad5afb071c88b789a987c6d8c2dd65dc4bfbf16d`  
		Last Modified: Wed, 01 Jun 2022 22:58:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0ade8df88187af31cea8632059bf709714e41aa1f2cf4a4bd3cee7562d3291`  
		Last Modified: Wed, 01 Jun 2022 23:17:26 GMT  
		Size: 7.0 MB (7047929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634c737128f1d3d767c417a20c9a5faaab86feb02d4e7a179046b7da981707f7`  
		Last Modified: Wed, 01 Jun 2022 23:17:25 GMT  
		Size: 1.2 MB (1243129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d94f95e9c108ec4db470dfbacda85ff19601a76bcfb7c7328b26c4fa4b09b9`  
		Last Modified: Wed, 01 Jun 2022 23:17:25 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.1-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:80ca8f74f642d7218cc111d5ea59115a305c4cd6030325cb4c4a7fad93d4c5a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `caddy:2.5.1-builder-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull caddy@sha256:9ccfa9fc4fc4236cf295417a18c7d16b0a79495b916cd1b95c231e18daed3423
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2674256754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e7531282f56b1596b6475bd16a7058aaa9dc1e6884e7902f556e23b3eccf951`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 22:21:43 GMT
ENV GIT_VERSION=2.23.0
# Tue, 10 May 2022 22:21:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 10 May 2022 22:21:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 10 May 2022 22:21:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 10 May 2022 22:23:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:23:36 GMT
ENV GOPATH=C:\go
# Tue, 10 May 2022 22:24:28 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 10 May 2022 22:40:47 GMT
ENV GOLANG_VERSION=1.17.10
# Tue, 10 May 2022 22:44:40 GMT
RUN $url = 'https://dl.google.com/go/go1.17.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ba9198a29fa5c4f322212d21569e8507165c3b34e1ed1f1f9cf6dfb71ddcdeb2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:44:47 GMT
WORKDIR C:\go
# Tue, 10 May 2022 23:33:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:33:03 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 10 May 2022 23:33:04 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:33:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 10 May 2022 23:34:01 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 10 May 2022 23:34:02 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01012ab52f3f9693dd4b85e6e19a0b2659b4f869d6b5b5d2ea62afe84c9037c`  
		Last Modified: Tue, 10 May 2022 22:55:50 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988abb6e02c6ab2eb0330641b6378c4e110c132c761de086dfc1629462491e90`  
		Last Modified: Tue, 10 May 2022 22:55:48 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b62ac07a4cd6e0fd762f7f6e904be7b001affa78e8fbfeb8ca017a6f643d62c`  
		Last Modified: Tue, 10 May 2022 22:55:47 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e235721feec6368d5a652fd467681dffe74326d42da4bed8e43f777bc39c47`  
		Last Modified: Tue, 10 May 2022 22:55:47 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8195b6f87245387233358bc8fcc2679a23d9aa46cd4bfef94ac49284694c5c42`  
		Last Modified: Tue, 10 May 2022 22:56:13 GMT  
		Size: 25.6 MB (25580295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cfe0249f2fac54d31ea467ce63bdc69e4504b726a87d969fb1b42ab2ab3853`  
		Last Modified: Tue, 10 May 2022 22:55:45 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c97dcc9056ac36ad6120d94049a937f5366e71fda7c478ff3462d542cc0645`  
		Last Modified: Tue, 10 May 2022 22:55:45 GMT  
		Size: 322.0 KB (321981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4753086b1ed8db6655e0993e3f676d7f71455415cce16cd5593b330f9a89b3a`  
		Last Modified: Tue, 10 May 2022 23:05:04 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66134c7f83737bd3064ea2c3dce37ea0157cde99b46bbf80744100fd7f18a0aa`  
		Last Modified: Tue, 10 May 2022 23:07:31 GMT  
		Size: 142.6 MB (142588622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0697a4af489e787e5def466bbf9614e20bf5b1cea211f3a8f8ce2f0b5a10a3f`  
		Last Modified: Tue, 10 May 2022 23:05:04 GMT  
		Size: 1.6 KB (1566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c242b44aab0e82a2f6bf16213c350b73347e55ad15ecafa05877414e1327e96b`  
		Last Modified: Tue, 10 May 2022 23:36:29 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223dbf32ed9ac3b13af8e1196395df286392aa610ec5ba0bf809061dbf84a5cb`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a255b634df668adc897872554f8b720fdd5e6f4a9c47db0bbc489d25a0aaa66e`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe18292f9995b50f39e6e8ef4cfa31d2913132bef8804b56e260a907b205cd18`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168a524248b6a67f943614b53e6a0825bd107c0b90796733fccfe1184d013a45`  
		Last Modified: Tue, 10 May 2022 23:36:28 GMT  
		Size: 1.7 MB (1691907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4398dd61eb69a257d8e25ec572462f611d347efd5e30a944117a652f47314944`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.1-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:f5f71b248dea482aed03fe1e9ffdbd84e3e337044b6e4263956c9e8069ff8da2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `caddy:2.5.1-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.707; amd64

```console
$ docker pull caddy@sha256:5577ab08abcc0385dd65f73089851d37eb4cd88a29a3cd1d511c6c526221fc42
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2415395050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8e125146193f9e2329bf6ce618db8d09adc336b804bec5cd23b54463959d504`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 22:16:59 GMT
ENV GIT_VERSION=2.23.0
# Tue, 10 May 2022 22:17:00 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 10 May 2022 22:17:01 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 10 May 2022 22:17:02 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 10 May 2022 22:17:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:17:52 GMT
ENV GOPATH=C:\go
# Tue, 10 May 2022 22:18:24 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 10 May 2022 22:18:25 GMT
ENV GOLANG_VERSION=1.18.2
# Tue, 10 May 2022 22:21:20 GMT
RUN $url = 'https://dl.google.com/go/go1.18.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '41fc44109c39a98e0c3672989ac5ad205cbb5768067e099dc4fb2b75cba922cf'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:21:26 GMT
WORKDIR C:\go
# Tue, 10 May 2022 23:34:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:34:18 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 10 May 2022 23:34:19 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:34:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 10 May 2022 23:34:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 10 May 2022 23:34:53 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb2ee3c21cb72c263da0dc4c6080f1d34c7ce3c7f24dcce76815784ec99440f`  
		Last Modified: Tue, 10 May 2022 22:52:57 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db422a46fd25683fe2e5990dc5db827b96c7b135679867ac162c2a318803463`  
		Last Modified: Tue, 10 May 2022 22:52:56 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4110a58975fa9bc64fa3a7d64804d47aa9ba813231538466dfedf4c35658cae7`  
		Last Modified: Tue, 10 May 2022 22:52:55 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e110f1696433dc412066aa30ea4222e641d7d377d593568f539b471b865a664`  
		Last Modified: Tue, 10 May 2022 22:52:55 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aca2a7cb069b5fd7ea06af17cd99249cae08f77d945258e72108af23fb4570a`  
		Last Modified: Tue, 10 May 2022 22:53:21 GMT  
		Size: 25.7 MB (25692112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc78480e80903590627dacfc79a3c978709b8c787cc193391852c4f8bf2ffca`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f488db75670938176d831a4bc8ddd4bb629e7a61e9ce5101882db134c0d162`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 541.2 KB (541163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7e0fbd217082bd92c424bbe5de58f546b38e43068d1f7b3a1121e42ffcbac6`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d268be7c91150b1073b85f55a434b87a1602a325ad6af8f2c2896f34f83388`  
		Last Modified: Tue, 10 May 2022 22:55:29 GMT  
		Size: 149.7 MB (149697865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3786f32f80e906fe1e08346c7294bfcfaa5d640b7c8cd920c91fb3b33f8bb6e4`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 1.5 KB (1536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd4f585b833fb8fb9f417326d46999e8726e1aa94e3796e9005a10daf16e12d`  
		Last Modified: Tue, 10 May 2022 23:36:48 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707272d91e9f672f1fe7a0de3ecaeefc72c1d00ee1025438e7cfb0dc74a77ee2`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a90464121b8d7fd8edb1f37124b634fe69680d1b4af3a6b853417ab05e9243a0`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20695dc76bb11cb698c1e429bbcb5e3011dfd00666a09a81c2cbd4f4607b1da`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884b6dd02ff92d7127e63601c97c036dee9230f73ecfe1d2d382466b705e9836`  
		Last Modified: Tue, 10 May 2022 23:36:46 GMT  
		Size: 1.9 MB (1910625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f0345f50b887c52e7c023a68e29e1332dac19143806fc334ea4d6e9a2cb0d5`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.1-windowsservercore`

```console
$ docker pull caddy@sha256:285398d41e72fa7778b741796f7a0892454ea9bdc4ed67b25cec85cd7494f9cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2928; amd64
	-	windows version 10.0.20348.707; amd64

### `caddy:2.5.1-windowsservercore` - windows version 10.0.17763.2928; amd64

```console
$ docker pull caddy@sha256:8ad6979cdadd3d080deeb3a2f13d37c23789748ea80b29ac44624cf39bd589ff
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2518898800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8393d2b14b909a4ce523ae0d4999f2a492deb9e76ac12cc8dc111b5f0e3bd74d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:28:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 10 May 2022 23:28:55 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:29:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('4294796c4bd4bed0c593d83606a5413de30f35f88d624e1b1e5b6cd8672ffbcc7a689d7ce4ef30c1abea0e95eda62220faac15d2a6aca0c3e2b418abe7a74118')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 10 May 2022 23:29:54 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 10 May 2022 23:29:56 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 10 May 2022 23:29:57 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Tue, 10 May 2022 23:29:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 10 May 2022 23:29:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 10 May 2022 23:29:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 10 May 2022 23:30:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 10 May 2022 23:30:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 10 May 2022 23:30:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 10 May 2022 23:30:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 10 May 2022 23:30:04 GMT
EXPOSE 80
# Tue, 10 May 2022 23:30:05 GMT
EXPOSE 443
# Tue, 10 May 2022 23:30:06 GMT
EXPOSE 2019
# Tue, 10 May 2022 23:30:47 GMT
RUN caddy version
# Tue, 10 May 2022 23:30:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d722bd7a5ed597b5a9ed7c5144caa608e784120c4442579352b7c2325ce47ffc`  
		Last Modified: Tue, 10 May 2022 23:35:41 GMT  
		Size: 498.2 KB (498231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0dfede5e37c630a175a1c987d90aaf1ec1db8cd7d43e3d63648743c6ace743`  
		Last Modified: Tue, 10 May 2022 23:35:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef201446c9bd5610f78b8e5a1680047ff45fadb77727762c323d5e48d77f9f2`  
		Last Modified: Tue, 10 May 2022 23:35:44 GMT  
		Size: 14.0 MB (14007489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b824e8abcb45a47ada825f0b722a588cbc9d1f68f5536a76b7afed2c5eb15a0c`  
		Last Modified: Tue, 10 May 2022 23:35:39 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b01057f474e19bdcaebab2c156622642945d2c7074276c82de663baeb418143`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520fb9c4921f60cfaea07cfa8d5733cf7f4f0810e56106911d7b25f59e86e997`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74d9e7abc08a32b35b26f8bba23c597b1e19d604766b326f61e77da0b494285`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595304462c9d3aa03aa9e164a98a38be5e1f5307c2981b65aa228101c73ce91b`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e307ee1571a8185932bbd90267a8b8d367f784859d99a2742d44e89e19e8b6c0`  
		Last Modified: Tue, 10 May 2022 23:35:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b335f1fddf0ed6abcc0e715ff827614cc2f0f4bbe8a0e1565145951d841c96`  
		Last Modified: Tue, 10 May 2022 23:35:36 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0974b9a20e0fa84c8a353a7c04992bec9e06825ed808054a358b84409744ba`  
		Last Modified: Tue, 10 May 2022 23:35:35 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d5086c691961c9f1a18b9d161cf8cb3dbd7b581c68ab75760b8c5e62647928`  
		Last Modified: Tue, 10 May 2022 23:35:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9194a8cf5ac8d920d218d9100152393ac6cce9142b15904894374694ae2d2fc`  
		Last Modified: Tue, 10 May 2022 23:35:36 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd07be490606caadc3893d219aee0682d6f8b71b2a4a8f2fb2ca826cdffb74`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b19beef4c4a6634592447260a670c8ee571e59cb775833787d39b815e9ba511`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2dab7fd2beddb5439029e7d8a75fc7c7fe2d3a534a63f51a04f85dd371cd1c`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e195aa5e2a95379397baf57f681e2c39a7c673d3c06d0ff3e4eeed3d8cecee1`  
		Last Modified: Tue, 10 May 2022 23:35:34 GMT  
		Size: 314.6 KB (314586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87827ca78b495430e19218a9e3f7f2837078a77df34bb929124ea20614287d5`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.1-windowsservercore` - windows version 10.0.20348.707; amd64

```console
$ docker pull caddy@sha256:a3894222673d46b3e350553c6b7d4f92ab27b85a87fa1f773e9b090d5774ca9e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2252723203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:063f1879bd2783934ad3ac23aa37bf45f19be756f6b018f4c3a67d2d4a759c7c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:31:41 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 10 May 2022 23:31:42 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:32:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('4294796c4bd4bed0c593d83606a5413de30f35f88d624e1b1e5b6cd8672ffbcc7a689d7ce4ef30c1abea0e95eda62220faac15d2a6aca0c3e2b418abe7a74118')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 10 May 2022 23:32:11 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 10 May 2022 23:32:12 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 10 May 2022 23:32:13 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Tue, 10 May 2022 23:32:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 10 May 2022 23:32:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 10 May 2022 23:32:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 10 May 2022 23:32:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 10 May 2022 23:32:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 10 May 2022 23:32:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 10 May 2022 23:32:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 10 May 2022 23:32:21 GMT
EXPOSE 80
# Tue, 10 May 2022 23:32:22 GMT
EXPOSE 443
# Tue, 10 May 2022 23:32:23 GMT
EXPOSE 2019
# Tue, 10 May 2022 23:32:42 GMT
RUN caddy version
# Tue, 10 May 2022 23:32:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9baa8a196af04dc55746ee82c0774537bce72a589b75d9efce1a4680f03e35`  
		Last Modified: Tue, 10 May 2022 23:36:04 GMT  
		Size: 616.1 KB (616130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe60c7e90fdaeffa9bce60d9a7c7b340dedc357bfb70a2ce8c6d7b8bd0e74a11`  
		Last Modified: Tue, 10 May 2022 23:36:04 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f955bea173999b55d2087a27b9cc80e92bf168918c6e892175c2a75bdbfac933`  
		Last Modified: Tue, 10 May 2022 23:36:07 GMT  
		Size: 14.2 MB (14224642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e1ab4508d5347b929d5a33f71e0f24f653e61c147260200d32e3bd7cdd2340`  
		Last Modified: Tue, 10 May 2022 23:36:02 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8044ca4427c5edfee653001205397a2cc33f8fb4416c16c4a4936317c572ed`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f144416d38a1aa75558e0b93b88fcb3de122ee88349826ee99d596e1b00d9cc0`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32edbcceba80e7a70e44725926012bb70624bb0ae91c85db2766ca2e4c5a5d7c`  
		Last Modified: Tue, 10 May 2022 23:36:02 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd90105a2a3136e4d25d0add2b6fbe5798d51588215367128f1566d66b255289`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e448ed08c6c6ca9f854cb7014ea2e79c04e83f1905f78f578b67303b709fa3`  
		Last Modified: Tue, 10 May 2022 23:36:00 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d49b1b3778cd2ebf32521f530e29275a9a473afa997654b32338ff4349bf5c`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2112945425b7d069bc5705be1345e5ad6e27206e1531b10d0bc92d9c69ea9c3`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7243327255edd82b277f456085138a672f5a43d616e80f73156c8eb31139121d`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1a14330360d7ab3af40d4fb6f2de975e42e05f8e4cb064cc49fe1d9446e6b1`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808ce6a15ca3e6ad031229bcad8a3ed69171a7005c05ef4e77ffcfd777e9d1f7`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdfcf611e614d42a256d103775233f59ab7bb6ad0b00ca2f915bf739600f8d6`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3811622d464d497ce363eed806c75f9b994cd1d04b3009b2d0671af2863ebd0`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b006092864e6cfdfedd054a2635236c62958e97de81c720d9e38772276ee11`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 325.9 KB (325870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2afb0ece27a359f16126f263176baa74c3d3f2f2733cce186e4e31ad0eca4f8`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.1-windowsservercore-1809`

```console
$ docker pull caddy@sha256:61aa7b1019d479a8c0c21f043ffbec427336684486cad3858e71de43f3962e7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `caddy:2.5.1-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull caddy@sha256:8ad6979cdadd3d080deeb3a2f13d37c23789748ea80b29ac44624cf39bd589ff
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2518898800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8393d2b14b909a4ce523ae0d4999f2a492deb9e76ac12cc8dc111b5f0e3bd74d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:28:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 10 May 2022 23:28:55 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:29:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('4294796c4bd4bed0c593d83606a5413de30f35f88d624e1b1e5b6cd8672ffbcc7a689d7ce4ef30c1abea0e95eda62220faac15d2a6aca0c3e2b418abe7a74118')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 10 May 2022 23:29:54 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 10 May 2022 23:29:56 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 10 May 2022 23:29:57 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Tue, 10 May 2022 23:29:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 10 May 2022 23:29:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 10 May 2022 23:29:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 10 May 2022 23:30:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 10 May 2022 23:30:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 10 May 2022 23:30:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 10 May 2022 23:30:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 10 May 2022 23:30:04 GMT
EXPOSE 80
# Tue, 10 May 2022 23:30:05 GMT
EXPOSE 443
# Tue, 10 May 2022 23:30:06 GMT
EXPOSE 2019
# Tue, 10 May 2022 23:30:47 GMT
RUN caddy version
# Tue, 10 May 2022 23:30:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d722bd7a5ed597b5a9ed7c5144caa608e784120c4442579352b7c2325ce47ffc`  
		Last Modified: Tue, 10 May 2022 23:35:41 GMT  
		Size: 498.2 KB (498231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0dfede5e37c630a175a1c987d90aaf1ec1db8cd7d43e3d63648743c6ace743`  
		Last Modified: Tue, 10 May 2022 23:35:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef201446c9bd5610f78b8e5a1680047ff45fadb77727762c323d5e48d77f9f2`  
		Last Modified: Tue, 10 May 2022 23:35:44 GMT  
		Size: 14.0 MB (14007489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b824e8abcb45a47ada825f0b722a588cbc9d1f68f5536a76b7afed2c5eb15a0c`  
		Last Modified: Tue, 10 May 2022 23:35:39 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b01057f474e19bdcaebab2c156622642945d2c7074276c82de663baeb418143`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520fb9c4921f60cfaea07cfa8d5733cf7f4f0810e56106911d7b25f59e86e997`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74d9e7abc08a32b35b26f8bba23c597b1e19d604766b326f61e77da0b494285`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595304462c9d3aa03aa9e164a98a38be5e1f5307c2981b65aa228101c73ce91b`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e307ee1571a8185932bbd90267a8b8d367f784859d99a2742d44e89e19e8b6c0`  
		Last Modified: Tue, 10 May 2022 23:35:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b335f1fddf0ed6abcc0e715ff827614cc2f0f4bbe8a0e1565145951d841c96`  
		Last Modified: Tue, 10 May 2022 23:35:36 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0974b9a20e0fa84c8a353a7c04992bec9e06825ed808054a358b84409744ba`  
		Last Modified: Tue, 10 May 2022 23:35:35 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d5086c691961c9f1a18b9d161cf8cb3dbd7b581c68ab75760b8c5e62647928`  
		Last Modified: Tue, 10 May 2022 23:35:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9194a8cf5ac8d920d218d9100152393ac6cce9142b15904894374694ae2d2fc`  
		Last Modified: Tue, 10 May 2022 23:35:36 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd07be490606caadc3893d219aee0682d6f8b71b2a4a8f2fb2ca826cdffb74`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b19beef4c4a6634592447260a670c8ee571e59cb775833787d39b815e9ba511`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2dab7fd2beddb5439029e7d8a75fc7c7fe2d3a534a63f51a04f85dd371cd1c`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e195aa5e2a95379397baf57f681e2c39a7c673d3c06d0ff3e4eeed3d8cecee1`  
		Last Modified: Tue, 10 May 2022 23:35:34 GMT  
		Size: 314.6 KB (314586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87827ca78b495430e19218a9e3f7f2837078a77df34bb929124ea20614287d5`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.1-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:88a75e54141f2e7531d3262b5a00a17002af383f24e29dab09212e4cbbfa2fdd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `caddy:2.5.1-windowsservercore-ltsc2022` - windows version 10.0.20348.707; amd64

```console
$ docker pull caddy@sha256:a3894222673d46b3e350553c6b7d4f92ab27b85a87fa1f773e9b090d5774ca9e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2252723203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:063f1879bd2783934ad3ac23aa37bf45f19be756f6b018f4c3a67d2d4a759c7c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:31:41 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 10 May 2022 23:31:42 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:32:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('4294796c4bd4bed0c593d83606a5413de30f35f88d624e1b1e5b6cd8672ffbcc7a689d7ce4ef30c1abea0e95eda62220faac15d2a6aca0c3e2b418abe7a74118')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 10 May 2022 23:32:11 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 10 May 2022 23:32:12 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 10 May 2022 23:32:13 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Tue, 10 May 2022 23:32:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 10 May 2022 23:32:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 10 May 2022 23:32:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 10 May 2022 23:32:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 10 May 2022 23:32:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 10 May 2022 23:32:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 10 May 2022 23:32:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 10 May 2022 23:32:21 GMT
EXPOSE 80
# Tue, 10 May 2022 23:32:22 GMT
EXPOSE 443
# Tue, 10 May 2022 23:32:23 GMT
EXPOSE 2019
# Tue, 10 May 2022 23:32:42 GMT
RUN caddy version
# Tue, 10 May 2022 23:32:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9baa8a196af04dc55746ee82c0774537bce72a589b75d9efce1a4680f03e35`  
		Last Modified: Tue, 10 May 2022 23:36:04 GMT  
		Size: 616.1 KB (616130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe60c7e90fdaeffa9bce60d9a7c7b340dedc357bfb70a2ce8c6d7b8bd0e74a11`  
		Last Modified: Tue, 10 May 2022 23:36:04 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f955bea173999b55d2087a27b9cc80e92bf168918c6e892175c2a75bdbfac933`  
		Last Modified: Tue, 10 May 2022 23:36:07 GMT  
		Size: 14.2 MB (14224642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e1ab4508d5347b929d5a33f71e0f24f653e61c147260200d32e3bd7cdd2340`  
		Last Modified: Tue, 10 May 2022 23:36:02 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8044ca4427c5edfee653001205397a2cc33f8fb4416c16c4a4936317c572ed`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f144416d38a1aa75558e0b93b88fcb3de122ee88349826ee99d596e1b00d9cc0`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32edbcceba80e7a70e44725926012bb70624bb0ae91c85db2766ca2e4c5a5d7c`  
		Last Modified: Tue, 10 May 2022 23:36:02 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd90105a2a3136e4d25d0add2b6fbe5798d51588215367128f1566d66b255289`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e448ed08c6c6ca9f854cb7014ea2e79c04e83f1905f78f578b67303b709fa3`  
		Last Modified: Tue, 10 May 2022 23:36:00 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d49b1b3778cd2ebf32521f530e29275a9a473afa997654b32338ff4349bf5c`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2112945425b7d069bc5705be1345e5ad6e27206e1531b10d0bc92d9c69ea9c3`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7243327255edd82b277f456085138a672f5a43d616e80f73156c8eb31139121d`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1a14330360d7ab3af40d4fb6f2de975e42e05f8e4cb064cc49fe1d9446e6b1`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808ce6a15ca3e6ad031229bcad8a3ed69171a7005c05ef4e77ffcfd777e9d1f7`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdfcf611e614d42a256d103775233f59ab7bb6ad0b00ca2f915bf739600f8d6`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3811622d464d497ce363eed806c75f9b994cd1d04b3009b2d0671af2863ebd0`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b006092864e6cfdfedd054a2635236c62958e97de81c720d9e38772276ee11`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 325.9 KB (325870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2afb0ece27a359f16126f263176baa74c3d3f2f2733cce186e4e31ad0eca4f8`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:0033b34d2df3fe0bf94088c36e7d722ceca1b38cbdd49c08b2c10b9f9aa58912
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:alpine` - linux; amd64

```console
$ docker pull caddy@sha256:6e62b63d4d7a4826f9e93c904a0e5b886a8bea2234b6569e300924282a2e8e6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16788470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e63f36e9049faf60b3a47c774237eddacb8916cacb003e418f2591de1a3bee29`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:25:00 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:19:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:19:24 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:19:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:19:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:19:26 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:19:26 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:19:27 GMT
EXPOSE 80
# Fri, 06 May 2022 19:19:27 GMT
EXPOSE 443
# Fri, 06 May 2022 19:19:28 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:19:28 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:19:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87ed6b8c4412bcd2bb1f40611012b40444b12071baf4884d0e75044fc1f32c1`  
		Last Modified: Tue, 05 Apr 2022 04:25:48 GMT  
		Size: 291.5 KB (291522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4c78357cc2da49b060ec4367d3d35d9837faf50e873e07ab40822e9fa57d00`  
		Last Modified: Fri, 06 May 2022 19:19:49 GMT  
		Size: 5.8 KB (5836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3edd190820fd86aaeb4fc1b7a28d7ff52e776414d3830f1a14d103967b455965`  
		Last Modified: Fri, 06 May 2022 19:19:51 GMT  
		Size: 13.7 MB (13676400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b96fea00470fa7356d42265c310e3940426e4c5572f288e8f7111a03b2fdddc`  
		Last Modified: Fri, 06 May 2022 19:19:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:813c33aa7f94275843088c57b0e44ea6c190d5296b664d7795f66bf3c3804392
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16056332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ee6ea861df7cd9fff1d948de8590f2bac9f2b90ebea7bc71ef7c7654f2d8d40`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:15:01 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:49:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:49:35 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:49:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:49:42 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:49:42 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:49:42 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:49:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:49:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:49:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:49:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:49:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:49:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:49:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:49:46 GMT
EXPOSE 80
# Fri, 06 May 2022 19:49:46 GMT
EXPOSE 443
# Fri, 06 May 2022 19:49:46 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:49:47 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:49:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b230dd773e10769a2eb3e507260d2470a646efd48a639739ba8852b2915302`  
		Last Modified: Tue, 05 Apr 2022 03:18:10 GMT  
		Size: 291.7 KB (291685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd82040b030d75398d6d6fb1c3d12cc9e25a954a92227895e1e5f7ea54736c20`  
		Last Modified: Fri, 06 May 2022 19:51:07 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583abcfacbc800cc0863a5117f1911222bec7ea3fcaed7c36ce4b94b489c3b3e`  
		Last Modified: Fri, 06 May 2022 19:51:16 GMT  
		Size: 13.1 MB (13136691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6903af22655a77183d11fb6d870f6ebc4776e6d9222e9de261b0a377cb81bbcf`  
		Last Modified: Fri, 06 May 2022 19:51:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:2e61a3ed70ad9a4784ff95cf49efa7ec58255c5263c3faba6a5270a847542a41
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.8 MB (15835582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93c6db987e0721fcd4f557ec160b55012a73d2f69de7198fac316514b27ed58f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:33:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:57:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:57:32 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:57:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:57:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:57:39 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:57:39 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:57:40 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:57:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:57:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:57:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:57:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:57:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:57:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:57:42 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:57:43 GMT
EXPOSE 80
# Fri, 06 May 2022 19:57:43 GMT
EXPOSE 443
# Fri, 06 May 2022 19:57:44 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:57:44 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:57:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03203881a2568530a735b6e0e7a40ebb79adedc5193a675807b04eeb92cc6ed1`  
		Last Modified: Tue, 05 Apr 2022 06:35:07 GMT  
		Size: 290.7 KB (290668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507adf96fcab6911303d2b3d14aeb43223c106ee9901b3e31f30668a4dbd5ffb`  
		Last Modified: Fri, 06 May 2022 19:59:02 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23435dc592c99e66d2e9f715136b809e73116ee6725847ed8fd158135e3283be`  
		Last Modified: Fri, 06 May 2022 19:59:11 GMT  
		Size: 13.1 MB (13114610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e55b7a8b43f4fdfecf61cea01ddddc80930ed485d9aafc41c26f84380f858f3`  
		Last Modified: Fri, 06 May 2022 19:59:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:cda45585c425161575996ee5d954166745d44d39928846423ecdce6b61a9fb4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.5 MB (15523770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:890cdb4fef0cc66aabb117ff1b3e11fb86de5117d28a5b0e64a743efb92c4269`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:12:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:39:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:39:32 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:39:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:39:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:39:37 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:39:38 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:39:39 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:39:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:39:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:39:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:39:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:39:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:39:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:39:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:39:47 GMT
EXPOSE 80
# Fri, 06 May 2022 19:39:48 GMT
EXPOSE 443
# Fri, 06 May 2022 19:39:49 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:39:50 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:39:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83aa37f2341b1e6d98420668c9bc849a47f2c471d159b2303885040bd8d0a92f`  
		Last Modified: Tue, 05 Apr 2022 03:13:38 GMT  
		Size: 291.3 KB (291301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc050d3d6ffb91c2f68db47e3d5f056afad26e465a03ae7e43383df0fc8ad89`  
		Last Modified: Fri, 06 May 2022 19:40:32 GMT  
		Size: 5.8 KB (5753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8adaff0bd78d0b115843dd841c83d1690484b25369e804b1133b838b7ad5ce8f`  
		Last Modified: Fri, 06 May 2022 19:40:35 GMT  
		Size: 12.5 MB (12510086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f703c61da5ec8e48b081aceac2cb64fb25162c2f0ba1ad16a104610b676f50f6`  
		Last Modified: Fri, 06 May 2022 19:40:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:d1ab9f3165d5b23b9ff5bd4fcb74b3f8bbf834ba34c42c58e496b3d33017ca59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15203958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfbb2004b1ba3aace5176af38455ef6b8328a074388b16b35358d61330ad2658`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:08:34 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:16:53 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:16:58 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:17:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:17:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:17:25 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:17:32 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:17:36 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:17:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:17:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:17:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:17:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:17:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:18:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:18:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:18:13 GMT
EXPOSE 80
# Fri, 06 May 2022 19:18:17 GMT
EXPOSE 443
# Fri, 06 May 2022 19:18:19 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:18:22 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:18:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743509d6ced044a369685ebb068417e8757981a39d1b397c7b0182ab89f83528`  
		Last Modified: Tue, 05 Apr 2022 07:11:24 GMT  
		Size: 293.7 KB (293721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b659dd8890d066269209696348c58ed19351199266936a5e81f1991a52333d1`  
		Last Modified: Fri, 06 May 2022 19:19:31 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86272ae554176010d052c51dcc5540948b8e59082743b04ac5bb67d05c3fdcd`  
		Last Modified: Fri, 06 May 2022 19:19:33 GMT  
		Size: 12.1 MB (12093067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff57ff409904cc43937df14c68e6d97e1269adde095e91671fb5438dc58a1808`  
		Last Modified: Fri, 06 May 2022 19:19:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:fbee089e769bc54babbe3ac3217c0e5b60c4a5157b76b0f37aa73cc71486c8fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16129299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f94fa793c943e1cb1c5bda77b0e7077b344648635da2222a1061307e3e61ca96`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:19:41 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:41:25 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:41:25 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:41:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:41:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:41:28 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:41:28 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:41:28 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:41:29 GMT
EXPOSE 80
# Fri, 06 May 2022 19:41:29 GMT
EXPOSE 443
# Fri, 06 May 2022 19:41:30 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:41:30 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:41:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8cc7c7c7ffd67f5740add448d341753330a2abdc6ed06e995cb7d28de381ab`  
		Last Modified: Tue, 05 Apr 2022 06:20:44 GMT  
		Size: 291.8 KB (291821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3d2fae470dbad90c4c4c1262110f14447a47b6e81edc4e0e80ceb50538fe57`  
		Last Modified: Fri, 06 May 2022 19:42:10 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a8f9dbbf38ad9456666a4e6a3eda871b385d4ef76ab6dc25e31030d1daf71c`  
		Last Modified: Fri, 06 May 2022 19:42:12 GMT  
		Size: 13.2 MB (13231118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf07e991258bc58c5e8a5785f741bc746e75848423d2c27d26448015c5887f1`  
		Last Modified: Fri, 06 May 2022 19:42:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:81fcae6c8754b60a6694fa9de78ad16f624bf2746f50e224dbd447d197597ae5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2928; amd64
	-	windows version 10.0.20348.707; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:1e292f2e17935f1d904222aa4291d4b4f0a3f48ddd2c73af04039226c812d84b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126492209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c80070b3eb6003cffb12fd895325316a7ad91a7f7116a69ce3970897ef0742d3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:19:44 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:19:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:19:45 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:20:38 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:22:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 22:22:12 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:22:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:22:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:22:13 GMT
WORKDIR /go
# Wed, 01 Jun 2022 22:49:16 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 22:49:16 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 22:49:16 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 22:49:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 22:49:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 22:49:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 22:49:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea60b727a1ce729d031ec1e4f2521a246e71bdb72d3fd9c9c04711cce80e1722`  
		Last Modified: Wed, 25 May 2022 00:24:05 GMT  
		Size: 271.8 KB (271822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c4a77219572e69864cd3069b7b47e55202681be151bd7394f9cb6645b5687b`  
		Last Modified: Wed, 25 May 2022 00:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370296b7ddb629fff1cc98d8d390acf0782fdb8f55cf4054637f6127bbcfe2a9`  
		Last Modified: Wed, 01 Jun 2022 22:30:44 GMT  
		Size: 115.2 MB (115199527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6cee850709034cc7b53152e226caba834fdeb704dab0621f1813bc9081173c`  
		Last Modified: Wed, 01 Jun 2022 22:30:29 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1136d32ff848474c9a359e03d2fcc678a7b8f0dc7e73222ae72e60f7fd4d74`  
		Last Modified: Wed, 01 Jun 2022 22:49:37 GMT  
		Size: 6.9 MB (6931847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c29192c5c8d89201d847a27e2e77e0c4e47f3cef0219cb077dcd8b5bdd9fe1`  
		Last Modified: Wed, 01 Jun 2022 22:49:36 GMT  
		Size: 1.3 MB (1289410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865185451556d5e92a06e01ff04ae2d479a7ff41a4cef4d7f3e27cdb3d0a559e`  
		Last Modified: Wed, 01 Jun 2022 22:49:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:7de3187171d024e8352c7d65d8c0f7264ecba7b1a0f704295fd611019cb3570f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.5 MB (122503603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d3ac773c95b35b7b4dbac45428257530fdef319e97ee68be2648997c9e4bcd5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:49:39 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:49:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:51:15 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:55:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 22:55:14 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:55:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:55:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:55:16 GMT
WORKDIR /go
# Wed, 01 Jun 2022 23:30:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 23:30:47 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 23:30:48 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 23:30:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 23:30:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 23:30:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 23:30:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6c67ddc305b7f97a531083e369316343b3d19da2352e4e3274db751bba38e2`  
		Last Modified: Wed, 25 May 2022 00:59:27 GMT  
		Size: 272.0 KB (272047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8a37c8e9266706ee6b9ca75c42931dfe1320723ad6a20f0ad4c97554998348`  
		Last Modified: Wed, 25 May 2022 00:59:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d540be111b8c098590378841899d81bec5b744ccbd9ab573bc9b5101566901c`  
		Last Modified: Wed, 01 Jun 2022 23:09:53 GMT  
		Size: 111.6 MB (111598618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cafdd66ccebe1705fc4faa98039c9de106fbcbe091c52f158673fe04e82f802e`  
		Last Modified: Wed, 01 Jun 2022 23:08:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96872e0a675044607ec984baa827068687c978aa91bb47e3f49960519818427`  
		Last Modified: Wed, 01 Jun 2022 23:31:59 GMT  
		Size: 6.8 MB (6796920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3293e1352a64f4c075b505e4c5b86af54f57290c7d7f30c7881824677027cc2`  
		Last Modified: Wed, 01 Jun 2022 23:31:56 GMT  
		Size: 1.2 MB (1229160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4753da45404db22fc7c2a859da39a898b3708ecbfc5cfea606ee7431d28666e4`  
		Last Modified: Wed, 01 Jun 2022 23:31:55 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:011ac9678dff1b4c8b7b55ed5e314c4cff6da6b30703063ebd229e6b72d63cd6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121343857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48dd50101a28b86b1db7401d9cb0cf460f9f9e9a5543d3b3abe69cf3a4290028`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 03:51:19 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 03:51:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 03:51:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 23:01:24 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 23:05:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 23:05:24 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 23:05:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 23:05:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 23:05:28 GMT
WORKDIR /go
# Wed, 01 Jun 2022 23:54:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 23:54:05 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 23:54:05 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 23:54:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 23:54:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 23:54:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 23:54:09 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e4e5a89e8a0366f9710ba7cb04de284f11234b8cb3dba3e69e35a76dd1c62`  
		Last Modified: Wed, 25 May 2022 04:03:05 GMT  
		Size: 271.0 KB (270972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3b879ada9b059c6167f45b720f44118516dfc73e29b727218447700619fbc5`  
		Last Modified: Wed, 25 May 2022 04:03:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fc48eab20f513149fdf3afa2d29409fae14ca579ba77b44d39b1c7d30bd160`  
		Last Modified: Wed, 01 Jun 2022 23:29:17 GMT  
		Size: 111.4 MB (111376293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4611066e57bc80a36e6249e8637f907272e5888e39790c2360619a7e0cba4833`  
		Last Modified: Wed, 01 Jun 2022 23:28:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65e673e15769cdf43d8d431796fdce20817845053df123db32c4d1ebb097dda`  
		Last Modified: Wed, 01 Jun 2022 23:55:15 GMT  
		Size: 6.1 MB (6056216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f57b87d4f5a15b224a843782ea88621460db848ce77a22ea9556319c9e5c0c`  
		Last Modified: Wed, 01 Jun 2022 23:55:13 GMT  
		Size: 1.2 MB (1228015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a540258c6d4d9ec99d0f270d7f398f2a784a811119862c84d641faf27d9d52f`  
		Last Modified: Wed, 01 Jun 2022 23:55:12 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:499ea69b717472a063a52ae5197f6deb99d1b2bf52f6ffe632ae6ee4b151e8d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121425869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8397cebecc3630e1971e7a6391326e81bf1f7987dad0cd00d290554058a8e96`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:40:10 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:40:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:40:12 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:41:13 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:43:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 22:43:14 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:43:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:43:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:43:16 GMT
WORKDIR /go
# Wed, 01 Jun 2022 23:12:50 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 23:12:51 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 23:12:51 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 23:12:52 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 23:12:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 23:12:56 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 23:12:56 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a3192eca97ce26527d2bdbb26d1130abcc1c9dd7b800ce2fd14619fa422640`  
		Last Modified: Wed, 25 May 2022 00:45:29 GMT  
		Size: 271.7 KB (271711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a050256f5b6fc0800b8ae0d96e136745091c36ce8e53ba74d8ab3eed65966a59`  
		Last Modified: Wed, 25 May 2022 00:45:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656be50a0ddc84123afb23ccbb17811b43648fa17b4c8664716e9e07553c8b35`  
		Last Modified: Wed, 01 Jun 2022 22:54:01 GMT  
		Size: 110.2 MB (110233232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbca73fdf42200f09770a4826a8cc1004903cd4e9005eff055c63246812a376`  
		Last Modified: Wed, 01 Jun 2022 22:53:46 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab89aed908fe45f53da57dfae1a8b8c6cd86095ae16ff74114042f8a979f1932`  
		Last Modified: Wed, 01 Jun 2022 23:13:30 GMT  
		Size: 7.0 MB (7036774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb64d47dd3ed3c1225ae6e128fbf6d24fcc3c845ef16f462a471531f409af29`  
		Last Modified: Wed, 01 Jun 2022 23:13:29 GMT  
		Size: 1.2 MB (1189006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9128167bb5002c5f6502cafb32b7004c893d437d65d07a486683d6a4827295`  
		Last Modified: Wed, 01 Jun 2022 23:13:28 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:51489e35e697983a57f901922b0dabd40e875688ab29307b905d29ce55fbaab9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121929763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ab8036b8f55aab1eb0d1627d8569e7b7b92390a17e595ffaf9dfe82da24529`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:17:40 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:17:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:17:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 May 2022 00:18:07 GMT
ENV GOLANG_VERSION=1.18.2
# Wed, 25 May 2022 00:21:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 25 May 2022 00:21:40 GMT
ENV GOPATH=/go
# Wed, 25 May 2022 00:21:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 May 2022 00:21:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 25 May 2022 00:21:58 GMT
WORKDIR /go
# Wed, 25 May 2022 00:45:35 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 25 May 2022 00:45:39 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 25 May 2022 00:45:43 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 25 May 2022 00:45:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 25 May 2022 00:45:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 25 May 2022 00:45:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 25 May 2022 00:46:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211c1f83aeafafff903bb460e7e24594fe138ebceeb1b56e898cf0158ea3daaf`  
		Last Modified: Wed, 25 May 2022 00:27:59 GMT  
		Size: 274.2 KB (274180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8365966bf1e6bd302f9e7c3d8e027aef3cfab1652ed22b8bd53311ef9517f0d3`  
		Last Modified: Wed, 25 May 2022 00:27:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6a047513e9ca46258b5a80c34d0bb9eef5b7e2c8004c5ddd1ca930e7c33659`  
		Last Modified: Wed, 25 May 2022 00:28:25 GMT  
		Size: 110.2 MB (110219016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4216cfe6259a3cf57000a58c453b0ffda2da2dd8b841017c33f4f9e33c8fa5da`  
		Last Modified: Wed, 25 May 2022 00:27:58 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2f4bee20e80c6473651d3ce23e74677476c7b12c9aa9bb880a3b819b0137d9`  
		Last Modified: Wed, 25 May 2022 00:46:38 GMT  
		Size: 7.5 MB (7469747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e99268d0161e857b0995380335a9c16bad6eaad709fc33fe99363301fc93c28`  
		Last Modified: Wed, 25 May 2022 00:46:38 GMT  
		Size: 1.2 MB (1176359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fa65f829c67a09aeb16d10c849ef12dcac7f86668154a677c8caa2bcc02c49`  
		Last Modified: Wed, 25 May 2022 00:46:37 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:2999d8fa276be8936078596794d15be8b708720ee296803ac88d976675f8b84a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124255828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc7070a321e5a4b1b7616b221cf9a73591e4fc00c310bfaad9825483eb4eb0d8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:41:57 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:41:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:41:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:43:25 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:45:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 22:46:11 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:46:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:46:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:46:13 GMT
WORKDIR /go
# Wed, 01 Jun 2022 23:16:35 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 23:16:36 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 23:16:37 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 23:16:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 23:16:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 23:16:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 23:16:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e497ff1a375465e6a6ba78259a6f2e9f7986cf27789ba79ddfd1cca023a160`  
		Last Modified: Wed, 25 May 2022 00:50:39 GMT  
		Size: 272.2 KB (272155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e413365aa9b9c967651e3a27f41641db43d81f24ff58ea4de0ce2c662c5d5f`  
		Last Modified: Wed, 25 May 2022 00:50:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e76ee5124cc2e0e213f5fc781375c53acc53fda6cb50eb09ce717d9ce4626ce`  
		Last Modified: Wed, 01 Jun 2022 22:58:35 GMT  
		Size: 113.1 MB (113111409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43db1e7eb380ed189bd16b98ad5afb071c88b789a987c6d8c2dd65dc4bfbf16d`  
		Last Modified: Wed, 01 Jun 2022 22:58:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0ade8df88187af31cea8632059bf709714e41aa1f2cf4a4bd3cee7562d3291`  
		Last Modified: Wed, 01 Jun 2022 23:17:26 GMT  
		Size: 7.0 MB (7047929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634c737128f1d3d767c417a20c9a5faaab86feb02d4e7a179046b7da981707f7`  
		Last Modified: Wed, 01 Jun 2022 23:17:25 GMT  
		Size: 1.2 MB (1243129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d94f95e9c108ec4db470dfbacda85ff19601a76bcfb7c7328b26c4fa4b09b9`  
		Last Modified: Wed, 01 Jun 2022 23:17:25 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.2928; amd64

```console
$ docker pull caddy@sha256:9ccfa9fc4fc4236cf295417a18c7d16b0a79495b916cd1b95c231e18daed3423
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2674256754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e7531282f56b1596b6475bd16a7058aaa9dc1e6884e7902f556e23b3eccf951`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 22:21:43 GMT
ENV GIT_VERSION=2.23.0
# Tue, 10 May 2022 22:21:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 10 May 2022 22:21:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 10 May 2022 22:21:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 10 May 2022 22:23:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:23:36 GMT
ENV GOPATH=C:\go
# Tue, 10 May 2022 22:24:28 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 10 May 2022 22:40:47 GMT
ENV GOLANG_VERSION=1.17.10
# Tue, 10 May 2022 22:44:40 GMT
RUN $url = 'https://dl.google.com/go/go1.17.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ba9198a29fa5c4f322212d21569e8507165c3b34e1ed1f1f9cf6dfb71ddcdeb2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:44:47 GMT
WORKDIR C:\go
# Tue, 10 May 2022 23:33:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:33:03 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 10 May 2022 23:33:04 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:33:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 10 May 2022 23:34:01 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 10 May 2022 23:34:02 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01012ab52f3f9693dd4b85e6e19a0b2659b4f869d6b5b5d2ea62afe84c9037c`  
		Last Modified: Tue, 10 May 2022 22:55:50 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988abb6e02c6ab2eb0330641b6378c4e110c132c761de086dfc1629462491e90`  
		Last Modified: Tue, 10 May 2022 22:55:48 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b62ac07a4cd6e0fd762f7f6e904be7b001affa78e8fbfeb8ca017a6f643d62c`  
		Last Modified: Tue, 10 May 2022 22:55:47 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e235721feec6368d5a652fd467681dffe74326d42da4bed8e43f777bc39c47`  
		Last Modified: Tue, 10 May 2022 22:55:47 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8195b6f87245387233358bc8fcc2679a23d9aa46cd4bfef94ac49284694c5c42`  
		Last Modified: Tue, 10 May 2022 22:56:13 GMT  
		Size: 25.6 MB (25580295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cfe0249f2fac54d31ea467ce63bdc69e4504b726a87d969fb1b42ab2ab3853`  
		Last Modified: Tue, 10 May 2022 22:55:45 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c97dcc9056ac36ad6120d94049a937f5366e71fda7c478ff3462d542cc0645`  
		Last Modified: Tue, 10 May 2022 22:55:45 GMT  
		Size: 322.0 KB (321981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4753086b1ed8db6655e0993e3f676d7f71455415cce16cd5593b330f9a89b3a`  
		Last Modified: Tue, 10 May 2022 23:05:04 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66134c7f83737bd3064ea2c3dce37ea0157cde99b46bbf80744100fd7f18a0aa`  
		Last Modified: Tue, 10 May 2022 23:07:31 GMT  
		Size: 142.6 MB (142588622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0697a4af489e787e5def466bbf9614e20bf5b1cea211f3a8f8ce2f0b5a10a3f`  
		Last Modified: Tue, 10 May 2022 23:05:04 GMT  
		Size: 1.6 KB (1566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c242b44aab0e82a2f6bf16213c350b73347e55ad15ecafa05877414e1327e96b`  
		Last Modified: Tue, 10 May 2022 23:36:29 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223dbf32ed9ac3b13af8e1196395df286392aa610ec5ba0bf809061dbf84a5cb`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a255b634df668adc897872554f8b720fdd5e6f4a9c47db0bbc489d25a0aaa66e`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe18292f9995b50f39e6e8ef4cfa31d2913132bef8804b56e260a907b205cd18`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168a524248b6a67f943614b53e6a0825bd107c0b90796733fccfe1184d013a45`  
		Last Modified: Tue, 10 May 2022 23:36:28 GMT  
		Size: 1.7 MB (1691907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4398dd61eb69a257d8e25ec572462f611d347efd5e30a944117a652f47314944`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.20348.707; amd64

```console
$ docker pull caddy@sha256:5577ab08abcc0385dd65f73089851d37eb4cd88a29a3cd1d511c6c526221fc42
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2415395050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8e125146193f9e2329bf6ce618db8d09adc336b804bec5cd23b54463959d504`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 22:16:59 GMT
ENV GIT_VERSION=2.23.0
# Tue, 10 May 2022 22:17:00 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 10 May 2022 22:17:01 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 10 May 2022 22:17:02 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 10 May 2022 22:17:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:17:52 GMT
ENV GOPATH=C:\go
# Tue, 10 May 2022 22:18:24 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 10 May 2022 22:18:25 GMT
ENV GOLANG_VERSION=1.18.2
# Tue, 10 May 2022 22:21:20 GMT
RUN $url = 'https://dl.google.com/go/go1.18.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '41fc44109c39a98e0c3672989ac5ad205cbb5768067e099dc4fb2b75cba922cf'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:21:26 GMT
WORKDIR C:\go
# Tue, 10 May 2022 23:34:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:34:18 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 10 May 2022 23:34:19 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:34:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 10 May 2022 23:34:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 10 May 2022 23:34:53 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb2ee3c21cb72c263da0dc4c6080f1d34c7ce3c7f24dcce76815784ec99440f`  
		Last Modified: Tue, 10 May 2022 22:52:57 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db422a46fd25683fe2e5990dc5db827b96c7b135679867ac162c2a318803463`  
		Last Modified: Tue, 10 May 2022 22:52:56 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4110a58975fa9bc64fa3a7d64804d47aa9ba813231538466dfedf4c35658cae7`  
		Last Modified: Tue, 10 May 2022 22:52:55 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e110f1696433dc412066aa30ea4222e641d7d377d593568f539b471b865a664`  
		Last Modified: Tue, 10 May 2022 22:52:55 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aca2a7cb069b5fd7ea06af17cd99249cae08f77d945258e72108af23fb4570a`  
		Last Modified: Tue, 10 May 2022 22:53:21 GMT  
		Size: 25.7 MB (25692112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc78480e80903590627dacfc79a3c978709b8c787cc193391852c4f8bf2ffca`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f488db75670938176d831a4bc8ddd4bb629e7a61e9ce5101882db134c0d162`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 541.2 KB (541163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7e0fbd217082bd92c424bbe5de58f546b38e43068d1f7b3a1121e42ffcbac6`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d268be7c91150b1073b85f55a434b87a1602a325ad6af8f2c2896f34f83388`  
		Last Modified: Tue, 10 May 2022 22:55:29 GMT  
		Size: 149.7 MB (149697865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3786f32f80e906fe1e08346c7294bfcfaa5d640b7c8cd920c91fb3b33f8bb6e4`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 1.5 KB (1536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd4f585b833fb8fb9f417326d46999e8726e1aa94e3796e9005a10daf16e12d`  
		Last Modified: Tue, 10 May 2022 23:36:48 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707272d91e9f672f1fe7a0de3ecaeefc72c1d00ee1025438e7cfb0dc74a77ee2`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a90464121b8d7fd8edb1f37124b634fe69680d1b4af3a6b853417ab05e9243a0`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20695dc76bb11cb698c1e429bbcb5e3011dfd00666a09a81c2cbd4f4607b1da`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884b6dd02ff92d7127e63601c97c036dee9230f73ecfe1d2d382466b705e9836`  
		Last Modified: Tue, 10 May 2022 23:36:46 GMT  
		Size: 1.9 MB (1910625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f0345f50b887c52e7c023a68e29e1332dac19143806fc334ea4d6e9a2cb0d5`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:ffbabc549906ee81026a50566ab1b254cafdafcc6e43c09abcc61fde1d323146
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:1e292f2e17935f1d904222aa4291d4b4f0a3f48ddd2c73af04039226c812d84b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126492209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c80070b3eb6003cffb12fd895325316a7ad91a7f7116a69ce3970897ef0742d3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:19:44 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:19:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:19:45 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:20:38 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:22:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 22:22:12 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:22:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:22:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:22:13 GMT
WORKDIR /go
# Wed, 01 Jun 2022 22:49:16 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 22:49:16 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 22:49:16 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 22:49:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 22:49:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 22:49:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 22:49:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea60b727a1ce729d031ec1e4f2521a246e71bdb72d3fd9c9c04711cce80e1722`  
		Last Modified: Wed, 25 May 2022 00:24:05 GMT  
		Size: 271.8 KB (271822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c4a77219572e69864cd3069b7b47e55202681be151bd7394f9cb6645b5687b`  
		Last Modified: Wed, 25 May 2022 00:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370296b7ddb629fff1cc98d8d390acf0782fdb8f55cf4054637f6127bbcfe2a9`  
		Last Modified: Wed, 01 Jun 2022 22:30:44 GMT  
		Size: 115.2 MB (115199527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6cee850709034cc7b53152e226caba834fdeb704dab0621f1813bc9081173c`  
		Last Modified: Wed, 01 Jun 2022 22:30:29 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1136d32ff848474c9a359e03d2fcc678a7b8f0dc7e73222ae72e60f7fd4d74`  
		Last Modified: Wed, 01 Jun 2022 22:49:37 GMT  
		Size: 6.9 MB (6931847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c29192c5c8d89201d847a27e2e77e0c4e47f3cef0219cb077dcd8b5bdd9fe1`  
		Last Modified: Wed, 01 Jun 2022 22:49:36 GMT  
		Size: 1.3 MB (1289410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865185451556d5e92a06e01ff04ae2d479a7ff41a4cef4d7f3e27cdb3d0a559e`  
		Last Modified: Wed, 01 Jun 2022 22:49:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:7de3187171d024e8352c7d65d8c0f7264ecba7b1a0f704295fd611019cb3570f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.5 MB (122503603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d3ac773c95b35b7b4dbac45428257530fdef319e97ee68be2648997c9e4bcd5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:49:39 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:49:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:51:15 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:55:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 22:55:14 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:55:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:55:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:55:16 GMT
WORKDIR /go
# Wed, 01 Jun 2022 23:30:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 23:30:47 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 23:30:48 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 23:30:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 23:30:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 23:30:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 23:30:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6c67ddc305b7f97a531083e369316343b3d19da2352e4e3274db751bba38e2`  
		Last Modified: Wed, 25 May 2022 00:59:27 GMT  
		Size: 272.0 KB (272047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8a37c8e9266706ee6b9ca75c42931dfe1320723ad6a20f0ad4c97554998348`  
		Last Modified: Wed, 25 May 2022 00:59:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d540be111b8c098590378841899d81bec5b744ccbd9ab573bc9b5101566901c`  
		Last Modified: Wed, 01 Jun 2022 23:09:53 GMT  
		Size: 111.6 MB (111598618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cafdd66ccebe1705fc4faa98039c9de106fbcbe091c52f158673fe04e82f802e`  
		Last Modified: Wed, 01 Jun 2022 23:08:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96872e0a675044607ec984baa827068687c978aa91bb47e3f49960519818427`  
		Last Modified: Wed, 01 Jun 2022 23:31:59 GMT  
		Size: 6.8 MB (6796920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3293e1352a64f4c075b505e4c5b86af54f57290c7d7f30c7881824677027cc2`  
		Last Modified: Wed, 01 Jun 2022 23:31:56 GMT  
		Size: 1.2 MB (1229160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4753da45404db22fc7c2a859da39a898b3708ecbfc5cfea606ee7431d28666e4`  
		Last Modified: Wed, 01 Jun 2022 23:31:55 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:011ac9678dff1b4c8b7b55ed5e314c4cff6da6b30703063ebd229e6b72d63cd6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121343857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48dd50101a28b86b1db7401d9cb0cf460f9f9e9a5543d3b3abe69cf3a4290028`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 03:51:19 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 03:51:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 03:51:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 23:01:24 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 23:05:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 23:05:24 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 23:05:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 23:05:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 23:05:28 GMT
WORKDIR /go
# Wed, 01 Jun 2022 23:54:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 23:54:05 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 23:54:05 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 23:54:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 23:54:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 23:54:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 23:54:09 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e4e5a89e8a0366f9710ba7cb04de284f11234b8cb3dba3e69e35a76dd1c62`  
		Last Modified: Wed, 25 May 2022 04:03:05 GMT  
		Size: 271.0 KB (270972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3b879ada9b059c6167f45b720f44118516dfc73e29b727218447700619fbc5`  
		Last Modified: Wed, 25 May 2022 04:03:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fc48eab20f513149fdf3afa2d29409fae14ca579ba77b44d39b1c7d30bd160`  
		Last Modified: Wed, 01 Jun 2022 23:29:17 GMT  
		Size: 111.4 MB (111376293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4611066e57bc80a36e6249e8637f907272e5888e39790c2360619a7e0cba4833`  
		Last Modified: Wed, 01 Jun 2022 23:28:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65e673e15769cdf43d8d431796fdce20817845053df123db32c4d1ebb097dda`  
		Last Modified: Wed, 01 Jun 2022 23:55:15 GMT  
		Size: 6.1 MB (6056216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f57b87d4f5a15b224a843782ea88621460db848ce77a22ea9556319c9e5c0c`  
		Last Modified: Wed, 01 Jun 2022 23:55:13 GMT  
		Size: 1.2 MB (1228015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a540258c6d4d9ec99d0f270d7f398f2a784a811119862c84d641faf27d9d52f`  
		Last Modified: Wed, 01 Jun 2022 23:55:12 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:499ea69b717472a063a52ae5197f6deb99d1b2bf52f6ffe632ae6ee4b151e8d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121425869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8397cebecc3630e1971e7a6391326e81bf1f7987dad0cd00d290554058a8e96`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:40:10 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:40:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:40:12 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:41:13 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:43:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 22:43:14 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:43:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:43:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:43:16 GMT
WORKDIR /go
# Wed, 01 Jun 2022 23:12:50 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 23:12:51 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 23:12:51 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 23:12:52 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 23:12:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 23:12:56 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 23:12:56 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a3192eca97ce26527d2bdbb26d1130abcc1c9dd7b800ce2fd14619fa422640`  
		Last Modified: Wed, 25 May 2022 00:45:29 GMT  
		Size: 271.7 KB (271711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a050256f5b6fc0800b8ae0d96e136745091c36ce8e53ba74d8ab3eed65966a59`  
		Last Modified: Wed, 25 May 2022 00:45:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656be50a0ddc84123afb23ccbb17811b43648fa17b4c8664716e9e07553c8b35`  
		Last Modified: Wed, 01 Jun 2022 22:54:01 GMT  
		Size: 110.2 MB (110233232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbca73fdf42200f09770a4826a8cc1004903cd4e9005eff055c63246812a376`  
		Last Modified: Wed, 01 Jun 2022 22:53:46 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab89aed908fe45f53da57dfae1a8b8c6cd86095ae16ff74114042f8a979f1932`  
		Last Modified: Wed, 01 Jun 2022 23:13:30 GMT  
		Size: 7.0 MB (7036774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb64d47dd3ed3c1225ae6e128fbf6d24fcc3c845ef16f462a471531f409af29`  
		Last Modified: Wed, 01 Jun 2022 23:13:29 GMT  
		Size: 1.2 MB (1189006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9128167bb5002c5f6502cafb32b7004c893d437d65d07a486683d6a4827295`  
		Last Modified: Wed, 01 Jun 2022 23:13:28 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:51489e35e697983a57f901922b0dabd40e875688ab29307b905d29ce55fbaab9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121929763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ab8036b8f55aab1eb0d1627d8569e7b7b92390a17e595ffaf9dfe82da24529`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:17:40 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:17:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:17:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 May 2022 00:18:07 GMT
ENV GOLANG_VERSION=1.18.2
# Wed, 25 May 2022 00:21:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 25 May 2022 00:21:40 GMT
ENV GOPATH=/go
# Wed, 25 May 2022 00:21:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 May 2022 00:21:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 25 May 2022 00:21:58 GMT
WORKDIR /go
# Wed, 25 May 2022 00:45:35 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 25 May 2022 00:45:39 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 25 May 2022 00:45:43 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 25 May 2022 00:45:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 25 May 2022 00:45:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 25 May 2022 00:45:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 25 May 2022 00:46:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211c1f83aeafafff903bb460e7e24594fe138ebceeb1b56e898cf0158ea3daaf`  
		Last Modified: Wed, 25 May 2022 00:27:59 GMT  
		Size: 274.2 KB (274180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8365966bf1e6bd302f9e7c3d8e027aef3cfab1652ed22b8bd53311ef9517f0d3`  
		Last Modified: Wed, 25 May 2022 00:27:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6a047513e9ca46258b5a80c34d0bb9eef5b7e2c8004c5ddd1ca930e7c33659`  
		Last Modified: Wed, 25 May 2022 00:28:25 GMT  
		Size: 110.2 MB (110219016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4216cfe6259a3cf57000a58c453b0ffda2da2dd8b841017c33f4f9e33c8fa5da`  
		Last Modified: Wed, 25 May 2022 00:27:58 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2f4bee20e80c6473651d3ce23e74677476c7b12c9aa9bb880a3b819b0137d9`  
		Last Modified: Wed, 25 May 2022 00:46:38 GMT  
		Size: 7.5 MB (7469747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e99268d0161e857b0995380335a9c16bad6eaad709fc33fe99363301fc93c28`  
		Last Modified: Wed, 25 May 2022 00:46:38 GMT  
		Size: 1.2 MB (1176359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fa65f829c67a09aeb16d10c849ef12dcac7f86668154a677c8caa2bcc02c49`  
		Last Modified: Wed, 25 May 2022 00:46:37 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:2999d8fa276be8936078596794d15be8b708720ee296803ac88d976675f8b84a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124255828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc7070a321e5a4b1b7616b221cf9a73591e4fc00c310bfaad9825483eb4eb0d8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:41:57 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:41:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:41:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:43:25 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:45:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Jun 2022 22:46:11 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:46:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:46:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:46:13 GMT
WORKDIR /go
# Wed, 01 Jun 2022 23:16:35 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 01 Jun 2022 23:16:36 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 01 Jun 2022 23:16:37 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 01 Jun 2022 23:16:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Jun 2022 23:16:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Jun 2022 23:16:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Jun 2022 23:16:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e497ff1a375465e6a6ba78259a6f2e9f7986cf27789ba79ddfd1cca023a160`  
		Last Modified: Wed, 25 May 2022 00:50:39 GMT  
		Size: 272.2 KB (272155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e413365aa9b9c967651e3a27f41641db43d81f24ff58ea4de0ce2c662c5d5f`  
		Last Modified: Wed, 25 May 2022 00:50:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e76ee5124cc2e0e213f5fc781375c53acc53fda6cb50eb09ce717d9ce4626ce`  
		Last Modified: Wed, 01 Jun 2022 22:58:35 GMT  
		Size: 113.1 MB (113111409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43db1e7eb380ed189bd16b98ad5afb071c88b789a987c6d8c2dd65dc4bfbf16d`  
		Last Modified: Wed, 01 Jun 2022 22:58:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0ade8df88187af31cea8632059bf709714e41aa1f2cf4a4bd3cee7562d3291`  
		Last Modified: Wed, 01 Jun 2022 23:17:26 GMT  
		Size: 7.0 MB (7047929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634c737128f1d3d767c417a20c9a5faaab86feb02d4e7a179046b7da981707f7`  
		Last Modified: Wed, 01 Jun 2022 23:17:25 GMT  
		Size: 1.2 MB (1243129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d94f95e9c108ec4db470dfbacda85ff19601a76bcfb7c7328b26c4fa4b09b9`  
		Last Modified: Wed, 01 Jun 2022 23:17:25 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:80ca8f74f642d7218cc111d5ea59115a305c4cd6030325cb4c4a7fad93d4c5a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull caddy@sha256:9ccfa9fc4fc4236cf295417a18c7d16b0a79495b916cd1b95c231e18daed3423
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2674256754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e7531282f56b1596b6475bd16a7058aaa9dc1e6884e7902f556e23b3eccf951`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 22:21:43 GMT
ENV GIT_VERSION=2.23.0
# Tue, 10 May 2022 22:21:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 10 May 2022 22:21:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 10 May 2022 22:21:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 10 May 2022 22:23:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:23:36 GMT
ENV GOPATH=C:\go
# Tue, 10 May 2022 22:24:28 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 10 May 2022 22:40:47 GMT
ENV GOLANG_VERSION=1.17.10
# Tue, 10 May 2022 22:44:40 GMT
RUN $url = 'https://dl.google.com/go/go1.17.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ba9198a29fa5c4f322212d21569e8507165c3b34e1ed1f1f9cf6dfb71ddcdeb2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:44:47 GMT
WORKDIR C:\go
# Tue, 10 May 2022 23:33:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:33:03 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 10 May 2022 23:33:04 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:33:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 10 May 2022 23:34:01 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 10 May 2022 23:34:02 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01012ab52f3f9693dd4b85e6e19a0b2659b4f869d6b5b5d2ea62afe84c9037c`  
		Last Modified: Tue, 10 May 2022 22:55:50 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988abb6e02c6ab2eb0330641b6378c4e110c132c761de086dfc1629462491e90`  
		Last Modified: Tue, 10 May 2022 22:55:48 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b62ac07a4cd6e0fd762f7f6e904be7b001affa78e8fbfeb8ca017a6f643d62c`  
		Last Modified: Tue, 10 May 2022 22:55:47 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e235721feec6368d5a652fd467681dffe74326d42da4bed8e43f777bc39c47`  
		Last Modified: Tue, 10 May 2022 22:55:47 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8195b6f87245387233358bc8fcc2679a23d9aa46cd4bfef94ac49284694c5c42`  
		Last Modified: Tue, 10 May 2022 22:56:13 GMT  
		Size: 25.6 MB (25580295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cfe0249f2fac54d31ea467ce63bdc69e4504b726a87d969fb1b42ab2ab3853`  
		Last Modified: Tue, 10 May 2022 22:55:45 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c97dcc9056ac36ad6120d94049a937f5366e71fda7c478ff3462d542cc0645`  
		Last Modified: Tue, 10 May 2022 22:55:45 GMT  
		Size: 322.0 KB (321981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4753086b1ed8db6655e0993e3f676d7f71455415cce16cd5593b330f9a89b3a`  
		Last Modified: Tue, 10 May 2022 23:05:04 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66134c7f83737bd3064ea2c3dce37ea0157cde99b46bbf80744100fd7f18a0aa`  
		Last Modified: Tue, 10 May 2022 23:07:31 GMT  
		Size: 142.6 MB (142588622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0697a4af489e787e5def466bbf9614e20bf5b1cea211f3a8f8ce2f0b5a10a3f`  
		Last Modified: Tue, 10 May 2022 23:05:04 GMT  
		Size: 1.6 KB (1566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c242b44aab0e82a2f6bf16213c350b73347e55ad15ecafa05877414e1327e96b`  
		Last Modified: Tue, 10 May 2022 23:36:29 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223dbf32ed9ac3b13af8e1196395df286392aa610ec5ba0bf809061dbf84a5cb`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a255b634df668adc897872554f8b720fdd5e6f4a9c47db0bbc489d25a0aaa66e`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe18292f9995b50f39e6e8ef4cfa31d2913132bef8804b56e260a907b205cd18`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168a524248b6a67f943614b53e6a0825bd107c0b90796733fccfe1184d013a45`  
		Last Modified: Tue, 10 May 2022 23:36:28 GMT  
		Size: 1.7 MB (1691907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4398dd61eb69a257d8e25ec572462f611d347efd5e30a944117a652f47314944`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:f5f71b248dea482aed03fe1e9ffdbd84e3e337044b6e4263956c9e8069ff8da2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `caddy:builder-windowsservercore-ltsc2022` - windows version 10.0.20348.707; amd64

```console
$ docker pull caddy@sha256:5577ab08abcc0385dd65f73089851d37eb4cd88a29a3cd1d511c6c526221fc42
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2415395050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8e125146193f9e2329bf6ce618db8d09adc336b804bec5cd23b54463959d504`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 22:16:59 GMT
ENV GIT_VERSION=2.23.0
# Tue, 10 May 2022 22:17:00 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 10 May 2022 22:17:01 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 10 May 2022 22:17:02 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 10 May 2022 22:17:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:17:52 GMT
ENV GOPATH=C:\go
# Tue, 10 May 2022 22:18:24 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 10 May 2022 22:18:25 GMT
ENV GOLANG_VERSION=1.18.2
# Tue, 10 May 2022 22:21:20 GMT
RUN $url = 'https://dl.google.com/go/go1.18.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '41fc44109c39a98e0c3672989ac5ad205cbb5768067e099dc4fb2b75cba922cf'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:21:26 GMT
WORKDIR C:\go
# Tue, 10 May 2022 23:34:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:34:18 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 10 May 2022 23:34:19 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:34:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 10 May 2022 23:34:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 10 May 2022 23:34:53 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb2ee3c21cb72c263da0dc4c6080f1d34c7ce3c7f24dcce76815784ec99440f`  
		Last Modified: Tue, 10 May 2022 22:52:57 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db422a46fd25683fe2e5990dc5db827b96c7b135679867ac162c2a318803463`  
		Last Modified: Tue, 10 May 2022 22:52:56 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4110a58975fa9bc64fa3a7d64804d47aa9ba813231538466dfedf4c35658cae7`  
		Last Modified: Tue, 10 May 2022 22:52:55 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e110f1696433dc412066aa30ea4222e641d7d377d593568f539b471b865a664`  
		Last Modified: Tue, 10 May 2022 22:52:55 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aca2a7cb069b5fd7ea06af17cd99249cae08f77d945258e72108af23fb4570a`  
		Last Modified: Tue, 10 May 2022 22:53:21 GMT  
		Size: 25.7 MB (25692112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc78480e80903590627dacfc79a3c978709b8c787cc193391852c4f8bf2ffca`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f488db75670938176d831a4bc8ddd4bb629e7a61e9ce5101882db134c0d162`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 541.2 KB (541163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7e0fbd217082bd92c424bbe5de58f546b38e43068d1f7b3a1121e42ffcbac6`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d268be7c91150b1073b85f55a434b87a1602a325ad6af8f2c2896f34f83388`  
		Last Modified: Tue, 10 May 2022 22:55:29 GMT  
		Size: 149.7 MB (149697865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3786f32f80e906fe1e08346c7294bfcfaa5d640b7c8cd920c91fb3b33f8bb6e4`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 1.5 KB (1536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd4f585b833fb8fb9f417326d46999e8726e1aa94e3796e9005a10daf16e12d`  
		Last Modified: Tue, 10 May 2022 23:36:48 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707272d91e9f672f1fe7a0de3ecaeefc72c1d00ee1025438e7cfb0dc74a77ee2`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a90464121b8d7fd8edb1f37124b634fe69680d1b4af3a6b853417ab05e9243a0`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20695dc76bb11cb698c1e429bbcb5e3011dfd00666a09a81c2cbd4f4607b1da`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884b6dd02ff92d7127e63601c97c036dee9230f73ecfe1d2d382466b705e9836`  
		Last Modified: Tue, 10 May 2022 23:36:46 GMT  
		Size: 1.9 MB (1910625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f0345f50b887c52e7c023a68e29e1332dac19143806fc334ea4d6e9a2cb0d5`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:eb2cce28a50cb1f20f1e4a13181f3e453e58d20999cffa7750222d9907023b6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2928; amd64
	-	windows version 10.0.20348.707; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:6e62b63d4d7a4826f9e93c904a0e5b886a8bea2234b6569e300924282a2e8e6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16788470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e63f36e9049faf60b3a47c774237eddacb8916cacb003e418f2591de1a3bee29`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:25:00 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:19:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:19:24 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:19:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:19:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:19:26 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:19:26 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:19:27 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:19:27 GMT
EXPOSE 80
# Fri, 06 May 2022 19:19:27 GMT
EXPOSE 443
# Fri, 06 May 2022 19:19:28 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:19:28 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:19:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87ed6b8c4412bcd2bb1f40611012b40444b12071baf4884d0e75044fc1f32c1`  
		Last Modified: Tue, 05 Apr 2022 04:25:48 GMT  
		Size: 291.5 KB (291522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4c78357cc2da49b060ec4367d3d35d9837faf50e873e07ab40822e9fa57d00`  
		Last Modified: Fri, 06 May 2022 19:19:49 GMT  
		Size: 5.8 KB (5836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3edd190820fd86aaeb4fc1b7a28d7ff52e776414d3830f1a14d103967b455965`  
		Last Modified: Fri, 06 May 2022 19:19:51 GMT  
		Size: 13.7 MB (13676400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b96fea00470fa7356d42265c310e3940426e4c5572f288e8f7111a03b2fdddc`  
		Last Modified: Fri, 06 May 2022 19:19:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:813c33aa7f94275843088c57b0e44ea6c190d5296b664d7795f66bf3c3804392
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16056332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ee6ea861df7cd9fff1d948de8590f2bac9f2b90ebea7bc71ef7c7654f2d8d40`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:15:01 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:49:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:49:35 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:49:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:49:42 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:49:42 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:49:42 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:49:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:49:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:49:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:49:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:49:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:49:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:49:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:49:46 GMT
EXPOSE 80
# Fri, 06 May 2022 19:49:46 GMT
EXPOSE 443
# Fri, 06 May 2022 19:49:46 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:49:47 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:49:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b230dd773e10769a2eb3e507260d2470a646efd48a639739ba8852b2915302`  
		Last Modified: Tue, 05 Apr 2022 03:18:10 GMT  
		Size: 291.7 KB (291685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd82040b030d75398d6d6fb1c3d12cc9e25a954a92227895e1e5f7ea54736c20`  
		Last Modified: Fri, 06 May 2022 19:51:07 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583abcfacbc800cc0863a5117f1911222bec7ea3fcaed7c36ce4b94b489c3b3e`  
		Last Modified: Fri, 06 May 2022 19:51:16 GMT  
		Size: 13.1 MB (13136691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6903af22655a77183d11fb6d870f6ebc4776e6d9222e9de261b0a377cb81bbcf`  
		Last Modified: Fri, 06 May 2022 19:51:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:2e61a3ed70ad9a4784ff95cf49efa7ec58255c5263c3faba6a5270a847542a41
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.8 MB (15835582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93c6db987e0721fcd4f557ec160b55012a73d2f69de7198fac316514b27ed58f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:33:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:57:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:57:32 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:57:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:57:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:57:39 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:57:39 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:57:40 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:57:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:57:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:57:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:57:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:57:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:57:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:57:42 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:57:43 GMT
EXPOSE 80
# Fri, 06 May 2022 19:57:43 GMT
EXPOSE 443
# Fri, 06 May 2022 19:57:44 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:57:44 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:57:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03203881a2568530a735b6e0e7a40ebb79adedc5193a675807b04eeb92cc6ed1`  
		Last Modified: Tue, 05 Apr 2022 06:35:07 GMT  
		Size: 290.7 KB (290668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507adf96fcab6911303d2b3d14aeb43223c106ee9901b3e31f30668a4dbd5ffb`  
		Last Modified: Fri, 06 May 2022 19:59:02 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23435dc592c99e66d2e9f715136b809e73116ee6725847ed8fd158135e3283be`  
		Last Modified: Fri, 06 May 2022 19:59:11 GMT  
		Size: 13.1 MB (13114610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e55b7a8b43f4fdfecf61cea01ddddc80930ed485d9aafc41c26f84380f858f3`  
		Last Modified: Fri, 06 May 2022 19:59:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:cda45585c425161575996ee5d954166745d44d39928846423ecdce6b61a9fb4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.5 MB (15523770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:890cdb4fef0cc66aabb117ff1b3e11fb86de5117d28a5b0e64a743efb92c4269`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:12:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:39:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:39:32 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:39:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:39:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:39:37 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:39:38 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:39:39 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:39:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:39:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:39:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:39:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:39:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:39:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:39:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:39:47 GMT
EXPOSE 80
# Fri, 06 May 2022 19:39:48 GMT
EXPOSE 443
# Fri, 06 May 2022 19:39:49 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:39:50 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:39:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83aa37f2341b1e6d98420668c9bc849a47f2c471d159b2303885040bd8d0a92f`  
		Last Modified: Tue, 05 Apr 2022 03:13:38 GMT  
		Size: 291.3 KB (291301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc050d3d6ffb91c2f68db47e3d5f056afad26e465a03ae7e43383df0fc8ad89`  
		Last Modified: Fri, 06 May 2022 19:40:32 GMT  
		Size: 5.8 KB (5753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8adaff0bd78d0b115843dd841c83d1690484b25369e804b1133b838b7ad5ce8f`  
		Last Modified: Fri, 06 May 2022 19:40:35 GMT  
		Size: 12.5 MB (12510086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f703c61da5ec8e48b081aceac2cb64fb25162c2f0ba1ad16a104610b676f50f6`  
		Last Modified: Fri, 06 May 2022 19:40:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:d1ab9f3165d5b23b9ff5bd4fcb74b3f8bbf834ba34c42c58e496b3d33017ca59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15203958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfbb2004b1ba3aace5176af38455ef6b8328a074388b16b35358d61330ad2658`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:08:34 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:16:53 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:16:58 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:17:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:17:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:17:25 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:17:32 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:17:36 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:17:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:17:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:17:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:17:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:17:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:18:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:18:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:18:13 GMT
EXPOSE 80
# Fri, 06 May 2022 19:18:17 GMT
EXPOSE 443
# Fri, 06 May 2022 19:18:19 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:18:22 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:18:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743509d6ced044a369685ebb068417e8757981a39d1b397c7b0182ab89f83528`  
		Last Modified: Tue, 05 Apr 2022 07:11:24 GMT  
		Size: 293.7 KB (293721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b659dd8890d066269209696348c58ed19351199266936a5e81f1991a52333d1`  
		Last Modified: Fri, 06 May 2022 19:19:31 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86272ae554176010d052c51dcc5540948b8e59082743b04ac5bb67d05c3fdcd`  
		Last Modified: Fri, 06 May 2022 19:19:33 GMT  
		Size: 12.1 MB (12093067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff57ff409904cc43937df14c68e6d97e1269adde095e91671fb5438dc58a1808`  
		Last Modified: Fri, 06 May 2022 19:19:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:fbee089e769bc54babbe3ac3217c0e5b60c4a5157b76b0f37aa73cc71486c8fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16129299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f94fa793c943e1cb1c5bda77b0e7077b344648635da2222a1061307e3e61ca96`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:19:41 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:41:25 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:41:25 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:41:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:41:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:41:28 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:41:28 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:41:28 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:41:29 GMT
EXPOSE 80
# Fri, 06 May 2022 19:41:29 GMT
EXPOSE 443
# Fri, 06 May 2022 19:41:30 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:41:30 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:41:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8cc7c7c7ffd67f5740add448d341753330a2abdc6ed06e995cb7d28de381ab`  
		Last Modified: Tue, 05 Apr 2022 06:20:44 GMT  
		Size: 291.8 KB (291821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3d2fae470dbad90c4c4c1262110f14447a47b6e81edc4e0e80ceb50538fe57`  
		Last Modified: Fri, 06 May 2022 19:42:10 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a8f9dbbf38ad9456666a4e6a3eda871b385d4ef76ab6dc25e31030d1daf71c`  
		Last Modified: Fri, 06 May 2022 19:42:12 GMT  
		Size: 13.2 MB (13231118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf07e991258bc58c5e8a5785f741bc746e75848423d2c27d26448015c5887f1`  
		Last Modified: Fri, 06 May 2022 19:42:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.2928; amd64

```console
$ docker pull caddy@sha256:8ad6979cdadd3d080deeb3a2f13d37c23789748ea80b29ac44624cf39bd589ff
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2518898800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8393d2b14b909a4ce523ae0d4999f2a492deb9e76ac12cc8dc111b5f0e3bd74d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:28:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 10 May 2022 23:28:55 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:29:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('4294796c4bd4bed0c593d83606a5413de30f35f88d624e1b1e5b6cd8672ffbcc7a689d7ce4ef30c1abea0e95eda62220faac15d2a6aca0c3e2b418abe7a74118')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 10 May 2022 23:29:54 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 10 May 2022 23:29:56 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 10 May 2022 23:29:57 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Tue, 10 May 2022 23:29:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 10 May 2022 23:29:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 10 May 2022 23:29:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 10 May 2022 23:30:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 10 May 2022 23:30:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 10 May 2022 23:30:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 10 May 2022 23:30:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 10 May 2022 23:30:04 GMT
EXPOSE 80
# Tue, 10 May 2022 23:30:05 GMT
EXPOSE 443
# Tue, 10 May 2022 23:30:06 GMT
EXPOSE 2019
# Tue, 10 May 2022 23:30:47 GMT
RUN caddy version
# Tue, 10 May 2022 23:30:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d722bd7a5ed597b5a9ed7c5144caa608e784120c4442579352b7c2325ce47ffc`  
		Last Modified: Tue, 10 May 2022 23:35:41 GMT  
		Size: 498.2 KB (498231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0dfede5e37c630a175a1c987d90aaf1ec1db8cd7d43e3d63648743c6ace743`  
		Last Modified: Tue, 10 May 2022 23:35:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef201446c9bd5610f78b8e5a1680047ff45fadb77727762c323d5e48d77f9f2`  
		Last Modified: Tue, 10 May 2022 23:35:44 GMT  
		Size: 14.0 MB (14007489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b824e8abcb45a47ada825f0b722a588cbc9d1f68f5536a76b7afed2c5eb15a0c`  
		Last Modified: Tue, 10 May 2022 23:35:39 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b01057f474e19bdcaebab2c156622642945d2c7074276c82de663baeb418143`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520fb9c4921f60cfaea07cfa8d5733cf7f4f0810e56106911d7b25f59e86e997`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74d9e7abc08a32b35b26f8bba23c597b1e19d604766b326f61e77da0b494285`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595304462c9d3aa03aa9e164a98a38be5e1f5307c2981b65aa228101c73ce91b`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e307ee1571a8185932bbd90267a8b8d367f784859d99a2742d44e89e19e8b6c0`  
		Last Modified: Tue, 10 May 2022 23:35:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b335f1fddf0ed6abcc0e715ff827614cc2f0f4bbe8a0e1565145951d841c96`  
		Last Modified: Tue, 10 May 2022 23:35:36 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0974b9a20e0fa84c8a353a7c04992bec9e06825ed808054a358b84409744ba`  
		Last Modified: Tue, 10 May 2022 23:35:35 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d5086c691961c9f1a18b9d161cf8cb3dbd7b581c68ab75760b8c5e62647928`  
		Last Modified: Tue, 10 May 2022 23:35:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9194a8cf5ac8d920d218d9100152393ac6cce9142b15904894374694ae2d2fc`  
		Last Modified: Tue, 10 May 2022 23:35:36 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd07be490606caadc3893d219aee0682d6f8b71b2a4a8f2fb2ca826cdffb74`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b19beef4c4a6634592447260a670c8ee571e59cb775833787d39b815e9ba511`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2dab7fd2beddb5439029e7d8a75fc7c7fe2d3a534a63f51a04f85dd371cd1c`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e195aa5e2a95379397baf57f681e2c39a7c673d3c06d0ff3e4eeed3d8cecee1`  
		Last Modified: Tue, 10 May 2022 23:35:34 GMT  
		Size: 314.6 KB (314586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87827ca78b495430e19218a9e3f7f2837078a77df34bb929124ea20614287d5`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.20348.707; amd64

```console
$ docker pull caddy@sha256:a3894222673d46b3e350553c6b7d4f92ab27b85a87fa1f773e9b090d5774ca9e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2252723203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:063f1879bd2783934ad3ac23aa37bf45f19be756f6b018f4c3a67d2d4a759c7c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:31:41 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 10 May 2022 23:31:42 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:32:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('4294796c4bd4bed0c593d83606a5413de30f35f88d624e1b1e5b6cd8672ffbcc7a689d7ce4ef30c1abea0e95eda62220faac15d2a6aca0c3e2b418abe7a74118')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 10 May 2022 23:32:11 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 10 May 2022 23:32:12 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 10 May 2022 23:32:13 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Tue, 10 May 2022 23:32:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 10 May 2022 23:32:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 10 May 2022 23:32:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 10 May 2022 23:32:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 10 May 2022 23:32:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 10 May 2022 23:32:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 10 May 2022 23:32:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 10 May 2022 23:32:21 GMT
EXPOSE 80
# Tue, 10 May 2022 23:32:22 GMT
EXPOSE 443
# Tue, 10 May 2022 23:32:23 GMT
EXPOSE 2019
# Tue, 10 May 2022 23:32:42 GMT
RUN caddy version
# Tue, 10 May 2022 23:32:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9baa8a196af04dc55746ee82c0774537bce72a589b75d9efce1a4680f03e35`  
		Last Modified: Tue, 10 May 2022 23:36:04 GMT  
		Size: 616.1 KB (616130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe60c7e90fdaeffa9bce60d9a7c7b340dedc357bfb70a2ce8c6d7b8bd0e74a11`  
		Last Modified: Tue, 10 May 2022 23:36:04 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f955bea173999b55d2087a27b9cc80e92bf168918c6e892175c2a75bdbfac933`  
		Last Modified: Tue, 10 May 2022 23:36:07 GMT  
		Size: 14.2 MB (14224642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e1ab4508d5347b929d5a33f71e0f24f653e61c147260200d32e3bd7cdd2340`  
		Last Modified: Tue, 10 May 2022 23:36:02 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8044ca4427c5edfee653001205397a2cc33f8fb4416c16c4a4936317c572ed`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f144416d38a1aa75558e0b93b88fcb3de122ee88349826ee99d596e1b00d9cc0`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32edbcceba80e7a70e44725926012bb70624bb0ae91c85db2766ca2e4c5a5d7c`  
		Last Modified: Tue, 10 May 2022 23:36:02 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd90105a2a3136e4d25d0add2b6fbe5798d51588215367128f1566d66b255289`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e448ed08c6c6ca9f854cb7014ea2e79c04e83f1905f78f578b67303b709fa3`  
		Last Modified: Tue, 10 May 2022 23:36:00 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d49b1b3778cd2ebf32521f530e29275a9a473afa997654b32338ff4349bf5c`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2112945425b7d069bc5705be1345e5ad6e27206e1531b10d0bc92d9c69ea9c3`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7243327255edd82b277f456085138a672f5a43d616e80f73156c8eb31139121d`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1a14330360d7ab3af40d4fb6f2de975e42e05f8e4cb064cc49fe1d9446e6b1`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808ce6a15ca3e6ad031229bcad8a3ed69171a7005c05ef4e77ffcfd777e9d1f7`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdfcf611e614d42a256d103775233f59ab7bb6ad0b00ca2f915bf739600f8d6`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3811622d464d497ce363eed806c75f9b994cd1d04b3009b2d0671af2863ebd0`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b006092864e6cfdfedd054a2635236c62958e97de81c720d9e38772276ee11`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 325.9 KB (325870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2afb0ece27a359f16126f263176baa74c3d3f2f2733cce186e4e31ad0eca4f8`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:285398d41e72fa7778b741796f7a0892454ea9bdc4ed67b25cec85cd7494f9cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2928; amd64
	-	windows version 10.0.20348.707; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.2928; amd64

```console
$ docker pull caddy@sha256:8ad6979cdadd3d080deeb3a2f13d37c23789748ea80b29ac44624cf39bd589ff
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2518898800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8393d2b14b909a4ce523ae0d4999f2a492deb9e76ac12cc8dc111b5f0e3bd74d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:28:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 10 May 2022 23:28:55 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:29:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('4294796c4bd4bed0c593d83606a5413de30f35f88d624e1b1e5b6cd8672ffbcc7a689d7ce4ef30c1abea0e95eda62220faac15d2a6aca0c3e2b418abe7a74118')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 10 May 2022 23:29:54 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 10 May 2022 23:29:56 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 10 May 2022 23:29:57 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Tue, 10 May 2022 23:29:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 10 May 2022 23:29:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 10 May 2022 23:29:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 10 May 2022 23:30:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 10 May 2022 23:30:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 10 May 2022 23:30:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 10 May 2022 23:30:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 10 May 2022 23:30:04 GMT
EXPOSE 80
# Tue, 10 May 2022 23:30:05 GMT
EXPOSE 443
# Tue, 10 May 2022 23:30:06 GMT
EXPOSE 2019
# Tue, 10 May 2022 23:30:47 GMT
RUN caddy version
# Tue, 10 May 2022 23:30:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d722bd7a5ed597b5a9ed7c5144caa608e784120c4442579352b7c2325ce47ffc`  
		Last Modified: Tue, 10 May 2022 23:35:41 GMT  
		Size: 498.2 KB (498231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0dfede5e37c630a175a1c987d90aaf1ec1db8cd7d43e3d63648743c6ace743`  
		Last Modified: Tue, 10 May 2022 23:35:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef201446c9bd5610f78b8e5a1680047ff45fadb77727762c323d5e48d77f9f2`  
		Last Modified: Tue, 10 May 2022 23:35:44 GMT  
		Size: 14.0 MB (14007489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b824e8abcb45a47ada825f0b722a588cbc9d1f68f5536a76b7afed2c5eb15a0c`  
		Last Modified: Tue, 10 May 2022 23:35:39 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b01057f474e19bdcaebab2c156622642945d2c7074276c82de663baeb418143`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520fb9c4921f60cfaea07cfa8d5733cf7f4f0810e56106911d7b25f59e86e997`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74d9e7abc08a32b35b26f8bba23c597b1e19d604766b326f61e77da0b494285`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595304462c9d3aa03aa9e164a98a38be5e1f5307c2981b65aa228101c73ce91b`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e307ee1571a8185932bbd90267a8b8d367f784859d99a2742d44e89e19e8b6c0`  
		Last Modified: Tue, 10 May 2022 23:35:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b335f1fddf0ed6abcc0e715ff827614cc2f0f4bbe8a0e1565145951d841c96`  
		Last Modified: Tue, 10 May 2022 23:35:36 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0974b9a20e0fa84c8a353a7c04992bec9e06825ed808054a358b84409744ba`  
		Last Modified: Tue, 10 May 2022 23:35:35 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d5086c691961c9f1a18b9d161cf8cb3dbd7b581c68ab75760b8c5e62647928`  
		Last Modified: Tue, 10 May 2022 23:35:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9194a8cf5ac8d920d218d9100152393ac6cce9142b15904894374694ae2d2fc`  
		Last Modified: Tue, 10 May 2022 23:35:36 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd07be490606caadc3893d219aee0682d6f8b71b2a4a8f2fb2ca826cdffb74`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b19beef4c4a6634592447260a670c8ee571e59cb775833787d39b815e9ba511`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2dab7fd2beddb5439029e7d8a75fc7c7fe2d3a534a63f51a04f85dd371cd1c`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e195aa5e2a95379397baf57f681e2c39a7c673d3c06d0ff3e4eeed3d8cecee1`  
		Last Modified: Tue, 10 May 2022 23:35:34 GMT  
		Size: 314.6 KB (314586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87827ca78b495430e19218a9e3f7f2837078a77df34bb929124ea20614287d5`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.20348.707; amd64

```console
$ docker pull caddy@sha256:a3894222673d46b3e350553c6b7d4f92ab27b85a87fa1f773e9b090d5774ca9e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2252723203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:063f1879bd2783934ad3ac23aa37bf45f19be756f6b018f4c3a67d2d4a759c7c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:31:41 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 10 May 2022 23:31:42 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:32:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('4294796c4bd4bed0c593d83606a5413de30f35f88d624e1b1e5b6cd8672ffbcc7a689d7ce4ef30c1abea0e95eda62220faac15d2a6aca0c3e2b418abe7a74118')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 10 May 2022 23:32:11 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 10 May 2022 23:32:12 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 10 May 2022 23:32:13 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Tue, 10 May 2022 23:32:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 10 May 2022 23:32:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 10 May 2022 23:32:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 10 May 2022 23:32:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 10 May 2022 23:32:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 10 May 2022 23:32:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 10 May 2022 23:32:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 10 May 2022 23:32:21 GMT
EXPOSE 80
# Tue, 10 May 2022 23:32:22 GMT
EXPOSE 443
# Tue, 10 May 2022 23:32:23 GMT
EXPOSE 2019
# Tue, 10 May 2022 23:32:42 GMT
RUN caddy version
# Tue, 10 May 2022 23:32:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9baa8a196af04dc55746ee82c0774537bce72a589b75d9efce1a4680f03e35`  
		Last Modified: Tue, 10 May 2022 23:36:04 GMT  
		Size: 616.1 KB (616130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe60c7e90fdaeffa9bce60d9a7c7b340dedc357bfb70a2ce8c6d7b8bd0e74a11`  
		Last Modified: Tue, 10 May 2022 23:36:04 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f955bea173999b55d2087a27b9cc80e92bf168918c6e892175c2a75bdbfac933`  
		Last Modified: Tue, 10 May 2022 23:36:07 GMT  
		Size: 14.2 MB (14224642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e1ab4508d5347b929d5a33f71e0f24f653e61c147260200d32e3bd7cdd2340`  
		Last Modified: Tue, 10 May 2022 23:36:02 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8044ca4427c5edfee653001205397a2cc33f8fb4416c16c4a4936317c572ed`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f144416d38a1aa75558e0b93b88fcb3de122ee88349826ee99d596e1b00d9cc0`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32edbcceba80e7a70e44725926012bb70624bb0ae91c85db2766ca2e4c5a5d7c`  
		Last Modified: Tue, 10 May 2022 23:36:02 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd90105a2a3136e4d25d0add2b6fbe5798d51588215367128f1566d66b255289`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e448ed08c6c6ca9f854cb7014ea2e79c04e83f1905f78f578b67303b709fa3`  
		Last Modified: Tue, 10 May 2022 23:36:00 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d49b1b3778cd2ebf32521f530e29275a9a473afa997654b32338ff4349bf5c`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2112945425b7d069bc5705be1345e5ad6e27206e1531b10d0bc92d9c69ea9c3`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7243327255edd82b277f456085138a672f5a43d616e80f73156c8eb31139121d`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1a14330360d7ab3af40d4fb6f2de975e42e05f8e4cb064cc49fe1d9446e6b1`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808ce6a15ca3e6ad031229bcad8a3ed69171a7005c05ef4e77ffcfd777e9d1f7`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdfcf611e614d42a256d103775233f59ab7bb6ad0b00ca2f915bf739600f8d6`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3811622d464d497ce363eed806c75f9b994cd1d04b3009b2d0671af2863ebd0`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b006092864e6cfdfedd054a2635236c62958e97de81c720d9e38772276ee11`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 325.9 KB (325870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2afb0ece27a359f16126f263176baa74c3d3f2f2733cce186e4e31ad0eca4f8`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:61aa7b1019d479a8c0c21f043ffbec427336684486cad3858e71de43f3962e7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull caddy@sha256:8ad6979cdadd3d080deeb3a2f13d37c23789748ea80b29ac44624cf39bd589ff
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2518898800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8393d2b14b909a4ce523ae0d4999f2a492deb9e76ac12cc8dc111b5f0e3bd74d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:28:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 10 May 2022 23:28:55 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:29:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('4294796c4bd4bed0c593d83606a5413de30f35f88d624e1b1e5b6cd8672ffbcc7a689d7ce4ef30c1abea0e95eda62220faac15d2a6aca0c3e2b418abe7a74118')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 10 May 2022 23:29:54 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 10 May 2022 23:29:56 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 10 May 2022 23:29:57 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Tue, 10 May 2022 23:29:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 10 May 2022 23:29:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 10 May 2022 23:29:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 10 May 2022 23:30:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 10 May 2022 23:30:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 10 May 2022 23:30:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 10 May 2022 23:30:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 10 May 2022 23:30:04 GMT
EXPOSE 80
# Tue, 10 May 2022 23:30:05 GMT
EXPOSE 443
# Tue, 10 May 2022 23:30:06 GMT
EXPOSE 2019
# Tue, 10 May 2022 23:30:47 GMT
RUN caddy version
# Tue, 10 May 2022 23:30:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d722bd7a5ed597b5a9ed7c5144caa608e784120c4442579352b7c2325ce47ffc`  
		Last Modified: Tue, 10 May 2022 23:35:41 GMT  
		Size: 498.2 KB (498231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0dfede5e37c630a175a1c987d90aaf1ec1db8cd7d43e3d63648743c6ace743`  
		Last Modified: Tue, 10 May 2022 23:35:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef201446c9bd5610f78b8e5a1680047ff45fadb77727762c323d5e48d77f9f2`  
		Last Modified: Tue, 10 May 2022 23:35:44 GMT  
		Size: 14.0 MB (14007489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b824e8abcb45a47ada825f0b722a588cbc9d1f68f5536a76b7afed2c5eb15a0c`  
		Last Modified: Tue, 10 May 2022 23:35:39 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b01057f474e19bdcaebab2c156622642945d2c7074276c82de663baeb418143`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520fb9c4921f60cfaea07cfa8d5733cf7f4f0810e56106911d7b25f59e86e997`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74d9e7abc08a32b35b26f8bba23c597b1e19d604766b326f61e77da0b494285`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595304462c9d3aa03aa9e164a98a38be5e1f5307c2981b65aa228101c73ce91b`  
		Last Modified: Tue, 10 May 2022 23:35:38 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e307ee1571a8185932bbd90267a8b8d367f784859d99a2742d44e89e19e8b6c0`  
		Last Modified: Tue, 10 May 2022 23:35:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b335f1fddf0ed6abcc0e715ff827614cc2f0f4bbe8a0e1565145951d841c96`  
		Last Modified: Tue, 10 May 2022 23:35:36 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0974b9a20e0fa84c8a353a7c04992bec9e06825ed808054a358b84409744ba`  
		Last Modified: Tue, 10 May 2022 23:35:35 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d5086c691961c9f1a18b9d161cf8cb3dbd7b581c68ab75760b8c5e62647928`  
		Last Modified: Tue, 10 May 2022 23:35:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9194a8cf5ac8d920d218d9100152393ac6cce9142b15904894374694ae2d2fc`  
		Last Modified: Tue, 10 May 2022 23:35:36 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd07be490606caadc3893d219aee0682d6f8b71b2a4a8f2fb2ca826cdffb74`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b19beef4c4a6634592447260a670c8ee571e59cb775833787d39b815e9ba511`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2dab7fd2beddb5439029e7d8a75fc7c7fe2d3a534a63f51a04f85dd371cd1c`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e195aa5e2a95379397baf57f681e2c39a7c673d3c06d0ff3e4eeed3d8cecee1`  
		Last Modified: Tue, 10 May 2022 23:35:34 GMT  
		Size: 314.6 KB (314586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87827ca78b495430e19218a9e3f7f2837078a77df34bb929124ea20614287d5`  
		Last Modified: Tue, 10 May 2022 23:35:33 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:88a75e54141f2e7531d3262b5a00a17002af383f24e29dab09212e4cbbfa2fdd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `caddy:windowsservercore-ltsc2022` - windows version 10.0.20348.707; amd64

```console
$ docker pull caddy@sha256:a3894222673d46b3e350553c6b7d4f92ab27b85a87fa1f773e9b090d5774ca9e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2252723203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:063f1879bd2783934ad3ac23aa37bf45f19be756f6b018f4c3a67d2d4a759c7c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:31:41 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 10 May 2022 23:31:42 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:32:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('4294796c4bd4bed0c593d83606a5413de30f35f88d624e1b1e5b6cd8672ffbcc7a689d7ce4ef30c1abea0e95eda62220faac15d2a6aca0c3e2b418abe7a74118')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 10 May 2022 23:32:11 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 10 May 2022 23:32:12 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 10 May 2022 23:32:13 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Tue, 10 May 2022 23:32:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 10 May 2022 23:32:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 10 May 2022 23:32:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 10 May 2022 23:32:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 10 May 2022 23:32:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 10 May 2022 23:32:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 10 May 2022 23:32:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 10 May 2022 23:32:21 GMT
EXPOSE 80
# Tue, 10 May 2022 23:32:22 GMT
EXPOSE 443
# Tue, 10 May 2022 23:32:23 GMT
EXPOSE 2019
# Tue, 10 May 2022 23:32:42 GMT
RUN caddy version
# Tue, 10 May 2022 23:32:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9baa8a196af04dc55746ee82c0774537bce72a589b75d9efce1a4680f03e35`  
		Last Modified: Tue, 10 May 2022 23:36:04 GMT  
		Size: 616.1 KB (616130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe60c7e90fdaeffa9bce60d9a7c7b340dedc357bfb70a2ce8c6d7b8bd0e74a11`  
		Last Modified: Tue, 10 May 2022 23:36:04 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f955bea173999b55d2087a27b9cc80e92bf168918c6e892175c2a75bdbfac933`  
		Last Modified: Tue, 10 May 2022 23:36:07 GMT  
		Size: 14.2 MB (14224642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e1ab4508d5347b929d5a33f71e0f24f653e61c147260200d32e3bd7cdd2340`  
		Last Modified: Tue, 10 May 2022 23:36:02 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8044ca4427c5edfee653001205397a2cc33f8fb4416c16c4a4936317c572ed`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f144416d38a1aa75558e0b93b88fcb3de122ee88349826ee99d596e1b00d9cc0`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32edbcceba80e7a70e44725926012bb70624bb0ae91c85db2766ca2e4c5a5d7c`  
		Last Modified: Tue, 10 May 2022 23:36:02 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd90105a2a3136e4d25d0add2b6fbe5798d51588215367128f1566d66b255289`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e448ed08c6c6ca9f854cb7014ea2e79c04e83f1905f78f578b67303b709fa3`  
		Last Modified: Tue, 10 May 2022 23:36:00 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d49b1b3778cd2ebf32521f530e29275a9a473afa997654b32338ff4349bf5c`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2112945425b7d069bc5705be1345e5ad6e27206e1531b10d0bc92d9c69ea9c3`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7243327255edd82b277f456085138a672f5a43d616e80f73156c8eb31139121d`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1a14330360d7ab3af40d4fb6f2de975e42e05f8e4cb064cc49fe1d9446e6b1`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808ce6a15ca3e6ad031229bcad8a3ed69171a7005c05ef4e77ffcfd777e9d1f7`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdfcf611e614d42a256d103775233f59ab7bb6ad0b00ca2f915bf739600f8d6`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3811622d464d497ce363eed806c75f9b994cd1d04b3009b2d0671af2863ebd0`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b006092864e6cfdfedd054a2635236c62958e97de81c720d9e38772276ee11`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 325.9 KB (325870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2afb0ece27a359f16126f263176baa74c3d3f2f2733cce186e4e31ad0eca4f8`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
