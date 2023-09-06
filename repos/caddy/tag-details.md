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
-	[`caddy:2.7`](#caddy27)
-	[`caddy:2.7-alpine`](#caddy27-alpine)
-	[`caddy:2.7-builder`](#caddy27-builder)
-	[`caddy:2.7-builder-alpine`](#caddy27-builder-alpine)
-	[`caddy:2.7-builder-windowsservercore-1809`](#caddy27-builder-windowsservercore-1809)
-	[`caddy:2.7-builder-windowsservercore-ltsc2022`](#caddy27-builder-windowsservercore-ltsc2022)
-	[`caddy:2.7-windowsservercore`](#caddy27-windowsservercore)
-	[`caddy:2.7-windowsservercore-1809`](#caddy27-windowsservercore-1809)
-	[`caddy:2.7-windowsservercore-ltsc2022`](#caddy27-windowsservercore-ltsc2022)
-	[`caddy:2.7.4`](#caddy274)
-	[`caddy:2.7.4-alpine`](#caddy274-alpine)
-	[`caddy:2.7.4-builder`](#caddy274-builder)
-	[`caddy:2.7.4-builder-alpine`](#caddy274-builder-alpine)
-	[`caddy:2.7.4-builder-windowsservercore-1809`](#caddy274-builder-windowsservercore-1809)
-	[`caddy:2.7.4-builder-windowsservercore-ltsc2022`](#caddy274-builder-windowsservercore-ltsc2022)
-	[`caddy:2.7.4-windowsservercore`](#caddy274-windowsservercore)
-	[`caddy:2.7.4-windowsservercore-1809`](#caddy274-windowsservercore-1809)
-	[`caddy:2.7.4-windowsservercore-ltsc2022`](#caddy274-windowsservercore-ltsc2022)
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
$ docker pull caddy@sha256:2332c4ebc4ae778b9697043d3fa3aaef6879dd17abc03200285af9d315353008
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4737; amd64
	-	windows version 10.0.20348.1906; amd64

### `caddy:2` - linux; amd64

```console
$ docker pull caddy@sha256:733fe94133c4bd22c6ee8f9b9802bce8fede5e7b766bebde205a45dd4ac04aea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18363908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1e1b7ae170b7d7d7e524717fe978e0090023cc82a7d9ffe48e344b0351a3ee1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:09:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 18:20:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:19:38 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:19:41 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:19:41 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:19:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:19:42 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:19:42 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:19:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0aa7b81ef11c65f43b0b58323a33dd9e07eb785529f0d75b452f87a309db00c`  
		Last Modified: Mon, 07 Aug 2023 20:09:40 GMT  
		Size: 350.8 KB (350844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b3b3e68e52dc5ab939c72a9bbac39cff4bef4b87de399ddf28657471df6845`  
		Last Modified: Mon, 14 Aug 2023 18:20:42 GMT  
		Size: 7.5 KB (7502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c55d3259542348ddb70edc18dda7d48aeca5654962aed568a7034f3667d2ca`  
		Last Modified: Thu, 17 Aug 2023 22:20:10 GMT  
		Size: 14.6 MB (14603949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:dd029220558032e5d1f91173d32a0078dad12ec9b5114bef422ed4cdf05dec52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17314204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1de0523ee8d8173472fb08aa9a74a37bcd054af2b796b7631d847ba8a46986b5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:38:27 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:49:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:49:12 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:49:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:49:16 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:49:16 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:49:17 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:49:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172ef460a93549b8a3e73f6a515bccad93512788d1e8f095e7230ba41967c25a`  
		Last Modified: Wed, 09 Aug 2023 03:38:53 GMT  
		Size: 347.7 KB (347686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7aae78767a581df85fd1a51ccd646619aec320896ca016ef0f05a41b16bcbfe`  
		Last Modified: Mon, 14 Aug 2023 17:49:36 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82560a340155261ecbd1d99d87890c5aa0cfd64d571e1dcafc03e3b6a8132d48`  
		Last Modified: Thu, 17 Aug 2023 22:49:41 GMT  
		Size: 13.8 MB (13814204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:24649e9de43354963118f9cdf6ad1f4522c6993735f316763a2f5d1f76cba267
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17042831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb4a48fd29d50802cbf030949e2c9767eb6888e8412330f64246f322bc3b49c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:51:41 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:57:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:57:18 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:57:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:57:22 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:57:22 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:57:24 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:57:24 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:57:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a47b73e04459258b08555443754e92e2db20bde113c58ca18e1a6f07878f72`  
		Last Modified: Tue, 08 Aug 2023 01:52:05 GMT  
		Size: 344.5 KB (344462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e1b3e18d5e992f1805072b2d52405d575830bdce21726ef99dea99e31d8277`  
		Last Modified: Mon, 14 Aug 2023 17:57:42 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5879767a5d1969beb154b9a4991a767b0ed5be0c9739a972f07d03e825312fa5`  
		Last Modified: Thu, 17 Aug 2023 22:57:51 GMT  
		Size: 13.8 MB (13791384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:ed967fcd1968be6dc4699ff835cdd2d6f3f49105b9677f878c8a6960fd1a0643
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17162547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed7b6600470cab547aa1090baa39a6192ec83119989884ac742a63ed23be3da2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:09:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:39:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:39:17 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:39:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:39:19 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:39:19 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:39:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:39:20 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:39:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a699f78cfb85f60e17fc7c13495876ea0cb4495bbe39e8c65f3e8559b0d7169`  
		Last Modified: Mon, 07 Aug 2023 21:09:34 GMT  
		Size: 360.6 KB (360642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7488af8b96c79b6db13955a0302653c4e9f314d0833201984ae06c1ed697f06`  
		Last Modified: Mon, 14 Aug 2023 17:39:41 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597bfc484ba18727d2df98120cb9d559f346ade9e3a23be6a9af3e76dca89edd`  
		Last Modified: Thu, 17 Aug 2023 22:39:42 GMT  
		Size: 13.5 MB (13463635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:c3679836562d0252e6341a112d2729b8dae0eae550449bfe91fe2798171fd4ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16944934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc5ac831dce746cd0f4448640b7edaf0ce9457d09618e246ba72ee76ea63dcbe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:44:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 18:18:00 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:16:24 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:16:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:16:29 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:16:29 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:16:29 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:16:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:16:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:16:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:16:32 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:16:33 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:16:33 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:16:34 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:16:34 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:16:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f40714f45e39ac41e865ccbf2877db62255ce5a5c36a47eadf00b9d174f042`  
		Last Modified: Tue, 08 Aug 2023 00:45:18 GMT  
		Size: 362.2 KB (362173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d19953b5eb53ddaa0e25905527dc138e0c4111467bb7d71f81fa94976091351`  
		Last Modified: Mon, 14 Aug 2023 18:18:54 GMT  
		Size: 7.5 KB (7509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf4bf695323732c5ce84bbb0b976c5cd981eaf6814515a86f521af4a0e64582`  
		Last Modified: Thu, 17 Aug 2023 22:17:22 GMT  
		Size: 13.2 MB (13229001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:ca7ab0dcf4ab146df48cfa8ae6e07fed804feeed4a36358fa652c8eac52b40da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17720356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d4d019ffc0cd69ea8c5d3b8fb0a39c89d3aa1b2037c1012a9ba4bed6abb94dc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:14:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:41:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:41:35 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:41:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:41:39 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:41:39 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:41:39 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:41:40 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:41:41 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:41:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df19abd0ca1d4a821a4174a2c0831a57d6fd584073f056abcae085a51f0b3848`  
		Last Modified: Mon, 07 Aug 2023 20:14:50 GMT  
		Size: 354.9 KB (354950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308478977890baa82477ee70a3065fb9da2080efcc95facf1a87ac021b06a8e9`  
		Last Modified: Mon, 14 Aug 2023 17:42:17 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2394cd7c9416df19c45596c558f5a7ee05adc5a7fd166f58dcbf26f1ac6ecae6`  
		Last Modified: Thu, 17 Aug 2023 22:42:16 GMT  
		Size: 14.1 MB (14143708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:8d641d87b059de975dc94ff579d47434e347b333b33a4a8f15cd679c062a14c0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2011934670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e21b2ad9f1a3657d84dd869da76d22704a2848d4a92f831acbfef09e26e80cc6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 14 Aug 2023 18:16:58 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 17 Aug 2023 22:14:59 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:16:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 17 Aug 2023 22:16:13 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 17 Aug 2023 22:16:14 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 17 Aug 2023 22:16:15 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:16:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:16:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:16:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:16:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:16:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:16:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:16:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:16:21 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:16:22 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:16:23 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:16:24 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:17:19 GMT
RUN caddy version
# Thu, 17 Aug 2023 22:17:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d698e8ba8bfd4c31116f0d2c87cfcf2ff17baa1a5c678b116b3aa1ac8ed73d`  
		Last Modified: Mon, 14 Aug 2023 18:23:17 GMT  
		Size: 483.6 KB (483626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dcf545f7c90cab6f6962d3099898462129da2e6b06a80802d52ff1e9d2fca08`  
		Last Modified: Thu, 17 Aug 2023 22:21:12 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65ecc8b4521923b522dd6392a862d0dff9edd10c1e3b520de8f130de2170880`  
		Last Modified: Thu, 17 Aug 2023 22:21:16 GMT  
		Size: 15.2 MB (15201779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ddd9c690b84a4a4744ec5ac91059e12e1aa92378220080fcfbf616c59b4c26`  
		Last Modified: Thu, 17 Aug 2023 22:21:12 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63adbcb9cba5e8d67eac5e059c7bbb9dfe3040f0933afb5e1f8cb7d4c211b4a`  
		Last Modified: Thu, 17 Aug 2023 22:21:11 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e15ff22938f514e6118606619ff28e9e5ee145d6f3dc6de1de62ea4051575c1`  
		Last Modified: Thu, 17 Aug 2023 22:21:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438a6cab105b637f625a3fd00d7ecaa6792ad5dc120bf1be36e7d6e19ee44b4d`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfd206f96497c8e0730c72c36ecedea57379a6a219903785dc1478b50b3945`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e651df7142dc872814a59faff8cf791ab4e4413ee6a9b043fe02a2af9da24fe`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b7f62d857ed7e15d08d52d1ef08f3c21e25751d17e8a5418c02f6adc366eab`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6347f1227dc933d98b8f02d22cd440529284e7c8e415e96cee265ae2c7445b3`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2776f9f89b2242d27c9c49da3465d2ff6acb224dd3315837bda709f3fa0aa4ff`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aaab02f29add47735607e798c40625216306d00d57988d1ece40f43b93f706c`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ed26555e0c9e51aa5dbf4125ef3ea56c6d84274b4d8160ce10c3c0d9e7106d`  
		Last Modified: Thu, 17 Aug 2023 22:21:08 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392c0484ea6d941786f507e72c143bd1c64d4c42bcd773bd745330a55b89d356`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef07137395441a56a870d882d84faac751156b0486c6528fa18b6d706ff250d8`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2950cf3d51ba47c2b41415fccf9b67e813735f67ccc34a0ce5f1a1a4a34e56dc`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25de03b5a8b8f2752cde31b881d457ec5900438b781cc65cda3aca9444b2377f`  
		Last Modified: Thu, 17 Aug 2023 22:21:07 GMT  
		Size: 269.9 KB (269882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f3d70fb1dd11e79f9128736ada85993e1b4fd603b2f8164aac49ac1efda548`  
		Last Modified: Thu, 17 Aug 2023 22:21:07 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:f4791cb0179b98b28e760842405262d782735176b147c84f26709bd1361c8798
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1813299019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b759bf39605cbc0d0ceaaa8eda1623452b1acd67deb11c0d22defff59f2058`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 14 Aug 2023 18:19:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 17 Aug 2023 22:17:27 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:17:55 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 17 Aug 2023 22:17:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 17 Aug 2023 22:17:56 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 17 Aug 2023 22:17:57 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:17:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:17:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:17:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:18:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:18:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:18:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:18:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:18:04 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:18:04 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:18:05 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:18:06 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:18:21 GMT
RUN caddy version
# Thu, 17 Aug 2023 22:18:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c23e01ee014d9e05e276268c94980b00a0720fcb5488a368b20ee74701ed78`  
		Last Modified: Mon, 14 Aug 2023 18:23:42 GMT  
		Size: 461.2 KB (461170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8a7576f0b2ff121a0e9658821e52a7b356abbd90c9215b750ab7fc2127f6ae`  
		Last Modified: Thu, 17 Aug 2023 22:21:41 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ecc6db59a89a0a9f61364702d6af7202fa4f3f742ec6dff93c3a5b53e3826`  
		Last Modified: Thu, 17 Aug 2023 22:21:44 GMT  
		Size: 15.2 MB (15169088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9323e4528d7a59819754484fdbeb047240a6f1f0dd262b734a226a4249dc0a0`  
		Last Modified: Thu, 17 Aug 2023 22:21:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb3a3b69dd93b979cdcd1e0759ee1199bc8d5a510a6ce9bca3856201d747468`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56ce33676578802911228ae7aba31fe1898897ede8c69e12a0959a37a11d130`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c896eeb3f2c45b2bba4fe5e5da02be1289c4cabcf574a38c19d1616ebf552d4c`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6563dd3d5f912ae2b7bd629d2dc731df89b1dd107e2cbb85dee24a0d5c550a1`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420011263062842c72720998f13fa245d9bef077622fde4e17cc60cef3e00bce`  
		Last Modified: Thu, 17 Aug 2023 22:21:38 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2385fc0cb7a281a35df415654aba711bf70fa23b963faf0a3f0055d760f5c41c`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a58351f25f399f8a9399e60dd315cd8c695972a9e51f2271e3377151cf621d`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506eb3a97b70fc7dc1c1c3464a89512890cd48c354658e58e61d5acfee63f1c3`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86cf8c25cfcaf858db6ffd2630a26ca3a13ad2fdc941a01438ea9ea80ccb20c`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcedddef9863d16c4d713280050f604b44968bc253844c27e46cb8871eb17a99`  
		Last Modified: Thu, 17 Aug 2023 22:21:36 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d01313141e38a9b2b15a3e831a2d11a3eb47611bf99b0677be3c49693984f64`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504a80bc0f7aa0c98a143033f551be8fcf0653046e7313c0de080b82ad97ad52`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280053e45030e2421ea4d1cdfd721c24f40d30518b1ce8af7e0811363daf6eca`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0d07466cd8f053bf957a35cbe340d419f5c2f6ff48565bb8a5b255998e3e94`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 280.9 KB (280938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad52776067d7be890960cfd7082041a93a802b96fea6d31fc724192c49eb00`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:7e01c08308bc94c1ef3e495f0b2ba469d1f7e8d1a4f2caa2fbe189edf48866a6
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
$ docker pull caddy@sha256:733fe94133c4bd22c6ee8f9b9802bce8fede5e7b766bebde205a45dd4ac04aea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18363908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1e1b7ae170b7d7d7e524717fe978e0090023cc82a7d9ffe48e344b0351a3ee1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:09:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 18:20:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:19:38 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:19:41 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:19:41 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:19:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:19:42 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:19:42 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:19:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0aa7b81ef11c65f43b0b58323a33dd9e07eb785529f0d75b452f87a309db00c`  
		Last Modified: Mon, 07 Aug 2023 20:09:40 GMT  
		Size: 350.8 KB (350844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b3b3e68e52dc5ab939c72a9bbac39cff4bef4b87de399ddf28657471df6845`  
		Last Modified: Mon, 14 Aug 2023 18:20:42 GMT  
		Size: 7.5 KB (7502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c55d3259542348ddb70edc18dda7d48aeca5654962aed568a7034f3667d2ca`  
		Last Modified: Thu, 17 Aug 2023 22:20:10 GMT  
		Size: 14.6 MB (14603949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:dd029220558032e5d1f91173d32a0078dad12ec9b5114bef422ed4cdf05dec52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17314204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1de0523ee8d8173472fb08aa9a74a37bcd054af2b796b7631d847ba8a46986b5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:38:27 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:49:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:49:12 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:49:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:49:16 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:49:16 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:49:17 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:49:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172ef460a93549b8a3e73f6a515bccad93512788d1e8f095e7230ba41967c25a`  
		Last Modified: Wed, 09 Aug 2023 03:38:53 GMT  
		Size: 347.7 KB (347686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7aae78767a581df85fd1a51ccd646619aec320896ca016ef0f05a41b16bcbfe`  
		Last Modified: Mon, 14 Aug 2023 17:49:36 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82560a340155261ecbd1d99d87890c5aa0cfd64d571e1dcafc03e3b6a8132d48`  
		Last Modified: Thu, 17 Aug 2023 22:49:41 GMT  
		Size: 13.8 MB (13814204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:24649e9de43354963118f9cdf6ad1f4522c6993735f316763a2f5d1f76cba267
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17042831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb4a48fd29d50802cbf030949e2c9767eb6888e8412330f64246f322bc3b49c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:51:41 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:57:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:57:18 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:57:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:57:22 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:57:22 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:57:24 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:57:24 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:57:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a47b73e04459258b08555443754e92e2db20bde113c58ca18e1a6f07878f72`  
		Last Modified: Tue, 08 Aug 2023 01:52:05 GMT  
		Size: 344.5 KB (344462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e1b3e18d5e992f1805072b2d52405d575830bdce21726ef99dea99e31d8277`  
		Last Modified: Mon, 14 Aug 2023 17:57:42 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5879767a5d1969beb154b9a4991a767b0ed5be0c9739a972f07d03e825312fa5`  
		Last Modified: Thu, 17 Aug 2023 22:57:51 GMT  
		Size: 13.8 MB (13791384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:ed967fcd1968be6dc4699ff835cdd2d6f3f49105b9677f878c8a6960fd1a0643
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17162547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed7b6600470cab547aa1090baa39a6192ec83119989884ac742a63ed23be3da2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:09:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:39:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:39:17 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:39:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:39:19 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:39:19 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:39:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:39:20 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:39:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a699f78cfb85f60e17fc7c13495876ea0cb4495bbe39e8c65f3e8559b0d7169`  
		Last Modified: Mon, 07 Aug 2023 21:09:34 GMT  
		Size: 360.6 KB (360642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7488af8b96c79b6db13955a0302653c4e9f314d0833201984ae06c1ed697f06`  
		Last Modified: Mon, 14 Aug 2023 17:39:41 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597bfc484ba18727d2df98120cb9d559f346ade9e3a23be6a9af3e76dca89edd`  
		Last Modified: Thu, 17 Aug 2023 22:39:42 GMT  
		Size: 13.5 MB (13463635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:c3679836562d0252e6341a112d2729b8dae0eae550449bfe91fe2798171fd4ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16944934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc5ac831dce746cd0f4448640b7edaf0ce9457d09618e246ba72ee76ea63dcbe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:44:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 18:18:00 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:16:24 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:16:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:16:29 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:16:29 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:16:29 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:16:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:16:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:16:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:16:32 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:16:33 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:16:33 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:16:34 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:16:34 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:16:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f40714f45e39ac41e865ccbf2877db62255ce5a5c36a47eadf00b9d174f042`  
		Last Modified: Tue, 08 Aug 2023 00:45:18 GMT  
		Size: 362.2 KB (362173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d19953b5eb53ddaa0e25905527dc138e0c4111467bb7d71f81fa94976091351`  
		Last Modified: Mon, 14 Aug 2023 18:18:54 GMT  
		Size: 7.5 KB (7509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf4bf695323732c5ce84bbb0b976c5cd981eaf6814515a86f521af4a0e64582`  
		Last Modified: Thu, 17 Aug 2023 22:17:22 GMT  
		Size: 13.2 MB (13229001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:ca7ab0dcf4ab146df48cfa8ae6e07fed804feeed4a36358fa652c8eac52b40da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17720356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d4d019ffc0cd69ea8c5d3b8fb0a39c89d3aa1b2037c1012a9ba4bed6abb94dc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:14:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:41:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:41:35 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:41:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:41:39 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:41:39 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:41:39 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:41:40 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:41:41 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:41:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df19abd0ca1d4a821a4174a2c0831a57d6fd584073f056abcae085a51f0b3848`  
		Last Modified: Mon, 07 Aug 2023 20:14:50 GMT  
		Size: 354.9 KB (354950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308478977890baa82477ee70a3065fb9da2080efcc95facf1a87ac021b06a8e9`  
		Last Modified: Mon, 14 Aug 2023 17:42:17 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2394cd7c9416df19c45596c558f5a7ee05adc5a7fd166f58dcbf26f1ac6ecae6`  
		Last Modified: Thu, 17 Aug 2023 22:42:16 GMT  
		Size: 14.1 MB (14143708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:eafc66404950e4170122aba0977f7079d888e544bed6df61a144b50bcf06bbb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4737; amd64
	-	windows version 10.0.20348.1906; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:716dc5ded2a0c7090ac3cf0d298122538ac67a0152c97b88a17520c2b0419d82
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76949834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0789fd27a45de2db1b44ab683c8b91c2f63b230c312d20bb2b45294d44c8d02b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:36:47 GMT
RUN apk add --no-cache ca-certificates
# Wed, 09 Aug 2023 04:41:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:29 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:31:40 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:31:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:31:41 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:58:36 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:58:37 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:58:37 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:58:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:58:37 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:58:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:58:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:58:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d48a809fc2256f8aa0aeee47998488d64409855adba00a7cb3007ab9f3286e`  
		Last Modified: Wed, 09 Aug 2023 03:37:02 GMT  
		Size: 284.7 KB (284693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60be0ca469417450769350b29d9d86e57dc60849c11fab3e8d0b556fcc35005`  
		Last Modified: Wed, 06 Sep 2023 18:37:24 GMT  
		Size: 67.0 MB (67002091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb14ea137979420ee28a5d750e5d62200f15a09c2461e13a8f10023e5fbf5a2`  
		Last Modified: Wed, 06 Sep 2023 18:37:12 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d4cebe2e13d01b24cfdc9eaeae90b4a21f72815fffd9a6a0bb96d99bd0552a`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 5.0 MB (4958640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb64c4e131a2a58133f92ec61aefa25cfb66ef81c5dc749f4de450feb5349c8`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 1.3 MB (1302236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce602f0d9b5db7d56aabf2bf531824f371f52db43d9dc61da5ac5856f69c7359`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:0a1d4936666edfd074f88e0eeeefc1402111cc54a0fcc57963ae88dde642fdca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75388438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c765f590b091ce124e5856c924f7305627163a3a17955d23a482fb20592c338`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:12:05 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:12:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:30:47 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:31:16 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:31:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:31:17 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:54:56 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:54:56 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:54:56 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:54:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:54:56 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:54:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:54:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:54:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8564ce36feee688566265012773f1c8c7c046ceefe86ca763eb702682f4e6e75`  
		Last Modified: Tue, 08 Aug 2023 23:15:06 GMT  
		Size: 284.9 KB (284876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63353306cb1a8907bf53eeefec13043d0f70b554332a60aa92bb4c3861b93c8`  
		Last Modified: Wed, 06 Sep 2023 18:37:56 GMT  
		Size: 65.8 MB (65758368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a286c00e60caea02b9c22fac7d8a91c9ffa40d7fc56aea06e0f8f67c5d3001b8`  
		Last Modified: Wed, 06 Sep 2023 18:37:33 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6650d2d716414907ceaad018d0c2a57750f812da3ce864c723329a9691bfab`  
		Last Modified: Wed, 06 Sep 2023 18:55:14 GMT  
		Size: 5.0 MB (4951168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ebf8a554fac09b4da4a7072225799fa9bc12129c257b93d7dfabc9b7370c0a`  
		Last Modified: Wed, 06 Sep 2023 18:55:14 GMT  
		Size: 1.2 MB (1248657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9711d57485a382ed790b0a10b1af2b8a817f3973693a9add4edf8752b7aae66c`  
		Last Modified: Wed, 06 Sep 2023 18:55:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fe3ec3b57937f6ee95b60afb48874baeee931a06cbb59c944943b498a9016d1c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74690125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590b4483c17141a335fd0eb382750e044c6c5b452db059d3eb1d1aef7950dd3e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:39:47 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 01:39:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:45 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:32:02 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:32:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:32:04 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:58:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:58:39 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:58:39 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:58:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:58:39 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:58:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:58:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:58:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47bd95d78f565e902bafd0264a979eb4f6f71e22c0464011bf9db6feb0579e6`  
		Last Modified: Tue, 08 Aug 2023 01:48:34 GMT  
		Size: 284.1 KB (284073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812db0f4af4ab09f020f5a4b3fb1803a8afdf60db3d0e0c2d451a717141054ca`  
		Last Modified: Wed, 06 Sep 2023 18:40:37 GMT  
		Size: 65.8 MB (65758511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f0657fffaca6c4a15be6c893e54fcf97d14db5815402a0a65f47d5f64b0937`  
		Last Modified: Wed, 06 Sep 2023 18:40:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083d5d74986bc09d57d6a94953a8cb9ab9fbfa44318c32ae6ef17887246f4e9a`  
		Last Modified: Wed, 06 Sep 2023 18:58:57 GMT  
		Size: 4.5 MB (4501414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85d58c05537603de5ce91a6463ef5a223b7ae94f24e05f506b943a930c13a6d`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 1.2 MB (1246086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db284285eec9597c8be93b8c4bd04c0c3b98bf4b089bd52ac26deca4af958251`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:54be0967bfdce111e3176e2c420aab107673db7adc6518b9063186a5bbf6041d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73978310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09ffe7cfa702a73c974a46cf5861ef5c87d89301c99cdda3a283fa9f2ed80442`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:10:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:10:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:18 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:31:28 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:31:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:31:28 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:53:26 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:53:26 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:53:27 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:53:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:53:27 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:53:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:53:28 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:53:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d54e960e981301b0098c80d2e61d694333b5ab480a007a3a8d0fa629662d377`  
		Last Modified: Tue, 08 Aug 2023 23:14:21 GMT  
		Size: 286.3 KB (286298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f000f33a92ab709a2599fbb82fa02eca8bca5b4fda93be45a8d0f1daabb73205`  
		Last Modified: Wed, 06 Sep 2023 18:36:08 GMT  
		Size: 64.1 MB (64108346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447d217685f511c828462bf16ea4579fdb55b103cb1a78d6ba5f0ab6a11db3f8`  
		Last Modified: Wed, 06 Sep 2023 18:35:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13822537d61bbdeb74e6e4458b659dbe1f0d9e3d45af3f50566be42e4b7c809`  
		Last Modified: Wed, 06 Sep 2023 18:53:44 GMT  
		Size: 5.1 MB (5053893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e7da4574a51623195c2699e1b61e06fcc41a5dbde49d5fc96691297a6cd780`  
		Last Modified: Wed, 06 Sep 2023 18:53:43 GMT  
		Size: 1.2 MB (1198447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2621576cb4d382e73ece4231dc51aef77167014d8f83460cbf64238db1fcc45c`  
		Last Modified: Wed, 06 Sep 2023 18:53:43 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:327d6fc238b35334c09db1685ededbacde6621b970825db074650fd341377f2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74185704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0eb6c48fb9239e3fb240aa27acdc3ee85d23fe96322a0606b54ce159b6c2b49`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:25:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 00:25:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:13 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:32:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:32:46 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:32:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:32:50 GMT
WORKDIR /go
# Wed, 06 Sep 2023 19:02:19 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 19:02:21 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 19:02:24 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 19:02:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 19:02:29 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 19:02:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 19:02:35 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 19:02:37 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c966ad2cdd35689da92e7c8fd39bd37cd6080c484e6ccaf00672c154cd4f6c2a`  
		Last Modified: Tue, 08 Aug 2023 00:39:35 GMT  
		Size: 286.7 KB (286662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679e04809663a2145818569201c1dcf2d46798f2198322a8e7910805a9b7dffd`  
		Last Modified: Wed, 06 Sep 2023 18:43:51 GMT  
		Size: 64.1 MB (64116069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1f0b6eb00af4cec1a2c3a203cf9a97b7b5b1e669db11dbabc36635b0207c79`  
		Last Modified: Wed, 06 Sep 2023 18:40:01 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcccd971afab022c32a88b23bc041273f72068caf215514da40b393e06632d93`  
		Last Modified: Wed, 06 Sep 2023 19:02:58 GMT  
		Size: 5.2 MB (5249983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc46690ff4c485e0fea9ac4b7505da047150045d9fcda46c2732480dc1f702`  
		Last Modified: Wed, 06 Sep 2023 19:02:58 GMT  
		Size: 1.2 MB (1186177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b59573283fbd9dc92a2d9a89bd66c6ee4d768933cc1388180a9c1ec35fed90d`  
		Last Modified: Wed, 06 Sep 2023 19:02:57 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:962738aef2725a7bbec2affa560a8497519a54f466f2c84dbfce42be5ab69896
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76084584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2852f51f18c2cd12f1e50eebc15bffa67e107a714382697c8beabe14b1ba6d0f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:41 GMT
RUN apk add --no-cache ca-certificates
# Mon, 07 Aug 2023 20:19:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:19 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:32:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:32:47 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:32:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:32:48 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:57:37 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:57:37 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:57:37 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:57:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:57:37 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:57:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:57:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:57:39 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec90be18226e5c99d10161aed1a143f4134093c55b4d6979bbdbbe4b0683eb11`  
		Last Modified: Mon, 07 Aug 2023 20:30:59 GMT  
		Size: 285.1 KB (285089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53e61151a7324ffa6693144a2516060d0505b80fe8f27915b1e77165106c2a4`  
		Last Modified: Wed, 06 Sep 2023 18:40:12 GMT  
		Size: 66.2 MB (66222411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1f0b6eb00af4cec1a2c3a203cf9a97b7b5b1e669db11dbabc36635b0207c79`  
		Last Modified: Wed, 06 Sep 2023 18:40:01 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178fae6c6c7b745dbb7be349b0656255d25dc06d0c808f85cce56fdf95543af6`  
		Last Modified: Wed, 06 Sep 2023 18:58:02 GMT  
		Size: 5.1 MB (5099943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bda7158ac61debfc44dddd51b20bf5e411c5f34ec92ad21dfffe9a0eeb5ae76`  
		Last Modified: Wed, 06 Sep 2023 18:58:02 GMT  
		Size: 1.3 MB (1262386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13aa15f1f389977eef4ccb0c676963b08cbf0600c3979659a8852b95689e91e8`  
		Last Modified: Wed, 06 Sep 2023 18:58:02 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:dc29929d7895f513f69e34dede7fb945b1bf1540fb37abda23f6fa2edcaa5150
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2092646318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03e3e89d97096b15070b9c1274ebdfe7a5e0de7816cd24a72782cdcb25b33dc3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:39:54 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:39:56 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:41:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:41:12 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:42:07 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:42:08 GMT
ENV GOLANG_VERSION=1.21.0
# Thu, 10 Aug 2023 00:45:16 GMT
RUN $url = 'https://dl.google.com/go/go1.21.0.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '732121e64e0ecb07c77fdf6cc1bc5ce7b242c2d40d4ac29021ad4c64a08731f6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:45:17 GMT
WORKDIR C:\go
# Thu, 17 Aug 2023 22:18:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Aug 2023 22:18:30 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 17 Aug 2023 22:18:31 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:18:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 17 Aug 2023 22:19:38 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 17 Aug 2023 22:19:39 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594083c5c2094c95b4e52723d54c14e0d70881f4f176720c3170012275accc3b`  
		Last Modified: Thu, 10 Aug 2023 01:02:54 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e2c2a5b75ced3a3a50be088c4a6c2d7df926b1fe6515b2d0c021312e3642f4`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d28688050deeec928289543beadf5c75bb2a8246576cb7c066e23818016217`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e5fbc50e7e0fefb7c9e349038ecb00ed5c000bcab8c4d82b1e1000c4273c01`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0544e07bd9df923e11e09c7dc042da614f2f14589eb6fa79005ebbbf2731e97d`  
		Last Modified: Thu, 10 Aug 2023 01:02:57 GMT  
		Size: 25.6 MB (25560980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555a82506c4fcec2bd90ae77756e5b03788e30c89f1a3820aa0b6a7ae6ad58ae`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bcfb422b104764156fc5ba099b5e3ae9fa9f760fd2db1c21acd8969b3d73de`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 220.8 KB (220796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:decc470f4f54c3be087cde5dfcbd816bc68a441d25189983c12219fb4504e9e0`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4589eb0957da5bce467ff89344ebebb2f584a815991fd3004ae3f4890b74f51`  
		Last Modified: Thu, 10 Aug 2023 01:03:10 GMT  
		Size: 69.2 MB (69210847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a698ba14b77be2efdb0e931dc9abf7efc7c749ce53fa2d1c277cd009f295c0`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.5 KB (1517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265b35725533ea18f9e8b7d3422e1b960406141ca305f83de8f61dd49b340c74`  
		Last Modified: Thu, 17 Aug 2023 22:22:07 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3cd40483d2a2e0aae25c4caf3e900aca669895009d08c100e8754768099257`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1aaed9881a7c5017bdf3b46a5ba81399cd7bdaf9be397334872bbf8826386b`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00f7ca68792eb07043e7b43dec1b74b4e211701549286cdcc7993a3b76fdbce`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2516df9efacfe0206db24dbf7d952da6820b3ba9189c715b7aeb069bf903b0b`  
		Last Modified: Thu, 17 Aug 2023 22:22:05 GMT  
		Size: 1.7 MB (1680500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ed01fbe50be0cb731bfdaf18ffaad3e427b9cd10eaabf4930a0dda4b98450`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:16053b4036029cc1457cb147a03be7a416b3fd01393e467beeb72def1f482edf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1894119169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e467c74cf811ff36bfae3619793832f5179eba1986cd92d51528fa3631e15b67`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:36:23 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:36:24 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:36:25 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:36:26 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:36:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:37:00 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:37:19 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:37:20 GMT
ENV GOLANG_VERSION=1.21.0
# Thu, 10 Aug 2023 00:39:40 GMT
RUN $url = 'https://dl.google.com/go/go1.21.0.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '732121e64e0ecb07c77fdf6cc1bc5ce7b242c2d40d4ac29021ad4c64a08731f6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:39:42 GMT
WORKDIR C:\go
# Thu, 17 Aug 2023 22:19:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Aug 2023 22:19:58 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 17 Aug 2023 22:19:58 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:19:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 17 Aug 2023 22:20:24 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 17 Aug 2023 22:20:25 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877256a6389e5e2563da79ad5bd201e7ee136abf14ff7cb0d4efbf3b24e5f127`  
		Last Modified: Thu, 10 Aug 2023 01:02:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a39df29b3c0b2f7e691c47273110db4a46e5c8e299f6bb95f77a9c61f79872`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8574d63bce1547e3177d0b76237a782a9b016d4880375dcd1a7b6a1c5dee3dc`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ef34b3c96316bcdd92e24c8c4eebdc3a35f245c013ef87edfae0dde091a305`  
		Last Modified: Thu, 10 Aug 2023 01:02:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a481babc5b629f694446a96dba8d77c020257c98334c605aff94162b9a917279`  
		Last Modified: Thu, 10 Aug 2023 01:02:23 GMT  
		Size: 25.6 MB (25554169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281178ea1c103ff07ea7e4fb647eb0dbe4f865742da6ef9944e04f37974fc27c`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b5d34adf2aacfe87580143f3e17c635dc8dbd4068377b79b35d665f49bbad9`  
		Last Modified: Thu, 10 Aug 2023 01:02:16 GMT  
		Size: 275.9 KB (275946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5b48235253668711a8e6a2ff934add92fea681c9256325d0ad13a01141c047`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4fb7d9dc956e10b22252d8212c98e2dee64526f471fa548eb6c842d5f05ae9`  
		Last Modified: Thu, 10 Aug 2023 01:02:35 GMT  
		Size: 69.2 MB (69216081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b888078988d2c04f6dae8641365e345f00127285805315ff6f554d6b93ac473c`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.5 KB (1451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b841ebd982703c219e6682e9f6ce05952af17249b1feeac24f29b4758db36694`  
		Last Modified: Thu, 17 Aug 2023 22:22:23 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fde1a85f81e8aec976e03a445fd68b44a23b9f74e66320c7dfce58a75409c25`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0498fcf11a96e26aace74390231497cf74c1d199da68217be38339f5e4108a3`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e49f04c5395ab27a41689cde8841498c15d6b18d029bb336e25274009098cc6`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c1983f7985d2513515cbe76bf211a71393e1a54cfd8e6b755d82fef2120d4a`  
		Last Modified: Thu, 17 Aug 2023 22:22:22 GMT  
		Size: 1.7 MB (1690677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d561bf1c2c8101b9e952ebca483dfa257b2d839feabe3857a1a2694e7d5d83f9`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:49505e7a951d9bba52ba419765e3efdee346bce23e25fdb3260a33d0429c7ce9
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
$ docker pull caddy@sha256:716dc5ded2a0c7090ac3cf0d298122538ac67a0152c97b88a17520c2b0419d82
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76949834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0789fd27a45de2db1b44ab683c8b91c2f63b230c312d20bb2b45294d44c8d02b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:36:47 GMT
RUN apk add --no-cache ca-certificates
# Wed, 09 Aug 2023 04:41:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:29 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:31:40 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:31:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:31:41 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:58:36 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:58:37 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:58:37 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:58:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:58:37 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:58:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:58:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:58:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d48a809fc2256f8aa0aeee47998488d64409855adba00a7cb3007ab9f3286e`  
		Last Modified: Wed, 09 Aug 2023 03:37:02 GMT  
		Size: 284.7 KB (284693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60be0ca469417450769350b29d9d86e57dc60849c11fab3e8d0b556fcc35005`  
		Last Modified: Wed, 06 Sep 2023 18:37:24 GMT  
		Size: 67.0 MB (67002091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb14ea137979420ee28a5d750e5d62200f15a09c2461e13a8f10023e5fbf5a2`  
		Last Modified: Wed, 06 Sep 2023 18:37:12 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d4cebe2e13d01b24cfdc9eaeae90b4a21f72815fffd9a6a0bb96d99bd0552a`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 5.0 MB (4958640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb64c4e131a2a58133f92ec61aefa25cfb66ef81c5dc749f4de450feb5349c8`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 1.3 MB (1302236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce602f0d9b5db7d56aabf2bf531824f371f52db43d9dc61da5ac5856f69c7359`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:0a1d4936666edfd074f88e0eeeefc1402111cc54a0fcc57963ae88dde642fdca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75388438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c765f590b091ce124e5856c924f7305627163a3a17955d23a482fb20592c338`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:12:05 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:12:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:30:47 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:31:16 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:31:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:31:17 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:54:56 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:54:56 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:54:56 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:54:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:54:56 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:54:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:54:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:54:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8564ce36feee688566265012773f1c8c7c046ceefe86ca763eb702682f4e6e75`  
		Last Modified: Tue, 08 Aug 2023 23:15:06 GMT  
		Size: 284.9 KB (284876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63353306cb1a8907bf53eeefec13043d0f70b554332a60aa92bb4c3861b93c8`  
		Last Modified: Wed, 06 Sep 2023 18:37:56 GMT  
		Size: 65.8 MB (65758368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a286c00e60caea02b9c22fac7d8a91c9ffa40d7fc56aea06e0f8f67c5d3001b8`  
		Last Modified: Wed, 06 Sep 2023 18:37:33 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6650d2d716414907ceaad018d0c2a57750f812da3ce864c723329a9691bfab`  
		Last Modified: Wed, 06 Sep 2023 18:55:14 GMT  
		Size: 5.0 MB (4951168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ebf8a554fac09b4da4a7072225799fa9bc12129c257b93d7dfabc9b7370c0a`  
		Last Modified: Wed, 06 Sep 2023 18:55:14 GMT  
		Size: 1.2 MB (1248657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9711d57485a382ed790b0a10b1af2b8a817f3973693a9add4edf8752b7aae66c`  
		Last Modified: Wed, 06 Sep 2023 18:55:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fe3ec3b57937f6ee95b60afb48874baeee931a06cbb59c944943b498a9016d1c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74690125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590b4483c17141a335fd0eb382750e044c6c5b452db059d3eb1d1aef7950dd3e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:39:47 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 01:39:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:45 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:32:02 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:32:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:32:04 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:58:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:58:39 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:58:39 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:58:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:58:39 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:58:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:58:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:58:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47bd95d78f565e902bafd0264a979eb4f6f71e22c0464011bf9db6feb0579e6`  
		Last Modified: Tue, 08 Aug 2023 01:48:34 GMT  
		Size: 284.1 KB (284073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812db0f4af4ab09f020f5a4b3fb1803a8afdf60db3d0e0c2d451a717141054ca`  
		Last Modified: Wed, 06 Sep 2023 18:40:37 GMT  
		Size: 65.8 MB (65758511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f0657fffaca6c4a15be6c893e54fcf97d14db5815402a0a65f47d5f64b0937`  
		Last Modified: Wed, 06 Sep 2023 18:40:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083d5d74986bc09d57d6a94953a8cb9ab9fbfa44318c32ae6ef17887246f4e9a`  
		Last Modified: Wed, 06 Sep 2023 18:58:57 GMT  
		Size: 4.5 MB (4501414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85d58c05537603de5ce91a6463ef5a223b7ae94f24e05f506b943a930c13a6d`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 1.2 MB (1246086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db284285eec9597c8be93b8c4bd04c0c3b98bf4b089bd52ac26deca4af958251`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:54be0967bfdce111e3176e2c420aab107673db7adc6518b9063186a5bbf6041d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73978310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09ffe7cfa702a73c974a46cf5861ef5c87d89301c99cdda3a283fa9f2ed80442`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:10:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:10:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:18 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:31:28 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:31:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:31:28 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:53:26 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:53:26 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:53:27 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:53:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:53:27 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:53:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:53:28 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:53:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d54e960e981301b0098c80d2e61d694333b5ab480a007a3a8d0fa629662d377`  
		Last Modified: Tue, 08 Aug 2023 23:14:21 GMT  
		Size: 286.3 KB (286298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f000f33a92ab709a2599fbb82fa02eca8bca5b4fda93be45a8d0f1daabb73205`  
		Last Modified: Wed, 06 Sep 2023 18:36:08 GMT  
		Size: 64.1 MB (64108346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447d217685f511c828462bf16ea4579fdb55b103cb1a78d6ba5f0ab6a11db3f8`  
		Last Modified: Wed, 06 Sep 2023 18:35:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13822537d61bbdeb74e6e4458b659dbe1f0d9e3d45af3f50566be42e4b7c809`  
		Last Modified: Wed, 06 Sep 2023 18:53:44 GMT  
		Size: 5.1 MB (5053893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e7da4574a51623195c2699e1b61e06fcc41a5dbde49d5fc96691297a6cd780`  
		Last Modified: Wed, 06 Sep 2023 18:53:43 GMT  
		Size: 1.2 MB (1198447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2621576cb4d382e73ece4231dc51aef77167014d8f83460cbf64238db1fcc45c`  
		Last Modified: Wed, 06 Sep 2023 18:53:43 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:327d6fc238b35334c09db1685ededbacde6621b970825db074650fd341377f2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74185704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0eb6c48fb9239e3fb240aa27acdc3ee85d23fe96322a0606b54ce159b6c2b49`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:25:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 00:25:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:13 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:32:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:32:46 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:32:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:32:50 GMT
WORKDIR /go
# Wed, 06 Sep 2023 19:02:19 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 19:02:21 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 19:02:24 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 19:02:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 19:02:29 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 19:02:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 19:02:35 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 19:02:37 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c966ad2cdd35689da92e7c8fd39bd37cd6080c484e6ccaf00672c154cd4f6c2a`  
		Last Modified: Tue, 08 Aug 2023 00:39:35 GMT  
		Size: 286.7 KB (286662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679e04809663a2145818569201c1dcf2d46798f2198322a8e7910805a9b7dffd`  
		Last Modified: Wed, 06 Sep 2023 18:43:51 GMT  
		Size: 64.1 MB (64116069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1f0b6eb00af4cec1a2c3a203cf9a97b7b5b1e669db11dbabc36635b0207c79`  
		Last Modified: Wed, 06 Sep 2023 18:40:01 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcccd971afab022c32a88b23bc041273f72068caf215514da40b393e06632d93`  
		Last Modified: Wed, 06 Sep 2023 19:02:58 GMT  
		Size: 5.2 MB (5249983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc46690ff4c485e0fea9ac4b7505da047150045d9fcda46c2732480dc1f702`  
		Last Modified: Wed, 06 Sep 2023 19:02:58 GMT  
		Size: 1.2 MB (1186177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b59573283fbd9dc92a2d9a89bd66c6ee4d768933cc1388180a9c1ec35fed90d`  
		Last Modified: Wed, 06 Sep 2023 19:02:57 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:962738aef2725a7bbec2affa560a8497519a54f466f2c84dbfce42be5ab69896
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76084584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2852f51f18c2cd12f1e50eebc15bffa67e107a714382697c8beabe14b1ba6d0f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:41 GMT
RUN apk add --no-cache ca-certificates
# Mon, 07 Aug 2023 20:19:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:19 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:32:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:32:47 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:32:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:32:48 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:57:37 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:57:37 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:57:37 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:57:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:57:37 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:57:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:57:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:57:39 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec90be18226e5c99d10161aed1a143f4134093c55b4d6979bbdbbe4b0683eb11`  
		Last Modified: Mon, 07 Aug 2023 20:30:59 GMT  
		Size: 285.1 KB (285089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53e61151a7324ffa6693144a2516060d0505b80fe8f27915b1e77165106c2a4`  
		Last Modified: Wed, 06 Sep 2023 18:40:12 GMT  
		Size: 66.2 MB (66222411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1f0b6eb00af4cec1a2c3a203cf9a97b7b5b1e669db11dbabc36635b0207c79`  
		Last Modified: Wed, 06 Sep 2023 18:40:01 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178fae6c6c7b745dbb7be349b0656255d25dc06d0c808f85cce56fdf95543af6`  
		Last Modified: Wed, 06 Sep 2023 18:58:02 GMT  
		Size: 5.1 MB (5099943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bda7158ac61debfc44dddd51b20bf5e411c5f34ec92ad21dfffe9a0eeb5ae76`  
		Last Modified: Wed, 06 Sep 2023 18:58:02 GMT  
		Size: 1.3 MB (1262386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13aa15f1f389977eef4ccb0c676963b08cbf0600c3979659a8852b95689e91e8`  
		Last Modified: Wed, 06 Sep 2023 18:58:02 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:795ac7c3a409b95ae5a486743690a31dea9328bc5af293a50f64b63112a9adf6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:dc29929d7895f513f69e34dede7fb945b1bf1540fb37abda23f6fa2edcaa5150
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2092646318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03e3e89d97096b15070b9c1274ebdfe7a5e0de7816cd24a72782cdcb25b33dc3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:39:54 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:39:56 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:41:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:41:12 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:42:07 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:42:08 GMT
ENV GOLANG_VERSION=1.21.0
# Thu, 10 Aug 2023 00:45:16 GMT
RUN $url = 'https://dl.google.com/go/go1.21.0.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '732121e64e0ecb07c77fdf6cc1bc5ce7b242c2d40d4ac29021ad4c64a08731f6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:45:17 GMT
WORKDIR C:\go
# Thu, 17 Aug 2023 22:18:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Aug 2023 22:18:30 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 17 Aug 2023 22:18:31 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:18:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 17 Aug 2023 22:19:38 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 17 Aug 2023 22:19:39 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594083c5c2094c95b4e52723d54c14e0d70881f4f176720c3170012275accc3b`  
		Last Modified: Thu, 10 Aug 2023 01:02:54 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e2c2a5b75ced3a3a50be088c4a6c2d7df926b1fe6515b2d0c021312e3642f4`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d28688050deeec928289543beadf5c75bb2a8246576cb7c066e23818016217`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e5fbc50e7e0fefb7c9e349038ecb00ed5c000bcab8c4d82b1e1000c4273c01`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0544e07bd9df923e11e09c7dc042da614f2f14589eb6fa79005ebbbf2731e97d`  
		Last Modified: Thu, 10 Aug 2023 01:02:57 GMT  
		Size: 25.6 MB (25560980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555a82506c4fcec2bd90ae77756e5b03788e30c89f1a3820aa0b6a7ae6ad58ae`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bcfb422b104764156fc5ba099b5e3ae9fa9f760fd2db1c21acd8969b3d73de`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 220.8 KB (220796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:decc470f4f54c3be087cde5dfcbd816bc68a441d25189983c12219fb4504e9e0`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4589eb0957da5bce467ff89344ebebb2f584a815991fd3004ae3f4890b74f51`  
		Last Modified: Thu, 10 Aug 2023 01:03:10 GMT  
		Size: 69.2 MB (69210847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a698ba14b77be2efdb0e931dc9abf7efc7c749ce53fa2d1c277cd009f295c0`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.5 KB (1517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265b35725533ea18f9e8b7d3422e1b960406141ca305f83de8f61dd49b340c74`  
		Last Modified: Thu, 17 Aug 2023 22:22:07 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3cd40483d2a2e0aae25c4caf3e900aca669895009d08c100e8754768099257`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1aaed9881a7c5017bdf3b46a5ba81399cd7bdaf9be397334872bbf8826386b`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00f7ca68792eb07043e7b43dec1b74b4e211701549286cdcc7993a3b76fdbce`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2516df9efacfe0206db24dbf7d952da6820b3ba9189c715b7aeb069bf903b0b`  
		Last Modified: Thu, 17 Aug 2023 22:22:05 GMT  
		Size: 1.7 MB (1680500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ed01fbe50be0cb731bfdaf18ffaad3e427b9cd10eaabf4930a0dda4b98450`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:f8893322f81862d0d41473494adb769699011eab49c16e9c66a37e7c5d1a61e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1906; amd64

### `caddy:2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:16053b4036029cc1457cb147a03be7a416b3fd01393e467beeb72def1f482edf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1894119169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e467c74cf811ff36bfae3619793832f5179eba1986cd92d51528fa3631e15b67`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:36:23 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:36:24 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:36:25 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:36:26 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:36:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:37:00 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:37:19 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:37:20 GMT
ENV GOLANG_VERSION=1.21.0
# Thu, 10 Aug 2023 00:39:40 GMT
RUN $url = 'https://dl.google.com/go/go1.21.0.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '732121e64e0ecb07c77fdf6cc1bc5ce7b242c2d40d4ac29021ad4c64a08731f6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:39:42 GMT
WORKDIR C:\go
# Thu, 17 Aug 2023 22:19:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Aug 2023 22:19:58 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 17 Aug 2023 22:19:58 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:19:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 17 Aug 2023 22:20:24 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 17 Aug 2023 22:20:25 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877256a6389e5e2563da79ad5bd201e7ee136abf14ff7cb0d4efbf3b24e5f127`  
		Last Modified: Thu, 10 Aug 2023 01:02:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a39df29b3c0b2f7e691c47273110db4a46e5c8e299f6bb95f77a9c61f79872`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8574d63bce1547e3177d0b76237a782a9b016d4880375dcd1a7b6a1c5dee3dc`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ef34b3c96316bcdd92e24c8c4eebdc3a35f245c013ef87edfae0dde091a305`  
		Last Modified: Thu, 10 Aug 2023 01:02:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a481babc5b629f694446a96dba8d77c020257c98334c605aff94162b9a917279`  
		Last Modified: Thu, 10 Aug 2023 01:02:23 GMT  
		Size: 25.6 MB (25554169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281178ea1c103ff07ea7e4fb647eb0dbe4f865742da6ef9944e04f37974fc27c`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b5d34adf2aacfe87580143f3e17c635dc8dbd4068377b79b35d665f49bbad9`  
		Last Modified: Thu, 10 Aug 2023 01:02:16 GMT  
		Size: 275.9 KB (275946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5b48235253668711a8e6a2ff934add92fea681c9256325d0ad13a01141c047`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4fb7d9dc956e10b22252d8212c98e2dee64526f471fa548eb6c842d5f05ae9`  
		Last Modified: Thu, 10 Aug 2023 01:02:35 GMT  
		Size: 69.2 MB (69216081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b888078988d2c04f6dae8641365e345f00127285805315ff6f554d6b93ac473c`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.5 KB (1451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b841ebd982703c219e6682e9f6ce05952af17249b1feeac24f29b4758db36694`  
		Last Modified: Thu, 17 Aug 2023 22:22:23 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fde1a85f81e8aec976e03a445fd68b44a23b9f74e66320c7dfce58a75409c25`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0498fcf11a96e26aace74390231497cf74c1d199da68217be38339f5e4108a3`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e49f04c5395ab27a41689cde8841498c15d6b18d029bb336e25274009098cc6`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c1983f7985d2513515cbe76bf211a71393e1a54cfd8e6b755d82fef2120d4a`  
		Last Modified: Thu, 17 Aug 2023 22:22:22 GMT  
		Size: 1.7 MB (1690677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d561bf1c2c8101b9e952ebca483dfa257b2d839feabe3857a1a2694e7d5d83f9`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:9b2d0e89dc4f5f508ec90143d8b6b6d2cdbe9067fea9d0930cbb9812eb816b01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4737; amd64
	-	windows version 10.0.20348.1906; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:8d641d87b059de975dc94ff579d47434e347b333b33a4a8f15cd679c062a14c0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2011934670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e21b2ad9f1a3657d84dd869da76d22704a2848d4a92f831acbfef09e26e80cc6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 14 Aug 2023 18:16:58 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 17 Aug 2023 22:14:59 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:16:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 17 Aug 2023 22:16:13 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 17 Aug 2023 22:16:14 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 17 Aug 2023 22:16:15 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:16:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:16:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:16:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:16:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:16:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:16:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:16:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:16:21 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:16:22 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:16:23 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:16:24 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:17:19 GMT
RUN caddy version
# Thu, 17 Aug 2023 22:17:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d698e8ba8bfd4c31116f0d2c87cfcf2ff17baa1a5c678b116b3aa1ac8ed73d`  
		Last Modified: Mon, 14 Aug 2023 18:23:17 GMT  
		Size: 483.6 KB (483626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dcf545f7c90cab6f6962d3099898462129da2e6b06a80802d52ff1e9d2fca08`  
		Last Modified: Thu, 17 Aug 2023 22:21:12 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65ecc8b4521923b522dd6392a862d0dff9edd10c1e3b520de8f130de2170880`  
		Last Modified: Thu, 17 Aug 2023 22:21:16 GMT  
		Size: 15.2 MB (15201779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ddd9c690b84a4a4744ec5ac91059e12e1aa92378220080fcfbf616c59b4c26`  
		Last Modified: Thu, 17 Aug 2023 22:21:12 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63adbcb9cba5e8d67eac5e059c7bbb9dfe3040f0933afb5e1f8cb7d4c211b4a`  
		Last Modified: Thu, 17 Aug 2023 22:21:11 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e15ff22938f514e6118606619ff28e9e5ee145d6f3dc6de1de62ea4051575c1`  
		Last Modified: Thu, 17 Aug 2023 22:21:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438a6cab105b637f625a3fd00d7ecaa6792ad5dc120bf1be36e7d6e19ee44b4d`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfd206f96497c8e0730c72c36ecedea57379a6a219903785dc1478b50b3945`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e651df7142dc872814a59faff8cf791ab4e4413ee6a9b043fe02a2af9da24fe`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b7f62d857ed7e15d08d52d1ef08f3c21e25751d17e8a5418c02f6adc366eab`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6347f1227dc933d98b8f02d22cd440529284e7c8e415e96cee265ae2c7445b3`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2776f9f89b2242d27c9c49da3465d2ff6acb224dd3315837bda709f3fa0aa4ff`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aaab02f29add47735607e798c40625216306d00d57988d1ece40f43b93f706c`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ed26555e0c9e51aa5dbf4125ef3ea56c6d84274b4d8160ce10c3c0d9e7106d`  
		Last Modified: Thu, 17 Aug 2023 22:21:08 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392c0484ea6d941786f507e72c143bd1c64d4c42bcd773bd745330a55b89d356`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef07137395441a56a870d882d84faac751156b0486c6528fa18b6d706ff250d8`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2950cf3d51ba47c2b41415fccf9b67e813735f67ccc34a0ce5f1a1a4a34e56dc`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25de03b5a8b8f2752cde31b881d457ec5900438b781cc65cda3aca9444b2377f`  
		Last Modified: Thu, 17 Aug 2023 22:21:07 GMT  
		Size: 269.9 KB (269882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f3d70fb1dd11e79f9128736ada85993e1b4fd603b2f8164aac49ac1efda548`  
		Last Modified: Thu, 17 Aug 2023 22:21:07 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:f4791cb0179b98b28e760842405262d782735176b147c84f26709bd1361c8798
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1813299019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b759bf39605cbc0d0ceaaa8eda1623452b1acd67deb11c0d22defff59f2058`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 14 Aug 2023 18:19:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 17 Aug 2023 22:17:27 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:17:55 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 17 Aug 2023 22:17:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 17 Aug 2023 22:17:56 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 17 Aug 2023 22:17:57 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:17:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:17:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:17:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:18:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:18:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:18:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:18:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:18:04 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:18:04 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:18:05 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:18:06 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:18:21 GMT
RUN caddy version
# Thu, 17 Aug 2023 22:18:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c23e01ee014d9e05e276268c94980b00a0720fcb5488a368b20ee74701ed78`  
		Last Modified: Mon, 14 Aug 2023 18:23:42 GMT  
		Size: 461.2 KB (461170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8a7576f0b2ff121a0e9658821e52a7b356abbd90c9215b750ab7fc2127f6ae`  
		Last Modified: Thu, 17 Aug 2023 22:21:41 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ecc6db59a89a0a9f61364702d6af7202fa4f3f742ec6dff93c3a5b53e3826`  
		Last Modified: Thu, 17 Aug 2023 22:21:44 GMT  
		Size: 15.2 MB (15169088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9323e4528d7a59819754484fdbeb047240a6f1f0dd262b734a226a4249dc0a0`  
		Last Modified: Thu, 17 Aug 2023 22:21:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb3a3b69dd93b979cdcd1e0759ee1199bc8d5a510a6ce9bca3856201d747468`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56ce33676578802911228ae7aba31fe1898897ede8c69e12a0959a37a11d130`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c896eeb3f2c45b2bba4fe5e5da02be1289c4cabcf574a38c19d1616ebf552d4c`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6563dd3d5f912ae2b7bd629d2dc731df89b1dd107e2cbb85dee24a0d5c550a1`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420011263062842c72720998f13fa245d9bef077622fde4e17cc60cef3e00bce`  
		Last Modified: Thu, 17 Aug 2023 22:21:38 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2385fc0cb7a281a35df415654aba711bf70fa23b963faf0a3f0055d760f5c41c`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a58351f25f399f8a9399e60dd315cd8c695972a9e51f2271e3377151cf621d`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506eb3a97b70fc7dc1c1c3464a89512890cd48c354658e58e61d5acfee63f1c3`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86cf8c25cfcaf858db6ffd2630a26ca3a13ad2fdc941a01438ea9ea80ccb20c`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcedddef9863d16c4d713280050f604b44968bc253844c27e46cb8871eb17a99`  
		Last Modified: Thu, 17 Aug 2023 22:21:36 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d01313141e38a9b2b15a3e831a2d11a3eb47611bf99b0677be3c49693984f64`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504a80bc0f7aa0c98a143033f551be8fcf0653046e7313c0de080b82ad97ad52`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280053e45030e2421ea4d1cdfd721c24f40d30518b1ce8af7e0811363daf6eca`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0d07466cd8f053bf957a35cbe340d419f5c2f6ff48565bb8a5b255998e3e94`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 280.9 KB (280938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad52776067d7be890960cfd7082041a93a802b96fea6d31fc724192c49eb00`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:44adcd32029ece40e50aef18ba70e3020cbba5b53153929078326ec23613226c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:8d641d87b059de975dc94ff579d47434e347b333b33a4a8f15cd679c062a14c0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2011934670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e21b2ad9f1a3657d84dd869da76d22704a2848d4a92f831acbfef09e26e80cc6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 14 Aug 2023 18:16:58 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 17 Aug 2023 22:14:59 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:16:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 17 Aug 2023 22:16:13 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 17 Aug 2023 22:16:14 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 17 Aug 2023 22:16:15 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:16:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:16:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:16:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:16:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:16:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:16:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:16:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:16:21 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:16:22 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:16:23 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:16:24 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:17:19 GMT
RUN caddy version
# Thu, 17 Aug 2023 22:17:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d698e8ba8bfd4c31116f0d2c87cfcf2ff17baa1a5c678b116b3aa1ac8ed73d`  
		Last Modified: Mon, 14 Aug 2023 18:23:17 GMT  
		Size: 483.6 KB (483626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dcf545f7c90cab6f6962d3099898462129da2e6b06a80802d52ff1e9d2fca08`  
		Last Modified: Thu, 17 Aug 2023 22:21:12 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65ecc8b4521923b522dd6392a862d0dff9edd10c1e3b520de8f130de2170880`  
		Last Modified: Thu, 17 Aug 2023 22:21:16 GMT  
		Size: 15.2 MB (15201779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ddd9c690b84a4a4744ec5ac91059e12e1aa92378220080fcfbf616c59b4c26`  
		Last Modified: Thu, 17 Aug 2023 22:21:12 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63adbcb9cba5e8d67eac5e059c7bbb9dfe3040f0933afb5e1f8cb7d4c211b4a`  
		Last Modified: Thu, 17 Aug 2023 22:21:11 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e15ff22938f514e6118606619ff28e9e5ee145d6f3dc6de1de62ea4051575c1`  
		Last Modified: Thu, 17 Aug 2023 22:21:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438a6cab105b637f625a3fd00d7ecaa6792ad5dc120bf1be36e7d6e19ee44b4d`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfd206f96497c8e0730c72c36ecedea57379a6a219903785dc1478b50b3945`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e651df7142dc872814a59faff8cf791ab4e4413ee6a9b043fe02a2af9da24fe`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b7f62d857ed7e15d08d52d1ef08f3c21e25751d17e8a5418c02f6adc366eab`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6347f1227dc933d98b8f02d22cd440529284e7c8e415e96cee265ae2c7445b3`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2776f9f89b2242d27c9c49da3465d2ff6acb224dd3315837bda709f3fa0aa4ff`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aaab02f29add47735607e798c40625216306d00d57988d1ece40f43b93f706c`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ed26555e0c9e51aa5dbf4125ef3ea56c6d84274b4d8160ce10c3c0d9e7106d`  
		Last Modified: Thu, 17 Aug 2023 22:21:08 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392c0484ea6d941786f507e72c143bd1c64d4c42bcd773bd745330a55b89d356`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef07137395441a56a870d882d84faac751156b0486c6528fa18b6d706ff250d8`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2950cf3d51ba47c2b41415fccf9b67e813735f67ccc34a0ce5f1a1a4a34e56dc`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25de03b5a8b8f2752cde31b881d457ec5900438b781cc65cda3aca9444b2377f`  
		Last Modified: Thu, 17 Aug 2023 22:21:07 GMT  
		Size: 269.9 KB (269882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f3d70fb1dd11e79f9128736ada85993e1b4fd603b2f8164aac49ac1efda548`  
		Last Modified: Thu, 17 Aug 2023 22:21:07 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:25814323b2b1cf78a7dfadd252104b12d24aa4dc9512441a2717cd13b1d3da8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1906; amd64

### `caddy:2-windowsservercore-ltsc2022` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:f4791cb0179b98b28e760842405262d782735176b147c84f26709bd1361c8798
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1813299019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b759bf39605cbc0d0ceaaa8eda1623452b1acd67deb11c0d22defff59f2058`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 14 Aug 2023 18:19:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 17 Aug 2023 22:17:27 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:17:55 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 17 Aug 2023 22:17:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 17 Aug 2023 22:17:56 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 17 Aug 2023 22:17:57 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:17:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:17:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:17:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:18:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:18:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:18:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:18:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:18:04 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:18:04 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:18:05 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:18:06 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:18:21 GMT
RUN caddy version
# Thu, 17 Aug 2023 22:18:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c23e01ee014d9e05e276268c94980b00a0720fcb5488a368b20ee74701ed78`  
		Last Modified: Mon, 14 Aug 2023 18:23:42 GMT  
		Size: 461.2 KB (461170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8a7576f0b2ff121a0e9658821e52a7b356abbd90c9215b750ab7fc2127f6ae`  
		Last Modified: Thu, 17 Aug 2023 22:21:41 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ecc6db59a89a0a9f61364702d6af7202fa4f3f742ec6dff93c3a5b53e3826`  
		Last Modified: Thu, 17 Aug 2023 22:21:44 GMT  
		Size: 15.2 MB (15169088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9323e4528d7a59819754484fdbeb047240a6f1f0dd262b734a226a4249dc0a0`  
		Last Modified: Thu, 17 Aug 2023 22:21:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb3a3b69dd93b979cdcd1e0759ee1199bc8d5a510a6ce9bca3856201d747468`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56ce33676578802911228ae7aba31fe1898897ede8c69e12a0959a37a11d130`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c896eeb3f2c45b2bba4fe5e5da02be1289c4cabcf574a38c19d1616ebf552d4c`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6563dd3d5f912ae2b7bd629d2dc731df89b1dd107e2cbb85dee24a0d5c550a1`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420011263062842c72720998f13fa245d9bef077622fde4e17cc60cef3e00bce`  
		Last Modified: Thu, 17 Aug 2023 22:21:38 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2385fc0cb7a281a35df415654aba711bf70fa23b963faf0a3f0055d760f5c41c`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a58351f25f399f8a9399e60dd315cd8c695972a9e51f2271e3377151cf621d`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506eb3a97b70fc7dc1c1c3464a89512890cd48c354658e58e61d5acfee63f1c3`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86cf8c25cfcaf858db6ffd2630a26ca3a13ad2fdc941a01438ea9ea80ccb20c`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcedddef9863d16c4d713280050f604b44968bc253844c27e46cb8871eb17a99`  
		Last Modified: Thu, 17 Aug 2023 22:21:36 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d01313141e38a9b2b15a3e831a2d11a3eb47611bf99b0677be3c49693984f64`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504a80bc0f7aa0c98a143033f551be8fcf0653046e7313c0de080b82ad97ad52`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280053e45030e2421ea4d1cdfd721c24f40d30518b1ce8af7e0811363daf6eca`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0d07466cd8f053bf957a35cbe340d419f5c2f6ff48565bb8a5b255998e3e94`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 280.9 KB (280938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad52776067d7be890960cfd7082041a93a802b96fea6d31fc724192c49eb00`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7`

```console
$ docker pull caddy@sha256:2332c4ebc4ae778b9697043d3fa3aaef6879dd17abc03200285af9d315353008
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4737; amd64
	-	windows version 10.0.20348.1906; amd64

### `caddy:2.7` - linux; amd64

```console
$ docker pull caddy@sha256:733fe94133c4bd22c6ee8f9b9802bce8fede5e7b766bebde205a45dd4ac04aea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18363908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1e1b7ae170b7d7d7e524717fe978e0090023cc82a7d9ffe48e344b0351a3ee1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:09:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 18:20:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:19:38 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:19:41 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:19:41 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:19:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:19:42 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:19:42 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:19:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0aa7b81ef11c65f43b0b58323a33dd9e07eb785529f0d75b452f87a309db00c`  
		Last Modified: Mon, 07 Aug 2023 20:09:40 GMT  
		Size: 350.8 KB (350844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b3b3e68e52dc5ab939c72a9bbac39cff4bef4b87de399ddf28657471df6845`  
		Last Modified: Mon, 14 Aug 2023 18:20:42 GMT  
		Size: 7.5 KB (7502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c55d3259542348ddb70edc18dda7d48aeca5654962aed568a7034f3667d2ca`  
		Last Modified: Thu, 17 Aug 2023 22:20:10 GMT  
		Size: 14.6 MB (14603949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - linux; arm variant v6

```console
$ docker pull caddy@sha256:dd029220558032e5d1f91173d32a0078dad12ec9b5114bef422ed4cdf05dec52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17314204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1de0523ee8d8173472fb08aa9a74a37bcd054af2b796b7631d847ba8a46986b5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:38:27 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:49:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:49:12 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:49:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:49:16 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:49:16 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:49:17 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:49:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172ef460a93549b8a3e73f6a515bccad93512788d1e8f095e7230ba41967c25a`  
		Last Modified: Wed, 09 Aug 2023 03:38:53 GMT  
		Size: 347.7 KB (347686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7aae78767a581df85fd1a51ccd646619aec320896ca016ef0f05a41b16bcbfe`  
		Last Modified: Mon, 14 Aug 2023 17:49:36 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82560a340155261ecbd1d99d87890c5aa0cfd64d571e1dcafc03e3b6a8132d48`  
		Last Modified: Thu, 17 Aug 2023 22:49:41 GMT  
		Size: 13.8 MB (13814204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - linux; arm variant v7

```console
$ docker pull caddy@sha256:24649e9de43354963118f9cdf6ad1f4522c6993735f316763a2f5d1f76cba267
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17042831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb4a48fd29d50802cbf030949e2c9767eb6888e8412330f64246f322bc3b49c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:51:41 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:57:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:57:18 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:57:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:57:22 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:57:22 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:57:24 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:57:24 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:57:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a47b73e04459258b08555443754e92e2db20bde113c58ca18e1a6f07878f72`  
		Last Modified: Tue, 08 Aug 2023 01:52:05 GMT  
		Size: 344.5 KB (344462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e1b3e18d5e992f1805072b2d52405d575830bdce21726ef99dea99e31d8277`  
		Last Modified: Mon, 14 Aug 2023 17:57:42 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5879767a5d1969beb154b9a4991a767b0ed5be0c9739a972f07d03e825312fa5`  
		Last Modified: Thu, 17 Aug 2023 22:57:51 GMT  
		Size: 13.8 MB (13791384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:ed967fcd1968be6dc4699ff835cdd2d6f3f49105b9677f878c8a6960fd1a0643
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17162547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed7b6600470cab547aa1090baa39a6192ec83119989884ac742a63ed23be3da2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:09:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:39:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:39:17 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:39:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:39:19 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:39:19 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:39:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:39:20 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:39:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a699f78cfb85f60e17fc7c13495876ea0cb4495bbe39e8c65f3e8559b0d7169`  
		Last Modified: Mon, 07 Aug 2023 21:09:34 GMT  
		Size: 360.6 KB (360642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7488af8b96c79b6db13955a0302653c4e9f314d0833201984ae06c1ed697f06`  
		Last Modified: Mon, 14 Aug 2023 17:39:41 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597bfc484ba18727d2df98120cb9d559f346ade9e3a23be6a9af3e76dca89edd`  
		Last Modified: Thu, 17 Aug 2023 22:39:42 GMT  
		Size: 13.5 MB (13463635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - linux; ppc64le

```console
$ docker pull caddy@sha256:c3679836562d0252e6341a112d2729b8dae0eae550449bfe91fe2798171fd4ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16944934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc5ac831dce746cd0f4448640b7edaf0ce9457d09618e246ba72ee76ea63dcbe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:44:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 18:18:00 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:16:24 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:16:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:16:29 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:16:29 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:16:29 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:16:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:16:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:16:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:16:32 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:16:33 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:16:33 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:16:34 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:16:34 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:16:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f40714f45e39ac41e865ccbf2877db62255ce5a5c36a47eadf00b9d174f042`  
		Last Modified: Tue, 08 Aug 2023 00:45:18 GMT  
		Size: 362.2 KB (362173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d19953b5eb53ddaa0e25905527dc138e0c4111467bb7d71f81fa94976091351`  
		Last Modified: Mon, 14 Aug 2023 18:18:54 GMT  
		Size: 7.5 KB (7509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf4bf695323732c5ce84bbb0b976c5cd981eaf6814515a86f521af4a0e64582`  
		Last Modified: Thu, 17 Aug 2023 22:17:22 GMT  
		Size: 13.2 MB (13229001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - linux; s390x

```console
$ docker pull caddy@sha256:ca7ab0dcf4ab146df48cfa8ae6e07fed804feeed4a36358fa652c8eac52b40da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17720356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d4d019ffc0cd69ea8c5d3b8fb0a39c89d3aa1b2037c1012a9ba4bed6abb94dc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:14:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:41:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:41:35 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:41:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:41:39 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:41:39 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:41:39 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:41:40 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:41:41 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:41:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df19abd0ca1d4a821a4174a2c0831a57d6fd584073f056abcae085a51f0b3848`  
		Last Modified: Mon, 07 Aug 2023 20:14:50 GMT  
		Size: 354.9 KB (354950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308478977890baa82477ee70a3065fb9da2080efcc95facf1a87ac021b06a8e9`  
		Last Modified: Mon, 14 Aug 2023 17:42:17 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2394cd7c9416df19c45596c558f5a7ee05adc5a7fd166f58dcbf26f1ac6ecae6`  
		Last Modified: Thu, 17 Aug 2023 22:42:16 GMT  
		Size: 14.1 MB (14143708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:8d641d87b059de975dc94ff579d47434e347b333b33a4a8f15cd679c062a14c0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2011934670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e21b2ad9f1a3657d84dd869da76d22704a2848d4a92f831acbfef09e26e80cc6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 14 Aug 2023 18:16:58 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 17 Aug 2023 22:14:59 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:16:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 17 Aug 2023 22:16:13 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 17 Aug 2023 22:16:14 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 17 Aug 2023 22:16:15 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:16:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:16:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:16:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:16:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:16:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:16:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:16:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:16:21 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:16:22 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:16:23 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:16:24 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:17:19 GMT
RUN caddy version
# Thu, 17 Aug 2023 22:17:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d698e8ba8bfd4c31116f0d2c87cfcf2ff17baa1a5c678b116b3aa1ac8ed73d`  
		Last Modified: Mon, 14 Aug 2023 18:23:17 GMT  
		Size: 483.6 KB (483626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dcf545f7c90cab6f6962d3099898462129da2e6b06a80802d52ff1e9d2fca08`  
		Last Modified: Thu, 17 Aug 2023 22:21:12 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65ecc8b4521923b522dd6392a862d0dff9edd10c1e3b520de8f130de2170880`  
		Last Modified: Thu, 17 Aug 2023 22:21:16 GMT  
		Size: 15.2 MB (15201779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ddd9c690b84a4a4744ec5ac91059e12e1aa92378220080fcfbf616c59b4c26`  
		Last Modified: Thu, 17 Aug 2023 22:21:12 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63adbcb9cba5e8d67eac5e059c7bbb9dfe3040f0933afb5e1f8cb7d4c211b4a`  
		Last Modified: Thu, 17 Aug 2023 22:21:11 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e15ff22938f514e6118606619ff28e9e5ee145d6f3dc6de1de62ea4051575c1`  
		Last Modified: Thu, 17 Aug 2023 22:21:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438a6cab105b637f625a3fd00d7ecaa6792ad5dc120bf1be36e7d6e19ee44b4d`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfd206f96497c8e0730c72c36ecedea57379a6a219903785dc1478b50b3945`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e651df7142dc872814a59faff8cf791ab4e4413ee6a9b043fe02a2af9da24fe`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b7f62d857ed7e15d08d52d1ef08f3c21e25751d17e8a5418c02f6adc366eab`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6347f1227dc933d98b8f02d22cd440529284e7c8e415e96cee265ae2c7445b3`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2776f9f89b2242d27c9c49da3465d2ff6acb224dd3315837bda709f3fa0aa4ff`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aaab02f29add47735607e798c40625216306d00d57988d1ece40f43b93f706c`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ed26555e0c9e51aa5dbf4125ef3ea56c6d84274b4d8160ce10c3c0d9e7106d`  
		Last Modified: Thu, 17 Aug 2023 22:21:08 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392c0484ea6d941786f507e72c143bd1c64d4c42bcd773bd745330a55b89d356`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef07137395441a56a870d882d84faac751156b0486c6528fa18b6d706ff250d8`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2950cf3d51ba47c2b41415fccf9b67e813735f67ccc34a0ce5f1a1a4a34e56dc`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25de03b5a8b8f2752cde31b881d457ec5900438b781cc65cda3aca9444b2377f`  
		Last Modified: Thu, 17 Aug 2023 22:21:07 GMT  
		Size: 269.9 KB (269882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f3d70fb1dd11e79f9128736ada85993e1b4fd603b2f8164aac49ac1efda548`  
		Last Modified: Thu, 17 Aug 2023 22:21:07 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:f4791cb0179b98b28e760842405262d782735176b147c84f26709bd1361c8798
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1813299019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b759bf39605cbc0d0ceaaa8eda1623452b1acd67deb11c0d22defff59f2058`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 14 Aug 2023 18:19:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 17 Aug 2023 22:17:27 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:17:55 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 17 Aug 2023 22:17:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 17 Aug 2023 22:17:56 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 17 Aug 2023 22:17:57 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:17:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:17:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:17:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:18:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:18:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:18:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:18:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:18:04 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:18:04 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:18:05 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:18:06 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:18:21 GMT
RUN caddy version
# Thu, 17 Aug 2023 22:18:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c23e01ee014d9e05e276268c94980b00a0720fcb5488a368b20ee74701ed78`  
		Last Modified: Mon, 14 Aug 2023 18:23:42 GMT  
		Size: 461.2 KB (461170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8a7576f0b2ff121a0e9658821e52a7b356abbd90c9215b750ab7fc2127f6ae`  
		Last Modified: Thu, 17 Aug 2023 22:21:41 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ecc6db59a89a0a9f61364702d6af7202fa4f3f742ec6dff93c3a5b53e3826`  
		Last Modified: Thu, 17 Aug 2023 22:21:44 GMT  
		Size: 15.2 MB (15169088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9323e4528d7a59819754484fdbeb047240a6f1f0dd262b734a226a4249dc0a0`  
		Last Modified: Thu, 17 Aug 2023 22:21:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb3a3b69dd93b979cdcd1e0759ee1199bc8d5a510a6ce9bca3856201d747468`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56ce33676578802911228ae7aba31fe1898897ede8c69e12a0959a37a11d130`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c896eeb3f2c45b2bba4fe5e5da02be1289c4cabcf574a38c19d1616ebf552d4c`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6563dd3d5f912ae2b7bd629d2dc731df89b1dd107e2cbb85dee24a0d5c550a1`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420011263062842c72720998f13fa245d9bef077622fde4e17cc60cef3e00bce`  
		Last Modified: Thu, 17 Aug 2023 22:21:38 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2385fc0cb7a281a35df415654aba711bf70fa23b963faf0a3f0055d760f5c41c`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a58351f25f399f8a9399e60dd315cd8c695972a9e51f2271e3377151cf621d`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506eb3a97b70fc7dc1c1c3464a89512890cd48c354658e58e61d5acfee63f1c3`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86cf8c25cfcaf858db6ffd2630a26ca3a13ad2fdc941a01438ea9ea80ccb20c`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcedddef9863d16c4d713280050f604b44968bc253844c27e46cb8871eb17a99`  
		Last Modified: Thu, 17 Aug 2023 22:21:36 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d01313141e38a9b2b15a3e831a2d11a3eb47611bf99b0677be3c49693984f64`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504a80bc0f7aa0c98a143033f551be8fcf0653046e7313c0de080b82ad97ad52`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280053e45030e2421ea4d1cdfd721c24f40d30518b1ce8af7e0811363daf6eca`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0d07466cd8f053bf957a35cbe340d419f5c2f6ff48565bb8a5b255998e3e94`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 280.9 KB (280938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad52776067d7be890960cfd7082041a93a802b96fea6d31fc724192c49eb00`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-alpine`

```console
$ docker pull caddy@sha256:7e01c08308bc94c1ef3e495f0b2ba469d1f7e8d1a4f2caa2fbe189edf48866a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.7-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:733fe94133c4bd22c6ee8f9b9802bce8fede5e7b766bebde205a45dd4ac04aea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18363908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1e1b7ae170b7d7d7e524717fe978e0090023cc82a7d9ffe48e344b0351a3ee1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:09:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 18:20:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:19:38 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:19:41 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:19:41 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:19:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:19:42 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:19:42 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:19:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0aa7b81ef11c65f43b0b58323a33dd9e07eb785529f0d75b452f87a309db00c`  
		Last Modified: Mon, 07 Aug 2023 20:09:40 GMT  
		Size: 350.8 KB (350844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b3b3e68e52dc5ab939c72a9bbac39cff4bef4b87de399ddf28657471df6845`  
		Last Modified: Mon, 14 Aug 2023 18:20:42 GMT  
		Size: 7.5 KB (7502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c55d3259542348ddb70edc18dda7d48aeca5654962aed568a7034f3667d2ca`  
		Last Modified: Thu, 17 Aug 2023 22:20:10 GMT  
		Size: 14.6 MB (14603949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:dd029220558032e5d1f91173d32a0078dad12ec9b5114bef422ed4cdf05dec52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17314204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1de0523ee8d8173472fb08aa9a74a37bcd054af2b796b7631d847ba8a46986b5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:38:27 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:49:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:49:12 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:49:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:49:16 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:49:16 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:49:17 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:49:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172ef460a93549b8a3e73f6a515bccad93512788d1e8f095e7230ba41967c25a`  
		Last Modified: Wed, 09 Aug 2023 03:38:53 GMT  
		Size: 347.7 KB (347686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7aae78767a581df85fd1a51ccd646619aec320896ca016ef0f05a41b16bcbfe`  
		Last Modified: Mon, 14 Aug 2023 17:49:36 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82560a340155261ecbd1d99d87890c5aa0cfd64d571e1dcafc03e3b6a8132d48`  
		Last Modified: Thu, 17 Aug 2023 22:49:41 GMT  
		Size: 13.8 MB (13814204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:24649e9de43354963118f9cdf6ad1f4522c6993735f316763a2f5d1f76cba267
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17042831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb4a48fd29d50802cbf030949e2c9767eb6888e8412330f64246f322bc3b49c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:51:41 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:57:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:57:18 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:57:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:57:22 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:57:22 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:57:24 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:57:24 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:57:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a47b73e04459258b08555443754e92e2db20bde113c58ca18e1a6f07878f72`  
		Last Modified: Tue, 08 Aug 2023 01:52:05 GMT  
		Size: 344.5 KB (344462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e1b3e18d5e992f1805072b2d52405d575830bdce21726ef99dea99e31d8277`  
		Last Modified: Mon, 14 Aug 2023 17:57:42 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5879767a5d1969beb154b9a4991a767b0ed5be0c9739a972f07d03e825312fa5`  
		Last Modified: Thu, 17 Aug 2023 22:57:51 GMT  
		Size: 13.8 MB (13791384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:ed967fcd1968be6dc4699ff835cdd2d6f3f49105b9677f878c8a6960fd1a0643
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17162547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed7b6600470cab547aa1090baa39a6192ec83119989884ac742a63ed23be3da2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:09:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:39:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:39:17 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:39:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:39:19 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:39:19 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:39:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:39:20 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:39:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a699f78cfb85f60e17fc7c13495876ea0cb4495bbe39e8c65f3e8559b0d7169`  
		Last Modified: Mon, 07 Aug 2023 21:09:34 GMT  
		Size: 360.6 KB (360642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7488af8b96c79b6db13955a0302653c4e9f314d0833201984ae06c1ed697f06`  
		Last Modified: Mon, 14 Aug 2023 17:39:41 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597bfc484ba18727d2df98120cb9d559f346ade9e3a23be6a9af3e76dca89edd`  
		Last Modified: Thu, 17 Aug 2023 22:39:42 GMT  
		Size: 13.5 MB (13463635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:c3679836562d0252e6341a112d2729b8dae0eae550449bfe91fe2798171fd4ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16944934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc5ac831dce746cd0f4448640b7edaf0ce9457d09618e246ba72ee76ea63dcbe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:44:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 18:18:00 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:16:24 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:16:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:16:29 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:16:29 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:16:29 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:16:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:16:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:16:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:16:32 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:16:33 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:16:33 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:16:34 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:16:34 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:16:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f40714f45e39ac41e865ccbf2877db62255ce5a5c36a47eadf00b9d174f042`  
		Last Modified: Tue, 08 Aug 2023 00:45:18 GMT  
		Size: 362.2 KB (362173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d19953b5eb53ddaa0e25905527dc138e0c4111467bb7d71f81fa94976091351`  
		Last Modified: Mon, 14 Aug 2023 18:18:54 GMT  
		Size: 7.5 KB (7509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf4bf695323732c5ce84bbb0b976c5cd981eaf6814515a86f521af4a0e64582`  
		Last Modified: Thu, 17 Aug 2023 22:17:22 GMT  
		Size: 13.2 MB (13229001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:ca7ab0dcf4ab146df48cfa8ae6e07fed804feeed4a36358fa652c8eac52b40da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17720356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d4d019ffc0cd69ea8c5d3b8fb0a39c89d3aa1b2037c1012a9ba4bed6abb94dc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:14:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:41:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:41:35 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:41:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:41:39 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:41:39 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:41:39 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:41:40 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:41:41 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:41:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df19abd0ca1d4a821a4174a2c0831a57d6fd584073f056abcae085a51f0b3848`  
		Last Modified: Mon, 07 Aug 2023 20:14:50 GMT  
		Size: 354.9 KB (354950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308478977890baa82477ee70a3065fb9da2080efcc95facf1a87ac021b06a8e9`  
		Last Modified: Mon, 14 Aug 2023 17:42:17 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2394cd7c9416df19c45596c558f5a7ee05adc5a7fd166f58dcbf26f1ac6ecae6`  
		Last Modified: Thu, 17 Aug 2023 22:42:16 GMT  
		Size: 14.1 MB (14143708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-builder`

```console
$ docker pull caddy@sha256:eafc66404950e4170122aba0977f7079d888e544bed6df61a144b50bcf06bbb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4737; amd64
	-	windows version 10.0.20348.1906; amd64

### `caddy:2.7-builder` - linux; amd64

```console
$ docker pull caddy@sha256:716dc5ded2a0c7090ac3cf0d298122538ac67a0152c97b88a17520c2b0419d82
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76949834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0789fd27a45de2db1b44ab683c8b91c2f63b230c312d20bb2b45294d44c8d02b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:36:47 GMT
RUN apk add --no-cache ca-certificates
# Wed, 09 Aug 2023 04:41:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:29 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:31:40 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:31:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:31:41 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:58:36 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:58:37 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:58:37 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:58:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:58:37 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:58:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:58:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:58:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d48a809fc2256f8aa0aeee47998488d64409855adba00a7cb3007ab9f3286e`  
		Last Modified: Wed, 09 Aug 2023 03:37:02 GMT  
		Size: 284.7 KB (284693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60be0ca469417450769350b29d9d86e57dc60849c11fab3e8d0b556fcc35005`  
		Last Modified: Wed, 06 Sep 2023 18:37:24 GMT  
		Size: 67.0 MB (67002091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb14ea137979420ee28a5d750e5d62200f15a09c2461e13a8f10023e5fbf5a2`  
		Last Modified: Wed, 06 Sep 2023 18:37:12 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d4cebe2e13d01b24cfdc9eaeae90b4a21f72815fffd9a6a0bb96d99bd0552a`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 5.0 MB (4958640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb64c4e131a2a58133f92ec61aefa25cfb66ef81c5dc749f4de450feb5349c8`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 1.3 MB (1302236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce602f0d9b5db7d56aabf2bf531824f371f52db43d9dc61da5ac5856f69c7359`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:0a1d4936666edfd074f88e0eeeefc1402111cc54a0fcc57963ae88dde642fdca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75388438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c765f590b091ce124e5856c924f7305627163a3a17955d23a482fb20592c338`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:12:05 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:12:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:30:47 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:31:16 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:31:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:31:17 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:54:56 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:54:56 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:54:56 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:54:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:54:56 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:54:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:54:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:54:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8564ce36feee688566265012773f1c8c7c046ceefe86ca763eb702682f4e6e75`  
		Last Modified: Tue, 08 Aug 2023 23:15:06 GMT  
		Size: 284.9 KB (284876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63353306cb1a8907bf53eeefec13043d0f70b554332a60aa92bb4c3861b93c8`  
		Last Modified: Wed, 06 Sep 2023 18:37:56 GMT  
		Size: 65.8 MB (65758368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a286c00e60caea02b9c22fac7d8a91c9ffa40d7fc56aea06e0f8f67c5d3001b8`  
		Last Modified: Wed, 06 Sep 2023 18:37:33 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6650d2d716414907ceaad018d0c2a57750f812da3ce864c723329a9691bfab`  
		Last Modified: Wed, 06 Sep 2023 18:55:14 GMT  
		Size: 5.0 MB (4951168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ebf8a554fac09b4da4a7072225799fa9bc12129c257b93d7dfabc9b7370c0a`  
		Last Modified: Wed, 06 Sep 2023 18:55:14 GMT  
		Size: 1.2 MB (1248657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9711d57485a382ed790b0a10b1af2b8a817f3973693a9add4edf8752b7aae66c`  
		Last Modified: Wed, 06 Sep 2023 18:55:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fe3ec3b57937f6ee95b60afb48874baeee931a06cbb59c944943b498a9016d1c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74690125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590b4483c17141a335fd0eb382750e044c6c5b452db059d3eb1d1aef7950dd3e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:39:47 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 01:39:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:45 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:32:02 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:32:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:32:04 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:58:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:58:39 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:58:39 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:58:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:58:39 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:58:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:58:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:58:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47bd95d78f565e902bafd0264a979eb4f6f71e22c0464011bf9db6feb0579e6`  
		Last Modified: Tue, 08 Aug 2023 01:48:34 GMT  
		Size: 284.1 KB (284073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812db0f4af4ab09f020f5a4b3fb1803a8afdf60db3d0e0c2d451a717141054ca`  
		Last Modified: Wed, 06 Sep 2023 18:40:37 GMT  
		Size: 65.8 MB (65758511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f0657fffaca6c4a15be6c893e54fcf97d14db5815402a0a65f47d5f64b0937`  
		Last Modified: Wed, 06 Sep 2023 18:40:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083d5d74986bc09d57d6a94953a8cb9ab9fbfa44318c32ae6ef17887246f4e9a`  
		Last Modified: Wed, 06 Sep 2023 18:58:57 GMT  
		Size: 4.5 MB (4501414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85d58c05537603de5ce91a6463ef5a223b7ae94f24e05f506b943a930c13a6d`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 1.2 MB (1246086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db284285eec9597c8be93b8c4bd04c0c3b98bf4b089bd52ac26deca4af958251`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:54be0967bfdce111e3176e2c420aab107673db7adc6518b9063186a5bbf6041d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73978310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09ffe7cfa702a73c974a46cf5861ef5c87d89301c99cdda3a283fa9f2ed80442`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:10:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:10:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:18 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:31:28 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:31:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:31:28 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:53:26 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:53:26 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:53:27 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:53:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:53:27 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:53:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:53:28 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:53:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d54e960e981301b0098c80d2e61d694333b5ab480a007a3a8d0fa629662d377`  
		Last Modified: Tue, 08 Aug 2023 23:14:21 GMT  
		Size: 286.3 KB (286298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f000f33a92ab709a2599fbb82fa02eca8bca5b4fda93be45a8d0f1daabb73205`  
		Last Modified: Wed, 06 Sep 2023 18:36:08 GMT  
		Size: 64.1 MB (64108346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447d217685f511c828462bf16ea4579fdb55b103cb1a78d6ba5f0ab6a11db3f8`  
		Last Modified: Wed, 06 Sep 2023 18:35:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13822537d61bbdeb74e6e4458b659dbe1f0d9e3d45af3f50566be42e4b7c809`  
		Last Modified: Wed, 06 Sep 2023 18:53:44 GMT  
		Size: 5.1 MB (5053893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e7da4574a51623195c2699e1b61e06fcc41a5dbde49d5fc96691297a6cd780`  
		Last Modified: Wed, 06 Sep 2023 18:53:43 GMT  
		Size: 1.2 MB (1198447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2621576cb4d382e73ece4231dc51aef77167014d8f83460cbf64238db1fcc45c`  
		Last Modified: Wed, 06 Sep 2023 18:53:43 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:327d6fc238b35334c09db1685ededbacde6621b970825db074650fd341377f2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74185704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0eb6c48fb9239e3fb240aa27acdc3ee85d23fe96322a0606b54ce159b6c2b49`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:25:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 00:25:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:13 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:32:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:32:46 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:32:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:32:50 GMT
WORKDIR /go
# Wed, 06 Sep 2023 19:02:19 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 19:02:21 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 19:02:24 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 19:02:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 19:02:29 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 19:02:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 19:02:35 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 19:02:37 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c966ad2cdd35689da92e7c8fd39bd37cd6080c484e6ccaf00672c154cd4f6c2a`  
		Last Modified: Tue, 08 Aug 2023 00:39:35 GMT  
		Size: 286.7 KB (286662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679e04809663a2145818569201c1dcf2d46798f2198322a8e7910805a9b7dffd`  
		Last Modified: Wed, 06 Sep 2023 18:43:51 GMT  
		Size: 64.1 MB (64116069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1f0b6eb00af4cec1a2c3a203cf9a97b7b5b1e669db11dbabc36635b0207c79`  
		Last Modified: Wed, 06 Sep 2023 18:40:01 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcccd971afab022c32a88b23bc041273f72068caf215514da40b393e06632d93`  
		Last Modified: Wed, 06 Sep 2023 19:02:58 GMT  
		Size: 5.2 MB (5249983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc46690ff4c485e0fea9ac4b7505da047150045d9fcda46c2732480dc1f702`  
		Last Modified: Wed, 06 Sep 2023 19:02:58 GMT  
		Size: 1.2 MB (1186177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b59573283fbd9dc92a2d9a89bd66c6ee4d768933cc1388180a9c1ec35fed90d`  
		Last Modified: Wed, 06 Sep 2023 19:02:57 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; s390x

```console
$ docker pull caddy@sha256:962738aef2725a7bbec2affa560a8497519a54f466f2c84dbfce42be5ab69896
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76084584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2852f51f18c2cd12f1e50eebc15bffa67e107a714382697c8beabe14b1ba6d0f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:41 GMT
RUN apk add --no-cache ca-certificates
# Mon, 07 Aug 2023 20:19:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:19 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:32:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:32:47 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:32:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:32:48 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:57:37 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:57:37 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:57:37 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:57:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:57:37 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:57:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:57:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:57:39 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec90be18226e5c99d10161aed1a143f4134093c55b4d6979bbdbbe4b0683eb11`  
		Last Modified: Mon, 07 Aug 2023 20:30:59 GMT  
		Size: 285.1 KB (285089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53e61151a7324ffa6693144a2516060d0505b80fe8f27915b1e77165106c2a4`  
		Last Modified: Wed, 06 Sep 2023 18:40:12 GMT  
		Size: 66.2 MB (66222411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1f0b6eb00af4cec1a2c3a203cf9a97b7b5b1e669db11dbabc36635b0207c79`  
		Last Modified: Wed, 06 Sep 2023 18:40:01 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178fae6c6c7b745dbb7be349b0656255d25dc06d0c808f85cce56fdf95543af6`  
		Last Modified: Wed, 06 Sep 2023 18:58:02 GMT  
		Size: 5.1 MB (5099943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bda7158ac61debfc44dddd51b20bf5e411c5f34ec92ad21dfffe9a0eeb5ae76`  
		Last Modified: Wed, 06 Sep 2023 18:58:02 GMT  
		Size: 1.3 MB (1262386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13aa15f1f389977eef4ccb0c676963b08cbf0600c3979659a8852b95689e91e8`  
		Last Modified: Wed, 06 Sep 2023 18:58:02 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:dc29929d7895f513f69e34dede7fb945b1bf1540fb37abda23f6fa2edcaa5150
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2092646318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03e3e89d97096b15070b9c1274ebdfe7a5e0de7816cd24a72782cdcb25b33dc3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:39:54 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:39:56 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:41:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:41:12 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:42:07 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:42:08 GMT
ENV GOLANG_VERSION=1.21.0
# Thu, 10 Aug 2023 00:45:16 GMT
RUN $url = 'https://dl.google.com/go/go1.21.0.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '732121e64e0ecb07c77fdf6cc1bc5ce7b242c2d40d4ac29021ad4c64a08731f6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:45:17 GMT
WORKDIR C:\go
# Thu, 17 Aug 2023 22:18:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Aug 2023 22:18:30 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 17 Aug 2023 22:18:31 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:18:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 17 Aug 2023 22:19:38 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 17 Aug 2023 22:19:39 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594083c5c2094c95b4e52723d54c14e0d70881f4f176720c3170012275accc3b`  
		Last Modified: Thu, 10 Aug 2023 01:02:54 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e2c2a5b75ced3a3a50be088c4a6c2d7df926b1fe6515b2d0c021312e3642f4`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d28688050deeec928289543beadf5c75bb2a8246576cb7c066e23818016217`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e5fbc50e7e0fefb7c9e349038ecb00ed5c000bcab8c4d82b1e1000c4273c01`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0544e07bd9df923e11e09c7dc042da614f2f14589eb6fa79005ebbbf2731e97d`  
		Last Modified: Thu, 10 Aug 2023 01:02:57 GMT  
		Size: 25.6 MB (25560980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555a82506c4fcec2bd90ae77756e5b03788e30c89f1a3820aa0b6a7ae6ad58ae`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bcfb422b104764156fc5ba099b5e3ae9fa9f760fd2db1c21acd8969b3d73de`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 220.8 KB (220796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:decc470f4f54c3be087cde5dfcbd816bc68a441d25189983c12219fb4504e9e0`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4589eb0957da5bce467ff89344ebebb2f584a815991fd3004ae3f4890b74f51`  
		Last Modified: Thu, 10 Aug 2023 01:03:10 GMT  
		Size: 69.2 MB (69210847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a698ba14b77be2efdb0e931dc9abf7efc7c749ce53fa2d1c277cd009f295c0`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.5 KB (1517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265b35725533ea18f9e8b7d3422e1b960406141ca305f83de8f61dd49b340c74`  
		Last Modified: Thu, 17 Aug 2023 22:22:07 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3cd40483d2a2e0aae25c4caf3e900aca669895009d08c100e8754768099257`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1aaed9881a7c5017bdf3b46a5ba81399cd7bdaf9be397334872bbf8826386b`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00f7ca68792eb07043e7b43dec1b74b4e211701549286cdcc7993a3b76fdbce`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2516df9efacfe0206db24dbf7d952da6820b3ba9189c715b7aeb069bf903b0b`  
		Last Modified: Thu, 17 Aug 2023 22:22:05 GMT  
		Size: 1.7 MB (1680500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ed01fbe50be0cb731bfdaf18ffaad3e427b9cd10eaabf4930a0dda4b98450`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:16053b4036029cc1457cb147a03be7a416b3fd01393e467beeb72def1f482edf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1894119169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e467c74cf811ff36bfae3619793832f5179eba1986cd92d51528fa3631e15b67`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:36:23 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:36:24 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:36:25 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:36:26 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:36:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:37:00 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:37:19 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:37:20 GMT
ENV GOLANG_VERSION=1.21.0
# Thu, 10 Aug 2023 00:39:40 GMT
RUN $url = 'https://dl.google.com/go/go1.21.0.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '732121e64e0ecb07c77fdf6cc1bc5ce7b242c2d40d4ac29021ad4c64a08731f6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:39:42 GMT
WORKDIR C:\go
# Thu, 17 Aug 2023 22:19:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Aug 2023 22:19:58 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 17 Aug 2023 22:19:58 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:19:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 17 Aug 2023 22:20:24 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 17 Aug 2023 22:20:25 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877256a6389e5e2563da79ad5bd201e7ee136abf14ff7cb0d4efbf3b24e5f127`  
		Last Modified: Thu, 10 Aug 2023 01:02:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a39df29b3c0b2f7e691c47273110db4a46e5c8e299f6bb95f77a9c61f79872`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8574d63bce1547e3177d0b76237a782a9b016d4880375dcd1a7b6a1c5dee3dc`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ef34b3c96316bcdd92e24c8c4eebdc3a35f245c013ef87edfae0dde091a305`  
		Last Modified: Thu, 10 Aug 2023 01:02:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a481babc5b629f694446a96dba8d77c020257c98334c605aff94162b9a917279`  
		Last Modified: Thu, 10 Aug 2023 01:02:23 GMT  
		Size: 25.6 MB (25554169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281178ea1c103ff07ea7e4fb647eb0dbe4f865742da6ef9944e04f37974fc27c`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b5d34adf2aacfe87580143f3e17c635dc8dbd4068377b79b35d665f49bbad9`  
		Last Modified: Thu, 10 Aug 2023 01:02:16 GMT  
		Size: 275.9 KB (275946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5b48235253668711a8e6a2ff934add92fea681c9256325d0ad13a01141c047`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4fb7d9dc956e10b22252d8212c98e2dee64526f471fa548eb6c842d5f05ae9`  
		Last Modified: Thu, 10 Aug 2023 01:02:35 GMT  
		Size: 69.2 MB (69216081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b888078988d2c04f6dae8641365e345f00127285805315ff6f554d6b93ac473c`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.5 KB (1451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b841ebd982703c219e6682e9f6ce05952af17249b1feeac24f29b4758db36694`  
		Last Modified: Thu, 17 Aug 2023 22:22:23 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fde1a85f81e8aec976e03a445fd68b44a23b9f74e66320c7dfce58a75409c25`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0498fcf11a96e26aace74390231497cf74c1d199da68217be38339f5e4108a3`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e49f04c5395ab27a41689cde8841498c15d6b18d029bb336e25274009098cc6`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c1983f7985d2513515cbe76bf211a71393e1a54cfd8e6b755d82fef2120d4a`  
		Last Modified: Thu, 17 Aug 2023 22:22:22 GMT  
		Size: 1.7 MB (1690677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d561bf1c2c8101b9e952ebca483dfa257b2d839feabe3857a1a2694e7d5d83f9`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-builder-alpine`

```console
$ docker pull caddy@sha256:49505e7a951d9bba52ba419765e3efdee346bce23e25fdb3260a33d0429c7ce9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.7-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:716dc5ded2a0c7090ac3cf0d298122538ac67a0152c97b88a17520c2b0419d82
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76949834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0789fd27a45de2db1b44ab683c8b91c2f63b230c312d20bb2b45294d44c8d02b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:36:47 GMT
RUN apk add --no-cache ca-certificates
# Wed, 09 Aug 2023 04:41:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:29 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:31:40 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:31:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:31:41 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:58:36 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:58:37 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:58:37 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:58:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:58:37 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:58:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:58:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:58:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d48a809fc2256f8aa0aeee47998488d64409855adba00a7cb3007ab9f3286e`  
		Last Modified: Wed, 09 Aug 2023 03:37:02 GMT  
		Size: 284.7 KB (284693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60be0ca469417450769350b29d9d86e57dc60849c11fab3e8d0b556fcc35005`  
		Last Modified: Wed, 06 Sep 2023 18:37:24 GMT  
		Size: 67.0 MB (67002091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb14ea137979420ee28a5d750e5d62200f15a09c2461e13a8f10023e5fbf5a2`  
		Last Modified: Wed, 06 Sep 2023 18:37:12 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d4cebe2e13d01b24cfdc9eaeae90b4a21f72815fffd9a6a0bb96d99bd0552a`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 5.0 MB (4958640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb64c4e131a2a58133f92ec61aefa25cfb66ef81c5dc749f4de450feb5349c8`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 1.3 MB (1302236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce602f0d9b5db7d56aabf2bf531824f371f52db43d9dc61da5ac5856f69c7359`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:0a1d4936666edfd074f88e0eeeefc1402111cc54a0fcc57963ae88dde642fdca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75388438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c765f590b091ce124e5856c924f7305627163a3a17955d23a482fb20592c338`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:12:05 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:12:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:30:47 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:31:16 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:31:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:31:17 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:54:56 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:54:56 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:54:56 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:54:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:54:56 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:54:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:54:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:54:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8564ce36feee688566265012773f1c8c7c046ceefe86ca763eb702682f4e6e75`  
		Last Modified: Tue, 08 Aug 2023 23:15:06 GMT  
		Size: 284.9 KB (284876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63353306cb1a8907bf53eeefec13043d0f70b554332a60aa92bb4c3861b93c8`  
		Last Modified: Wed, 06 Sep 2023 18:37:56 GMT  
		Size: 65.8 MB (65758368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a286c00e60caea02b9c22fac7d8a91c9ffa40d7fc56aea06e0f8f67c5d3001b8`  
		Last Modified: Wed, 06 Sep 2023 18:37:33 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6650d2d716414907ceaad018d0c2a57750f812da3ce864c723329a9691bfab`  
		Last Modified: Wed, 06 Sep 2023 18:55:14 GMT  
		Size: 5.0 MB (4951168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ebf8a554fac09b4da4a7072225799fa9bc12129c257b93d7dfabc9b7370c0a`  
		Last Modified: Wed, 06 Sep 2023 18:55:14 GMT  
		Size: 1.2 MB (1248657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9711d57485a382ed790b0a10b1af2b8a817f3973693a9add4edf8752b7aae66c`  
		Last Modified: Wed, 06 Sep 2023 18:55:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fe3ec3b57937f6ee95b60afb48874baeee931a06cbb59c944943b498a9016d1c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74690125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590b4483c17141a335fd0eb382750e044c6c5b452db059d3eb1d1aef7950dd3e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:39:47 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 01:39:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:45 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:32:02 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:32:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:32:04 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:58:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:58:39 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:58:39 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:58:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:58:39 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:58:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:58:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:58:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47bd95d78f565e902bafd0264a979eb4f6f71e22c0464011bf9db6feb0579e6`  
		Last Modified: Tue, 08 Aug 2023 01:48:34 GMT  
		Size: 284.1 KB (284073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812db0f4af4ab09f020f5a4b3fb1803a8afdf60db3d0e0c2d451a717141054ca`  
		Last Modified: Wed, 06 Sep 2023 18:40:37 GMT  
		Size: 65.8 MB (65758511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f0657fffaca6c4a15be6c893e54fcf97d14db5815402a0a65f47d5f64b0937`  
		Last Modified: Wed, 06 Sep 2023 18:40:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083d5d74986bc09d57d6a94953a8cb9ab9fbfa44318c32ae6ef17887246f4e9a`  
		Last Modified: Wed, 06 Sep 2023 18:58:57 GMT  
		Size: 4.5 MB (4501414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85d58c05537603de5ce91a6463ef5a223b7ae94f24e05f506b943a930c13a6d`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 1.2 MB (1246086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db284285eec9597c8be93b8c4bd04c0c3b98bf4b089bd52ac26deca4af958251`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:54be0967bfdce111e3176e2c420aab107673db7adc6518b9063186a5bbf6041d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73978310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09ffe7cfa702a73c974a46cf5861ef5c87d89301c99cdda3a283fa9f2ed80442`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:10:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:10:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:18 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:31:28 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:31:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:31:28 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:53:26 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:53:26 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:53:27 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:53:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:53:27 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:53:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:53:28 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:53:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d54e960e981301b0098c80d2e61d694333b5ab480a007a3a8d0fa629662d377`  
		Last Modified: Tue, 08 Aug 2023 23:14:21 GMT  
		Size: 286.3 KB (286298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f000f33a92ab709a2599fbb82fa02eca8bca5b4fda93be45a8d0f1daabb73205`  
		Last Modified: Wed, 06 Sep 2023 18:36:08 GMT  
		Size: 64.1 MB (64108346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447d217685f511c828462bf16ea4579fdb55b103cb1a78d6ba5f0ab6a11db3f8`  
		Last Modified: Wed, 06 Sep 2023 18:35:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13822537d61bbdeb74e6e4458b659dbe1f0d9e3d45af3f50566be42e4b7c809`  
		Last Modified: Wed, 06 Sep 2023 18:53:44 GMT  
		Size: 5.1 MB (5053893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e7da4574a51623195c2699e1b61e06fcc41a5dbde49d5fc96691297a6cd780`  
		Last Modified: Wed, 06 Sep 2023 18:53:43 GMT  
		Size: 1.2 MB (1198447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2621576cb4d382e73ece4231dc51aef77167014d8f83460cbf64238db1fcc45c`  
		Last Modified: Wed, 06 Sep 2023 18:53:43 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:327d6fc238b35334c09db1685ededbacde6621b970825db074650fd341377f2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74185704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0eb6c48fb9239e3fb240aa27acdc3ee85d23fe96322a0606b54ce159b6c2b49`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:25:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 00:25:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:13 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:32:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:32:46 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:32:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:32:50 GMT
WORKDIR /go
# Wed, 06 Sep 2023 19:02:19 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 19:02:21 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 19:02:24 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 19:02:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 19:02:29 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 19:02:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 19:02:35 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 19:02:37 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c966ad2cdd35689da92e7c8fd39bd37cd6080c484e6ccaf00672c154cd4f6c2a`  
		Last Modified: Tue, 08 Aug 2023 00:39:35 GMT  
		Size: 286.7 KB (286662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679e04809663a2145818569201c1dcf2d46798f2198322a8e7910805a9b7dffd`  
		Last Modified: Wed, 06 Sep 2023 18:43:51 GMT  
		Size: 64.1 MB (64116069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1f0b6eb00af4cec1a2c3a203cf9a97b7b5b1e669db11dbabc36635b0207c79`  
		Last Modified: Wed, 06 Sep 2023 18:40:01 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcccd971afab022c32a88b23bc041273f72068caf215514da40b393e06632d93`  
		Last Modified: Wed, 06 Sep 2023 19:02:58 GMT  
		Size: 5.2 MB (5249983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc46690ff4c485e0fea9ac4b7505da047150045d9fcda46c2732480dc1f702`  
		Last Modified: Wed, 06 Sep 2023 19:02:58 GMT  
		Size: 1.2 MB (1186177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b59573283fbd9dc92a2d9a89bd66c6ee4d768933cc1388180a9c1ec35fed90d`  
		Last Modified: Wed, 06 Sep 2023 19:02:57 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:962738aef2725a7bbec2affa560a8497519a54f466f2c84dbfce42be5ab69896
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76084584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2852f51f18c2cd12f1e50eebc15bffa67e107a714382697c8beabe14b1ba6d0f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:41 GMT
RUN apk add --no-cache ca-certificates
# Mon, 07 Aug 2023 20:19:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:19 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:32:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:32:47 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:32:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:32:48 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:57:37 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:57:37 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:57:37 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:57:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:57:37 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:57:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:57:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:57:39 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec90be18226e5c99d10161aed1a143f4134093c55b4d6979bbdbbe4b0683eb11`  
		Last Modified: Mon, 07 Aug 2023 20:30:59 GMT  
		Size: 285.1 KB (285089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53e61151a7324ffa6693144a2516060d0505b80fe8f27915b1e77165106c2a4`  
		Last Modified: Wed, 06 Sep 2023 18:40:12 GMT  
		Size: 66.2 MB (66222411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1f0b6eb00af4cec1a2c3a203cf9a97b7b5b1e669db11dbabc36635b0207c79`  
		Last Modified: Wed, 06 Sep 2023 18:40:01 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178fae6c6c7b745dbb7be349b0656255d25dc06d0c808f85cce56fdf95543af6`  
		Last Modified: Wed, 06 Sep 2023 18:58:02 GMT  
		Size: 5.1 MB (5099943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bda7158ac61debfc44dddd51b20bf5e411c5f34ec92ad21dfffe9a0eeb5ae76`  
		Last Modified: Wed, 06 Sep 2023 18:58:02 GMT  
		Size: 1.3 MB (1262386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13aa15f1f389977eef4ccb0c676963b08cbf0600c3979659a8852b95689e91e8`  
		Last Modified: Wed, 06 Sep 2023 18:58:02 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:795ac7c3a409b95ae5a486743690a31dea9328bc5af293a50f64b63112a9adf6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `caddy:2.7-builder-windowsservercore-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:dc29929d7895f513f69e34dede7fb945b1bf1540fb37abda23f6fa2edcaa5150
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2092646318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03e3e89d97096b15070b9c1274ebdfe7a5e0de7816cd24a72782cdcb25b33dc3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:39:54 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:39:56 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:41:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:41:12 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:42:07 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:42:08 GMT
ENV GOLANG_VERSION=1.21.0
# Thu, 10 Aug 2023 00:45:16 GMT
RUN $url = 'https://dl.google.com/go/go1.21.0.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '732121e64e0ecb07c77fdf6cc1bc5ce7b242c2d40d4ac29021ad4c64a08731f6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:45:17 GMT
WORKDIR C:\go
# Thu, 17 Aug 2023 22:18:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Aug 2023 22:18:30 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 17 Aug 2023 22:18:31 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:18:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 17 Aug 2023 22:19:38 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 17 Aug 2023 22:19:39 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594083c5c2094c95b4e52723d54c14e0d70881f4f176720c3170012275accc3b`  
		Last Modified: Thu, 10 Aug 2023 01:02:54 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e2c2a5b75ced3a3a50be088c4a6c2d7df926b1fe6515b2d0c021312e3642f4`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d28688050deeec928289543beadf5c75bb2a8246576cb7c066e23818016217`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e5fbc50e7e0fefb7c9e349038ecb00ed5c000bcab8c4d82b1e1000c4273c01`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0544e07bd9df923e11e09c7dc042da614f2f14589eb6fa79005ebbbf2731e97d`  
		Last Modified: Thu, 10 Aug 2023 01:02:57 GMT  
		Size: 25.6 MB (25560980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555a82506c4fcec2bd90ae77756e5b03788e30c89f1a3820aa0b6a7ae6ad58ae`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bcfb422b104764156fc5ba099b5e3ae9fa9f760fd2db1c21acd8969b3d73de`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 220.8 KB (220796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:decc470f4f54c3be087cde5dfcbd816bc68a441d25189983c12219fb4504e9e0`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4589eb0957da5bce467ff89344ebebb2f584a815991fd3004ae3f4890b74f51`  
		Last Modified: Thu, 10 Aug 2023 01:03:10 GMT  
		Size: 69.2 MB (69210847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a698ba14b77be2efdb0e931dc9abf7efc7c749ce53fa2d1c277cd009f295c0`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.5 KB (1517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265b35725533ea18f9e8b7d3422e1b960406141ca305f83de8f61dd49b340c74`  
		Last Modified: Thu, 17 Aug 2023 22:22:07 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3cd40483d2a2e0aae25c4caf3e900aca669895009d08c100e8754768099257`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1aaed9881a7c5017bdf3b46a5ba81399cd7bdaf9be397334872bbf8826386b`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00f7ca68792eb07043e7b43dec1b74b4e211701549286cdcc7993a3b76fdbce`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2516df9efacfe0206db24dbf7d952da6820b3ba9189c715b7aeb069bf903b0b`  
		Last Modified: Thu, 17 Aug 2023 22:22:05 GMT  
		Size: 1.7 MB (1680500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ed01fbe50be0cb731bfdaf18ffaad3e427b9cd10eaabf4930a0dda4b98450`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:f8893322f81862d0d41473494adb769699011eab49c16e9c66a37e7c5d1a61e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1906; amd64

### `caddy:2.7-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:16053b4036029cc1457cb147a03be7a416b3fd01393e467beeb72def1f482edf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1894119169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e467c74cf811ff36bfae3619793832f5179eba1986cd92d51528fa3631e15b67`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:36:23 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:36:24 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:36:25 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:36:26 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:36:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:37:00 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:37:19 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:37:20 GMT
ENV GOLANG_VERSION=1.21.0
# Thu, 10 Aug 2023 00:39:40 GMT
RUN $url = 'https://dl.google.com/go/go1.21.0.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '732121e64e0ecb07c77fdf6cc1bc5ce7b242c2d40d4ac29021ad4c64a08731f6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:39:42 GMT
WORKDIR C:\go
# Thu, 17 Aug 2023 22:19:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Aug 2023 22:19:58 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 17 Aug 2023 22:19:58 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:19:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 17 Aug 2023 22:20:24 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 17 Aug 2023 22:20:25 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877256a6389e5e2563da79ad5bd201e7ee136abf14ff7cb0d4efbf3b24e5f127`  
		Last Modified: Thu, 10 Aug 2023 01:02:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a39df29b3c0b2f7e691c47273110db4a46e5c8e299f6bb95f77a9c61f79872`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8574d63bce1547e3177d0b76237a782a9b016d4880375dcd1a7b6a1c5dee3dc`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ef34b3c96316bcdd92e24c8c4eebdc3a35f245c013ef87edfae0dde091a305`  
		Last Modified: Thu, 10 Aug 2023 01:02:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a481babc5b629f694446a96dba8d77c020257c98334c605aff94162b9a917279`  
		Last Modified: Thu, 10 Aug 2023 01:02:23 GMT  
		Size: 25.6 MB (25554169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281178ea1c103ff07ea7e4fb647eb0dbe4f865742da6ef9944e04f37974fc27c`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b5d34adf2aacfe87580143f3e17c635dc8dbd4068377b79b35d665f49bbad9`  
		Last Modified: Thu, 10 Aug 2023 01:02:16 GMT  
		Size: 275.9 KB (275946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5b48235253668711a8e6a2ff934add92fea681c9256325d0ad13a01141c047`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4fb7d9dc956e10b22252d8212c98e2dee64526f471fa548eb6c842d5f05ae9`  
		Last Modified: Thu, 10 Aug 2023 01:02:35 GMT  
		Size: 69.2 MB (69216081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b888078988d2c04f6dae8641365e345f00127285805315ff6f554d6b93ac473c`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.5 KB (1451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b841ebd982703c219e6682e9f6ce05952af17249b1feeac24f29b4758db36694`  
		Last Modified: Thu, 17 Aug 2023 22:22:23 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fde1a85f81e8aec976e03a445fd68b44a23b9f74e66320c7dfce58a75409c25`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0498fcf11a96e26aace74390231497cf74c1d199da68217be38339f5e4108a3`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e49f04c5395ab27a41689cde8841498c15d6b18d029bb336e25274009098cc6`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c1983f7985d2513515cbe76bf211a71393e1a54cfd8e6b755d82fef2120d4a`  
		Last Modified: Thu, 17 Aug 2023 22:22:22 GMT  
		Size: 1.7 MB (1690677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d561bf1c2c8101b9e952ebca483dfa257b2d839feabe3857a1a2694e7d5d83f9`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-windowsservercore`

```console
$ docker pull caddy@sha256:9b2d0e89dc4f5f508ec90143d8b6b6d2cdbe9067fea9d0930cbb9812eb816b01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4737; amd64
	-	windows version 10.0.20348.1906; amd64

### `caddy:2.7-windowsservercore` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:8d641d87b059de975dc94ff579d47434e347b333b33a4a8f15cd679c062a14c0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2011934670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e21b2ad9f1a3657d84dd869da76d22704a2848d4a92f831acbfef09e26e80cc6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 14 Aug 2023 18:16:58 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 17 Aug 2023 22:14:59 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:16:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 17 Aug 2023 22:16:13 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 17 Aug 2023 22:16:14 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 17 Aug 2023 22:16:15 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:16:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:16:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:16:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:16:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:16:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:16:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:16:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:16:21 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:16:22 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:16:23 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:16:24 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:17:19 GMT
RUN caddy version
# Thu, 17 Aug 2023 22:17:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d698e8ba8bfd4c31116f0d2c87cfcf2ff17baa1a5c678b116b3aa1ac8ed73d`  
		Last Modified: Mon, 14 Aug 2023 18:23:17 GMT  
		Size: 483.6 KB (483626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dcf545f7c90cab6f6962d3099898462129da2e6b06a80802d52ff1e9d2fca08`  
		Last Modified: Thu, 17 Aug 2023 22:21:12 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65ecc8b4521923b522dd6392a862d0dff9edd10c1e3b520de8f130de2170880`  
		Last Modified: Thu, 17 Aug 2023 22:21:16 GMT  
		Size: 15.2 MB (15201779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ddd9c690b84a4a4744ec5ac91059e12e1aa92378220080fcfbf616c59b4c26`  
		Last Modified: Thu, 17 Aug 2023 22:21:12 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63adbcb9cba5e8d67eac5e059c7bbb9dfe3040f0933afb5e1f8cb7d4c211b4a`  
		Last Modified: Thu, 17 Aug 2023 22:21:11 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e15ff22938f514e6118606619ff28e9e5ee145d6f3dc6de1de62ea4051575c1`  
		Last Modified: Thu, 17 Aug 2023 22:21:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438a6cab105b637f625a3fd00d7ecaa6792ad5dc120bf1be36e7d6e19ee44b4d`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfd206f96497c8e0730c72c36ecedea57379a6a219903785dc1478b50b3945`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e651df7142dc872814a59faff8cf791ab4e4413ee6a9b043fe02a2af9da24fe`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b7f62d857ed7e15d08d52d1ef08f3c21e25751d17e8a5418c02f6adc366eab`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6347f1227dc933d98b8f02d22cd440529284e7c8e415e96cee265ae2c7445b3`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2776f9f89b2242d27c9c49da3465d2ff6acb224dd3315837bda709f3fa0aa4ff`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aaab02f29add47735607e798c40625216306d00d57988d1ece40f43b93f706c`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ed26555e0c9e51aa5dbf4125ef3ea56c6d84274b4d8160ce10c3c0d9e7106d`  
		Last Modified: Thu, 17 Aug 2023 22:21:08 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392c0484ea6d941786f507e72c143bd1c64d4c42bcd773bd745330a55b89d356`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef07137395441a56a870d882d84faac751156b0486c6528fa18b6d706ff250d8`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2950cf3d51ba47c2b41415fccf9b67e813735f67ccc34a0ce5f1a1a4a34e56dc`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25de03b5a8b8f2752cde31b881d457ec5900438b781cc65cda3aca9444b2377f`  
		Last Modified: Thu, 17 Aug 2023 22:21:07 GMT  
		Size: 269.9 KB (269882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f3d70fb1dd11e79f9128736ada85993e1b4fd603b2f8164aac49ac1efda548`  
		Last Modified: Thu, 17 Aug 2023 22:21:07 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-windowsservercore` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:f4791cb0179b98b28e760842405262d782735176b147c84f26709bd1361c8798
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1813299019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b759bf39605cbc0d0ceaaa8eda1623452b1acd67deb11c0d22defff59f2058`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 14 Aug 2023 18:19:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 17 Aug 2023 22:17:27 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:17:55 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 17 Aug 2023 22:17:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 17 Aug 2023 22:17:56 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 17 Aug 2023 22:17:57 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:17:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:17:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:17:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:18:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:18:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:18:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:18:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:18:04 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:18:04 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:18:05 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:18:06 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:18:21 GMT
RUN caddy version
# Thu, 17 Aug 2023 22:18:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c23e01ee014d9e05e276268c94980b00a0720fcb5488a368b20ee74701ed78`  
		Last Modified: Mon, 14 Aug 2023 18:23:42 GMT  
		Size: 461.2 KB (461170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8a7576f0b2ff121a0e9658821e52a7b356abbd90c9215b750ab7fc2127f6ae`  
		Last Modified: Thu, 17 Aug 2023 22:21:41 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ecc6db59a89a0a9f61364702d6af7202fa4f3f742ec6dff93c3a5b53e3826`  
		Last Modified: Thu, 17 Aug 2023 22:21:44 GMT  
		Size: 15.2 MB (15169088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9323e4528d7a59819754484fdbeb047240a6f1f0dd262b734a226a4249dc0a0`  
		Last Modified: Thu, 17 Aug 2023 22:21:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb3a3b69dd93b979cdcd1e0759ee1199bc8d5a510a6ce9bca3856201d747468`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56ce33676578802911228ae7aba31fe1898897ede8c69e12a0959a37a11d130`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c896eeb3f2c45b2bba4fe5e5da02be1289c4cabcf574a38c19d1616ebf552d4c`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6563dd3d5f912ae2b7bd629d2dc731df89b1dd107e2cbb85dee24a0d5c550a1`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420011263062842c72720998f13fa245d9bef077622fde4e17cc60cef3e00bce`  
		Last Modified: Thu, 17 Aug 2023 22:21:38 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2385fc0cb7a281a35df415654aba711bf70fa23b963faf0a3f0055d760f5c41c`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a58351f25f399f8a9399e60dd315cd8c695972a9e51f2271e3377151cf621d`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506eb3a97b70fc7dc1c1c3464a89512890cd48c354658e58e61d5acfee63f1c3`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86cf8c25cfcaf858db6ffd2630a26ca3a13ad2fdc941a01438ea9ea80ccb20c`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcedddef9863d16c4d713280050f604b44968bc253844c27e46cb8871eb17a99`  
		Last Modified: Thu, 17 Aug 2023 22:21:36 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d01313141e38a9b2b15a3e831a2d11a3eb47611bf99b0677be3c49693984f64`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504a80bc0f7aa0c98a143033f551be8fcf0653046e7313c0de080b82ad97ad52`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280053e45030e2421ea4d1cdfd721c24f40d30518b1ce8af7e0811363daf6eca`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0d07466cd8f053bf957a35cbe340d419f5c2f6ff48565bb8a5b255998e3e94`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 280.9 KB (280938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad52776067d7be890960cfd7082041a93a802b96fea6d31fc724192c49eb00`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-windowsservercore-1809`

```console
$ docker pull caddy@sha256:44adcd32029ece40e50aef18ba70e3020cbba5b53153929078326ec23613226c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `caddy:2.7-windowsservercore-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:8d641d87b059de975dc94ff579d47434e347b333b33a4a8f15cd679c062a14c0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2011934670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e21b2ad9f1a3657d84dd869da76d22704a2848d4a92f831acbfef09e26e80cc6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 14 Aug 2023 18:16:58 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 17 Aug 2023 22:14:59 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:16:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 17 Aug 2023 22:16:13 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 17 Aug 2023 22:16:14 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 17 Aug 2023 22:16:15 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:16:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:16:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:16:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:16:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:16:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:16:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:16:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:16:21 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:16:22 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:16:23 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:16:24 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:17:19 GMT
RUN caddy version
# Thu, 17 Aug 2023 22:17:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d698e8ba8bfd4c31116f0d2c87cfcf2ff17baa1a5c678b116b3aa1ac8ed73d`  
		Last Modified: Mon, 14 Aug 2023 18:23:17 GMT  
		Size: 483.6 KB (483626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dcf545f7c90cab6f6962d3099898462129da2e6b06a80802d52ff1e9d2fca08`  
		Last Modified: Thu, 17 Aug 2023 22:21:12 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65ecc8b4521923b522dd6392a862d0dff9edd10c1e3b520de8f130de2170880`  
		Last Modified: Thu, 17 Aug 2023 22:21:16 GMT  
		Size: 15.2 MB (15201779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ddd9c690b84a4a4744ec5ac91059e12e1aa92378220080fcfbf616c59b4c26`  
		Last Modified: Thu, 17 Aug 2023 22:21:12 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63adbcb9cba5e8d67eac5e059c7bbb9dfe3040f0933afb5e1f8cb7d4c211b4a`  
		Last Modified: Thu, 17 Aug 2023 22:21:11 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e15ff22938f514e6118606619ff28e9e5ee145d6f3dc6de1de62ea4051575c1`  
		Last Modified: Thu, 17 Aug 2023 22:21:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438a6cab105b637f625a3fd00d7ecaa6792ad5dc120bf1be36e7d6e19ee44b4d`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfd206f96497c8e0730c72c36ecedea57379a6a219903785dc1478b50b3945`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e651df7142dc872814a59faff8cf791ab4e4413ee6a9b043fe02a2af9da24fe`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b7f62d857ed7e15d08d52d1ef08f3c21e25751d17e8a5418c02f6adc366eab`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6347f1227dc933d98b8f02d22cd440529284e7c8e415e96cee265ae2c7445b3`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2776f9f89b2242d27c9c49da3465d2ff6acb224dd3315837bda709f3fa0aa4ff`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aaab02f29add47735607e798c40625216306d00d57988d1ece40f43b93f706c`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ed26555e0c9e51aa5dbf4125ef3ea56c6d84274b4d8160ce10c3c0d9e7106d`  
		Last Modified: Thu, 17 Aug 2023 22:21:08 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392c0484ea6d941786f507e72c143bd1c64d4c42bcd773bd745330a55b89d356`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef07137395441a56a870d882d84faac751156b0486c6528fa18b6d706ff250d8`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2950cf3d51ba47c2b41415fccf9b67e813735f67ccc34a0ce5f1a1a4a34e56dc`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25de03b5a8b8f2752cde31b881d457ec5900438b781cc65cda3aca9444b2377f`  
		Last Modified: Thu, 17 Aug 2023 22:21:07 GMT  
		Size: 269.9 KB (269882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f3d70fb1dd11e79f9128736ada85993e1b4fd603b2f8164aac49ac1efda548`  
		Last Modified: Thu, 17 Aug 2023 22:21:07 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:25814323b2b1cf78a7dfadd252104b12d24aa4dc9512441a2717cd13b1d3da8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1906; amd64

### `caddy:2.7-windowsservercore-ltsc2022` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:f4791cb0179b98b28e760842405262d782735176b147c84f26709bd1361c8798
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1813299019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b759bf39605cbc0d0ceaaa8eda1623452b1acd67deb11c0d22defff59f2058`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 14 Aug 2023 18:19:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 17 Aug 2023 22:17:27 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:17:55 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 17 Aug 2023 22:17:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 17 Aug 2023 22:17:56 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 17 Aug 2023 22:17:57 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:17:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:17:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:17:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:18:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:18:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:18:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:18:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:18:04 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:18:04 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:18:05 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:18:06 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:18:21 GMT
RUN caddy version
# Thu, 17 Aug 2023 22:18:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c23e01ee014d9e05e276268c94980b00a0720fcb5488a368b20ee74701ed78`  
		Last Modified: Mon, 14 Aug 2023 18:23:42 GMT  
		Size: 461.2 KB (461170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8a7576f0b2ff121a0e9658821e52a7b356abbd90c9215b750ab7fc2127f6ae`  
		Last Modified: Thu, 17 Aug 2023 22:21:41 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ecc6db59a89a0a9f61364702d6af7202fa4f3f742ec6dff93c3a5b53e3826`  
		Last Modified: Thu, 17 Aug 2023 22:21:44 GMT  
		Size: 15.2 MB (15169088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9323e4528d7a59819754484fdbeb047240a6f1f0dd262b734a226a4249dc0a0`  
		Last Modified: Thu, 17 Aug 2023 22:21:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb3a3b69dd93b979cdcd1e0759ee1199bc8d5a510a6ce9bca3856201d747468`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56ce33676578802911228ae7aba31fe1898897ede8c69e12a0959a37a11d130`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c896eeb3f2c45b2bba4fe5e5da02be1289c4cabcf574a38c19d1616ebf552d4c`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6563dd3d5f912ae2b7bd629d2dc731df89b1dd107e2cbb85dee24a0d5c550a1`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420011263062842c72720998f13fa245d9bef077622fde4e17cc60cef3e00bce`  
		Last Modified: Thu, 17 Aug 2023 22:21:38 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2385fc0cb7a281a35df415654aba711bf70fa23b963faf0a3f0055d760f5c41c`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a58351f25f399f8a9399e60dd315cd8c695972a9e51f2271e3377151cf621d`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506eb3a97b70fc7dc1c1c3464a89512890cd48c354658e58e61d5acfee63f1c3`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86cf8c25cfcaf858db6ffd2630a26ca3a13ad2fdc941a01438ea9ea80ccb20c`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcedddef9863d16c4d713280050f604b44968bc253844c27e46cb8871eb17a99`  
		Last Modified: Thu, 17 Aug 2023 22:21:36 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d01313141e38a9b2b15a3e831a2d11a3eb47611bf99b0677be3c49693984f64`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504a80bc0f7aa0c98a143033f551be8fcf0653046e7313c0de080b82ad97ad52`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280053e45030e2421ea4d1cdfd721c24f40d30518b1ce8af7e0811363daf6eca`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0d07466cd8f053bf957a35cbe340d419f5c2f6ff48565bb8a5b255998e3e94`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 280.9 KB (280938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad52776067d7be890960cfd7082041a93a802b96fea6d31fc724192c49eb00`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.4`

```console
$ docker pull caddy@sha256:2332c4ebc4ae778b9697043d3fa3aaef6879dd17abc03200285af9d315353008
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4737; amd64
	-	windows version 10.0.20348.1906; amd64

### `caddy:2.7.4` - linux; amd64

```console
$ docker pull caddy@sha256:733fe94133c4bd22c6ee8f9b9802bce8fede5e7b766bebde205a45dd4ac04aea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18363908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1e1b7ae170b7d7d7e524717fe978e0090023cc82a7d9ffe48e344b0351a3ee1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:09:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 18:20:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:19:38 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:19:41 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:19:41 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:19:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:19:42 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:19:42 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:19:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0aa7b81ef11c65f43b0b58323a33dd9e07eb785529f0d75b452f87a309db00c`  
		Last Modified: Mon, 07 Aug 2023 20:09:40 GMT  
		Size: 350.8 KB (350844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b3b3e68e52dc5ab939c72a9bbac39cff4bef4b87de399ddf28657471df6845`  
		Last Modified: Mon, 14 Aug 2023 18:20:42 GMT  
		Size: 7.5 KB (7502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c55d3259542348ddb70edc18dda7d48aeca5654962aed568a7034f3667d2ca`  
		Last Modified: Thu, 17 Aug 2023 22:20:10 GMT  
		Size: 14.6 MB (14603949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4` - linux; arm variant v6

```console
$ docker pull caddy@sha256:dd029220558032e5d1f91173d32a0078dad12ec9b5114bef422ed4cdf05dec52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17314204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1de0523ee8d8173472fb08aa9a74a37bcd054af2b796b7631d847ba8a46986b5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:38:27 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:49:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:49:12 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:49:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:49:16 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:49:16 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:49:17 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:49:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172ef460a93549b8a3e73f6a515bccad93512788d1e8f095e7230ba41967c25a`  
		Last Modified: Wed, 09 Aug 2023 03:38:53 GMT  
		Size: 347.7 KB (347686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7aae78767a581df85fd1a51ccd646619aec320896ca016ef0f05a41b16bcbfe`  
		Last Modified: Mon, 14 Aug 2023 17:49:36 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82560a340155261ecbd1d99d87890c5aa0cfd64d571e1dcafc03e3b6a8132d48`  
		Last Modified: Thu, 17 Aug 2023 22:49:41 GMT  
		Size: 13.8 MB (13814204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4` - linux; arm variant v7

```console
$ docker pull caddy@sha256:24649e9de43354963118f9cdf6ad1f4522c6993735f316763a2f5d1f76cba267
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17042831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb4a48fd29d50802cbf030949e2c9767eb6888e8412330f64246f322bc3b49c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:51:41 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:57:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:57:18 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:57:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:57:22 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:57:22 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:57:24 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:57:24 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:57:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a47b73e04459258b08555443754e92e2db20bde113c58ca18e1a6f07878f72`  
		Last Modified: Tue, 08 Aug 2023 01:52:05 GMT  
		Size: 344.5 KB (344462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e1b3e18d5e992f1805072b2d52405d575830bdce21726ef99dea99e31d8277`  
		Last Modified: Mon, 14 Aug 2023 17:57:42 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5879767a5d1969beb154b9a4991a767b0ed5be0c9739a972f07d03e825312fa5`  
		Last Modified: Thu, 17 Aug 2023 22:57:51 GMT  
		Size: 13.8 MB (13791384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:ed967fcd1968be6dc4699ff835cdd2d6f3f49105b9677f878c8a6960fd1a0643
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17162547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed7b6600470cab547aa1090baa39a6192ec83119989884ac742a63ed23be3da2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:09:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:39:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:39:17 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:39:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:39:19 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:39:19 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:39:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:39:20 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:39:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a699f78cfb85f60e17fc7c13495876ea0cb4495bbe39e8c65f3e8559b0d7169`  
		Last Modified: Mon, 07 Aug 2023 21:09:34 GMT  
		Size: 360.6 KB (360642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7488af8b96c79b6db13955a0302653c4e9f314d0833201984ae06c1ed697f06`  
		Last Modified: Mon, 14 Aug 2023 17:39:41 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597bfc484ba18727d2df98120cb9d559f346ade9e3a23be6a9af3e76dca89edd`  
		Last Modified: Thu, 17 Aug 2023 22:39:42 GMT  
		Size: 13.5 MB (13463635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4` - linux; ppc64le

```console
$ docker pull caddy@sha256:c3679836562d0252e6341a112d2729b8dae0eae550449bfe91fe2798171fd4ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16944934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc5ac831dce746cd0f4448640b7edaf0ce9457d09618e246ba72ee76ea63dcbe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:44:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 18:18:00 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:16:24 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:16:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:16:29 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:16:29 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:16:29 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:16:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:16:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:16:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:16:32 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:16:33 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:16:33 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:16:34 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:16:34 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:16:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f40714f45e39ac41e865ccbf2877db62255ce5a5c36a47eadf00b9d174f042`  
		Last Modified: Tue, 08 Aug 2023 00:45:18 GMT  
		Size: 362.2 KB (362173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d19953b5eb53ddaa0e25905527dc138e0c4111467bb7d71f81fa94976091351`  
		Last Modified: Mon, 14 Aug 2023 18:18:54 GMT  
		Size: 7.5 KB (7509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf4bf695323732c5ce84bbb0b976c5cd981eaf6814515a86f521af4a0e64582`  
		Last Modified: Thu, 17 Aug 2023 22:17:22 GMT  
		Size: 13.2 MB (13229001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4` - linux; s390x

```console
$ docker pull caddy@sha256:ca7ab0dcf4ab146df48cfa8ae6e07fed804feeed4a36358fa652c8eac52b40da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17720356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d4d019ffc0cd69ea8c5d3b8fb0a39c89d3aa1b2037c1012a9ba4bed6abb94dc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:14:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:41:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:41:35 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:41:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:41:39 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:41:39 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:41:39 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:41:40 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:41:41 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:41:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df19abd0ca1d4a821a4174a2c0831a57d6fd584073f056abcae085a51f0b3848`  
		Last Modified: Mon, 07 Aug 2023 20:14:50 GMT  
		Size: 354.9 KB (354950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308478977890baa82477ee70a3065fb9da2080efcc95facf1a87ac021b06a8e9`  
		Last Modified: Mon, 14 Aug 2023 17:42:17 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2394cd7c9416df19c45596c558f5a7ee05adc5a7fd166f58dcbf26f1ac6ecae6`  
		Last Modified: Thu, 17 Aug 2023 22:42:16 GMT  
		Size: 14.1 MB (14143708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:8d641d87b059de975dc94ff579d47434e347b333b33a4a8f15cd679c062a14c0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2011934670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e21b2ad9f1a3657d84dd869da76d22704a2848d4a92f831acbfef09e26e80cc6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 14 Aug 2023 18:16:58 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 17 Aug 2023 22:14:59 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:16:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 17 Aug 2023 22:16:13 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 17 Aug 2023 22:16:14 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 17 Aug 2023 22:16:15 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:16:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:16:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:16:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:16:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:16:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:16:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:16:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:16:21 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:16:22 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:16:23 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:16:24 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:17:19 GMT
RUN caddy version
# Thu, 17 Aug 2023 22:17:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d698e8ba8bfd4c31116f0d2c87cfcf2ff17baa1a5c678b116b3aa1ac8ed73d`  
		Last Modified: Mon, 14 Aug 2023 18:23:17 GMT  
		Size: 483.6 KB (483626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dcf545f7c90cab6f6962d3099898462129da2e6b06a80802d52ff1e9d2fca08`  
		Last Modified: Thu, 17 Aug 2023 22:21:12 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65ecc8b4521923b522dd6392a862d0dff9edd10c1e3b520de8f130de2170880`  
		Last Modified: Thu, 17 Aug 2023 22:21:16 GMT  
		Size: 15.2 MB (15201779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ddd9c690b84a4a4744ec5ac91059e12e1aa92378220080fcfbf616c59b4c26`  
		Last Modified: Thu, 17 Aug 2023 22:21:12 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63adbcb9cba5e8d67eac5e059c7bbb9dfe3040f0933afb5e1f8cb7d4c211b4a`  
		Last Modified: Thu, 17 Aug 2023 22:21:11 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e15ff22938f514e6118606619ff28e9e5ee145d6f3dc6de1de62ea4051575c1`  
		Last Modified: Thu, 17 Aug 2023 22:21:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438a6cab105b637f625a3fd00d7ecaa6792ad5dc120bf1be36e7d6e19ee44b4d`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfd206f96497c8e0730c72c36ecedea57379a6a219903785dc1478b50b3945`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e651df7142dc872814a59faff8cf791ab4e4413ee6a9b043fe02a2af9da24fe`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b7f62d857ed7e15d08d52d1ef08f3c21e25751d17e8a5418c02f6adc366eab`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6347f1227dc933d98b8f02d22cd440529284e7c8e415e96cee265ae2c7445b3`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2776f9f89b2242d27c9c49da3465d2ff6acb224dd3315837bda709f3fa0aa4ff`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aaab02f29add47735607e798c40625216306d00d57988d1ece40f43b93f706c`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ed26555e0c9e51aa5dbf4125ef3ea56c6d84274b4d8160ce10c3c0d9e7106d`  
		Last Modified: Thu, 17 Aug 2023 22:21:08 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392c0484ea6d941786f507e72c143bd1c64d4c42bcd773bd745330a55b89d356`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef07137395441a56a870d882d84faac751156b0486c6528fa18b6d706ff250d8`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2950cf3d51ba47c2b41415fccf9b67e813735f67ccc34a0ce5f1a1a4a34e56dc`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25de03b5a8b8f2752cde31b881d457ec5900438b781cc65cda3aca9444b2377f`  
		Last Modified: Thu, 17 Aug 2023 22:21:07 GMT  
		Size: 269.9 KB (269882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f3d70fb1dd11e79f9128736ada85993e1b4fd603b2f8164aac49ac1efda548`  
		Last Modified: Thu, 17 Aug 2023 22:21:07 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:f4791cb0179b98b28e760842405262d782735176b147c84f26709bd1361c8798
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1813299019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b759bf39605cbc0d0ceaaa8eda1623452b1acd67deb11c0d22defff59f2058`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 14 Aug 2023 18:19:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 17 Aug 2023 22:17:27 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:17:55 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 17 Aug 2023 22:17:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 17 Aug 2023 22:17:56 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 17 Aug 2023 22:17:57 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:17:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:17:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:17:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:18:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:18:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:18:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:18:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:18:04 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:18:04 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:18:05 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:18:06 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:18:21 GMT
RUN caddy version
# Thu, 17 Aug 2023 22:18:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c23e01ee014d9e05e276268c94980b00a0720fcb5488a368b20ee74701ed78`  
		Last Modified: Mon, 14 Aug 2023 18:23:42 GMT  
		Size: 461.2 KB (461170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8a7576f0b2ff121a0e9658821e52a7b356abbd90c9215b750ab7fc2127f6ae`  
		Last Modified: Thu, 17 Aug 2023 22:21:41 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ecc6db59a89a0a9f61364702d6af7202fa4f3f742ec6dff93c3a5b53e3826`  
		Last Modified: Thu, 17 Aug 2023 22:21:44 GMT  
		Size: 15.2 MB (15169088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9323e4528d7a59819754484fdbeb047240a6f1f0dd262b734a226a4249dc0a0`  
		Last Modified: Thu, 17 Aug 2023 22:21:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb3a3b69dd93b979cdcd1e0759ee1199bc8d5a510a6ce9bca3856201d747468`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56ce33676578802911228ae7aba31fe1898897ede8c69e12a0959a37a11d130`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c896eeb3f2c45b2bba4fe5e5da02be1289c4cabcf574a38c19d1616ebf552d4c`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6563dd3d5f912ae2b7bd629d2dc731df89b1dd107e2cbb85dee24a0d5c550a1`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420011263062842c72720998f13fa245d9bef077622fde4e17cc60cef3e00bce`  
		Last Modified: Thu, 17 Aug 2023 22:21:38 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2385fc0cb7a281a35df415654aba711bf70fa23b963faf0a3f0055d760f5c41c`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a58351f25f399f8a9399e60dd315cd8c695972a9e51f2271e3377151cf621d`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506eb3a97b70fc7dc1c1c3464a89512890cd48c354658e58e61d5acfee63f1c3`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86cf8c25cfcaf858db6ffd2630a26ca3a13ad2fdc941a01438ea9ea80ccb20c`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcedddef9863d16c4d713280050f604b44968bc253844c27e46cb8871eb17a99`  
		Last Modified: Thu, 17 Aug 2023 22:21:36 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d01313141e38a9b2b15a3e831a2d11a3eb47611bf99b0677be3c49693984f64`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504a80bc0f7aa0c98a143033f551be8fcf0653046e7313c0de080b82ad97ad52`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280053e45030e2421ea4d1cdfd721c24f40d30518b1ce8af7e0811363daf6eca`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0d07466cd8f053bf957a35cbe340d419f5c2f6ff48565bb8a5b255998e3e94`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 280.9 KB (280938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad52776067d7be890960cfd7082041a93a802b96fea6d31fc724192c49eb00`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.4-alpine`

```console
$ docker pull caddy@sha256:7e01c08308bc94c1ef3e495f0b2ba469d1f7e8d1a4f2caa2fbe189edf48866a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.7.4-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:733fe94133c4bd22c6ee8f9b9802bce8fede5e7b766bebde205a45dd4ac04aea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18363908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1e1b7ae170b7d7d7e524717fe978e0090023cc82a7d9ffe48e344b0351a3ee1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:09:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 18:20:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:19:38 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:19:41 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:19:41 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:19:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:19:42 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:19:42 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:19:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0aa7b81ef11c65f43b0b58323a33dd9e07eb785529f0d75b452f87a309db00c`  
		Last Modified: Mon, 07 Aug 2023 20:09:40 GMT  
		Size: 350.8 KB (350844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b3b3e68e52dc5ab939c72a9bbac39cff4bef4b87de399ddf28657471df6845`  
		Last Modified: Mon, 14 Aug 2023 18:20:42 GMT  
		Size: 7.5 KB (7502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c55d3259542348ddb70edc18dda7d48aeca5654962aed568a7034f3667d2ca`  
		Last Modified: Thu, 17 Aug 2023 22:20:10 GMT  
		Size: 14.6 MB (14603949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:dd029220558032e5d1f91173d32a0078dad12ec9b5114bef422ed4cdf05dec52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17314204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1de0523ee8d8173472fb08aa9a74a37bcd054af2b796b7631d847ba8a46986b5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:38:27 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:49:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:49:12 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:49:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:49:16 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:49:16 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:49:17 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:49:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172ef460a93549b8a3e73f6a515bccad93512788d1e8f095e7230ba41967c25a`  
		Last Modified: Wed, 09 Aug 2023 03:38:53 GMT  
		Size: 347.7 KB (347686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7aae78767a581df85fd1a51ccd646619aec320896ca016ef0f05a41b16bcbfe`  
		Last Modified: Mon, 14 Aug 2023 17:49:36 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82560a340155261ecbd1d99d87890c5aa0cfd64d571e1dcafc03e3b6a8132d48`  
		Last Modified: Thu, 17 Aug 2023 22:49:41 GMT  
		Size: 13.8 MB (13814204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:24649e9de43354963118f9cdf6ad1f4522c6993735f316763a2f5d1f76cba267
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17042831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb4a48fd29d50802cbf030949e2c9767eb6888e8412330f64246f322bc3b49c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:51:41 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:57:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:57:18 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:57:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:57:22 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:57:22 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:57:24 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:57:24 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:57:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a47b73e04459258b08555443754e92e2db20bde113c58ca18e1a6f07878f72`  
		Last Modified: Tue, 08 Aug 2023 01:52:05 GMT  
		Size: 344.5 KB (344462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e1b3e18d5e992f1805072b2d52405d575830bdce21726ef99dea99e31d8277`  
		Last Modified: Mon, 14 Aug 2023 17:57:42 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5879767a5d1969beb154b9a4991a767b0ed5be0c9739a972f07d03e825312fa5`  
		Last Modified: Thu, 17 Aug 2023 22:57:51 GMT  
		Size: 13.8 MB (13791384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:ed967fcd1968be6dc4699ff835cdd2d6f3f49105b9677f878c8a6960fd1a0643
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17162547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed7b6600470cab547aa1090baa39a6192ec83119989884ac742a63ed23be3da2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:09:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:39:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:39:17 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:39:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:39:19 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:39:19 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:39:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:39:20 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:39:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a699f78cfb85f60e17fc7c13495876ea0cb4495bbe39e8c65f3e8559b0d7169`  
		Last Modified: Mon, 07 Aug 2023 21:09:34 GMT  
		Size: 360.6 KB (360642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7488af8b96c79b6db13955a0302653c4e9f314d0833201984ae06c1ed697f06`  
		Last Modified: Mon, 14 Aug 2023 17:39:41 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597bfc484ba18727d2df98120cb9d559f346ade9e3a23be6a9af3e76dca89edd`  
		Last Modified: Thu, 17 Aug 2023 22:39:42 GMT  
		Size: 13.5 MB (13463635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:c3679836562d0252e6341a112d2729b8dae0eae550449bfe91fe2798171fd4ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16944934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc5ac831dce746cd0f4448640b7edaf0ce9457d09618e246ba72ee76ea63dcbe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:44:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 18:18:00 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:16:24 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:16:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:16:29 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:16:29 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:16:29 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:16:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:16:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:16:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:16:32 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:16:33 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:16:33 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:16:34 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:16:34 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:16:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f40714f45e39ac41e865ccbf2877db62255ce5a5c36a47eadf00b9d174f042`  
		Last Modified: Tue, 08 Aug 2023 00:45:18 GMT  
		Size: 362.2 KB (362173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d19953b5eb53ddaa0e25905527dc138e0c4111467bb7d71f81fa94976091351`  
		Last Modified: Mon, 14 Aug 2023 18:18:54 GMT  
		Size: 7.5 KB (7509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf4bf695323732c5ce84bbb0b976c5cd981eaf6814515a86f521af4a0e64582`  
		Last Modified: Thu, 17 Aug 2023 22:17:22 GMT  
		Size: 13.2 MB (13229001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:ca7ab0dcf4ab146df48cfa8ae6e07fed804feeed4a36358fa652c8eac52b40da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17720356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d4d019ffc0cd69ea8c5d3b8fb0a39c89d3aa1b2037c1012a9ba4bed6abb94dc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:14:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:41:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:41:35 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:41:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:41:39 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:41:39 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:41:39 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:41:40 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:41:41 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:41:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df19abd0ca1d4a821a4174a2c0831a57d6fd584073f056abcae085a51f0b3848`  
		Last Modified: Mon, 07 Aug 2023 20:14:50 GMT  
		Size: 354.9 KB (354950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308478977890baa82477ee70a3065fb9da2080efcc95facf1a87ac021b06a8e9`  
		Last Modified: Mon, 14 Aug 2023 17:42:17 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2394cd7c9416df19c45596c558f5a7ee05adc5a7fd166f58dcbf26f1ac6ecae6`  
		Last Modified: Thu, 17 Aug 2023 22:42:16 GMT  
		Size: 14.1 MB (14143708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.4-builder`

```console
$ docker pull caddy@sha256:eafc66404950e4170122aba0977f7079d888e544bed6df61a144b50bcf06bbb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4737; amd64
	-	windows version 10.0.20348.1906; amd64

### `caddy:2.7.4-builder` - linux; amd64

```console
$ docker pull caddy@sha256:716dc5ded2a0c7090ac3cf0d298122538ac67a0152c97b88a17520c2b0419d82
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76949834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0789fd27a45de2db1b44ab683c8b91c2f63b230c312d20bb2b45294d44c8d02b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:36:47 GMT
RUN apk add --no-cache ca-certificates
# Wed, 09 Aug 2023 04:41:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:29 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:31:40 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:31:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:31:41 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:58:36 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:58:37 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:58:37 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:58:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:58:37 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:58:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:58:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:58:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d48a809fc2256f8aa0aeee47998488d64409855adba00a7cb3007ab9f3286e`  
		Last Modified: Wed, 09 Aug 2023 03:37:02 GMT  
		Size: 284.7 KB (284693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60be0ca469417450769350b29d9d86e57dc60849c11fab3e8d0b556fcc35005`  
		Last Modified: Wed, 06 Sep 2023 18:37:24 GMT  
		Size: 67.0 MB (67002091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb14ea137979420ee28a5d750e5d62200f15a09c2461e13a8f10023e5fbf5a2`  
		Last Modified: Wed, 06 Sep 2023 18:37:12 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d4cebe2e13d01b24cfdc9eaeae90b4a21f72815fffd9a6a0bb96d99bd0552a`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 5.0 MB (4958640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb64c4e131a2a58133f92ec61aefa25cfb66ef81c5dc749f4de450feb5349c8`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 1.3 MB (1302236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce602f0d9b5db7d56aabf2bf531824f371f52db43d9dc61da5ac5856f69c7359`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:0a1d4936666edfd074f88e0eeeefc1402111cc54a0fcc57963ae88dde642fdca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75388438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c765f590b091ce124e5856c924f7305627163a3a17955d23a482fb20592c338`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:12:05 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:12:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:30:47 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:31:16 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:31:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:31:17 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:54:56 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:54:56 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:54:56 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:54:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:54:56 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:54:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:54:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:54:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8564ce36feee688566265012773f1c8c7c046ceefe86ca763eb702682f4e6e75`  
		Last Modified: Tue, 08 Aug 2023 23:15:06 GMT  
		Size: 284.9 KB (284876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63353306cb1a8907bf53eeefec13043d0f70b554332a60aa92bb4c3861b93c8`  
		Last Modified: Wed, 06 Sep 2023 18:37:56 GMT  
		Size: 65.8 MB (65758368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a286c00e60caea02b9c22fac7d8a91c9ffa40d7fc56aea06e0f8f67c5d3001b8`  
		Last Modified: Wed, 06 Sep 2023 18:37:33 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6650d2d716414907ceaad018d0c2a57750f812da3ce864c723329a9691bfab`  
		Last Modified: Wed, 06 Sep 2023 18:55:14 GMT  
		Size: 5.0 MB (4951168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ebf8a554fac09b4da4a7072225799fa9bc12129c257b93d7dfabc9b7370c0a`  
		Last Modified: Wed, 06 Sep 2023 18:55:14 GMT  
		Size: 1.2 MB (1248657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9711d57485a382ed790b0a10b1af2b8a817f3973693a9add4edf8752b7aae66c`  
		Last Modified: Wed, 06 Sep 2023 18:55:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fe3ec3b57937f6ee95b60afb48874baeee931a06cbb59c944943b498a9016d1c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74690125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590b4483c17141a335fd0eb382750e044c6c5b452db059d3eb1d1aef7950dd3e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:39:47 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 01:39:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:45 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:32:02 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:32:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:32:04 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:58:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:58:39 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:58:39 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:58:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:58:39 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:58:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:58:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:58:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47bd95d78f565e902bafd0264a979eb4f6f71e22c0464011bf9db6feb0579e6`  
		Last Modified: Tue, 08 Aug 2023 01:48:34 GMT  
		Size: 284.1 KB (284073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812db0f4af4ab09f020f5a4b3fb1803a8afdf60db3d0e0c2d451a717141054ca`  
		Last Modified: Wed, 06 Sep 2023 18:40:37 GMT  
		Size: 65.8 MB (65758511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f0657fffaca6c4a15be6c893e54fcf97d14db5815402a0a65f47d5f64b0937`  
		Last Modified: Wed, 06 Sep 2023 18:40:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083d5d74986bc09d57d6a94953a8cb9ab9fbfa44318c32ae6ef17887246f4e9a`  
		Last Modified: Wed, 06 Sep 2023 18:58:57 GMT  
		Size: 4.5 MB (4501414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85d58c05537603de5ce91a6463ef5a223b7ae94f24e05f506b943a930c13a6d`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 1.2 MB (1246086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db284285eec9597c8be93b8c4bd04c0c3b98bf4b089bd52ac26deca4af958251`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:54be0967bfdce111e3176e2c420aab107673db7adc6518b9063186a5bbf6041d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73978310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09ffe7cfa702a73c974a46cf5861ef5c87d89301c99cdda3a283fa9f2ed80442`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:10:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:10:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:18 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:31:28 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:31:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:31:28 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:53:26 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:53:26 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:53:27 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:53:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:53:27 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:53:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:53:28 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:53:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d54e960e981301b0098c80d2e61d694333b5ab480a007a3a8d0fa629662d377`  
		Last Modified: Tue, 08 Aug 2023 23:14:21 GMT  
		Size: 286.3 KB (286298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f000f33a92ab709a2599fbb82fa02eca8bca5b4fda93be45a8d0f1daabb73205`  
		Last Modified: Wed, 06 Sep 2023 18:36:08 GMT  
		Size: 64.1 MB (64108346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447d217685f511c828462bf16ea4579fdb55b103cb1a78d6ba5f0ab6a11db3f8`  
		Last Modified: Wed, 06 Sep 2023 18:35:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13822537d61bbdeb74e6e4458b659dbe1f0d9e3d45af3f50566be42e4b7c809`  
		Last Modified: Wed, 06 Sep 2023 18:53:44 GMT  
		Size: 5.1 MB (5053893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e7da4574a51623195c2699e1b61e06fcc41a5dbde49d5fc96691297a6cd780`  
		Last Modified: Wed, 06 Sep 2023 18:53:43 GMT  
		Size: 1.2 MB (1198447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2621576cb4d382e73ece4231dc51aef77167014d8f83460cbf64238db1fcc45c`  
		Last Modified: Wed, 06 Sep 2023 18:53:43 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:327d6fc238b35334c09db1685ededbacde6621b970825db074650fd341377f2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74185704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0eb6c48fb9239e3fb240aa27acdc3ee85d23fe96322a0606b54ce159b6c2b49`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:25:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 00:25:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:13 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:32:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:32:46 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:32:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:32:50 GMT
WORKDIR /go
# Wed, 06 Sep 2023 19:02:19 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 19:02:21 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 19:02:24 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 19:02:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 19:02:29 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 19:02:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 19:02:35 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 19:02:37 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c966ad2cdd35689da92e7c8fd39bd37cd6080c484e6ccaf00672c154cd4f6c2a`  
		Last Modified: Tue, 08 Aug 2023 00:39:35 GMT  
		Size: 286.7 KB (286662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679e04809663a2145818569201c1dcf2d46798f2198322a8e7910805a9b7dffd`  
		Last Modified: Wed, 06 Sep 2023 18:43:51 GMT  
		Size: 64.1 MB (64116069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1f0b6eb00af4cec1a2c3a203cf9a97b7b5b1e669db11dbabc36635b0207c79`  
		Last Modified: Wed, 06 Sep 2023 18:40:01 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcccd971afab022c32a88b23bc041273f72068caf215514da40b393e06632d93`  
		Last Modified: Wed, 06 Sep 2023 19:02:58 GMT  
		Size: 5.2 MB (5249983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc46690ff4c485e0fea9ac4b7505da047150045d9fcda46c2732480dc1f702`  
		Last Modified: Wed, 06 Sep 2023 19:02:58 GMT  
		Size: 1.2 MB (1186177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b59573283fbd9dc92a2d9a89bd66c6ee4d768933cc1388180a9c1ec35fed90d`  
		Last Modified: Wed, 06 Sep 2023 19:02:57 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-builder` - linux; s390x

```console
$ docker pull caddy@sha256:962738aef2725a7bbec2affa560a8497519a54f466f2c84dbfce42be5ab69896
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76084584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2852f51f18c2cd12f1e50eebc15bffa67e107a714382697c8beabe14b1ba6d0f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:41 GMT
RUN apk add --no-cache ca-certificates
# Mon, 07 Aug 2023 20:19:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:19 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:32:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:32:47 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:32:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:32:48 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:57:37 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:57:37 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:57:37 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:57:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:57:37 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:57:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:57:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:57:39 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec90be18226e5c99d10161aed1a143f4134093c55b4d6979bbdbbe4b0683eb11`  
		Last Modified: Mon, 07 Aug 2023 20:30:59 GMT  
		Size: 285.1 KB (285089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53e61151a7324ffa6693144a2516060d0505b80fe8f27915b1e77165106c2a4`  
		Last Modified: Wed, 06 Sep 2023 18:40:12 GMT  
		Size: 66.2 MB (66222411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1f0b6eb00af4cec1a2c3a203cf9a97b7b5b1e669db11dbabc36635b0207c79`  
		Last Modified: Wed, 06 Sep 2023 18:40:01 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178fae6c6c7b745dbb7be349b0656255d25dc06d0c808f85cce56fdf95543af6`  
		Last Modified: Wed, 06 Sep 2023 18:58:02 GMT  
		Size: 5.1 MB (5099943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bda7158ac61debfc44dddd51b20bf5e411c5f34ec92ad21dfffe9a0eeb5ae76`  
		Last Modified: Wed, 06 Sep 2023 18:58:02 GMT  
		Size: 1.3 MB (1262386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13aa15f1f389977eef4ccb0c676963b08cbf0600c3979659a8852b95689e91e8`  
		Last Modified: Wed, 06 Sep 2023 18:58:02 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-builder` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:dc29929d7895f513f69e34dede7fb945b1bf1540fb37abda23f6fa2edcaa5150
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2092646318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03e3e89d97096b15070b9c1274ebdfe7a5e0de7816cd24a72782cdcb25b33dc3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:39:54 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:39:56 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:41:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:41:12 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:42:07 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:42:08 GMT
ENV GOLANG_VERSION=1.21.0
# Thu, 10 Aug 2023 00:45:16 GMT
RUN $url = 'https://dl.google.com/go/go1.21.0.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '732121e64e0ecb07c77fdf6cc1bc5ce7b242c2d40d4ac29021ad4c64a08731f6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:45:17 GMT
WORKDIR C:\go
# Thu, 17 Aug 2023 22:18:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Aug 2023 22:18:30 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 17 Aug 2023 22:18:31 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:18:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 17 Aug 2023 22:19:38 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 17 Aug 2023 22:19:39 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594083c5c2094c95b4e52723d54c14e0d70881f4f176720c3170012275accc3b`  
		Last Modified: Thu, 10 Aug 2023 01:02:54 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e2c2a5b75ced3a3a50be088c4a6c2d7df926b1fe6515b2d0c021312e3642f4`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d28688050deeec928289543beadf5c75bb2a8246576cb7c066e23818016217`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e5fbc50e7e0fefb7c9e349038ecb00ed5c000bcab8c4d82b1e1000c4273c01`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0544e07bd9df923e11e09c7dc042da614f2f14589eb6fa79005ebbbf2731e97d`  
		Last Modified: Thu, 10 Aug 2023 01:02:57 GMT  
		Size: 25.6 MB (25560980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555a82506c4fcec2bd90ae77756e5b03788e30c89f1a3820aa0b6a7ae6ad58ae`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bcfb422b104764156fc5ba099b5e3ae9fa9f760fd2db1c21acd8969b3d73de`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 220.8 KB (220796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:decc470f4f54c3be087cde5dfcbd816bc68a441d25189983c12219fb4504e9e0`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4589eb0957da5bce467ff89344ebebb2f584a815991fd3004ae3f4890b74f51`  
		Last Modified: Thu, 10 Aug 2023 01:03:10 GMT  
		Size: 69.2 MB (69210847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a698ba14b77be2efdb0e931dc9abf7efc7c749ce53fa2d1c277cd009f295c0`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.5 KB (1517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265b35725533ea18f9e8b7d3422e1b960406141ca305f83de8f61dd49b340c74`  
		Last Modified: Thu, 17 Aug 2023 22:22:07 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3cd40483d2a2e0aae25c4caf3e900aca669895009d08c100e8754768099257`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1aaed9881a7c5017bdf3b46a5ba81399cd7bdaf9be397334872bbf8826386b`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00f7ca68792eb07043e7b43dec1b74b4e211701549286cdcc7993a3b76fdbce`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2516df9efacfe0206db24dbf7d952da6820b3ba9189c715b7aeb069bf903b0b`  
		Last Modified: Thu, 17 Aug 2023 22:22:05 GMT  
		Size: 1.7 MB (1680500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ed01fbe50be0cb731bfdaf18ffaad3e427b9cd10eaabf4930a0dda4b98450`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-builder` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:16053b4036029cc1457cb147a03be7a416b3fd01393e467beeb72def1f482edf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1894119169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e467c74cf811ff36bfae3619793832f5179eba1986cd92d51528fa3631e15b67`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:36:23 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:36:24 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:36:25 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:36:26 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:36:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:37:00 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:37:19 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:37:20 GMT
ENV GOLANG_VERSION=1.21.0
# Thu, 10 Aug 2023 00:39:40 GMT
RUN $url = 'https://dl.google.com/go/go1.21.0.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '732121e64e0ecb07c77fdf6cc1bc5ce7b242c2d40d4ac29021ad4c64a08731f6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:39:42 GMT
WORKDIR C:\go
# Thu, 17 Aug 2023 22:19:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Aug 2023 22:19:58 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 17 Aug 2023 22:19:58 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:19:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 17 Aug 2023 22:20:24 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 17 Aug 2023 22:20:25 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877256a6389e5e2563da79ad5bd201e7ee136abf14ff7cb0d4efbf3b24e5f127`  
		Last Modified: Thu, 10 Aug 2023 01:02:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a39df29b3c0b2f7e691c47273110db4a46e5c8e299f6bb95f77a9c61f79872`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8574d63bce1547e3177d0b76237a782a9b016d4880375dcd1a7b6a1c5dee3dc`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ef34b3c96316bcdd92e24c8c4eebdc3a35f245c013ef87edfae0dde091a305`  
		Last Modified: Thu, 10 Aug 2023 01:02:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a481babc5b629f694446a96dba8d77c020257c98334c605aff94162b9a917279`  
		Last Modified: Thu, 10 Aug 2023 01:02:23 GMT  
		Size: 25.6 MB (25554169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281178ea1c103ff07ea7e4fb647eb0dbe4f865742da6ef9944e04f37974fc27c`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b5d34adf2aacfe87580143f3e17c635dc8dbd4068377b79b35d665f49bbad9`  
		Last Modified: Thu, 10 Aug 2023 01:02:16 GMT  
		Size: 275.9 KB (275946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5b48235253668711a8e6a2ff934add92fea681c9256325d0ad13a01141c047`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4fb7d9dc956e10b22252d8212c98e2dee64526f471fa548eb6c842d5f05ae9`  
		Last Modified: Thu, 10 Aug 2023 01:02:35 GMT  
		Size: 69.2 MB (69216081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b888078988d2c04f6dae8641365e345f00127285805315ff6f554d6b93ac473c`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.5 KB (1451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b841ebd982703c219e6682e9f6ce05952af17249b1feeac24f29b4758db36694`  
		Last Modified: Thu, 17 Aug 2023 22:22:23 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fde1a85f81e8aec976e03a445fd68b44a23b9f74e66320c7dfce58a75409c25`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0498fcf11a96e26aace74390231497cf74c1d199da68217be38339f5e4108a3`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e49f04c5395ab27a41689cde8841498c15d6b18d029bb336e25274009098cc6`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c1983f7985d2513515cbe76bf211a71393e1a54cfd8e6b755d82fef2120d4a`  
		Last Modified: Thu, 17 Aug 2023 22:22:22 GMT  
		Size: 1.7 MB (1690677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d561bf1c2c8101b9e952ebca483dfa257b2d839feabe3857a1a2694e7d5d83f9`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.4-builder-alpine`

```console
$ docker pull caddy@sha256:49505e7a951d9bba52ba419765e3efdee346bce23e25fdb3260a33d0429c7ce9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.7.4-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:716dc5ded2a0c7090ac3cf0d298122538ac67a0152c97b88a17520c2b0419d82
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76949834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0789fd27a45de2db1b44ab683c8b91c2f63b230c312d20bb2b45294d44c8d02b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:36:47 GMT
RUN apk add --no-cache ca-certificates
# Wed, 09 Aug 2023 04:41:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:29 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:31:40 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:31:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:31:41 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:58:36 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:58:37 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:58:37 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:58:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:58:37 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:58:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:58:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:58:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d48a809fc2256f8aa0aeee47998488d64409855adba00a7cb3007ab9f3286e`  
		Last Modified: Wed, 09 Aug 2023 03:37:02 GMT  
		Size: 284.7 KB (284693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60be0ca469417450769350b29d9d86e57dc60849c11fab3e8d0b556fcc35005`  
		Last Modified: Wed, 06 Sep 2023 18:37:24 GMT  
		Size: 67.0 MB (67002091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb14ea137979420ee28a5d750e5d62200f15a09c2461e13a8f10023e5fbf5a2`  
		Last Modified: Wed, 06 Sep 2023 18:37:12 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d4cebe2e13d01b24cfdc9eaeae90b4a21f72815fffd9a6a0bb96d99bd0552a`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 5.0 MB (4958640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb64c4e131a2a58133f92ec61aefa25cfb66ef81c5dc749f4de450feb5349c8`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 1.3 MB (1302236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce602f0d9b5db7d56aabf2bf531824f371f52db43d9dc61da5ac5856f69c7359`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:0a1d4936666edfd074f88e0eeeefc1402111cc54a0fcc57963ae88dde642fdca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75388438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c765f590b091ce124e5856c924f7305627163a3a17955d23a482fb20592c338`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:12:05 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:12:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:30:47 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:31:16 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:31:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:31:17 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:54:56 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:54:56 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:54:56 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:54:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:54:56 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:54:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:54:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:54:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8564ce36feee688566265012773f1c8c7c046ceefe86ca763eb702682f4e6e75`  
		Last Modified: Tue, 08 Aug 2023 23:15:06 GMT  
		Size: 284.9 KB (284876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63353306cb1a8907bf53eeefec13043d0f70b554332a60aa92bb4c3861b93c8`  
		Last Modified: Wed, 06 Sep 2023 18:37:56 GMT  
		Size: 65.8 MB (65758368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a286c00e60caea02b9c22fac7d8a91c9ffa40d7fc56aea06e0f8f67c5d3001b8`  
		Last Modified: Wed, 06 Sep 2023 18:37:33 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6650d2d716414907ceaad018d0c2a57750f812da3ce864c723329a9691bfab`  
		Last Modified: Wed, 06 Sep 2023 18:55:14 GMT  
		Size: 5.0 MB (4951168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ebf8a554fac09b4da4a7072225799fa9bc12129c257b93d7dfabc9b7370c0a`  
		Last Modified: Wed, 06 Sep 2023 18:55:14 GMT  
		Size: 1.2 MB (1248657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9711d57485a382ed790b0a10b1af2b8a817f3973693a9add4edf8752b7aae66c`  
		Last Modified: Wed, 06 Sep 2023 18:55:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fe3ec3b57937f6ee95b60afb48874baeee931a06cbb59c944943b498a9016d1c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74690125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590b4483c17141a335fd0eb382750e044c6c5b452db059d3eb1d1aef7950dd3e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:39:47 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 01:39:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:45 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:32:02 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:32:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:32:04 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:58:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:58:39 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:58:39 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:58:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:58:39 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:58:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:58:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:58:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47bd95d78f565e902bafd0264a979eb4f6f71e22c0464011bf9db6feb0579e6`  
		Last Modified: Tue, 08 Aug 2023 01:48:34 GMT  
		Size: 284.1 KB (284073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812db0f4af4ab09f020f5a4b3fb1803a8afdf60db3d0e0c2d451a717141054ca`  
		Last Modified: Wed, 06 Sep 2023 18:40:37 GMT  
		Size: 65.8 MB (65758511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f0657fffaca6c4a15be6c893e54fcf97d14db5815402a0a65f47d5f64b0937`  
		Last Modified: Wed, 06 Sep 2023 18:40:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083d5d74986bc09d57d6a94953a8cb9ab9fbfa44318c32ae6ef17887246f4e9a`  
		Last Modified: Wed, 06 Sep 2023 18:58:57 GMT  
		Size: 4.5 MB (4501414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85d58c05537603de5ce91a6463ef5a223b7ae94f24e05f506b943a930c13a6d`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 1.2 MB (1246086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db284285eec9597c8be93b8c4bd04c0c3b98bf4b089bd52ac26deca4af958251`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:54be0967bfdce111e3176e2c420aab107673db7adc6518b9063186a5bbf6041d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73978310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09ffe7cfa702a73c974a46cf5861ef5c87d89301c99cdda3a283fa9f2ed80442`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:10:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:10:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:18 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:31:28 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:31:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:31:28 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:53:26 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:53:26 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:53:27 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:53:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:53:27 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:53:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:53:28 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:53:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d54e960e981301b0098c80d2e61d694333b5ab480a007a3a8d0fa629662d377`  
		Last Modified: Tue, 08 Aug 2023 23:14:21 GMT  
		Size: 286.3 KB (286298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f000f33a92ab709a2599fbb82fa02eca8bca5b4fda93be45a8d0f1daabb73205`  
		Last Modified: Wed, 06 Sep 2023 18:36:08 GMT  
		Size: 64.1 MB (64108346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447d217685f511c828462bf16ea4579fdb55b103cb1a78d6ba5f0ab6a11db3f8`  
		Last Modified: Wed, 06 Sep 2023 18:35:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13822537d61bbdeb74e6e4458b659dbe1f0d9e3d45af3f50566be42e4b7c809`  
		Last Modified: Wed, 06 Sep 2023 18:53:44 GMT  
		Size: 5.1 MB (5053893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e7da4574a51623195c2699e1b61e06fcc41a5dbde49d5fc96691297a6cd780`  
		Last Modified: Wed, 06 Sep 2023 18:53:43 GMT  
		Size: 1.2 MB (1198447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2621576cb4d382e73ece4231dc51aef77167014d8f83460cbf64238db1fcc45c`  
		Last Modified: Wed, 06 Sep 2023 18:53:43 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:327d6fc238b35334c09db1685ededbacde6621b970825db074650fd341377f2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74185704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0eb6c48fb9239e3fb240aa27acdc3ee85d23fe96322a0606b54ce159b6c2b49`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:25:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 00:25:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:13 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:32:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:32:46 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:32:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:32:50 GMT
WORKDIR /go
# Wed, 06 Sep 2023 19:02:19 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 19:02:21 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 19:02:24 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 19:02:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 19:02:29 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 19:02:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 19:02:35 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 19:02:37 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c966ad2cdd35689da92e7c8fd39bd37cd6080c484e6ccaf00672c154cd4f6c2a`  
		Last Modified: Tue, 08 Aug 2023 00:39:35 GMT  
		Size: 286.7 KB (286662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679e04809663a2145818569201c1dcf2d46798f2198322a8e7910805a9b7dffd`  
		Last Modified: Wed, 06 Sep 2023 18:43:51 GMT  
		Size: 64.1 MB (64116069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1f0b6eb00af4cec1a2c3a203cf9a97b7b5b1e669db11dbabc36635b0207c79`  
		Last Modified: Wed, 06 Sep 2023 18:40:01 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcccd971afab022c32a88b23bc041273f72068caf215514da40b393e06632d93`  
		Last Modified: Wed, 06 Sep 2023 19:02:58 GMT  
		Size: 5.2 MB (5249983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc46690ff4c485e0fea9ac4b7505da047150045d9fcda46c2732480dc1f702`  
		Last Modified: Wed, 06 Sep 2023 19:02:58 GMT  
		Size: 1.2 MB (1186177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b59573283fbd9dc92a2d9a89bd66c6ee4d768933cc1388180a9c1ec35fed90d`  
		Last Modified: Wed, 06 Sep 2023 19:02:57 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:962738aef2725a7bbec2affa560a8497519a54f466f2c84dbfce42be5ab69896
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76084584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2852f51f18c2cd12f1e50eebc15bffa67e107a714382697c8beabe14b1ba6d0f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:41 GMT
RUN apk add --no-cache ca-certificates
# Mon, 07 Aug 2023 20:19:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:19 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:32:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:32:47 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:32:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:32:48 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:57:37 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:57:37 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:57:37 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:57:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:57:37 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:57:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:57:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:57:39 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec90be18226e5c99d10161aed1a143f4134093c55b4d6979bbdbbe4b0683eb11`  
		Last Modified: Mon, 07 Aug 2023 20:30:59 GMT  
		Size: 285.1 KB (285089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53e61151a7324ffa6693144a2516060d0505b80fe8f27915b1e77165106c2a4`  
		Last Modified: Wed, 06 Sep 2023 18:40:12 GMT  
		Size: 66.2 MB (66222411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1f0b6eb00af4cec1a2c3a203cf9a97b7b5b1e669db11dbabc36635b0207c79`  
		Last Modified: Wed, 06 Sep 2023 18:40:01 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178fae6c6c7b745dbb7be349b0656255d25dc06d0c808f85cce56fdf95543af6`  
		Last Modified: Wed, 06 Sep 2023 18:58:02 GMT  
		Size: 5.1 MB (5099943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bda7158ac61debfc44dddd51b20bf5e411c5f34ec92ad21dfffe9a0eeb5ae76`  
		Last Modified: Wed, 06 Sep 2023 18:58:02 GMT  
		Size: 1.3 MB (1262386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13aa15f1f389977eef4ccb0c676963b08cbf0600c3979659a8852b95689e91e8`  
		Last Modified: Wed, 06 Sep 2023 18:58:02 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.4-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:795ac7c3a409b95ae5a486743690a31dea9328bc5af293a50f64b63112a9adf6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `caddy:2.7.4-builder-windowsservercore-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:dc29929d7895f513f69e34dede7fb945b1bf1540fb37abda23f6fa2edcaa5150
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2092646318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03e3e89d97096b15070b9c1274ebdfe7a5e0de7816cd24a72782cdcb25b33dc3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:39:54 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:39:56 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:41:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:41:12 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:42:07 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:42:08 GMT
ENV GOLANG_VERSION=1.21.0
# Thu, 10 Aug 2023 00:45:16 GMT
RUN $url = 'https://dl.google.com/go/go1.21.0.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '732121e64e0ecb07c77fdf6cc1bc5ce7b242c2d40d4ac29021ad4c64a08731f6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:45:17 GMT
WORKDIR C:\go
# Thu, 17 Aug 2023 22:18:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Aug 2023 22:18:30 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 17 Aug 2023 22:18:31 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:18:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 17 Aug 2023 22:19:38 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 17 Aug 2023 22:19:39 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594083c5c2094c95b4e52723d54c14e0d70881f4f176720c3170012275accc3b`  
		Last Modified: Thu, 10 Aug 2023 01:02:54 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e2c2a5b75ced3a3a50be088c4a6c2d7df926b1fe6515b2d0c021312e3642f4`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d28688050deeec928289543beadf5c75bb2a8246576cb7c066e23818016217`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e5fbc50e7e0fefb7c9e349038ecb00ed5c000bcab8c4d82b1e1000c4273c01`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0544e07bd9df923e11e09c7dc042da614f2f14589eb6fa79005ebbbf2731e97d`  
		Last Modified: Thu, 10 Aug 2023 01:02:57 GMT  
		Size: 25.6 MB (25560980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555a82506c4fcec2bd90ae77756e5b03788e30c89f1a3820aa0b6a7ae6ad58ae`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bcfb422b104764156fc5ba099b5e3ae9fa9f760fd2db1c21acd8969b3d73de`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 220.8 KB (220796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:decc470f4f54c3be087cde5dfcbd816bc68a441d25189983c12219fb4504e9e0`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4589eb0957da5bce467ff89344ebebb2f584a815991fd3004ae3f4890b74f51`  
		Last Modified: Thu, 10 Aug 2023 01:03:10 GMT  
		Size: 69.2 MB (69210847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a698ba14b77be2efdb0e931dc9abf7efc7c749ce53fa2d1c277cd009f295c0`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.5 KB (1517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265b35725533ea18f9e8b7d3422e1b960406141ca305f83de8f61dd49b340c74`  
		Last Modified: Thu, 17 Aug 2023 22:22:07 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3cd40483d2a2e0aae25c4caf3e900aca669895009d08c100e8754768099257`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1aaed9881a7c5017bdf3b46a5ba81399cd7bdaf9be397334872bbf8826386b`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00f7ca68792eb07043e7b43dec1b74b4e211701549286cdcc7993a3b76fdbce`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2516df9efacfe0206db24dbf7d952da6820b3ba9189c715b7aeb069bf903b0b`  
		Last Modified: Thu, 17 Aug 2023 22:22:05 GMT  
		Size: 1.7 MB (1680500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ed01fbe50be0cb731bfdaf18ffaad3e427b9cd10eaabf4930a0dda4b98450`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.4-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:f8893322f81862d0d41473494adb769699011eab49c16e9c66a37e7c5d1a61e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1906; amd64

### `caddy:2.7.4-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:16053b4036029cc1457cb147a03be7a416b3fd01393e467beeb72def1f482edf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1894119169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e467c74cf811ff36bfae3619793832f5179eba1986cd92d51528fa3631e15b67`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:36:23 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:36:24 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:36:25 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:36:26 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:36:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:37:00 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:37:19 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:37:20 GMT
ENV GOLANG_VERSION=1.21.0
# Thu, 10 Aug 2023 00:39:40 GMT
RUN $url = 'https://dl.google.com/go/go1.21.0.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '732121e64e0ecb07c77fdf6cc1bc5ce7b242c2d40d4ac29021ad4c64a08731f6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:39:42 GMT
WORKDIR C:\go
# Thu, 17 Aug 2023 22:19:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Aug 2023 22:19:58 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 17 Aug 2023 22:19:58 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:19:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 17 Aug 2023 22:20:24 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 17 Aug 2023 22:20:25 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877256a6389e5e2563da79ad5bd201e7ee136abf14ff7cb0d4efbf3b24e5f127`  
		Last Modified: Thu, 10 Aug 2023 01:02:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a39df29b3c0b2f7e691c47273110db4a46e5c8e299f6bb95f77a9c61f79872`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8574d63bce1547e3177d0b76237a782a9b016d4880375dcd1a7b6a1c5dee3dc`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ef34b3c96316bcdd92e24c8c4eebdc3a35f245c013ef87edfae0dde091a305`  
		Last Modified: Thu, 10 Aug 2023 01:02:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a481babc5b629f694446a96dba8d77c020257c98334c605aff94162b9a917279`  
		Last Modified: Thu, 10 Aug 2023 01:02:23 GMT  
		Size: 25.6 MB (25554169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281178ea1c103ff07ea7e4fb647eb0dbe4f865742da6ef9944e04f37974fc27c`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b5d34adf2aacfe87580143f3e17c635dc8dbd4068377b79b35d665f49bbad9`  
		Last Modified: Thu, 10 Aug 2023 01:02:16 GMT  
		Size: 275.9 KB (275946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5b48235253668711a8e6a2ff934add92fea681c9256325d0ad13a01141c047`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4fb7d9dc956e10b22252d8212c98e2dee64526f471fa548eb6c842d5f05ae9`  
		Last Modified: Thu, 10 Aug 2023 01:02:35 GMT  
		Size: 69.2 MB (69216081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b888078988d2c04f6dae8641365e345f00127285805315ff6f554d6b93ac473c`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.5 KB (1451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b841ebd982703c219e6682e9f6ce05952af17249b1feeac24f29b4758db36694`  
		Last Modified: Thu, 17 Aug 2023 22:22:23 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fde1a85f81e8aec976e03a445fd68b44a23b9f74e66320c7dfce58a75409c25`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0498fcf11a96e26aace74390231497cf74c1d199da68217be38339f5e4108a3`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e49f04c5395ab27a41689cde8841498c15d6b18d029bb336e25274009098cc6`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c1983f7985d2513515cbe76bf211a71393e1a54cfd8e6b755d82fef2120d4a`  
		Last Modified: Thu, 17 Aug 2023 22:22:22 GMT  
		Size: 1.7 MB (1690677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d561bf1c2c8101b9e952ebca483dfa257b2d839feabe3857a1a2694e7d5d83f9`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.4-windowsservercore`

```console
$ docker pull caddy@sha256:9b2d0e89dc4f5f508ec90143d8b6b6d2cdbe9067fea9d0930cbb9812eb816b01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4737; amd64
	-	windows version 10.0.20348.1906; amd64

### `caddy:2.7.4-windowsservercore` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:8d641d87b059de975dc94ff579d47434e347b333b33a4a8f15cd679c062a14c0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2011934670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e21b2ad9f1a3657d84dd869da76d22704a2848d4a92f831acbfef09e26e80cc6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 14 Aug 2023 18:16:58 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 17 Aug 2023 22:14:59 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:16:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 17 Aug 2023 22:16:13 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 17 Aug 2023 22:16:14 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 17 Aug 2023 22:16:15 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:16:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:16:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:16:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:16:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:16:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:16:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:16:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:16:21 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:16:22 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:16:23 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:16:24 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:17:19 GMT
RUN caddy version
# Thu, 17 Aug 2023 22:17:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d698e8ba8bfd4c31116f0d2c87cfcf2ff17baa1a5c678b116b3aa1ac8ed73d`  
		Last Modified: Mon, 14 Aug 2023 18:23:17 GMT  
		Size: 483.6 KB (483626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dcf545f7c90cab6f6962d3099898462129da2e6b06a80802d52ff1e9d2fca08`  
		Last Modified: Thu, 17 Aug 2023 22:21:12 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65ecc8b4521923b522dd6392a862d0dff9edd10c1e3b520de8f130de2170880`  
		Last Modified: Thu, 17 Aug 2023 22:21:16 GMT  
		Size: 15.2 MB (15201779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ddd9c690b84a4a4744ec5ac91059e12e1aa92378220080fcfbf616c59b4c26`  
		Last Modified: Thu, 17 Aug 2023 22:21:12 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63adbcb9cba5e8d67eac5e059c7bbb9dfe3040f0933afb5e1f8cb7d4c211b4a`  
		Last Modified: Thu, 17 Aug 2023 22:21:11 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e15ff22938f514e6118606619ff28e9e5ee145d6f3dc6de1de62ea4051575c1`  
		Last Modified: Thu, 17 Aug 2023 22:21:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438a6cab105b637f625a3fd00d7ecaa6792ad5dc120bf1be36e7d6e19ee44b4d`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfd206f96497c8e0730c72c36ecedea57379a6a219903785dc1478b50b3945`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e651df7142dc872814a59faff8cf791ab4e4413ee6a9b043fe02a2af9da24fe`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b7f62d857ed7e15d08d52d1ef08f3c21e25751d17e8a5418c02f6adc366eab`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6347f1227dc933d98b8f02d22cd440529284e7c8e415e96cee265ae2c7445b3`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2776f9f89b2242d27c9c49da3465d2ff6acb224dd3315837bda709f3fa0aa4ff`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aaab02f29add47735607e798c40625216306d00d57988d1ece40f43b93f706c`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ed26555e0c9e51aa5dbf4125ef3ea56c6d84274b4d8160ce10c3c0d9e7106d`  
		Last Modified: Thu, 17 Aug 2023 22:21:08 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392c0484ea6d941786f507e72c143bd1c64d4c42bcd773bd745330a55b89d356`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef07137395441a56a870d882d84faac751156b0486c6528fa18b6d706ff250d8`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2950cf3d51ba47c2b41415fccf9b67e813735f67ccc34a0ce5f1a1a4a34e56dc`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25de03b5a8b8f2752cde31b881d457ec5900438b781cc65cda3aca9444b2377f`  
		Last Modified: Thu, 17 Aug 2023 22:21:07 GMT  
		Size: 269.9 KB (269882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f3d70fb1dd11e79f9128736ada85993e1b4fd603b2f8164aac49ac1efda548`  
		Last Modified: Thu, 17 Aug 2023 22:21:07 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-windowsservercore` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:f4791cb0179b98b28e760842405262d782735176b147c84f26709bd1361c8798
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1813299019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b759bf39605cbc0d0ceaaa8eda1623452b1acd67deb11c0d22defff59f2058`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 14 Aug 2023 18:19:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 17 Aug 2023 22:17:27 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:17:55 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 17 Aug 2023 22:17:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 17 Aug 2023 22:17:56 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 17 Aug 2023 22:17:57 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:17:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:17:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:17:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:18:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:18:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:18:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:18:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:18:04 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:18:04 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:18:05 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:18:06 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:18:21 GMT
RUN caddy version
# Thu, 17 Aug 2023 22:18:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c23e01ee014d9e05e276268c94980b00a0720fcb5488a368b20ee74701ed78`  
		Last Modified: Mon, 14 Aug 2023 18:23:42 GMT  
		Size: 461.2 KB (461170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8a7576f0b2ff121a0e9658821e52a7b356abbd90c9215b750ab7fc2127f6ae`  
		Last Modified: Thu, 17 Aug 2023 22:21:41 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ecc6db59a89a0a9f61364702d6af7202fa4f3f742ec6dff93c3a5b53e3826`  
		Last Modified: Thu, 17 Aug 2023 22:21:44 GMT  
		Size: 15.2 MB (15169088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9323e4528d7a59819754484fdbeb047240a6f1f0dd262b734a226a4249dc0a0`  
		Last Modified: Thu, 17 Aug 2023 22:21:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb3a3b69dd93b979cdcd1e0759ee1199bc8d5a510a6ce9bca3856201d747468`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56ce33676578802911228ae7aba31fe1898897ede8c69e12a0959a37a11d130`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c896eeb3f2c45b2bba4fe5e5da02be1289c4cabcf574a38c19d1616ebf552d4c`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6563dd3d5f912ae2b7bd629d2dc731df89b1dd107e2cbb85dee24a0d5c550a1`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420011263062842c72720998f13fa245d9bef077622fde4e17cc60cef3e00bce`  
		Last Modified: Thu, 17 Aug 2023 22:21:38 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2385fc0cb7a281a35df415654aba711bf70fa23b963faf0a3f0055d760f5c41c`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a58351f25f399f8a9399e60dd315cd8c695972a9e51f2271e3377151cf621d`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506eb3a97b70fc7dc1c1c3464a89512890cd48c354658e58e61d5acfee63f1c3`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86cf8c25cfcaf858db6ffd2630a26ca3a13ad2fdc941a01438ea9ea80ccb20c`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcedddef9863d16c4d713280050f604b44968bc253844c27e46cb8871eb17a99`  
		Last Modified: Thu, 17 Aug 2023 22:21:36 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d01313141e38a9b2b15a3e831a2d11a3eb47611bf99b0677be3c49693984f64`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504a80bc0f7aa0c98a143033f551be8fcf0653046e7313c0de080b82ad97ad52`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280053e45030e2421ea4d1cdfd721c24f40d30518b1ce8af7e0811363daf6eca`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0d07466cd8f053bf957a35cbe340d419f5c2f6ff48565bb8a5b255998e3e94`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 280.9 KB (280938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad52776067d7be890960cfd7082041a93a802b96fea6d31fc724192c49eb00`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.4-windowsservercore-1809`

```console
$ docker pull caddy@sha256:44adcd32029ece40e50aef18ba70e3020cbba5b53153929078326ec23613226c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `caddy:2.7.4-windowsservercore-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:8d641d87b059de975dc94ff579d47434e347b333b33a4a8f15cd679c062a14c0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2011934670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e21b2ad9f1a3657d84dd869da76d22704a2848d4a92f831acbfef09e26e80cc6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 14 Aug 2023 18:16:58 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 17 Aug 2023 22:14:59 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:16:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 17 Aug 2023 22:16:13 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 17 Aug 2023 22:16:14 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 17 Aug 2023 22:16:15 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:16:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:16:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:16:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:16:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:16:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:16:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:16:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:16:21 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:16:22 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:16:23 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:16:24 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:17:19 GMT
RUN caddy version
# Thu, 17 Aug 2023 22:17:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d698e8ba8bfd4c31116f0d2c87cfcf2ff17baa1a5c678b116b3aa1ac8ed73d`  
		Last Modified: Mon, 14 Aug 2023 18:23:17 GMT  
		Size: 483.6 KB (483626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dcf545f7c90cab6f6962d3099898462129da2e6b06a80802d52ff1e9d2fca08`  
		Last Modified: Thu, 17 Aug 2023 22:21:12 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65ecc8b4521923b522dd6392a862d0dff9edd10c1e3b520de8f130de2170880`  
		Last Modified: Thu, 17 Aug 2023 22:21:16 GMT  
		Size: 15.2 MB (15201779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ddd9c690b84a4a4744ec5ac91059e12e1aa92378220080fcfbf616c59b4c26`  
		Last Modified: Thu, 17 Aug 2023 22:21:12 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63adbcb9cba5e8d67eac5e059c7bbb9dfe3040f0933afb5e1f8cb7d4c211b4a`  
		Last Modified: Thu, 17 Aug 2023 22:21:11 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e15ff22938f514e6118606619ff28e9e5ee145d6f3dc6de1de62ea4051575c1`  
		Last Modified: Thu, 17 Aug 2023 22:21:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438a6cab105b637f625a3fd00d7ecaa6792ad5dc120bf1be36e7d6e19ee44b4d`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfd206f96497c8e0730c72c36ecedea57379a6a219903785dc1478b50b3945`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e651df7142dc872814a59faff8cf791ab4e4413ee6a9b043fe02a2af9da24fe`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b7f62d857ed7e15d08d52d1ef08f3c21e25751d17e8a5418c02f6adc366eab`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6347f1227dc933d98b8f02d22cd440529284e7c8e415e96cee265ae2c7445b3`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2776f9f89b2242d27c9c49da3465d2ff6acb224dd3315837bda709f3fa0aa4ff`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aaab02f29add47735607e798c40625216306d00d57988d1ece40f43b93f706c`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ed26555e0c9e51aa5dbf4125ef3ea56c6d84274b4d8160ce10c3c0d9e7106d`  
		Last Modified: Thu, 17 Aug 2023 22:21:08 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392c0484ea6d941786f507e72c143bd1c64d4c42bcd773bd745330a55b89d356`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef07137395441a56a870d882d84faac751156b0486c6528fa18b6d706ff250d8`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2950cf3d51ba47c2b41415fccf9b67e813735f67ccc34a0ce5f1a1a4a34e56dc`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25de03b5a8b8f2752cde31b881d457ec5900438b781cc65cda3aca9444b2377f`  
		Last Modified: Thu, 17 Aug 2023 22:21:07 GMT  
		Size: 269.9 KB (269882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f3d70fb1dd11e79f9128736ada85993e1b4fd603b2f8164aac49ac1efda548`  
		Last Modified: Thu, 17 Aug 2023 22:21:07 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.4-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:25814323b2b1cf78a7dfadd252104b12d24aa4dc9512441a2717cd13b1d3da8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1906; amd64

### `caddy:2.7.4-windowsservercore-ltsc2022` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:f4791cb0179b98b28e760842405262d782735176b147c84f26709bd1361c8798
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1813299019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b759bf39605cbc0d0ceaaa8eda1623452b1acd67deb11c0d22defff59f2058`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 14 Aug 2023 18:19:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 17 Aug 2023 22:17:27 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:17:55 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 17 Aug 2023 22:17:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 17 Aug 2023 22:17:56 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 17 Aug 2023 22:17:57 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:17:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:17:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:17:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:18:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:18:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:18:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:18:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:18:04 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:18:04 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:18:05 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:18:06 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:18:21 GMT
RUN caddy version
# Thu, 17 Aug 2023 22:18:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c23e01ee014d9e05e276268c94980b00a0720fcb5488a368b20ee74701ed78`  
		Last Modified: Mon, 14 Aug 2023 18:23:42 GMT  
		Size: 461.2 KB (461170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8a7576f0b2ff121a0e9658821e52a7b356abbd90c9215b750ab7fc2127f6ae`  
		Last Modified: Thu, 17 Aug 2023 22:21:41 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ecc6db59a89a0a9f61364702d6af7202fa4f3f742ec6dff93c3a5b53e3826`  
		Last Modified: Thu, 17 Aug 2023 22:21:44 GMT  
		Size: 15.2 MB (15169088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9323e4528d7a59819754484fdbeb047240a6f1f0dd262b734a226a4249dc0a0`  
		Last Modified: Thu, 17 Aug 2023 22:21:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb3a3b69dd93b979cdcd1e0759ee1199bc8d5a510a6ce9bca3856201d747468`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56ce33676578802911228ae7aba31fe1898897ede8c69e12a0959a37a11d130`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c896eeb3f2c45b2bba4fe5e5da02be1289c4cabcf574a38c19d1616ebf552d4c`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6563dd3d5f912ae2b7bd629d2dc731df89b1dd107e2cbb85dee24a0d5c550a1`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420011263062842c72720998f13fa245d9bef077622fde4e17cc60cef3e00bce`  
		Last Modified: Thu, 17 Aug 2023 22:21:38 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2385fc0cb7a281a35df415654aba711bf70fa23b963faf0a3f0055d760f5c41c`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a58351f25f399f8a9399e60dd315cd8c695972a9e51f2271e3377151cf621d`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506eb3a97b70fc7dc1c1c3464a89512890cd48c354658e58e61d5acfee63f1c3`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86cf8c25cfcaf858db6ffd2630a26ca3a13ad2fdc941a01438ea9ea80ccb20c`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcedddef9863d16c4d713280050f604b44968bc253844c27e46cb8871eb17a99`  
		Last Modified: Thu, 17 Aug 2023 22:21:36 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d01313141e38a9b2b15a3e831a2d11a3eb47611bf99b0677be3c49693984f64`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504a80bc0f7aa0c98a143033f551be8fcf0653046e7313c0de080b82ad97ad52`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280053e45030e2421ea4d1cdfd721c24f40d30518b1ce8af7e0811363daf6eca`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0d07466cd8f053bf957a35cbe340d419f5c2f6ff48565bb8a5b255998e3e94`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 280.9 KB (280938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad52776067d7be890960cfd7082041a93a802b96fea6d31fc724192c49eb00`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:7e01c08308bc94c1ef3e495f0b2ba469d1f7e8d1a4f2caa2fbe189edf48866a6
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
$ docker pull caddy@sha256:733fe94133c4bd22c6ee8f9b9802bce8fede5e7b766bebde205a45dd4ac04aea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18363908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1e1b7ae170b7d7d7e524717fe978e0090023cc82a7d9ffe48e344b0351a3ee1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:09:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 18:20:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:19:38 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:19:41 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:19:41 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:19:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:19:42 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:19:42 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:19:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0aa7b81ef11c65f43b0b58323a33dd9e07eb785529f0d75b452f87a309db00c`  
		Last Modified: Mon, 07 Aug 2023 20:09:40 GMT  
		Size: 350.8 KB (350844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b3b3e68e52dc5ab939c72a9bbac39cff4bef4b87de399ddf28657471df6845`  
		Last Modified: Mon, 14 Aug 2023 18:20:42 GMT  
		Size: 7.5 KB (7502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c55d3259542348ddb70edc18dda7d48aeca5654962aed568a7034f3667d2ca`  
		Last Modified: Thu, 17 Aug 2023 22:20:10 GMT  
		Size: 14.6 MB (14603949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:dd029220558032e5d1f91173d32a0078dad12ec9b5114bef422ed4cdf05dec52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17314204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1de0523ee8d8173472fb08aa9a74a37bcd054af2b796b7631d847ba8a46986b5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:38:27 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:49:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:49:12 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:49:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:49:16 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:49:16 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:49:17 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:49:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172ef460a93549b8a3e73f6a515bccad93512788d1e8f095e7230ba41967c25a`  
		Last Modified: Wed, 09 Aug 2023 03:38:53 GMT  
		Size: 347.7 KB (347686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7aae78767a581df85fd1a51ccd646619aec320896ca016ef0f05a41b16bcbfe`  
		Last Modified: Mon, 14 Aug 2023 17:49:36 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82560a340155261ecbd1d99d87890c5aa0cfd64d571e1dcafc03e3b6a8132d48`  
		Last Modified: Thu, 17 Aug 2023 22:49:41 GMT  
		Size: 13.8 MB (13814204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:24649e9de43354963118f9cdf6ad1f4522c6993735f316763a2f5d1f76cba267
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17042831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb4a48fd29d50802cbf030949e2c9767eb6888e8412330f64246f322bc3b49c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:51:41 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:57:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:57:18 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:57:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:57:22 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:57:22 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:57:24 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:57:24 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:57:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a47b73e04459258b08555443754e92e2db20bde113c58ca18e1a6f07878f72`  
		Last Modified: Tue, 08 Aug 2023 01:52:05 GMT  
		Size: 344.5 KB (344462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e1b3e18d5e992f1805072b2d52405d575830bdce21726ef99dea99e31d8277`  
		Last Modified: Mon, 14 Aug 2023 17:57:42 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5879767a5d1969beb154b9a4991a767b0ed5be0c9739a972f07d03e825312fa5`  
		Last Modified: Thu, 17 Aug 2023 22:57:51 GMT  
		Size: 13.8 MB (13791384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:ed967fcd1968be6dc4699ff835cdd2d6f3f49105b9677f878c8a6960fd1a0643
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17162547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed7b6600470cab547aa1090baa39a6192ec83119989884ac742a63ed23be3da2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:09:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:39:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:39:17 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:39:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:39:19 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:39:19 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:39:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:39:20 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:39:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a699f78cfb85f60e17fc7c13495876ea0cb4495bbe39e8c65f3e8559b0d7169`  
		Last Modified: Mon, 07 Aug 2023 21:09:34 GMT  
		Size: 360.6 KB (360642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7488af8b96c79b6db13955a0302653c4e9f314d0833201984ae06c1ed697f06`  
		Last Modified: Mon, 14 Aug 2023 17:39:41 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597bfc484ba18727d2df98120cb9d559f346ade9e3a23be6a9af3e76dca89edd`  
		Last Modified: Thu, 17 Aug 2023 22:39:42 GMT  
		Size: 13.5 MB (13463635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:c3679836562d0252e6341a112d2729b8dae0eae550449bfe91fe2798171fd4ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16944934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc5ac831dce746cd0f4448640b7edaf0ce9457d09618e246ba72ee76ea63dcbe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:44:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 18:18:00 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:16:24 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:16:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:16:29 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:16:29 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:16:29 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:16:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:16:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:16:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:16:32 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:16:33 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:16:33 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:16:34 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:16:34 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:16:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f40714f45e39ac41e865ccbf2877db62255ce5a5c36a47eadf00b9d174f042`  
		Last Modified: Tue, 08 Aug 2023 00:45:18 GMT  
		Size: 362.2 KB (362173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d19953b5eb53ddaa0e25905527dc138e0c4111467bb7d71f81fa94976091351`  
		Last Modified: Mon, 14 Aug 2023 18:18:54 GMT  
		Size: 7.5 KB (7509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf4bf695323732c5ce84bbb0b976c5cd981eaf6814515a86f521af4a0e64582`  
		Last Modified: Thu, 17 Aug 2023 22:17:22 GMT  
		Size: 13.2 MB (13229001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:ca7ab0dcf4ab146df48cfa8ae6e07fed804feeed4a36358fa652c8eac52b40da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17720356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d4d019ffc0cd69ea8c5d3b8fb0a39c89d3aa1b2037c1012a9ba4bed6abb94dc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:14:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:41:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:41:35 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:41:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:41:39 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:41:39 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:41:39 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:41:40 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:41:41 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:41:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df19abd0ca1d4a821a4174a2c0831a57d6fd584073f056abcae085a51f0b3848`  
		Last Modified: Mon, 07 Aug 2023 20:14:50 GMT  
		Size: 354.9 KB (354950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308478977890baa82477ee70a3065fb9da2080efcc95facf1a87ac021b06a8e9`  
		Last Modified: Mon, 14 Aug 2023 17:42:17 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2394cd7c9416df19c45596c558f5a7ee05adc5a7fd166f58dcbf26f1ac6ecae6`  
		Last Modified: Thu, 17 Aug 2023 22:42:16 GMT  
		Size: 14.1 MB (14143708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:eafc66404950e4170122aba0977f7079d888e544bed6df61a144b50bcf06bbb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4737; amd64
	-	windows version 10.0.20348.1906; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:716dc5ded2a0c7090ac3cf0d298122538ac67a0152c97b88a17520c2b0419d82
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76949834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0789fd27a45de2db1b44ab683c8b91c2f63b230c312d20bb2b45294d44c8d02b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:36:47 GMT
RUN apk add --no-cache ca-certificates
# Wed, 09 Aug 2023 04:41:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:29 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:31:40 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:31:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:31:41 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:58:36 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:58:37 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:58:37 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:58:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:58:37 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:58:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:58:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:58:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d48a809fc2256f8aa0aeee47998488d64409855adba00a7cb3007ab9f3286e`  
		Last Modified: Wed, 09 Aug 2023 03:37:02 GMT  
		Size: 284.7 KB (284693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60be0ca469417450769350b29d9d86e57dc60849c11fab3e8d0b556fcc35005`  
		Last Modified: Wed, 06 Sep 2023 18:37:24 GMT  
		Size: 67.0 MB (67002091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb14ea137979420ee28a5d750e5d62200f15a09c2461e13a8f10023e5fbf5a2`  
		Last Modified: Wed, 06 Sep 2023 18:37:12 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d4cebe2e13d01b24cfdc9eaeae90b4a21f72815fffd9a6a0bb96d99bd0552a`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 5.0 MB (4958640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb64c4e131a2a58133f92ec61aefa25cfb66ef81c5dc749f4de450feb5349c8`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 1.3 MB (1302236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce602f0d9b5db7d56aabf2bf531824f371f52db43d9dc61da5ac5856f69c7359`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:0a1d4936666edfd074f88e0eeeefc1402111cc54a0fcc57963ae88dde642fdca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75388438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c765f590b091ce124e5856c924f7305627163a3a17955d23a482fb20592c338`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:12:05 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:12:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:30:47 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:31:16 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:31:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:31:17 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:54:56 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:54:56 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:54:56 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:54:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:54:56 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:54:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:54:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:54:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8564ce36feee688566265012773f1c8c7c046ceefe86ca763eb702682f4e6e75`  
		Last Modified: Tue, 08 Aug 2023 23:15:06 GMT  
		Size: 284.9 KB (284876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63353306cb1a8907bf53eeefec13043d0f70b554332a60aa92bb4c3861b93c8`  
		Last Modified: Wed, 06 Sep 2023 18:37:56 GMT  
		Size: 65.8 MB (65758368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a286c00e60caea02b9c22fac7d8a91c9ffa40d7fc56aea06e0f8f67c5d3001b8`  
		Last Modified: Wed, 06 Sep 2023 18:37:33 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6650d2d716414907ceaad018d0c2a57750f812da3ce864c723329a9691bfab`  
		Last Modified: Wed, 06 Sep 2023 18:55:14 GMT  
		Size: 5.0 MB (4951168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ebf8a554fac09b4da4a7072225799fa9bc12129c257b93d7dfabc9b7370c0a`  
		Last Modified: Wed, 06 Sep 2023 18:55:14 GMT  
		Size: 1.2 MB (1248657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9711d57485a382ed790b0a10b1af2b8a817f3973693a9add4edf8752b7aae66c`  
		Last Modified: Wed, 06 Sep 2023 18:55:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fe3ec3b57937f6ee95b60afb48874baeee931a06cbb59c944943b498a9016d1c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74690125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590b4483c17141a335fd0eb382750e044c6c5b452db059d3eb1d1aef7950dd3e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:39:47 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 01:39:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:45 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:32:02 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:32:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:32:04 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:58:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:58:39 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:58:39 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:58:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:58:39 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:58:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:58:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:58:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47bd95d78f565e902bafd0264a979eb4f6f71e22c0464011bf9db6feb0579e6`  
		Last Modified: Tue, 08 Aug 2023 01:48:34 GMT  
		Size: 284.1 KB (284073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812db0f4af4ab09f020f5a4b3fb1803a8afdf60db3d0e0c2d451a717141054ca`  
		Last Modified: Wed, 06 Sep 2023 18:40:37 GMT  
		Size: 65.8 MB (65758511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f0657fffaca6c4a15be6c893e54fcf97d14db5815402a0a65f47d5f64b0937`  
		Last Modified: Wed, 06 Sep 2023 18:40:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083d5d74986bc09d57d6a94953a8cb9ab9fbfa44318c32ae6ef17887246f4e9a`  
		Last Modified: Wed, 06 Sep 2023 18:58:57 GMT  
		Size: 4.5 MB (4501414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85d58c05537603de5ce91a6463ef5a223b7ae94f24e05f506b943a930c13a6d`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 1.2 MB (1246086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db284285eec9597c8be93b8c4bd04c0c3b98bf4b089bd52ac26deca4af958251`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:54be0967bfdce111e3176e2c420aab107673db7adc6518b9063186a5bbf6041d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73978310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09ffe7cfa702a73c974a46cf5861ef5c87d89301c99cdda3a283fa9f2ed80442`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:10:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:10:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:18 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:31:28 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:31:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:31:28 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:53:26 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:53:26 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:53:27 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:53:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:53:27 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:53:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:53:28 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:53:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d54e960e981301b0098c80d2e61d694333b5ab480a007a3a8d0fa629662d377`  
		Last Modified: Tue, 08 Aug 2023 23:14:21 GMT  
		Size: 286.3 KB (286298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f000f33a92ab709a2599fbb82fa02eca8bca5b4fda93be45a8d0f1daabb73205`  
		Last Modified: Wed, 06 Sep 2023 18:36:08 GMT  
		Size: 64.1 MB (64108346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447d217685f511c828462bf16ea4579fdb55b103cb1a78d6ba5f0ab6a11db3f8`  
		Last Modified: Wed, 06 Sep 2023 18:35:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13822537d61bbdeb74e6e4458b659dbe1f0d9e3d45af3f50566be42e4b7c809`  
		Last Modified: Wed, 06 Sep 2023 18:53:44 GMT  
		Size: 5.1 MB (5053893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e7da4574a51623195c2699e1b61e06fcc41a5dbde49d5fc96691297a6cd780`  
		Last Modified: Wed, 06 Sep 2023 18:53:43 GMT  
		Size: 1.2 MB (1198447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2621576cb4d382e73ece4231dc51aef77167014d8f83460cbf64238db1fcc45c`  
		Last Modified: Wed, 06 Sep 2023 18:53:43 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:327d6fc238b35334c09db1685ededbacde6621b970825db074650fd341377f2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74185704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0eb6c48fb9239e3fb240aa27acdc3ee85d23fe96322a0606b54ce159b6c2b49`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:25:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 00:25:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:13 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:32:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:32:46 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:32:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:32:50 GMT
WORKDIR /go
# Wed, 06 Sep 2023 19:02:19 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 19:02:21 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 19:02:24 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 19:02:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 19:02:29 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 19:02:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 19:02:35 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 19:02:37 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c966ad2cdd35689da92e7c8fd39bd37cd6080c484e6ccaf00672c154cd4f6c2a`  
		Last Modified: Tue, 08 Aug 2023 00:39:35 GMT  
		Size: 286.7 KB (286662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679e04809663a2145818569201c1dcf2d46798f2198322a8e7910805a9b7dffd`  
		Last Modified: Wed, 06 Sep 2023 18:43:51 GMT  
		Size: 64.1 MB (64116069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1f0b6eb00af4cec1a2c3a203cf9a97b7b5b1e669db11dbabc36635b0207c79`  
		Last Modified: Wed, 06 Sep 2023 18:40:01 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcccd971afab022c32a88b23bc041273f72068caf215514da40b393e06632d93`  
		Last Modified: Wed, 06 Sep 2023 19:02:58 GMT  
		Size: 5.2 MB (5249983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc46690ff4c485e0fea9ac4b7505da047150045d9fcda46c2732480dc1f702`  
		Last Modified: Wed, 06 Sep 2023 19:02:58 GMT  
		Size: 1.2 MB (1186177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b59573283fbd9dc92a2d9a89bd66c6ee4d768933cc1388180a9c1ec35fed90d`  
		Last Modified: Wed, 06 Sep 2023 19:02:57 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:962738aef2725a7bbec2affa560a8497519a54f466f2c84dbfce42be5ab69896
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76084584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2852f51f18c2cd12f1e50eebc15bffa67e107a714382697c8beabe14b1ba6d0f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:41 GMT
RUN apk add --no-cache ca-certificates
# Mon, 07 Aug 2023 20:19:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:19 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:32:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:32:47 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:32:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:32:48 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:57:37 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:57:37 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:57:37 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:57:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:57:37 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:57:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:57:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:57:39 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec90be18226e5c99d10161aed1a143f4134093c55b4d6979bbdbbe4b0683eb11`  
		Last Modified: Mon, 07 Aug 2023 20:30:59 GMT  
		Size: 285.1 KB (285089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53e61151a7324ffa6693144a2516060d0505b80fe8f27915b1e77165106c2a4`  
		Last Modified: Wed, 06 Sep 2023 18:40:12 GMT  
		Size: 66.2 MB (66222411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1f0b6eb00af4cec1a2c3a203cf9a97b7b5b1e669db11dbabc36635b0207c79`  
		Last Modified: Wed, 06 Sep 2023 18:40:01 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178fae6c6c7b745dbb7be349b0656255d25dc06d0c808f85cce56fdf95543af6`  
		Last Modified: Wed, 06 Sep 2023 18:58:02 GMT  
		Size: 5.1 MB (5099943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bda7158ac61debfc44dddd51b20bf5e411c5f34ec92ad21dfffe9a0eeb5ae76`  
		Last Modified: Wed, 06 Sep 2023 18:58:02 GMT  
		Size: 1.3 MB (1262386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13aa15f1f389977eef4ccb0c676963b08cbf0600c3979659a8852b95689e91e8`  
		Last Modified: Wed, 06 Sep 2023 18:58:02 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:dc29929d7895f513f69e34dede7fb945b1bf1540fb37abda23f6fa2edcaa5150
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2092646318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03e3e89d97096b15070b9c1274ebdfe7a5e0de7816cd24a72782cdcb25b33dc3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:39:54 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:39:56 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:41:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:41:12 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:42:07 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:42:08 GMT
ENV GOLANG_VERSION=1.21.0
# Thu, 10 Aug 2023 00:45:16 GMT
RUN $url = 'https://dl.google.com/go/go1.21.0.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '732121e64e0ecb07c77fdf6cc1bc5ce7b242c2d40d4ac29021ad4c64a08731f6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:45:17 GMT
WORKDIR C:\go
# Thu, 17 Aug 2023 22:18:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Aug 2023 22:18:30 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 17 Aug 2023 22:18:31 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:18:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 17 Aug 2023 22:19:38 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 17 Aug 2023 22:19:39 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594083c5c2094c95b4e52723d54c14e0d70881f4f176720c3170012275accc3b`  
		Last Modified: Thu, 10 Aug 2023 01:02:54 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e2c2a5b75ced3a3a50be088c4a6c2d7df926b1fe6515b2d0c021312e3642f4`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d28688050deeec928289543beadf5c75bb2a8246576cb7c066e23818016217`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e5fbc50e7e0fefb7c9e349038ecb00ed5c000bcab8c4d82b1e1000c4273c01`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0544e07bd9df923e11e09c7dc042da614f2f14589eb6fa79005ebbbf2731e97d`  
		Last Modified: Thu, 10 Aug 2023 01:02:57 GMT  
		Size: 25.6 MB (25560980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555a82506c4fcec2bd90ae77756e5b03788e30c89f1a3820aa0b6a7ae6ad58ae`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bcfb422b104764156fc5ba099b5e3ae9fa9f760fd2db1c21acd8969b3d73de`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 220.8 KB (220796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:decc470f4f54c3be087cde5dfcbd816bc68a441d25189983c12219fb4504e9e0`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4589eb0957da5bce467ff89344ebebb2f584a815991fd3004ae3f4890b74f51`  
		Last Modified: Thu, 10 Aug 2023 01:03:10 GMT  
		Size: 69.2 MB (69210847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a698ba14b77be2efdb0e931dc9abf7efc7c749ce53fa2d1c277cd009f295c0`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.5 KB (1517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265b35725533ea18f9e8b7d3422e1b960406141ca305f83de8f61dd49b340c74`  
		Last Modified: Thu, 17 Aug 2023 22:22:07 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3cd40483d2a2e0aae25c4caf3e900aca669895009d08c100e8754768099257`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1aaed9881a7c5017bdf3b46a5ba81399cd7bdaf9be397334872bbf8826386b`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00f7ca68792eb07043e7b43dec1b74b4e211701549286cdcc7993a3b76fdbce`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2516df9efacfe0206db24dbf7d952da6820b3ba9189c715b7aeb069bf903b0b`  
		Last Modified: Thu, 17 Aug 2023 22:22:05 GMT  
		Size: 1.7 MB (1680500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ed01fbe50be0cb731bfdaf18ffaad3e427b9cd10eaabf4930a0dda4b98450`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:16053b4036029cc1457cb147a03be7a416b3fd01393e467beeb72def1f482edf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1894119169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e467c74cf811ff36bfae3619793832f5179eba1986cd92d51528fa3631e15b67`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:36:23 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:36:24 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:36:25 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:36:26 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:36:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:37:00 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:37:19 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:37:20 GMT
ENV GOLANG_VERSION=1.21.0
# Thu, 10 Aug 2023 00:39:40 GMT
RUN $url = 'https://dl.google.com/go/go1.21.0.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '732121e64e0ecb07c77fdf6cc1bc5ce7b242c2d40d4ac29021ad4c64a08731f6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:39:42 GMT
WORKDIR C:\go
# Thu, 17 Aug 2023 22:19:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Aug 2023 22:19:58 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 17 Aug 2023 22:19:58 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:19:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 17 Aug 2023 22:20:24 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 17 Aug 2023 22:20:25 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877256a6389e5e2563da79ad5bd201e7ee136abf14ff7cb0d4efbf3b24e5f127`  
		Last Modified: Thu, 10 Aug 2023 01:02:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a39df29b3c0b2f7e691c47273110db4a46e5c8e299f6bb95f77a9c61f79872`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8574d63bce1547e3177d0b76237a782a9b016d4880375dcd1a7b6a1c5dee3dc`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ef34b3c96316bcdd92e24c8c4eebdc3a35f245c013ef87edfae0dde091a305`  
		Last Modified: Thu, 10 Aug 2023 01:02:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a481babc5b629f694446a96dba8d77c020257c98334c605aff94162b9a917279`  
		Last Modified: Thu, 10 Aug 2023 01:02:23 GMT  
		Size: 25.6 MB (25554169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281178ea1c103ff07ea7e4fb647eb0dbe4f865742da6ef9944e04f37974fc27c`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b5d34adf2aacfe87580143f3e17c635dc8dbd4068377b79b35d665f49bbad9`  
		Last Modified: Thu, 10 Aug 2023 01:02:16 GMT  
		Size: 275.9 KB (275946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5b48235253668711a8e6a2ff934add92fea681c9256325d0ad13a01141c047`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4fb7d9dc956e10b22252d8212c98e2dee64526f471fa548eb6c842d5f05ae9`  
		Last Modified: Thu, 10 Aug 2023 01:02:35 GMT  
		Size: 69.2 MB (69216081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b888078988d2c04f6dae8641365e345f00127285805315ff6f554d6b93ac473c`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.5 KB (1451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b841ebd982703c219e6682e9f6ce05952af17249b1feeac24f29b4758db36694`  
		Last Modified: Thu, 17 Aug 2023 22:22:23 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fde1a85f81e8aec976e03a445fd68b44a23b9f74e66320c7dfce58a75409c25`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0498fcf11a96e26aace74390231497cf74c1d199da68217be38339f5e4108a3`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e49f04c5395ab27a41689cde8841498c15d6b18d029bb336e25274009098cc6`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c1983f7985d2513515cbe76bf211a71393e1a54cfd8e6b755d82fef2120d4a`  
		Last Modified: Thu, 17 Aug 2023 22:22:22 GMT  
		Size: 1.7 MB (1690677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d561bf1c2c8101b9e952ebca483dfa257b2d839feabe3857a1a2694e7d5d83f9`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:49505e7a951d9bba52ba419765e3efdee346bce23e25fdb3260a33d0429c7ce9
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
$ docker pull caddy@sha256:716dc5ded2a0c7090ac3cf0d298122538ac67a0152c97b88a17520c2b0419d82
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76949834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0789fd27a45de2db1b44ab683c8b91c2f63b230c312d20bb2b45294d44c8d02b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:36:47 GMT
RUN apk add --no-cache ca-certificates
# Wed, 09 Aug 2023 04:41:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:29 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:31:40 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:31:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:31:41 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:58:36 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:58:37 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:58:37 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:58:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:58:37 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:58:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:58:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:58:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d48a809fc2256f8aa0aeee47998488d64409855adba00a7cb3007ab9f3286e`  
		Last Modified: Wed, 09 Aug 2023 03:37:02 GMT  
		Size: 284.7 KB (284693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60be0ca469417450769350b29d9d86e57dc60849c11fab3e8d0b556fcc35005`  
		Last Modified: Wed, 06 Sep 2023 18:37:24 GMT  
		Size: 67.0 MB (67002091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb14ea137979420ee28a5d750e5d62200f15a09c2461e13a8f10023e5fbf5a2`  
		Last Modified: Wed, 06 Sep 2023 18:37:12 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d4cebe2e13d01b24cfdc9eaeae90b4a21f72815fffd9a6a0bb96d99bd0552a`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 5.0 MB (4958640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb64c4e131a2a58133f92ec61aefa25cfb66ef81c5dc749f4de450feb5349c8`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 1.3 MB (1302236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce602f0d9b5db7d56aabf2bf531824f371f52db43d9dc61da5ac5856f69c7359`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:0a1d4936666edfd074f88e0eeeefc1402111cc54a0fcc57963ae88dde642fdca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75388438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c765f590b091ce124e5856c924f7305627163a3a17955d23a482fb20592c338`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:12:05 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:12:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:30:47 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:31:16 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:31:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:31:17 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:54:56 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:54:56 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:54:56 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:54:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:54:56 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:54:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:54:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:54:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8564ce36feee688566265012773f1c8c7c046ceefe86ca763eb702682f4e6e75`  
		Last Modified: Tue, 08 Aug 2023 23:15:06 GMT  
		Size: 284.9 KB (284876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63353306cb1a8907bf53eeefec13043d0f70b554332a60aa92bb4c3861b93c8`  
		Last Modified: Wed, 06 Sep 2023 18:37:56 GMT  
		Size: 65.8 MB (65758368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a286c00e60caea02b9c22fac7d8a91c9ffa40d7fc56aea06e0f8f67c5d3001b8`  
		Last Modified: Wed, 06 Sep 2023 18:37:33 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6650d2d716414907ceaad018d0c2a57750f812da3ce864c723329a9691bfab`  
		Last Modified: Wed, 06 Sep 2023 18:55:14 GMT  
		Size: 5.0 MB (4951168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ebf8a554fac09b4da4a7072225799fa9bc12129c257b93d7dfabc9b7370c0a`  
		Last Modified: Wed, 06 Sep 2023 18:55:14 GMT  
		Size: 1.2 MB (1248657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9711d57485a382ed790b0a10b1af2b8a817f3973693a9add4edf8752b7aae66c`  
		Last Modified: Wed, 06 Sep 2023 18:55:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fe3ec3b57937f6ee95b60afb48874baeee931a06cbb59c944943b498a9016d1c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74690125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590b4483c17141a335fd0eb382750e044c6c5b452db059d3eb1d1aef7950dd3e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:39:47 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 01:39:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:45 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:32:02 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:32:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:32:04 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:58:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:58:39 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:58:39 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:58:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:58:39 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:58:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:58:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:58:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47bd95d78f565e902bafd0264a979eb4f6f71e22c0464011bf9db6feb0579e6`  
		Last Modified: Tue, 08 Aug 2023 01:48:34 GMT  
		Size: 284.1 KB (284073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812db0f4af4ab09f020f5a4b3fb1803a8afdf60db3d0e0c2d451a717141054ca`  
		Last Modified: Wed, 06 Sep 2023 18:40:37 GMT  
		Size: 65.8 MB (65758511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f0657fffaca6c4a15be6c893e54fcf97d14db5815402a0a65f47d5f64b0937`  
		Last Modified: Wed, 06 Sep 2023 18:40:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083d5d74986bc09d57d6a94953a8cb9ab9fbfa44318c32ae6ef17887246f4e9a`  
		Last Modified: Wed, 06 Sep 2023 18:58:57 GMT  
		Size: 4.5 MB (4501414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85d58c05537603de5ce91a6463ef5a223b7ae94f24e05f506b943a930c13a6d`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 1.2 MB (1246086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db284285eec9597c8be93b8c4bd04c0c3b98bf4b089bd52ac26deca4af958251`  
		Last Modified: Wed, 06 Sep 2023 18:58:56 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:54be0967bfdce111e3176e2c420aab107673db7adc6518b9063186a5bbf6041d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73978310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09ffe7cfa702a73c974a46cf5861ef5c87d89301c99cdda3a283fa9f2ed80442`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:10:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:10:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:18 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:31:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:31:28 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:31:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:31:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:31:28 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:53:26 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:53:26 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:53:27 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:53:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:53:27 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:53:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:53:28 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:53:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d54e960e981301b0098c80d2e61d694333b5ab480a007a3a8d0fa629662d377`  
		Last Modified: Tue, 08 Aug 2023 23:14:21 GMT  
		Size: 286.3 KB (286298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f000f33a92ab709a2599fbb82fa02eca8bca5b4fda93be45a8d0f1daabb73205`  
		Last Modified: Wed, 06 Sep 2023 18:36:08 GMT  
		Size: 64.1 MB (64108346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447d217685f511c828462bf16ea4579fdb55b103cb1a78d6ba5f0ab6a11db3f8`  
		Last Modified: Wed, 06 Sep 2023 18:35:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13822537d61bbdeb74e6e4458b659dbe1f0d9e3d45af3f50566be42e4b7c809`  
		Last Modified: Wed, 06 Sep 2023 18:53:44 GMT  
		Size: 5.1 MB (5053893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e7da4574a51623195c2699e1b61e06fcc41a5dbde49d5fc96691297a6cd780`  
		Last Modified: Wed, 06 Sep 2023 18:53:43 GMT  
		Size: 1.2 MB (1198447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2621576cb4d382e73ece4231dc51aef77167014d8f83460cbf64238db1fcc45c`  
		Last Modified: Wed, 06 Sep 2023 18:53:43 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:327d6fc238b35334c09db1685ededbacde6621b970825db074650fd341377f2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74185704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0eb6c48fb9239e3fb240aa27acdc3ee85d23fe96322a0606b54ce159b6c2b49`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:25:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 00:25:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:13 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:32:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:32:46 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:32:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:32:50 GMT
WORKDIR /go
# Wed, 06 Sep 2023 19:02:19 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 19:02:21 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 19:02:24 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 19:02:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 19:02:29 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 19:02:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 19:02:35 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 19:02:37 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c966ad2cdd35689da92e7c8fd39bd37cd6080c484e6ccaf00672c154cd4f6c2a`  
		Last Modified: Tue, 08 Aug 2023 00:39:35 GMT  
		Size: 286.7 KB (286662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679e04809663a2145818569201c1dcf2d46798f2198322a8e7910805a9b7dffd`  
		Last Modified: Wed, 06 Sep 2023 18:43:51 GMT  
		Size: 64.1 MB (64116069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1f0b6eb00af4cec1a2c3a203cf9a97b7b5b1e669db11dbabc36635b0207c79`  
		Last Modified: Wed, 06 Sep 2023 18:40:01 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcccd971afab022c32a88b23bc041273f72068caf215514da40b393e06632d93`  
		Last Modified: Wed, 06 Sep 2023 19:02:58 GMT  
		Size: 5.2 MB (5249983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc46690ff4c485e0fea9ac4b7505da047150045d9fcda46c2732480dc1f702`  
		Last Modified: Wed, 06 Sep 2023 19:02:58 GMT  
		Size: 1.2 MB (1186177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b59573283fbd9dc92a2d9a89bd66c6ee4d768933cc1388180a9c1ec35fed90d`  
		Last Modified: Wed, 06 Sep 2023 19:02:57 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:962738aef2725a7bbec2affa560a8497519a54f466f2c84dbfce42be5ab69896
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76084584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2852f51f18c2cd12f1e50eebc15bffa67e107a714382697c8beabe14b1ba6d0f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:41 GMT
RUN apk add --no-cache ca-certificates
# Mon, 07 Aug 2023 20:19:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:19 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:32:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 06 Sep 2023 18:32:47 GMT
ENV GOPATH=/go
# Wed, 06 Sep 2023 18:32:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 06 Sep 2023 18:32:48 GMT
WORKDIR /go
# Wed, 06 Sep 2023 18:57:37 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 06 Sep 2023 18:57:37 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 06 Sep 2023 18:57:37 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 06 Sep 2023 18:57:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Sep 2023 18:57:37 GMT
ENV XCADDY_SETCAP=1
# Wed, 06 Sep 2023 18:57:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Sep 2023 18:57:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Sep 2023 18:57:39 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec90be18226e5c99d10161aed1a143f4134093c55b4d6979bbdbbe4b0683eb11`  
		Last Modified: Mon, 07 Aug 2023 20:30:59 GMT  
		Size: 285.1 KB (285089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53e61151a7324ffa6693144a2516060d0505b80fe8f27915b1e77165106c2a4`  
		Last Modified: Wed, 06 Sep 2023 18:40:12 GMT  
		Size: 66.2 MB (66222411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1f0b6eb00af4cec1a2c3a203cf9a97b7b5b1e669db11dbabc36635b0207c79`  
		Last Modified: Wed, 06 Sep 2023 18:40:01 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178fae6c6c7b745dbb7be349b0656255d25dc06d0c808f85cce56fdf95543af6`  
		Last Modified: Wed, 06 Sep 2023 18:58:02 GMT  
		Size: 5.1 MB (5099943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bda7158ac61debfc44dddd51b20bf5e411c5f34ec92ad21dfffe9a0eeb5ae76`  
		Last Modified: Wed, 06 Sep 2023 18:58:02 GMT  
		Size: 1.3 MB (1262386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13aa15f1f389977eef4ccb0c676963b08cbf0600c3979659a8852b95689e91e8`  
		Last Modified: Wed, 06 Sep 2023 18:58:02 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:795ac7c3a409b95ae5a486743690a31dea9328bc5af293a50f64b63112a9adf6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:dc29929d7895f513f69e34dede7fb945b1bf1540fb37abda23f6fa2edcaa5150
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2092646318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03e3e89d97096b15070b9c1274ebdfe7a5e0de7816cd24a72782cdcb25b33dc3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:39:54 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:39:56 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:41:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:41:12 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:42:07 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:42:08 GMT
ENV GOLANG_VERSION=1.21.0
# Thu, 10 Aug 2023 00:45:16 GMT
RUN $url = 'https://dl.google.com/go/go1.21.0.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '732121e64e0ecb07c77fdf6cc1bc5ce7b242c2d40d4ac29021ad4c64a08731f6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:45:17 GMT
WORKDIR C:\go
# Thu, 17 Aug 2023 22:18:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Aug 2023 22:18:30 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 17 Aug 2023 22:18:31 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:18:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 17 Aug 2023 22:19:38 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 17 Aug 2023 22:19:39 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594083c5c2094c95b4e52723d54c14e0d70881f4f176720c3170012275accc3b`  
		Last Modified: Thu, 10 Aug 2023 01:02:54 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e2c2a5b75ced3a3a50be088c4a6c2d7df926b1fe6515b2d0c021312e3642f4`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d28688050deeec928289543beadf5c75bb2a8246576cb7c066e23818016217`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e5fbc50e7e0fefb7c9e349038ecb00ed5c000bcab8c4d82b1e1000c4273c01`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0544e07bd9df923e11e09c7dc042da614f2f14589eb6fa79005ebbbf2731e97d`  
		Last Modified: Thu, 10 Aug 2023 01:02:57 GMT  
		Size: 25.6 MB (25560980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555a82506c4fcec2bd90ae77756e5b03788e30c89f1a3820aa0b6a7ae6ad58ae`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bcfb422b104764156fc5ba099b5e3ae9fa9f760fd2db1c21acd8969b3d73de`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 220.8 KB (220796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:decc470f4f54c3be087cde5dfcbd816bc68a441d25189983c12219fb4504e9e0`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4589eb0957da5bce467ff89344ebebb2f584a815991fd3004ae3f4890b74f51`  
		Last Modified: Thu, 10 Aug 2023 01:03:10 GMT  
		Size: 69.2 MB (69210847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a698ba14b77be2efdb0e931dc9abf7efc7c749ce53fa2d1c277cd009f295c0`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.5 KB (1517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265b35725533ea18f9e8b7d3422e1b960406141ca305f83de8f61dd49b340c74`  
		Last Modified: Thu, 17 Aug 2023 22:22:07 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3cd40483d2a2e0aae25c4caf3e900aca669895009d08c100e8754768099257`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1aaed9881a7c5017bdf3b46a5ba81399cd7bdaf9be397334872bbf8826386b`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00f7ca68792eb07043e7b43dec1b74b4e211701549286cdcc7993a3b76fdbce`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2516df9efacfe0206db24dbf7d952da6820b3ba9189c715b7aeb069bf903b0b`  
		Last Modified: Thu, 17 Aug 2023 22:22:05 GMT  
		Size: 1.7 MB (1680500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ed01fbe50be0cb731bfdaf18ffaad3e427b9cd10eaabf4930a0dda4b98450`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:f8893322f81862d0d41473494adb769699011eab49c16e9c66a37e7c5d1a61e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1906; amd64

### `caddy:builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:16053b4036029cc1457cb147a03be7a416b3fd01393e467beeb72def1f482edf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1894119169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e467c74cf811ff36bfae3619793832f5179eba1986cd92d51528fa3631e15b67`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:36:23 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:36:24 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:36:25 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:36:26 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:36:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:37:00 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:37:19 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:37:20 GMT
ENV GOLANG_VERSION=1.21.0
# Thu, 10 Aug 2023 00:39:40 GMT
RUN $url = 'https://dl.google.com/go/go1.21.0.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '732121e64e0ecb07c77fdf6cc1bc5ce7b242c2d40d4ac29021ad4c64a08731f6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:39:42 GMT
WORKDIR C:\go
# Thu, 17 Aug 2023 22:19:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Aug 2023 22:19:58 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 17 Aug 2023 22:19:58 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:19:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 17 Aug 2023 22:20:24 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 17 Aug 2023 22:20:25 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877256a6389e5e2563da79ad5bd201e7ee136abf14ff7cb0d4efbf3b24e5f127`  
		Last Modified: Thu, 10 Aug 2023 01:02:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a39df29b3c0b2f7e691c47273110db4a46e5c8e299f6bb95f77a9c61f79872`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8574d63bce1547e3177d0b76237a782a9b016d4880375dcd1a7b6a1c5dee3dc`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ef34b3c96316bcdd92e24c8c4eebdc3a35f245c013ef87edfae0dde091a305`  
		Last Modified: Thu, 10 Aug 2023 01:02:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a481babc5b629f694446a96dba8d77c020257c98334c605aff94162b9a917279`  
		Last Modified: Thu, 10 Aug 2023 01:02:23 GMT  
		Size: 25.6 MB (25554169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281178ea1c103ff07ea7e4fb647eb0dbe4f865742da6ef9944e04f37974fc27c`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b5d34adf2aacfe87580143f3e17c635dc8dbd4068377b79b35d665f49bbad9`  
		Last Modified: Thu, 10 Aug 2023 01:02:16 GMT  
		Size: 275.9 KB (275946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5b48235253668711a8e6a2ff934add92fea681c9256325d0ad13a01141c047`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4fb7d9dc956e10b22252d8212c98e2dee64526f471fa548eb6c842d5f05ae9`  
		Last Modified: Thu, 10 Aug 2023 01:02:35 GMT  
		Size: 69.2 MB (69216081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b888078988d2c04f6dae8641365e345f00127285805315ff6f554d6b93ac473c`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.5 KB (1451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b841ebd982703c219e6682e9f6ce05952af17249b1feeac24f29b4758db36694`  
		Last Modified: Thu, 17 Aug 2023 22:22:23 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fde1a85f81e8aec976e03a445fd68b44a23b9f74e66320c7dfce58a75409c25`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0498fcf11a96e26aace74390231497cf74c1d199da68217be38339f5e4108a3`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e49f04c5395ab27a41689cde8841498c15d6b18d029bb336e25274009098cc6`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c1983f7985d2513515cbe76bf211a71393e1a54cfd8e6b755d82fef2120d4a`  
		Last Modified: Thu, 17 Aug 2023 22:22:22 GMT  
		Size: 1.7 MB (1690677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d561bf1c2c8101b9e952ebca483dfa257b2d839feabe3857a1a2694e7d5d83f9`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:2332c4ebc4ae778b9697043d3fa3aaef6879dd17abc03200285af9d315353008
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4737; amd64
	-	windows version 10.0.20348.1906; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:733fe94133c4bd22c6ee8f9b9802bce8fede5e7b766bebde205a45dd4ac04aea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18363908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1e1b7ae170b7d7d7e524717fe978e0090023cc82a7d9ffe48e344b0351a3ee1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:09:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 18:20:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:19:38 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:19:41 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:19:41 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:19:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:19:42 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:19:42 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:19:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0aa7b81ef11c65f43b0b58323a33dd9e07eb785529f0d75b452f87a309db00c`  
		Last Modified: Mon, 07 Aug 2023 20:09:40 GMT  
		Size: 350.8 KB (350844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b3b3e68e52dc5ab939c72a9bbac39cff4bef4b87de399ddf28657471df6845`  
		Last Modified: Mon, 14 Aug 2023 18:20:42 GMT  
		Size: 7.5 KB (7502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c55d3259542348ddb70edc18dda7d48aeca5654962aed568a7034f3667d2ca`  
		Last Modified: Thu, 17 Aug 2023 22:20:10 GMT  
		Size: 14.6 MB (14603949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:dd029220558032e5d1f91173d32a0078dad12ec9b5114bef422ed4cdf05dec52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17314204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1de0523ee8d8173472fb08aa9a74a37bcd054af2b796b7631d847ba8a46986b5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:38:27 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:49:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:49:12 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:49:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:49:16 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:49:16 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:49:17 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:49:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172ef460a93549b8a3e73f6a515bccad93512788d1e8f095e7230ba41967c25a`  
		Last Modified: Wed, 09 Aug 2023 03:38:53 GMT  
		Size: 347.7 KB (347686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7aae78767a581df85fd1a51ccd646619aec320896ca016ef0f05a41b16bcbfe`  
		Last Modified: Mon, 14 Aug 2023 17:49:36 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82560a340155261ecbd1d99d87890c5aa0cfd64d571e1dcafc03e3b6a8132d48`  
		Last Modified: Thu, 17 Aug 2023 22:49:41 GMT  
		Size: 13.8 MB (13814204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:24649e9de43354963118f9cdf6ad1f4522c6993735f316763a2f5d1f76cba267
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17042831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb4a48fd29d50802cbf030949e2c9767eb6888e8412330f64246f322bc3b49c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:51:41 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:57:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:57:18 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:57:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:57:22 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:57:22 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:57:24 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:57:24 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:57:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a47b73e04459258b08555443754e92e2db20bde113c58ca18e1a6f07878f72`  
		Last Modified: Tue, 08 Aug 2023 01:52:05 GMT  
		Size: 344.5 KB (344462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e1b3e18d5e992f1805072b2d52405d575830bdce21726ef99dea99e31d8277`  
		Last Modified: Mon, 14 Aug 2023 17:57:42 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5879767a5d1969beb154b9a4991a767b0ed5be0c9739a972f07d03e825312fa5`  
		Last Modified: Thu, 17 Aug 2023 22:57:51 GMT  
		Size: 13.8 MB (13791384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:ed967fcd1968be6dc4699ff835cdd2d6f3f49105b9677f878c8a6960fd1a0643
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17162547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed7b6600470cab547aa1090baa39a6192ec83119989884ac742a63ed23be3da2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:09:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:39:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:39:17 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:39:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:39:19 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:39:19 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:39:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:39:20 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:39:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a699f78cfb85f60e17fc7c13495876ea0cb4495bbe39e8c65f3e8559b0d7169`  
		Last Modified: Mon, 07 Aug 2023 21:09:34 GMT  
		Size: 360.6 KB (360642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7488af8b96c79b6db13955a0302653c4e9f314d0833201984ae06c1ed697f06`  
		Last Modified: Mon, 14 Aug 2023 17:39:41 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597bfc484ba18727d2df98120cb9d559f346ade9e3a23be6a9af3e76dca89edd`  
		Last Modified: Thu, 17 Aug 2023 22:39:42 GMT  
		Size: 13.5 MB (13463635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:c3679836562d0252e6341a112d2729b8dae0eae550449bfe91fe2798171fd4ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16944934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc5ac831dce746cd0f4448640b7edaf0ce9457d09618e246ba72ee76ea63dcbe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:44:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 18:18:00 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:16:24 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:16:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:16:29 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:16:29 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:16:29 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:16:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:16:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:16:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:16:32 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:16:33 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:16:33 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:16:34 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:16:34 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:16:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f40714f45e39ac41e865ccbf2877db62255ce5a5c36a47eadf00b9d174f042`  
		Last Modified: Tue, 08 Aug 2023 00:45:18 GMT  
		Size: 362.2 KB (362173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d19953b5eb53ddaa0e25905527dc138e0c4111467bb7d71f81fa94976091351`  
		Last Modified: Mon, 14 Aug 2023 18:18:54 GMT  
		Size: 7.5 KB (7509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf4bf695323732c5ce84bbb0b976c5cd981eaf6814515a86f521af4a0e64582`  
		Last Modified: Thu, 17 Aug 2023 22:17:22 GMT  
		Size: 13.2 MB (13229001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:ca7ab0dcf4ab146df48cfa8ae6e07fed804feeed4a36358fa652c8eac52b40da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17720356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d4d019ffc0cd69ea8c5d3b8fb0a39c89d3aa1b2037c1012a9ba4bed6abb94dc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:14:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:41:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:41:35 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:41:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:41:39 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:41:39 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:41:39 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:41:40 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:41:41 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:41:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df19abd0ca1d4a821a4174a2c0831a57d6fd584073f056abcae085a51f0b3848`  
		Last Modified: Mon, 07 Aug 2023 20:14:50 GMT  
		Size: 354.9 KB (354950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308478977890baa82477ee70a3065fb9da2080efcc95facf1a87ac021b06a8e9`  
		Last Modified: Mon, 14 Aug 2023 17:42:17 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2394cd7c9416df19c45596c558f5a7ee05adc5a7fd166f58dcbf26f1ac6ecae6`  
		Last Modified: Thu, 17 Aug 2023 22:42:16 GMT  
		Size: 14.1 MB (14143708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:8d641d87b059de975dc94ff579d47434e347b333b33a4a8f15cd679c062a14c0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2011934670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e21b2ad9f1a3657d84dd869da76d22704a2848d4a92f831acbfef09e26e80cc6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 14 Aug 2023 18:16:58 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 17 Aug 2023 22:14:59 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:16:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 17 Aug 2023 22:16:13 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 17 Aug 2023 22:16:14 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 17 Aug 2023 22:16:15 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:16:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:16:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:16:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:16:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:16:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:16:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:16:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:16:21 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:16:22 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:16:23 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:16:24 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:17:19 GMT
RUN caddy version
# Thu, 17 Aug 2023 22:17:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d698e8ba8bfd4c31116f0d2c87cfcf2ff17baa1a5c678b116b3aa1ac8ed73d`  
		Last Modified: Mon, 14 Aug 2023 18:23:17 GMT  
		Size: 483.6 KB (483626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dcf545f7c90cab6f6962d3099898462129da2e6b06a80802d52ff1e9d2fca08`  
		Last Modified: Thu, 17 Aug 2023 22:21:12 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65ecc8b4521923b522dd6392a862d0dff9edd10c1e3b520de8f130de2170880`  
		Last Modified: Thu, 17 Aug 2023 22:21:16 GMT  
		Size: 15.2 MB (15201779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ddd9c690b84a4a4744ec5ac91059e12e1aa92378220080fcfbf616c59b4c26`  
		Last Modified: Thu, 17 Aug 2023 22:21:12 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63adbcb9cba5e8d67eac5e059c7bbb9dfe3040f0933afb5e1f8cb7d4c211b4a`  
		Last Modified: Thu, 17 Aug 2023 22:21:11 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e15ff22938f514e6118606619ff28e9e5ee145d6f3dc6de1de62ea4051575c1`  
		Last Modified: Thu, 17 Aug 2023 22:21:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438a6cab105b637f625a3fd00d7ecaa6792ad5dc120bf1be36e7d6e19ee44b4d`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfd206f96497c8e0730c72c36ecedea57379a6a219903785dc1478b50b3945`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e651df7142dc872814a59faff8cf791ab4e4413ee6a9b043fe02a2af9da24fe`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b7f62d857ed7e15d08d52d1ef08f3c21e25751d17e8a5418c02f6adc366eab`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6347f1227dc933d98b8f02d22cd440529284e7c8e415e96cee265ae2c7445b3`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2776f9f89b2242d27c9c49da3465d2ff6acb224dd3315837bda709f3fa0aa4ff`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aaab02f29add47735607e798c40625216306d00d57988d1ece40f43b93f706c`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ed26555e0c9e51aa5dbf4125ef3ea56c6d84274b4d8160ce10c3c0d9e7106d`  
		Last Modified: Thu, 17 Aug 2023 22:21:08 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392c0484ea6d941786f507e72c143bd1c64d4c42bcd773bd745330a55b89d356`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef07137395441a56a870d882d84faac751156b0486c6528fa18b6d706ff250d8`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2950cf3d51ba47c2b41415fccf9b67e813735f67ccc34a0ce5f1a1a4a34e56dc`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25de03b5a8b8f2752cde31b881d457ec5900438b781cc65cda3aca9444b2377f`  
		Last Modified: Thu, 17 Aug 2023 22:21:07 GMT  
		Size: 269.9 KB (269882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f3d70fb1dd11e79f9128736ada85993e1b4fd603b2f8164aac49ac1efda548`  
		Last Modified: Thu, 17 Aug 2023 22:21:07 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:f4791cb0179b98b28e760842405262d782735176b147c84f26709bd1361c8798
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1813299019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b759bf39605cbc0d0ceaaa8eda1623452b1acd67deb11c0d22defff59f2058`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 14 Aug 2023 18:19:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 17 Aug 2023 22:17:27 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:17:55 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 17 Aug 2023 22:17:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 17 Aug 2023 22:17:56 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 17 Aug 2023 22:17:57 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:17:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:17:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:17:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:18:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:18:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:18:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:18:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:18:04 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:18:04 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:18:05 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:18:06 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:18:21 GMT
RUN caddy version
# Thu, 17 Aug 2023 22:18:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c23e01ee014d9e05e276268c94980b00a0720fcb5488a368b20ee74701ed78`  
		Last Modified: Mon, 14 Aug 2023 18:23:42 GMT  
		Size: 461.2 KB (461170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8a7576f0b2ff121a0e9658821e52a7b356abbd90c9215b750ab7fc2127f6ae`  
		Last Modified: Thu, 17 Aug 2023 22:21:41 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ecc6db59a89a0a9f61364702d6af7202fa4f3f742ec6dff93c3a5b53e3826`  
		Last Modified: Thu, 17 Aug 2023 22:21:44 GMT  
		Size: 15.2 MB (15169088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9323e4528d7a59819754484fdbeb047240a6f1f0dd262b734a226a4249dc0a0`  
		Last Modified: Thu, 17 Aug 2023 22:21:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb3a3b69dd93b979cdcd1e0759ee1199bc8d5a510a6ce9bca3856201d747468`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56ce33676578802911228ae7aba31fe1898897ede8c69e12a0959a37a11d130`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c896eeb3f2c45b2bba4fe5e5da02be1289c4cabcf574a38c19d1616ebf552d4c`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6563dd3d5f912ae2b7bd629d2dc731df89b1dd107e2cbb85dee24a0d5c550a1`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420011263062842c72720998f13fa245d9bef077622fde4e17cc60cef3e00bce`  
		Last Modified: Thu, 17 Aug 2023 22:21:38 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2385fc0cb7a281a35df415654aba711bf70fa23b963faf0a3f0055d760f5c41c`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a58351f25f399f8a9399e60dd315cd8c695972a9e51f2271e3377151cf621d`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506eb3a97b70fc7dc1c1c3464a89512890cd48c354658e58e61d5acfee63f1c3`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86cf8c25cfcaf858db6ffd2630a26ca3a13ad2fdc941a01438ea9ea80ccb20c`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcedddef9863d16c4d713280050f604b44968bc253844c27e46cb8871eb17a99`  
		Last Modified: Thu, 17 Aug 2023 22:21:36 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d01313141e38a9b2b15a3e831a2d11a3eb47611bf99b0677be3c49693984f64`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504a80bc0f7aa0c98a143033f551be8fcf0653046e7313c0de080b82ad97ad52`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280053e45030e2421ea4d1cdfd721c24f40d30518b1ce8af7e0811363daf6eca`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0d07466cd8f053bf957a35cbe340d419f5c2f6ff48565bb8a5b255998e3e94`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 280.9 KB (280938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad52776067d7be890960cfd7082041a93a802b96fea6d31fc724192c49eb00`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:9b2d0e89dc4f5f508ec90143d8b6b6d2cdbe9067fea9d0930cbb9812eb816b01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4737; amd64
	-	windows version 10.0.20348.1906; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:8d641d87b059de975dc94ff579d47434e347b333b33a4a8f15cd679c062a14c0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2011934670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e21b2ad9f1a3657d84dd869da76d22704a2848d4a92f831acbfef09e26e80cc6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 14 Aug 2023 18:16:58 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 17 Aug 2023 22:14:59 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:16:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 17 Aug 2023 22:16:13 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 17 Aug 2023 22:16:14 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 17 Aug 2023 22:16:15 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:16:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:16:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:16:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:16:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:16:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:16:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:16:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:16:21 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:16:22 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:16:23 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:16:24 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:17:19 GMT
RUN caddy version
# Thu, 17 Aug 2023 22:17:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d698e8ba8bfd4c31116f0d2c87cfcf2ff17baa1a5c678b116b3aa1ac8ed73d`  
		Last Modified: Mon, 14 Aug 2023 18:23:17 GMT  
		Size: 483.6 KB (483626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dcf545f7c90cab6f6962d3099898462129da2e6b06a80802d52ff1e9d2fca08`  
		Last Modified: Thu, 17 Aug 2023 22:21:12 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65ecc8b4521923b522dd6392a862d0dff9edd10c1e3b520de8f130de2170880`  
		Last Modified: Thu, 17 Aug 2023 22:21:16 GMT  
		Size: 15.2 MB (15201779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ddd9c690b84a4a4744ec5ac91059e12e1aa92378220080fcfbf616c59b4c26`  
		Last Modified: Thu, 17 Aug 2023 22:21:12 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63adbcb9cba5e8d67eac5e059c7bbb9dfe3040f0933afb5e1f8cb7d4c211b4a`  
		Last Modified: Thu, 17 Aug 2023 22:21:11 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e15ff22938f514e6118606619ff28e9e5ee145d6f3dc6de1de62ea4051575c1`  
		Last Modified: Thu, 17 Aug 2023 22:21:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438a6cab105b637f625a3fd00d7ecaa6792ad5dc120bf1be36e7d6e19ee44b4d`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfd206f96497c8e0730c72c36ecedea57379a6a219903785dc1478b50b3945`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e651df7142dc872814a59faff8cf791ab4e4413ee6a9b043fe02a2af9da24fe`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b7f62d857ed7e15d08d52d1ef08f3c21e25751d17e8a5418c02f6adc366eab`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6347f1227dc933d98b8f02d22cd440529284e7c8e415e96cee265ae2c7445b3`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2776f9f89b2242d27c9c49da3465d2ff6acb224dd3315837bda709f3fa0aa4ff`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aaab02f29add47735607e798c40625216306d00d57988d1ece40f43b93f706c`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ed26555e0c9e51aa5dbf4125ef3ea56c6d84274b4d8160ce10c3c0d9e7106d`  
		Last Modified: Thu, 17 Aug 2023 22:21:08 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392c0484ea6d941786f507e72c143bd1c64d4c42bcd773bd745330a55b89d356`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef07137395441a56a870d882d84faac751156b0486c6528fa18b6d706ff250d8`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2950cf3d51ba47c2b41415fccf9b67e813735f67ccc34a0ce5f1a1a4a34e56dc`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25de03b5a8b8f2752cde31b881d457ec5900438b781cc65cda3aca9444b2377f`  
		Last Modified: Thu, 17 Aug 2023 22:21:07 GMT  
		Size: 269.9 KB (269882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f3d70fb1dd11e79f9128736ada85993e1b4fd603b2f8164aac49ac1efda548`  
		Last Modified: Thu, 17 Aug 2023 22:21:07 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:f4791cb0179b98b28e760842405262d782735176b147c84f26709bd1361c8798
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1813299019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b759bf39605cbc0d0ceaaa8eda1623452b1acd67deb11c0d22defff59f2058`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 14 Aug 2023 18:19:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 17 Aug 2023 22:17:27 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:17:55 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 17 Aug 2023 22:17:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 17 Aug 2023 22:17:56 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 17 Aug 2023 22:17:57 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:17:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:17:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:17:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:18:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:18:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:18:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:18:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:18:04 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:18:04 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:18:05 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:18:06 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:18:21 GMT
RUN caddy version
# Thu, 17 Aug 2023 22:18:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c23e01ee014d9e05e276268c94980b00a0720fcb5488a368b20ee74701ed78`  
		Last Modified: Mon, 14 Aug 2023 18:23:42 GMT  
		Size: 461.2 KB (461170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8a7576f0b2ff121a0e9658821e52a7b356abbd90c9215b750ab7fc2127f6ae`  
		Last Modified: Thu, 17 Aug 2023 22:21:41 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ecc6db59a89a0a9f61364702d6af7202fa4f3f742ec6dff93c3a5b53e3826`  
		Last Modified: Thu, 17 Aug 2023 22:21:44 GMT  
		Size: 15.2 MB (15169088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9323e4528d7a59819754484fdbeb047240a6f1f0dd262b734a226a4249dc0a0`  
		Last Modified: Thu, 17 Aug 2023 22:21:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb3a3b69dd93b979cdcd1e0759ee1199bc8d5a510a6ce9bca3856201d747468`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56ce33676578802911228ae7aba31fe1898897ede8c69e12a0959a37a11d130`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c896eeb3f2c45b2bba4fe5e5da02be1289c4cabcf574a38c19d1616ebf552d4c`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6563dd3d5f912ae2b7bd629d2dc731df89b1dd107e2cbb85dee24a0d5c550a1`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420011263062842c72720998f13fa245d9bef077622fde4e17cc60cef3e00bce`  
		Last Modified: Thu, 17 Aug 2023 22:21:38 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2385fc0cb7a281a35df415654aba711bf70fa23b963faf0a3f0055d760f5c41c`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a58351f25f399f8a9399e60dd315cd8c695972a9e51f2271e3377151cf621d`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506eb3a97b70fc7dc1c1c3464a89512890cd48c354658e58e61d5acfee63f1c3`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86cf8c25cfcaf858db6ffd2630a26ca3a13ad2fdc941a01438ea9ea80ccb20c`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcedddef9863d16c4d713280050f604b44968bc253844c27e46cb8871eb17a99`  
		Last Modified: Thu, 17 Aug 2023 22:21:36 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d01313141e38a9b2b15a3e831a2d11a3eb47611bf99b0677be3c49693984f64`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504a80bc0f7aa0c98a143033f551be8fcf0653046e7313c0de080b82ad97ad52`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280053e45030e2421ea4d1cdfd721c24f40d30518b1ce8af7e0811363daf6eca`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0d07466cd8f053bf957a35cbe340d419f5c2f6ff48565bb8a5b255998e3e94`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 280.9 KB (280938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad52776067d7be890960cfd7082041a93a802b96fea6d31fc724192c49eb00`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:44adcd32029ece40e50aef18ba70e3020cbba5b53153929078326ec23613226c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:8d641d87b059de975dc94ff579d47434e347b333b33a4a8f15cd679c062a14c0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2011934670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e21b2ad9f1a3657d84dd869da76d22704a2848d4a92f831acbfef09e26e80cc6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 14 Aug 2023 18:16:58 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 17 Aug 2023 22:14:59 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:16:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 17 Aug 2023 22:16:13 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 17 Aug 2023 22:16:14 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 17 Aug 2023 22:16:15 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:16:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:16:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:16:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:16:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:16:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:16:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:16:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:16:21 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:16:22 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:16:23 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:16:24 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:17:19 GMT
RUN caddy version
# Thu, 17 Aug 2023 22:17:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d698e8ba8bfd4c31116f0d2c87cfcf2ff17baa1a5c678b116b3aa1ac8ed73d`  
		Last Modified: Mon, 14 Aug 2023 18:23:17 GMT  
		Size: 483.6 KB (483626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dcf545f7c90cab6f6962d3099898462129da2e6b06a80802d52ff1e9d2fca08`  
		Last Modified: Thu, 17 Aug 2023 22:21:12 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65ecc8b4521923b522dd6392a862d0dff9edd10c1e3b520de8f130de2170880`  
		Last Modified: Thu, 17 Aug 2023 22:21:16 GMT  
		Size: 15.2 MB (15201779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ddd9c690b84a4a4744ec5ac91059e12e1aa92378220080fcfbf616c59b4c26`  
		Last Modified: Thu, 17 Aug 2023 22:21:12 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63adbcb9cba5e8d67eac5e059c7bbb9dfe3040f0933afb5e1f8cb7d4c211b4a`  
		Last Modified: Thu, 17 Aug 2023 22:21:11 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e15ff22938f514e6118606619ff28e9e5ee145d6f3dc6de1de62ea4051575c1`  
		Last Modified: Thu, 17 Aug 2023 22:21:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438a6cab105b637f625a3fd00d7ecaa6792ad5dc120bf1be36e7d6e19ee44b4d`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfd206f96497c8e0730c72c36ecedea57379a6a219903785dc1478b50b3945`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e651df7142dc872814a59faff8cf791ab4e4413ee6a9b043fe02a2af9da24fe`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b7f62d857ed7e15d08d52d1ef08f3c21e25751d17e8a5418c02f6adc366eab`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6347f1227dc933d98b8f02d22cd440529284e7c8e415e96cee265ae2c7445b3`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2776f9f89b2242d27c9c49da3465d2ff6acb224dd3315837bda709f3fa0aa4ff`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aaab02f29add47735607e798c40625216306d00d57988d1ece40f43b93f706c`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ed26555e0c9e51aa5dbf4125ef3ea56c6d84274b4d8160ce10c3c0d9e7106d`  
		Last Modified: Thu, 17 Aug 2023 22:21:08 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392c0484ea6d941786f507e72c143bd1c64d4c42bcd773bd745330a55b89d356`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef07137395441a56a870d882d84faac751156b0486c6528fa18b6d706ff250d8`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2950cf3d51ba47c2b41415fccf9b67e813735f67ccc34a0ce5f1a1a4a34e56dc`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25de03b5a8b8f2752cde31b881d457ec5900438b781cc65cda3aca9444b2377f`  
		Last Modified: Thu, 17 Aug 2023 22:21:07 GMT  
		Size: 269.9 KB (269882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f3d70fb1dd11e79f9128736ada85993e1b4fd603b2f8164aac49ac1efda548`  
		Last Modified: Thu, 17 Aug 2023 22:21:07 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:25814323b2b1cf78a7dfadd252104b12d24aa4dc9512441a2717cd13b1d3da8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1906; amd64

### `caddy:windowsservercore-ltsc2022` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:f4791cb0179b98b28e760842405262d782735176b147c84f26709bd1361c8798
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1813299019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b759bf39605cbc0d0ceaaa8eda1623452b1acd67deb11c0d22defff59f2058`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 14 Aug 2023 18:19:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 17 Aug 2023 22:17:27 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:17:55 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 17 Aug 2023 22:17:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 17 Aug 2023 22:17:56 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 17 Aug 2023 22:17:57 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:17:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:17:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:17:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:18:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:18:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:18:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:18:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:18:04 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:18:04 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:18:05 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:18:06 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:18:21 GMT
RUN caddy version
# Thu, 17 Aug 2023 22:18:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c23e01ee014d9e05e276268c94980b00a0720fcb5488a368b20ee74701ed78`  
		Last Modified: Mon, 14 Aug 2023 18:23:42 GMT  
		Size: 461.2 KB (461170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8a7576f0b2ff121a0e9658821e52a7b356abbd90c9215b750ab7fc2127f6ae`  
		Last Modified: Thu, 17 Aug 2023 22:21:41 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ecc6db59a89a0a9f61364702d6af7202fa4f3f742ec6dff93c3a5b53e3826`  
		Last Modified: Thu, 17 Aug 2023 22:21:44 GMT  
		Size: 15.2 MB (15169088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9323e4528d7a59819754484fdbeb047240a6f1f0dd262b734a226a4249dc0a0`  
		Last Modified: Thu, 17 Aug 2023 22:21:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb3a3b69dd93b979cdcd1e0759ee1199bc8d5a510a6ce9bca3856201d747468`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56ce33676578802911228ae7aba31fe1898897ede8c69e12a0959a37a11d130`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c896eeb3f2c45b2bba4fe5e5da02be1289c4cabcf574a38c19d1616ebf552d4c`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6563dd3d5f912ae2b7bd629d2dc731df89b1dd107e2cbb85dee24a0d5c550a1`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420011263062842c72720998f13fa245d9bef077622fde4e17cc60cef3e00bce`  
		Last Modified: Thu, 17 Aug 2023 22:21:38 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2385fc0cb7a281a35df415654aba711bf70fa23b963faf0a3f0055d760f5c41c`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a58351f25f399f8a9399e60dd315cd8c695972a9e51f2271e3377151cf621d`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506eb3a97b70fc7dc1c1c3464a89512890cd48c354658e58e61d5acfee63f1c3`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86cf8c25cfcaf858db6ffd2630a26ca3a13ad2fdc941a01438ea9ea80ccb20c`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcedddef9863d16c4d713280050f604b44968bc253844c27e46cb8871eb17a99`  
		Last Modified: Thu, 17 Aug 2023 22:21:36 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d01313141e38a9b2b15a3e831a2d11a3eb47611bf99b0677be3c49693984f64`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504a80bc0f7aa0c98a143033f551be8fcf0653046e7313c0de080b82ad97ad52`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280053e45030e2421ea4d1cdfd721c24f40d30518b1ce8af7e0811363daf6eca`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0d07466cd8f053bf957a35cbe340d419f5c2f6ff48565bb8a5b255998e3e94`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 280.9 KB (280938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad52776067d7be890960cfd7082041a93a802b96fea6d31fc724192c49eb00`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
