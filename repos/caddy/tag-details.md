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
$ docker pull caddy@sha256:df239ca80315c8271f9e87a981fb47124831f8b5a7c85970249d2dfd712479a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4851; amd64
	-	windows version 10.0.20348.1970; amd64

### `caddy:2` - linux; amd64

```console
$ docker pull caddy@sha256:3d1bf053476f2415b40e728c37e1112ee7551fa154a63d6f62b275c13fea8166
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18364247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a7b2e234b158c1e01eab04f851fc4b1a33296dbaa68c57d11815ee38a3cafaf`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:43:13 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 22:43:15 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 22:43:15 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 22:43:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 22:43:17 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 22:43:17 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 22:43:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 22:43:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 22:43:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 80
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 443
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 22:43:18 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 22:43:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37be51084fb891c6796079e693b73f6f882266a5e66211344173031e2b0c8ffd`  
		Last Modified: Thu, 28 Sep 2023 22:43:35 GMT  
		Size: 350.8 KB (350826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d867aa37ac50364bf4082dc48c7d4e1b88ead3164d47855e1bbc2ef3678cfc`  
		Last Modified: Thu, 28 Sep 2023 22:43:35 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147aa3899aa3307c28e185f5385015c7a5f15dfa42578a8a8eca88bf2f1e7e3e`  
		Last Modified: Thu, 28 Sep 2023 22:43:37 GMT  
		Size: 14.6 MB (14603949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:239c4a78d1bd0540a44003332119cf019e6ff839f4d303cd9801b1cc9e755ec4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17314598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b41f754b4ebb826dde7fb5c0c3c6048823add70f27a7f9c8d9f8ff1a9636ed2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:59:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 21:59:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 21:59:13 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 21:59:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 21:59:16 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 21:59:16 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 21:59:16 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 21:59:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 21:59:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 80
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 443
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 21:59:17 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 21:59:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1018057a600163b1c1b92c21ade975c631b2f8ccde66d524cfe0ecdac8e1920d`  
		Last Modified: Thu, 28 Sep 2023 21:59:43 GMT  
		Size: 347.6 KB (347613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec54680cbf2cb1a25285c82a7888498ab47d03a68db200a160d7162325a5be19`  
		Last Modified: Thu, 28 Sep 2023 21:59:43 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d087db4282d622690fce98f1d8802151567e43bfdd884a3e2a4d084701229a1`  
		Last Modified: Thu, 28 Sep 2023 21:59:45 GMT  
		Size: 13.8 MB (13814189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:85dd4fae9241ac3330e98e1d3b052d36b7ecbe1cd69b4c860454c84976426e70
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17043239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f78b426118e91fcb43786aa4c3003cd91ee86ab5f896516a885f964056b08cae`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:19:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 23:19:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 23:19:20 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 23:19:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 23:19:24 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 23:19:24 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 80
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 443
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 23:19:25 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 23:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66901ba48d0ee53cd827f4eb2cfd8b049cebba8c3d307b69760e1be917f69476`  
		Last Modified: Thu, 28 Sep 2023 23:19:46 GMT  
		Size: 344.4 KB (344448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dddeb3f6febb36993d8a51ad919784fd152aab5f6e17fe00d579916f32e42911`  
		Last Modified: Thu, 28 Sep 2023 23:19:46 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f936b2c0499a587b75385edfeb1d22b8f16ed05dca7dd0999ccc0635e1904a`  
		Last Modified: Thu, 28 Sep 2023 23:19:48 GMT  
		Size: 13.8 MB (13791383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:595e5490450c9ed29cc960149e2c265210e8444f3b3ea5ff2fab62d0da5ec3d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17163627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23f8ae4a1af151ac93d2945855095990774bc44f70af5c0e4b058dbb7e8b8c09`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:16:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 29 Sep 2023 01:16:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 29 Sep 2023 01:16:13 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 01:16:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 29 Sep 2023 01:16:15 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 29 Sep 2023 01:16:15 GMT
ENV XDG_DATA_HOME=/data
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 80
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 443
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 443/udp
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 2019
# Fri, 29 Sep 2023 01:16:16 GMT
WORKDIR /srv
# Fri, 29 Sep 2023 01:16:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f21cb0286edf1f5fefb4a859b414a446bb81baa9e8901fc8f4eca55a43aeeec`  
		Last Modified: Fri, 29 Sep 2023 01:16:34 GMT  
		Size: 360.6 KB (360643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5444b3f9419d06a4b77a65935a3b1c6e657c607bcfb9e3bd1abebe57eae36e6a`  
		Last Modified: Fri, 29 Sep 2023 01:16:34 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3485ef64f848b891981d59d52e0b092b261205ad787b38ae389e5ac39eed493f`  
		Last Modified: Fri, 29 Sep 2023 01:16:35 GMT  
		Size: 13.5 MB (13463646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:65084a14a1557b92af5b8ba6fcba9a7a710ed5caef1e2310f9622166608c9531
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16945195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73ba45deaa04c3feac6474c22204ac6f5ebc380b331ff7d585ecd196284459b3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:17:03 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 29 Sep 2023 02:17:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 29 Sep 2023 02:17:06 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 02:17:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 29 Sep 2023 02:17:13 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 29 Sep 2023 02:17:14 GMT
ENV XDG_DATA_HOME=/data
# Fri, 29 Sep 2023 02:17:15 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Fri, 29 Sep 2023 02:17:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 29 Sep 2023 02:17:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 29 Sep 2023 02:17:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 29 Sep 2023 02:17:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 29 Sep 2023 02:17:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 29 Sep 2023 02:17:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 29 Sep 2023 02:17:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 29 Sep 2023 02:17:21 GMT
EXPOSE 80
# Fri, 29 Sep 2023 02:17:21 GMT
EXPOSE 443
# Fri, 29 Sep 2023 02:17:22 GMT
EXPOSE 443/udp
# Fri, 29 Sep 2023 02:17:22 GMT
EXPOSE 2019
# Fri, 29 Sep 2023 02:17:24 GMT
WORKDIR /srv
# Fri, 29 Sep 2023 02:17:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa65cea7f5d70d1e203b851e43ad676e92f28c930ad32b6691e84ff9b5cda87`  
		Last Modified: Fri, 29 Sep 2023 02:18:03 GMT  
		Size: 362.2 KB (362182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7089a1d537371e29a65d106f43b45f2a0367d4d1db0eb7d6b7099f8ba05645`  
		Last Modified: Fri, 29 Sep 2023 02:18:01 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b93ab741fa6270144ea59d6a5fa3c4138286a569f246fdccd829b317b051f3a`  
		Last Modified: Fri, 29 Sep 2023 02:18:05 GMT  
		Size: 13.2 MB (13228998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:9e13bd2b56147eecc80f1fe1710e4350ea63d5edfb389fa89e2c6de06c08593a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17721238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2f0101e0f893afb763d99b2050dbf4d68a44aae29785af6c05af5a552b0c1a7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:19:38 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 22:19:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 22:19:39 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 22:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 22:19:42 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 22:19:42 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 80
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 443
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 22:19:44 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 22:19:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed3df874173df47ad0bd0ef67b8ee598c77921810d84a67fd2984c4f8151c91`  
		Last Modified: Thu, 28 Sep 2023 22:20:14 GMT  
		Size: 354.9 KB (354948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95a69c42a5c7fc6d73c00c7f6eb68522f3881aae55db4f85a8400e83b678b181`  
		Last Modified: Thu, 28 Sep 2023 22:20:14 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793016dc78c9794c627c07afcd2fb34af4ee470ee7fef1a1596eff0c59ba6659`  
		Last Modified: Thu, 28 Sep 2023 22:20:16 GMT  
		Size: 14.1 MB (14143684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.4851; amd64

```console
$ docker pull caddy@sha256:3f230e8c687c5611e74c84c3ec6f7ef7844b3cc3443d9302e9bb778e6210bfe2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2032252342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea189389e39a38d33c2124e3c02e0a9bc2f3168e5605fa8a909e749ac52fc3f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:30:52 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:30:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:32:00 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:32:02 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:32:04 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:32:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:32:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:32:08 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:32:09 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:33:07 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:33:07 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2bc90334de89082943edb24d5f52a3bb36ef134c17a417ba45cc4e122be3b2`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 465.0 KB (465015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba1c9fb8dedf070862eb0526393862bb5a0f2c87a87bc3864b9b24b11af5524`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5249ade277243b1b7f8c198de7d036f2e106b8a679d777b7bfc885af7b9b76`  
		Last Modified: Wed, 13 Sep 2023 05:37:46 GMT  
		Size: 15.2 MB (15176891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224a0aed4c02b4a48f633ac01c40e020d4e8fbc32fe8896d93032f9d72f50cda`  
		Last Modified: Wed, 13 Sep 2023 05:37:42 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fc1c10b7da22b1e9a26f059801a53ce4ce22e7d24ab14ec56d343a806f3bc2`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bd26e7302c16a8d83a8a6b5d9d263b804279f2b4c7d2fcea59a97c1e187648`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f69e667aa7c5e5a21f7d8a8cdd213b9d20a8a0c790dd18fe51d4df9e5b08a7`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e456b9da79a468c972d487e55e3628f8a8917f78948550c359afc891a5ad24a`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bc4af3e90793180c1ed8b8b9ac6866e24a5de16881f363dacf0ecf47396c8`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0289dff328d597d94fcd8612bd4a726573e13f780790744c5c6f4b40b49823`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52ff2438c88a58e8be33368f668557c92bcfdc503bd58025d081c7b88ec88b`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0f1c855afa9fd7bcf5ded632c161f2ff013f4b08f5c233fa3bdf3d13701467`  
		Last Modified: Wed, 13 Sep 2023 05:37:38 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2e0bf79eee4bbd609b5a111793e394f22ad86eb897cf85c6df2c45d9a8d777`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff797288117550c2b80f9a39dd5a04cb449defc2660cf6a7589618b8d3606464`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa0d1665270ae2e22844b2386842b1deab36f8936506db82df0ec69dc72fb84`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c867297eb9d01dfe100695ae10a0c67bd38f2124de0ee7446d1e66b6dede5c06`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee97f69cfbd31f5a098d45934b159384d8e986d860ad3007140beee338aa4533`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b741c4ffade19f3d712c3fb839c3ae7f1ae4e39e5f777a2b24917b5e630d0f86`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 256.7 KB (256675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a415b22709a225227fa7ce65d7767f3f820c7e9e445b0d718dfb68ae2249832`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.20348.1970; amd64

```console
$ docker pull caddy@sha256:76214fe6feb9f96f1c46334c01e1b9d310eb2e745bb08ba4130547b2147f3677
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1853253940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f0e585ea0797bdd13d148afed1e86161022e8cf2a79d11337f9d4dde0a8efe6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 01:35:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:33:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:33:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:34:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:34:25 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:34:26 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:34:27 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:34:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:34:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:34:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:34:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:34:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:34:33 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:34:34 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:34:35 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:34:36 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:34:56 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:34:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f40969dbf1e035a6c49e7c40b216960e3ee98ec3b76f76f9fe4498d0110bee`  
		Last Modified: Wed, 13 Sep 2023 02:15:22 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2d313a26784edb67b74292171891c0393ea119a53238e09150b5b7bc52371f`  
		Last Modified: Wed, 13 Sep 2023 05:38:08 GMT  
		Size: 483.0 KB (482985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb50376a60c42178e92d96a048b0e7f2dbc2cafe73274ab76722cda86fb32ee`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeecad99d9c5b378a623153b24130f8c36442e9a48ef6a48f878c5f585a66bd4`  
		Last Modified: Wed, 13 Sep 2023 05:38:11 GMT  
		Size: 15.2 MB (15183860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6b7a19981a71c15e39afbc3a52ed5f0c065f77c1ccd55a88e5f1b51af88753`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd7340889e9a6bfc8018c7709595b75ef962cf2608d14398ffbc90b90804a04`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7537acdfe48467d248afb6a69dad6bdb09c62617600305d2b2adb8a45ece2f`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf3cb277ba29189d90269123acd401fa787771fb095f2f2ec532be7bba2a025`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64eb5cc4069279b73a665e35bf526fa42558af1a3a71fc13d76913846d96818`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74348cf2ecbfe3a00df246034f9ab755418e8584b24113c9d327fc80cb134829`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa3fef62dce81d37fff2c621b94314d2aa9d0318523407b0a1d7d2b1e079234`  
		Last Modified: Wed, 13 Sep 2023 05:38:04 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d033d5a006e7fa969026194ef48446c840a891ad252f0316d32bc01843f0e4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbef09c0840262b42ba39068c868fc9b353bed78bb7de251e953289149e9a64e`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea46de371cf13fdb02566c79fc3a22c7123bd7c8903d20645b9cfe34f7ca85d4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63cdcd333c2c131733511c6750d4154ea7f097d981934d1dda8944bf2840860`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8259824bfebcdadd0448ccc0a815b7257636f6eb420e7e00216359908281e7b`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51874919dc1cfa2121d50499f839a702c4cd7340e8708e90b2af042e9debba9`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee3a41ffde2d883c73932756f176ba6901eaeb7a680a351a2b476398263cc8`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73e8028e6f79476106af6c347aa4765644a8ed828c5b6c117ee3dcc2e22e1ef`  
		Last Modified: Wed, 13 Sep 2023 05:38:02 GMT  
		Size: 289.2 KB (289194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd87253476a12fff6cbe718338261ef5ec78a1eb19d8e222838e7f96c3100a0`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:11ae052d9015105757d19caf86dc51fc14403841f2b65e93fe320f4d0e197385
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
$ docker pull caddy@sha256:3d1bf053476f2415b40e728c37e1112ee7551fa154a63d6f62b275c13fea8166
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18364247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a7b2e234b158c1e01eab04f851fc4b1a33296dbaa68c57d11815ee38a3cafaf`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:43:13 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 22:43:15 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 22:43:15 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 22:43:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 22:43:17 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 22:43:17 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 22:43:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 22:43:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 22:43:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 80
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 443
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 22:43:18 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 22:43:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37be51084fb891c6796079e693b73f6f882266a5e66211344173031e2b0c8ffd`  
		Last Modified: Thu, 28 Sep 2023 22:43:35 GMT  
		Size: 350.8 KB (350826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d867aa37ac50364bf4082dc48c7d4e1b88ead3164d47855e1bbc2ef3678cfc`  
		Last Modified: Thu, 28 Sep 2023 22:43:35 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147aa3899aa3307c28e185f5385015c7a5f15dfa42578a8a8eca88bf2f1e7e3e`  
		Last Modified: Thu, 28 Sep 2023 22:43:37 GMT  
		Size: 14.6 MB (14603949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:239c4a78d1bd0540a44003332119cf019e6ff839f4d303cd9801b1cc9e755ec4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17314598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b41f754b4ebb826dde7fb5c0c3c6048823add70f27a7f9c8d9f8ff1a9636ed2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:59:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 21:59:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 21:59:13 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 21:59:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 21:59:16 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 21:59:16 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 21:59:16 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 21:59:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 21:59:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 80
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 443
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 21:59:17 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 21:59:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1018057a600163b1c1b92c21ade975c631b2f8ccde66d524cfe0ecdac8e1920d`  
		Last Modified: Thu, 28 Sep 2023 21:59:43 GMT  
		Size: 347.6 KB (347613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec54680cbf2cb1a25285c82a7888498ab47d03a68db200a160d7162325a5be19`  
		Last Modified: Thu, 28 Sep 2023 21:59:43 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d087db4282d622690fce98f1d8802151567e43bfdd884a3e2a4d084701229a1`  
		Last Modified: Thu, 28 Sep 2023 21:59:45 GMT  
		Size: 13.8 MB (13814189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:85dd4fae9241ac3330e98e1d3b052d36b7ecbe1cd69b4c860454c84976426e70
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17043239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f78b426118e91fcb43786aa4c3003cd91ee86ab5f896516a885f964056b08cae`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:19:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 23:19:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 23:19:20 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 23:19:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 23:19:24 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 23:19:24 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 80
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 443
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 23:19:25 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 23:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66901ba48d0ee53cd827f4eb2cfd8b049cebba8c3d307b69760e1be917f69476`  
		Last Modified: Thu, 28 Sep 2023 23:19:46 GMT  
		Size: 344.4 KB (344448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dddeb3f6febb36993d8a51ad919784fd152aab5f6e17fe00d579916f32e42911`  
		Last Modified: Thu, 28 Sep 2023 23:19:46 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f936b2c0499a587b75385edfeb1d22b8f16ed05dca7dd0999ccc0635e1904a`  
		Last Modified: Thu, 28 Sep 2023 23:19:48 GMT  
		Size: 13.8 MB (13791383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:595e5490450c9ed29cc960149e2c265210e8444f3b3ea5ff2fab62d0da5ec3d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17163627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23f8ae4a1af151ac93d2945855095990774bc44f70af5c0e4b058dbb7e8b8c09`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:16:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 29 Sep 2023 01:16:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 29 Sep 2023 01:16:13 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 01:16:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 29 Sep 2023 01:16:15 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 29 Sep 2023 01:16:15 GMT
ENV XDG_DATA_HOME=/data
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 80
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 443
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 443/udp
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 2019
# Fri, 29 Sep 2023 01:16:16 GMT
WORKDIR /srv
# Fri, 29 Sep 2023 01:16:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f21cb0286edf1f5fefb4a859b414a446bb81baa9e8901fc8f4eca55a43aeeec`  
		Last Modified: Fri, 29 Sep 2023 01:16:34 GMT  
		Size: 360.6 KB (360643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5444b3f9419d06a4b77a65935a3b1c6e657c607bcfb9e3bd1abebe57eae36e6a`  
		Last Modified: Fri, 29 Sep 2023 01:16:34 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3485ef64f848b891981d59d52e0b092b261205ad787b38ae389e5ac39eed493f`  
		Last Modified: Fri, 29 Sep 2023 01:16:35 GMT  
		Size: 13.5 MB (13463646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:65084a14a1557b92af5b8ba6fcba9a7a710ed5caef1e2310f9622166608c9531
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16945195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73ba45deaa04c3feac6474c22204ac6f5ebc380b331ff7d585ecd196284459b3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:17:03 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 29 Sep 2023 02:17:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 29 Sep 2023 02:17:06 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 02:17:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 29 Sep 2023 02:17:13 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 29 Sep 2023 02:17:14 GMT
ENV XDG_DATA_HOME=/data
# Fri, 29 Sep 2023 02:17:15 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Fri, 29 Sep 2023 02:17:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 29 Sep 2023 02:17:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 29 Sep 2023 02:17:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 29 Sep 2023 02:17:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 29 Sep 2023 02:17:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 29 Sep 2023 02:17:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 29 Sep 2023 02:17:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 29 Sep 2023 02:17:21 GMT
EXPOSE 80
# Fri, 29 Sep 2023 02:17:21 GMT
EXPOSE 443
# Fri, 29 Sep 2023 02:17:22 GMT
EXPOSE 443/udp
# Fri, 29 Sep 2023 02:17:22 GMT
EXPOSE 2019
# Fri, 29 Sep 2023 02:17:24 GMT
WORKDIR /srv
# Fri, 29 Sep 2023 02:17:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa65cea7f5d70d1e203b851e43ad676e92f28c930ad32b6691e84ff9b5cda87`  
		Last Modified: Fri, 29 Sep 2023 02:18:03 GMT  
		Size: 362.2 KB (362182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7089a1d537371e29a65d106f43b45f2a0367d4d1db0eb7d6b7099f8ba05645`  
		Last Modified: Fri, 29 Sep 2023 02:18:01 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b93ab741fa6270144ea59d6a5fa3c4138286a569f246fdccd829b317b051f3a`  
		Last Modified: Fri, 29 Sep 2023 02:18:05 GMT  
		Size: 13.2 MB (13228998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:9e13bd2b56147eecc80f1fe1710e4350ea63d5edfb389fa89e2c6de06c08593a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17721238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2f0101e0f893afb763d99b2050dbf4d68a44aae29785af6c05af5a552b0c1a7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:19:38 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 22:19:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 22:19:39 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 22:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 22:19:42 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 22:19:42 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 80
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 443
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 22:19:44 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 22:19:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed3df874173df47ad0bd0ef67b8ee598c77921810d84a67fd2984c4f8151c91`  
		Last Modified: Thu, 28 Sep 2023 22:20:14 GMT  
		Size: 354.9 KB (354948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95a69c42a5c7fc6d73c00c7f6eb68522f3881aae55db4f85a8400e83b678b181`  
		Last Modified: Thu, 28 Sep 2023 22:20:14 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793016dc78c9794c627c07afcd2fb34af4ee470ee7fef1a1596eff0c59ba6659`  
		Last Modified: Thu, 28 Sep 2023 22:20:16 GMT  
		Size: 14.1 MB (14143684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:33050f2d060171a04ef015097c2c431bebbef8e878f3d53db4adf2b93862e11d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4851; amd64
	-	windows version 10.0.20348.1970; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:1feb6492b7349402a4e1183682415d3a06e2c50998e55e05a23a7ff54104f12e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76961764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b60574c0fd570f746bcbc19dbe40382acf64d8088c9ec08e4e3ffe8e45f1f41`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:54:30 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:54:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:54:31 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 22:54:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 22:54:41 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 22:54:41 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 22:54:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:54:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 22:54:42 GMT
WORKDIR /go
# Fri, 29 Sep 2023 03:34:26 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Fri, 29 Sep 2023 03:34:26 GMT
ENV XCADDY_VERSION=v0.3.5
# Fri, 29 Sep 2023 03:34:26 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 03:34:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 29 Sep 2023 03:34:26 GMT
ENV XCADDY_SETCAP=1
# Fri, 29 Sep 2023 03:34:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 29 Sep 2023 03:34:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 29 Sep 2023 03:34:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc37b24bb09971feb8bf4882e861bce9db0c985a16a900adb0dc9de3f854243b`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 284.7 KB (284690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94517ad51c70c15adb540d431b757078be8f6214a2f1d2181afc9454fa65d281`  
		Last Modified: Thu, 28 Sep 2023 22:57:25 GMT  
		Size: 67.0 MB (67001967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2087470b845b2224ab3a61dafcdf2abbf9540f77be63368c3346b85ad2969fa6`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2981d490d3f8070423e8c669473d70f16909bf20541abd01afb263f326ce67c2`  
		Last Modified: Fri, 29 Sep 2023 03:34:47 GMT  
		Size: 5.0 MB (4970347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5299a94e56556856e0899be99ae303524bf1ef797eb49e7a358611d2d2b3f2`  
		Last Modified: Fri, 29 Sep 2023 03:34:46 GMT  
		Size: 1.3 MB (1302233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965d515814f9dd3e22b51ab0a9ea4f92d693760133d5cf9835588e835635e33d`  
		Last Modified: Fri, 29 Sep 2023 03:34:46 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:de02c3655970e860e68fd2840e08fd9656cebb751cf677a0982e67d8fc5538a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75403016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:636f8b72fc8192d5a346042bbf7f4b91636efcd463c388b6789b3d107346d09d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:55:22 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:55:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:55:22 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 21:55:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 21:55:37 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 21:55:37 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 21:55:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:55:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 21:55:37 GMT
WORKDIR /go
# Thu, 28 Sep 2023 21:59:22 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 28 Sep 2023 21:59:22 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 28 Sep 2023 21:59:22 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 21:59:23 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Sep 2023 21:59:23 GMT
ENV XCADDY_SETCAP=1
# Thu, 28 Sep 2023 21:59:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Sep 2023 21:59:24 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Sep 2023 21:59:24 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3da3b9e7a12f6bb6b7f56e9240c2c92ce8c9f5fd5ef3b3063b9a93d454919e`  
		Last Modified: Thu, 28 Sep 2023 21:58:05 GMT  
		Size: 284.9 KB (284887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db471c20f6642596c4a4eeca4a9348dd5a897aa1c3c2383fdf2fe2c2d6f1628`  
		Last Modified: Thu, 28 Sep 2023 21:58:18 GMT  
		Size: 65.8 MB (65758212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037298c7b9748af97a3a2906d0ebb91f2dd588f633a9e8f94e2e2b2a571ead1f`  
		Last Modified: Thu, 28 Sep 2023 21:58:05 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc923fd6dd565567ed402508a7420812a84f61bbecfa0e1f988bd9b2d7b772b`  
		Last Modified: Thu, 28 Sep 2023 22:00:17 GMT  
		Size: 5.0 MB (4965415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b055d2dc5239a960f27dc6b7a7dcbe9455defa55bfb2f41d11678f8d56591668`  
		Last Modified: Thu, 28 Sep 2023 22:00:17 GMT  
		Size: 1.2 MB (1248652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513967d31b50a4e0f6dd90e6b95fe92f327bab78e463b9ed3a5ab386b0796a0e`  
		Last Modified: Thu, 28 Sep 2023 22:00:16 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0ad7a5fed30df59cfe78f87f33dd741fcf2f9588b879cf4a999db785e17ce566
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74701068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e079a52ac41cfb0c167d0940a0ed4a65fac94f7728283be07ef1f9a9661f0cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:15:15 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:15:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:15:15 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 22:15:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 22:15:32 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 22:15:32 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 22:15:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:15:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 22:15:33 GMT
WORKDIR /go
# Thu, 28 Sep 2023 23:19:29 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 28 Sep 2023 23:19:30 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 28 Sep 2023 23:19:30 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 23:19:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Sep 2023 23:19:30 GMT
ENV XCADDY_SETCAP=1
# Thu, 28 Sep 2023 23:19:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Sep 2023 23:19:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Sep 2023 23:19:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e0aec75477c9a2cf6993e068fa40a45f0684d622ece61f54e6e02f9adebeb8`  
		Last Modified: Thu, 28 Sep 2023 22:19:29 GMT  
		Size: 284.1 KB (284076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b5f8bc58ed201378ca797f82d516632d7a864a26eb9f29c4314f061c253a5d`  
		Last Modified: Thu, 28 Sep 2023 22:19:45 GMT  
		Size: 65.8 MB (65758178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f7cae270f0f74f4af87304330243fa68170426cfac2ed3042885f518bd97fb`  
		Last Modified: Thu, 28 Sep 2023 22:19:29 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eda060e9fe56bc05ae87a1f04e06d4aa8e1b59f3143db70491a8b212f53eceb`  
		Last Modified: Thu, 28 Sep 2023 23:20:02 GMT  
		Size: 4.5 MB (4512263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56d31be6b7b9ec4232229a322a3e283089e9524392a0c2317b6870571a1f366`  
		Last Modified: Thu, 28 Sep 2023 23:20:01 GMT  
		Size: 1.2 MB (1246086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a8990e3e6f77162545c3d58676a3cded2b3260baa61c1c27f8255bb9afb3ba`  
		Last Modified: Thu, 28 Sep 2023 23:20:01 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:af47b965d6c7ddd0a5c0691ee19821ebec47fd96c8ceeb01ad0d12b2024be158
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73995021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf00a9d5850ec2c2a9fb5239a41e1f452b6798d56f52c5dcf8063e9bb8685055`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:03:38 GMT
RUN apk add --no-cache ca-certificates
# Fri, 29 Sep 2023 01:40:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Sep 2023 01:40:17 GMT
ENV GOLANG_VERSION=1.21.1
# Fri, 29 Sep 2023 01:40:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 29 Sep 2023 01:40:27 GMT
ENV GOTOOLCHAIN=local
# Fri, 29 Sep 2023 01:40:27 GMT
ENV GOPATH=/go
# Fri, 29 Sep 2023 01:40:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Sep 2023 01:40:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Fri, 29 Sep 2023 01:40:28 GMT
WORKDIR /go
# Fri, 29 Sep 2023 04:34:55 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Fri, 29 Sep 2023 04:34:55 GMT
ENV XCADDY_VERSION=v0.3.5
# Fri, 29 Sep 2023 04:34:55 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 04:34:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 29 Sep 2023 04:34:56 GMT
ENV XCADDY_SETCAP=1
# Fri, 29 Sep 2023 04:34:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 29 Sep 2023 04:34:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 29 Sep 2023 04:34:57 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c21914ef412ef71f6092299b025bf4d504a49024701bf684bc9efd218155c63`  
		Last Modified: Fri, 29 Sep 2023 01:03:48 GMT  
		Size: 286.3 KB (286306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5340c63a94930ed08fa6eea6fd627bdb38f335952054831c49716a27a8c8dfa0`  
		Last Modified: Fri, 29 Sep 2023 01:42:20 GMT  
		Size: 64.1 MB (64108807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3ca664c3732429a52e8e77a07dc94297fce7c851529dd6a572983f0bf99ae1`  
		Last Modified: Fri, 29 Sep 2023 01:42:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63283848834a5104fc3043f65de33b90d451c46dfbb2fa91874f41c1f0fcbdf2`  
		Last Modified: Fri, 29 Sep 2023 04:35:13 GMT  
		Size: 5.1 MB (5069067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a59c9f8a01ff922ae6c69e34038c2eb56dcc3bf0e7bc786804f9cabda360ec`  
		Last Modified: Fri, 29 Sep 2023 04:35:12 GMT  
		Size: 1.2 MB (1198450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a52b5eedc76b0958663cbb9be6e5ac8eaa51dff9778a4b4cff667120ab6da12`  
		Last Modified: Fri, 29 Sep 2023 04:35:12 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:55d9b4418c520166c8863db2e2993557191bf9caf6e028f7b04a5b8ab1b63a73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74205796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a71360173a10dc6951ba63109fda1b23d9e5356b14225bf346845fa455513541`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:13:11 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:13:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:13:12 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 22:13:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 22:13:47 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 22:13:48 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 22:13:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:13:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 22:13:52 GMT
WORKDIR /go
# Fri, 29 Sep 2023 02:17:36 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Fri, 29 Sep 2023 02:17:37 GMT
ENV XCADDY_VERSION=v0.3.5
# Fri, 29 Sep 2023 02:17:37 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 02:17:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 29 Sep 2023 02:17:38 GMT
ENV XCADDY_SETCAP=1
# Fri, 29 Sep 2023 02:17:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 29 Sep 2023 02:17:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 29 Sep 2023 02:17:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc67971d1767eae5019ffeaf8f893e6d81dbba50bde347da0c0433c56e3f2a3`  
		Last Modified: Thu, 28 Sep 2023 22:18:17 GMT  
		Size: 286.7 KB (286659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a20f495e184de0c46bb781c57dd99e2cfc30deaa14db48a8f0cc95fc20ed28b`  
		Last Modified: Thu, 28 Sep 2023 22:18:37 GMT  
		Size: 64.1 MB (64116623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9a2fd37dab154ff5a7a7f14553c32641833c766ad5fb9ab737767a24048145`  
		Last Modified: Thu, 28 Sep 2023 22:18:16 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f689a2a610338f9a37a48fa810fa16f44dc7777786d0ed4b2df7e7e4e01cb38`  
		Last Modified: Fri, 29 Sep 2023 02:18:20 GMT  
		Size: 5.3 MB (5269263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322aacb09420bf02551659cc5b56c905f8fc7944553e6c3b1c85b5eb92547d7f`  
		Last Modified: Fri, 29 Sep 2023 02:18:20 GMT  
		Size: 1.2 MB (1186183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490b3f0289dc37c4f918f9f29f48774d57525c152a6ee4708b66c38798b2421c`  
		Last Modified: Fri, 29 Sep 2023 02:18:19 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:b438b3cf1ad85b0cc2fe8f5319ac062a52640a6a231f4858917e081b1e773001
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76102753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1788e10f8a6f8ccdc56c8b2c4b5a6ebc9387eb3b66b2b9d2dd1f18b74223f3c2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:38:54 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:38:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:38:54 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 21:39:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 21:39:15 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 21:39:15 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 21:39:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:39:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 21:39:15 GMT
WORKDIR /go
# Thu, 28 Sep 2023 22:19:51 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 28 Sep 2023 22:19:51 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_SETCAP=1
# Thu, 28 Sep 2023 22:19:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Sep 2023 22:19:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Sep 2023 22:19:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0721f16693d4788a5add1bd0b22764c8887cdc62b24edf388ae895df440f4aa9`  
		Last Modified: Thu, 28 Sep 2023 21:46:22 GMT  
		Size: 285.1 KB (285095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40248878cac53fafdd0778844ffa03633e8f3cd73c5d5136e02da42557cb26f6`  
		Last Modified: Thu, 28 Sep 2023 21:46:16 GMT  
		Size: 66.2 MB (66224373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3d28e3790630932107b3adf42c8b1564c57d0ab97f15a759b1a8f835ee4101`  
		Last Modified: Thu, 28 Sep 2023 21:46:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d382e103bfc732fc0a4c2b972100a5426b9a8e99cd21d22eddb196e5bb029206`  
		Last Modified: Thu, 28 Sep 2023 22:20:30 GMT  
		Size: 5.1 MB (5115228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3232faabff7e982d010fd0c3775d8c4a6b80e55bc3acdb0af1e63077c07656`  
		Last Modified: Thu, 28 Sep 2023 22:20:30 GMT  
		Size: 1.3 MB (1262392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff69fb680d5cc18f0d5150ac6c2922176848b00c8456922df5843f6e1c993cc7`  
		Last Modified: Thu, 28 Sep 2023 22:20:29 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.4851; amd64

```console
$ docker pull caddy@sha256:95c666eeefee6beeed59b530714de1ebdd28f2ba6ad0703b37f26b729f5e3793
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2113168904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9bf61498c4479dace7e2fa1c8c4c29a0a0722e06138f3d5fa9226287d83f2d6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 01:39:14 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Sep 2023 01:39:15 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Sep 2023 01:39:16 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Sep 2023 01:39:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Sep 2023 01:40:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:40:50 GMT
ENV GOPATH=C:\go
# Wed, 13 Sep 2023 01:41:53 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Sep 2023 01:41:54 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 13 Sep 2023 01:45:02 GMT
RUN $url = 'https://dl.google.com/go/go1.21.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '10a4f5b63215d11d1770453733dbcbf024f3f74872f84e28d7ea59f0250316c6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:45:04 GMT
WORKDIR C:\go
# Wed, 13 Sep 2023 05:35:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:35:07 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 13 Sep 2023 05:35:07 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:35:08 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Sep 2023 05:36:24 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Sep 2023 05:36:25 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cdfacf538899a08fcbb1c6b92df02725dbfcc05c593d6f310371baf9cc5c28b`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaa9f7bc4f06074cd41e4c8f38f9019d00b30116cc81e7e57bb201a2cddbe76`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa369f25c61f03e75b9090231c21b059562345a9aa5b4710c1d4bd043232a46`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1338c790efe798520cb633291aa3dbf3b37552cfbd91737d2539bad7bcac882c`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af230316f5f5bdfd37af05e436ffaadf28ac7a31d97f315dbfb2924c4d1ca3c`  
		Last Modified: Wed, 13 Sep 2023 02:16:54 GMT  
		Size: 25.6 MB (25567707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606d89c5df48922aee4ed7b88afc9f9fc270b462891c28d20b75199f2726201e`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f90ec51ca481c33d4e3887adf74f8b37c2f82af9e60290d2755f34c55b70e9c`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 220.5 KB (220461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9741d5460d3c8c14c62fd6990864968f75fbb895dfd099803a72c140739264b`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac37fd27ee4a5046c706042d53bb4a5b5e2e9ac0ec76a27142f42a55f09c31aa`  
		Last Modified: Wed, 13 Sep 2023 02:17:12 GMT  
		Size: 69.3 MB (69345076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4460c6474f9af5dc17adefba85607fa63b6072fc39250bcf433f458742fd0987`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 1.6 KB (1559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8840f55013cb306bc30661534c9618bdfda370c585b638deb791ba84fbceee9c`  
		Last Modified: Wed, 13 Sep 2023 05:38:30 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f45db9ea611a79882cee37d8b10da3ddf761d7f9ae24bf1fe0cfdb58497a6ae`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51195ebf7ad1d0ac3972b387896050e20749e6e0bb65d49a1907f49ab5cec5f2`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56989aaa5684bbc2d72ae4bb645d01d4dd0c63d35c8f4515b4c8587d6611d519`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae11f7d16342cb14a92f5b67ee9ce0eeab5805f76829bedd3735c0eec9b1f744`  
		Last Modified: Wed, 13 Sep 2023 05:38:29 GMT  
		Size: 1.7 MB (1687175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f520ac11e32bd8e755e12beaef19d397e709b5d8b007fb948658b974af6c7e2`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.20348.1970; amd64

```console
$ docker pull caddy@sha256:0a56e01d98805d99f891740e4644f1afb62f725060c36ad3cdcad27f452c3952
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1934132962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f26855783f570cd07fa203aa143ae0ddab1ef24e3a100e66f3cac124f008c0e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 01:35:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 01:35:30 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Sep 2023 01:35:31 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Sep 2023 01:35:32 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Sep 2023 01:35:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Sep 2023 01:36:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:36:16 GMT
ENV GOPATH=C:\go
# Wed, 13 Sep 2023 01:36:38 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Sep 2023 01:36:39 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 13 Sep 2023 01:38:59 GMT
RUN $url = 'https://dl.google.com/go/go1.21.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '10a4f5b63215d11d1770453733dbcbf024f3f74872f84e28d7ea59f0250316c6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:39:01 GMT
WORKDIR C:\go
# Wed, 13 Sep 2023 05:36:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:36:35 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 13 Sep 2023 05:36:35 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:36:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Sep 2023 05:37:04 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Sep 2023 05:37:05 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f40969dbf1e035a6c49e7c40b216960e3ee98ec3b76f76f9fe4498d0110bee`  
		Last Modified: Wed, 13 Sep 2023 02:15:22 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a846e03791bc3a58cfed3f02e65f87e18a5f5f416405456368e8a0ec4f9364`  
		Last Modified: Wed, 13 Sep 2023 02:15:21 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bc2015fc36cda903dca8edfdc1c87b219753af24c4ff5a95db324fb0e1cc0c`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d1910b6e6c60b5b71a12c43af94e08cf0ba20718d9a6c16ad07734f4977311`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46353fb4c6176aee49921617b1cd3ac7dcbca49d4d7a734cb5ddef177b8354b2`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f70d11added5b27b9707831ac76b04e95d4fa92b406f09532472fa350df630`  
		Last Modified: Wed, 13 Sep 2023 02:15:25 GMT  
		Size: 25.6 MB (25551011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892bff3fc5428691c1922057d675611c2b50e50cf3c6d22c2054b270861bc53c`  
		Last Modified: Wed, 13 Sep 2023 02:15:17 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ee07c029ab53a292bbb7320390d24d86b21159530b1b77d968b2b5416e8f67`  
		Last Modified: Wed, 13 Sep 2023 02:15:18 GMT  
		Size: 277.5 KB (277484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02fba082f03e26936264b99820372415048914f7ffd7f2469a28d3c0edd9224d`  
		Last Modified: Wed, 13 Sep 2023 02:15:17 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5004044396790144a82fbe98df119c5d7ae1a9abaac51c4cf0813b0d43f3f58`  
		Last Modified: Wed, 13 Sep 2023 02:15:43 GMT  
		Size: 69.3 MB (69336704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d84e4497229ea334095327a0106b2812e1dd5261c636cb1461fd698efffc4b6`  
		Last Modified: Wed, 13 Sep 2023 02:15:17 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20bad1e33f8c7089f46cd563d46ed621e589ef95c6dd41ba7569e5649804f136`  
		Last Modified: Wed, 13 Sep 2023 05:38:48 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c872ac2c7792d27826114f417d42ecbf945599d2b446775726d828ee99aab2c0`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6aff62b7b35fb324b51b0049e8a19ba51736b4f6ba1bfd92511f117e51e794`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77347ece80c37436fa82eb033a03166eb1c797e7341a6b642bf3bb80c12e36d5`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d1c7afb782c38442247cae60bbf9b16689939a03c80d4394125a9ff0af783c`  
		Last Modified: Wed, 13 Sep 2023 05:38:47 GMT  
		Size: 1.7 MB (1675830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191cef90893a643b034d031ee3e41cd4daa1b59c1d2d0e2dc1640f7bedb6c55a`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:308ffbaa017c0bb533cfe7442c49460b33193a43192b2bb9744a0fa7080a50c3
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
$ docker pull caddy@sha256:1feb6492b7349402a4e1183682415d3a06e2c50998e55e05a23a7ff54104f12e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76961764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b60574c0fd570f746bcbc19dbe40382acf64d8088c9ec08e4e3ffe8e45f1f41`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:54:30 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:54:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:54:31 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 22:54:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 22:54:41 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 22:54:41 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 22:54:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:54:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 22:54:42 GMT
WORKDIR /go
# Fri, 29 Sep 2023 03:34:26 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Fri, 29 Sep 2023 03:34:26 GMT
ENV XCADDY_VERSION=v0.3.5
# Fri, 29 Sep 2023 03:34:26 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 03:34:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 29 Sep 2023 03:34:26 GMT
ENV XCADDY_SETCAP=1
# Fri, 29 Sep 2023 03:34:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 29 Sep 2023 03:34:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 29 Sep 2023 03:34:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc37b24bb09971feb8bf4882e861bce9db0c985a16a900adb0dc9de3f854243b`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 284.7 KB (284690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94517ad51c70c15adb540d431b757078be8f6214a2f1d2181afc9454fa65d281`  
		Last Modified: Thu, 28 Sep 2023 22:57:25 GMT  
		Size: 67.0 MB (67001967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2087470b845b2224ab3a61dafcdf2abbf9540f77be63368c3346b85ad2969fa6`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2981d490d3f8070423e8c669473d70f16909bf20541abd01afb263f326ce67c2`  
		Last Modified: Fri, 29 Sep 2023 03:34:47 GMT  
		Size: 5.0 MB (4970347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5299a94e56556856e0899be99ae303524bf1ef797eb49e7a358611d2d2b3f2`  
		Last Modified: Fri, 29 Sep 2023 03:34:46 GMT  
		Size: 1.3 MB (1302233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965d515814f9dd3e22b51ab0a9ea4f92d693760133d5cf9835588e835635e33d`  
		Last Modified: Fri, 29 Sep 2023 03:34:46 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:de02c3655970e860e68fd2840e08fd9656cebb751cf677a0982e67d8fc5538a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75403016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:636f8b72fc8192d5a346042bbf7f4b91636efcd463c388b6789b3d107346d09d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:55:22 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:55:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:55:22 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 21:55:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 21:55:37 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 21:55:37 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 21:55:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:55:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 21:55:37 GMT
WORKDIR /go
# Thu, 28 Sep 2023 21:59:22 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 28 Sep 2023 21:59:22 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 28 Sep 2023 21:59:22 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 21:59:23 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Sep 2023 21:59:23 GMT
ENV XCADDY_SETCAP=1
# Thu, 28 Sep 2023 21:59:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Sep 2023 21:59:24 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Sep 2023 21:59:24 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3da3b9e7a12f6bb6b7f56e9240c2c92ce8c9f5fd5ef3b3063b9a93d454919e`  
		Last Modified: Thu, 28 Sep 2023 21:58:05 GMT  
		Size: 284.9 KB (284887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db471c20f6642596c4a4eeca4a9348dd5a897aa1c3c2383fdf2fe2c2d6f1628`  
		Last Modified: Thu, 28 Sep 2023 21:58:18 GMT  
		Size: 65.8 MB (65758212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037298c7b9748af97a3a2906d0ebb91f2dd588f633a9e8f94e2e2b2a571ead1f`  
		Last Modified: Thu, 28 Sep 2023 21:58:05 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc923fd6dd565567ed402508a7420812a84f61bbecfa0e1f988bd9b2d7b772b`  
		Last Modified: Thu, 28 Sep 2023 22:00:17 GMT  
		Size: 5.0 MB (4965415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b055d2dc5239a960f27dc6b7a7dcbe9455defa55bfb2f41d11678f8d56591668`  
		Last Modified: Thu, 28 Sep 2023 22:00:17 GMT  
		Size: 1.2 MB (1248652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513967d31b50a4e0f6dd90e6b95fe92f327bab78e463b9ed3a5ab386b0796a0e`  
		Last Modified: Thu, 28 Sep 2023 22:00:16 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0ad7a5fed30df59cfe78f87f33dd741fcf2f9588b879cf4a999db785e17ce566
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74701068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e079a52ac41cfb0c167d0940a0ed4a65fac94f7728283be07ef1f9a9661f0cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:15:15 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:15:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:15:15 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 22:15:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 22:15:32 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 22:15:32 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 22:15:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:15:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 22:15:33 GMT
WORKDIR /go
# Thu, 28 Sep 2023 23:19:29 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 28 Sep 2023 23:19:30 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 28 Sep 2023 23:19:30 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 23:19:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Sep 2023 23:19:30 GMT
ENV XCADDY_SETCAP=1
# Thu, 28 Sep 2023 23:19:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Sep 2023 23:19:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Sep 2023 23:19:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e0aec75477c9a2cf6993e068fa40a45f0684d622ece61f54e6e02f9adebeb8`  
		Last Modified: Thu, 28 Sep 2023 22:19:29 GMT  
		Size: 284.1 KB (284076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b5f8bc58ed201378ca797f82d516632d7a864a26eb9f29c4314f061c253a5d`  
		Last Modified: Thu, 28 Sep 2023 22:19:45 GMT  
		Size: 65.8 MB (65758178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f7cae270f0f74f4af87304330243fa68170426cfac2ed3042885f518bd97fb`  
		Last Modified: Thu, 28 Sep 2023 22:19:29 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eda060e9fe56bc05ae87a1f04e06d4aa8e1b59f3143db70491a8b212f53eceb`  
		Last Modified: Thu, 28 Sep 2023 23:20:02 GMT  
		Size: 4.5 MB (4512263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56d31be6b7b9ec4232229a322a3e283089e9524392a0c2317b6870571a1f366`  
		Last Modified: Thu, 28 Sep 2023 23:20:01 GMT  
		Size: 1.2 MB (1246086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a8990e3e6f77162545c3d58676a3cded2b3260baa61c1c27f8255bb9afb3ba`  
		Last Modified: Thu, 28 Sep 2023 23:20:01 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:af47b965d6c7ddd0a5c0691ee19821ebec47fd96c8ceeb01ad0d12b2024be158
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73995021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf00a9d5850ec2c2a9fb5239a41e1f452b6798d56f52c5dcf8063e9bb8685055`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:03:38 GMT
RUN apk add --no-cache ca-certificates
# Fri, 29 Sep 2023 01:40:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Sep 2023 01:40:17 GMT
ENV GOLANG_VERSION=1.21.1
# Fri, 29 Sep 2023 01:40:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 29 Sep 2023 01:40:27 GMT
ENV GOTOOLCHAIN=local
# Fri, 29 Sep 2023 01:40:27 GMT
ENV GOPATH=/go
# Fri, 29 Sep 2023 01:40:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Sep 2023 01:40:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Fri, 29 Sep 2023 01:40:28 GMT
WORKDIR /go
# Fri, 29 Sep 2023 04:34:55 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Fri, 29 Sep 2023 04:34:55 GMT
ENV XCADDY_VERSION=v0.3.5
# Fri, 29 Sep 2023 04:34:55 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 04:34:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 29 Sep 2023 04:34:56 GMT
ENV XCADDY_SETCAP=1
# Fri, 29 Sep 2023 04:34:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 29 Sep 2023 04:34:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 29 Sep 2023 04:34:57 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c21914ef412ef71f6092299b025bf4d504a49024701bf684bc9efd218155c63`  
		Last Modified: Fri, 29 Sep 2023 01:03:48 GMT  
		Size: 286.3 KB (286306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5340c63a94930ed08fa6eea6fd627bdb38f335952054831c49716a27a8c8dfa0`  
		Last Modified: Fri, 29 Sep 2023 01:42:20 GMT  
		Size: 64.1 MB (64108807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3ca664c3732429a52e8e77a07dc94297fce7c851529dd6a572983f0bf99ae1`  
		Last Modified: Fri, 29 Sep 2023 01:42:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63283848834a5104fc3043f65de33b90d451c46dfbb2fa91874f41c1f0fcbdf2`  
		Last Modified: Fri, 29 Sep 2023 04:35:13 GMT  
		Size: 5.1 MB (5069067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a59c9f8a01ff922ae6c69e34038c2eb56dcc3bf0e7bc786804f9cabda360ec`  
		Last Modified: Fri, 29 Sep 2023 04:35:12 GMT  
		Size: 1.2 MB (1198450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a52b5eedc76b0958663cbb9be6e5ac8eaa51dff9778a4b4cff667120ab6da12`  
		Last Modified: Fri, 29 Sep 2023 04:35:12 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:55d9b4418c520166c8863db2e2993557191bf9caf6e028f7b04a5b8ab1b63a73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74205796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a71360173a10dc6951ba63109fda1b23d9e5356b14225bf346845fa455513541`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:13:11 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:13:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:13:12 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 22:13:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 22:13:47 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 22:13:48 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 22:13:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:13:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 22:13:52 GMT
WORKDIR /go
# Fri, 29 Sep 2023 02:17:36 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Fri, 29 Sep 2023 02:17:37 GMT
ENV XCADDY_VERSION=v0.3.5
# Fri, 29 Sep 2023 02:17:37 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 02:17:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 29 Sep 2023 02:17:38 GMT
ENV XCADDY_SETCAP=1
# Fri, 29 Sep 2023 02:17:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 29 Sep 2023 02:17:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 29 Sep 2023 02:17:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc67971d1767eae5019ffeaf8f893e6d81dbba50bde347da0c0433c56e3f2a3`  
		Last Modified: Thu, 28 Sep 2023 22:18:17 GMT  
		Size: 286.7 KB (286659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a20f495e184de0c46bb781c57dd99e2cfc30deaa14db48a8f0cc95fc20ed28b`  
		Last Modified: Thu, 28 Sep 2023 22:18:37 GMT  
		Size: 64.1 MB (64116623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9a2fd37dab154ff5a7a7f14553c32641833c766ad5fb9ab737767a24048145`  
		Last Modified: Thu, 28 Sep 2023 22:18:16 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f689a2a610338f9a37a48fa810fa16f44dc7777786d0ed4b2df7e7e4e01cb38`  
		Last Modified: Fri, 29 Sep 2023 02:18:20 GMT  
		Size: 5.3 MB (5269263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322aacb09420bf02551659cc5b56c905f8fc7944553e6c3b1c85b5eb92547d7f`  
		Last Modified: Fri, 29 Sep 2023 02:18:20 GMT  
		Size: 1.2 MB (1186183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490b3f0289dc37c4f918f9f29f48774d57525c152a6ee4708b66c38798b2421c`  
		Last Modified: Fri, 29 Sep 2023 02:18:19 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:b438b3cf1ad85b0cc2fe8f5319ac062a52640a6a231f4858917e081b1e773001
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76102753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1788e10f8a6f8ccdc56c8b2c4b5a6ebc9387eb3b66b2b9d2dd1f18b74223f3c2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:38:54 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:38:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:38:54 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 21:39:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 21:39:15 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 21:39:15 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 21:39:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:39:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 21:39:15 GMT
WORKDIR /go
# Thu, 28 Sep 2023 22:19:51 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 28 Sep 2023 22:19:51 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_SETCAP=1
# Thu, 28 Sep 2023 22:19:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Sep 2023 22:19:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Sep 2023 22:19:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0721f16693d4788a5add1bd0b22764c8887cdc62b24edf388ae895df440f4aa9`  
		Last Modified: Thu, 28 Sep 2023 21:46:22 GMT  
		Size: 285.1 KB (285095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40248878cac53fafdd0778844ffa03633e8f3cd73c5d5136e02da42557cb26f6`  
		Last Modified: Thu, 28 Sep 2023 21:46:16 GMT  
		Size: 66.2 MB (66224373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3d28e3790630932107b3adf42c8b1564c57d0ab97f15a759b1a8f835ee4101`  
		Last Modified: Thu, 28 Sep 2023 21:46:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d382e103bfc732fc0a4c2b972100a5426b9a8e99cd21d22eddb196e5bb029206`  
		Last Modified: Thu, 28 Sep 2023 22:20:30 GMT  
		Size: 5.1 MB (5115228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3232faabff7e982d010fd0c3775d8c4a6b80e55bc3acdb0af1e63077c07656`  
		Last Modified: Thu, 28 Sep 2023 22:20:30 GMT  
		Size: 1.3 MB (1262392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff69fb680d5cc18f0d5150ac6c2922176848b00c8456922df5843f6e1c993cc7`  
		Last Modified: Thu, 28 Sep 2023 22:20:29 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:1a9280c29c9c558a4f0870515605df3716ff711eeef8f648d8207f81f3577c8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull caddy@sha256:95c666eeefee6beeed59b530714de1ebdd28f2ba6ad0703b37f26b729f5e3793
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2113168904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9bf61498c4479dace7e2fa1c8c4c29a0a0722e06138f3d5fa9226287d83f2d6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 01:39:14 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Sep 2023 01:39:15 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Sep 2023 01:39:16 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Sep 2023 01:39:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Sep 2023 01:40:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:40:50 GMT
ENV GOPATH=C:\go
# Wed, 13 Sep 2023 01:41:53 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Sep 2023 01:41:54 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 13 Sep 2023 01:45:02 GMT
RUN $url = 'https://dl.google.com/go/go1.21.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '10a4f5b63215d11d1770453733dbcbf024f3f74872f84e28d7ea59f0250316c6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:45:04 GMT
WORKDIR C:\go
# Wed, 13 Sep 2023 05:35:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:35:07 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 13 Sep 2023 05:35:07 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:35:08 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Sep 2023 05:36:24 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Sep 2023 05:36:25 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cdfacf538899a08fcbb1c6b92df02725dbfcc05c593d6f310371baf9cc5c28b`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaa9f7bc4f06074cd41e4c8f38f9019d00b30116cc81e7e57bb201a2cddbe76`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa369f25c61f03e75b9090231c21b059562345a9aa5b4710c1d4bd043232a46`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1338c790efe798520cb633291aa3dbf3b37552cfbd91737d2539bad7bcac882c`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af230316f5f5bdfd37af05e436ffaadf28ac7a31d97f315dbfb2924c4d1ca3c`  
		Last Modified: Wed, 13 Sep 2023 02:16:54 GMT  
		Size: 25.6 MB (25567707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606d89c5df48922aee4ed7b88afc9f9fc270b462891c28d20b75199f2726201e`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f90ec51ca481c33d4e3887adf74f8b37c2f82af9e60290d2755f34c55b70e9c`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 220.5 KB (220461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9741d5460d3c8c14c62fd6990864968f75fbb895dfd099803a72c140739264b`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac37fd27ee4a5046c706042d53bb4a5b5e2e9ac0ec76a27142f42a55f09c31aa`  
		Last Modified: Wed, 13 Sep 2023 02:17:12 GMT  
		Size: 69.3 MB (69345076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4460c6474f9af5dc17adefba85607fa63b6072fc39250bcf433f458742fd0987`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 1.6 KB (1559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8840f55013cb306bc30661534c9618bdfda370c585b638deb791ba84fbceee9c`  
		Last Modified: Wed, 13 Sep 2023 05:38:30 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f45db9ea611a79882cee37d8b10da3ddf761d7f9ae24bf1fe0cfdb58497a6ae`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51195ebf7ad1d0ac3972b387896050e20749e6e0bb65d49a1907f49ab5cec5f2`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56989aaa5684bbc2d72ae4bb645d01d4dd0c63d35c8f4515b4c8587d6611d519`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae11f7d16342cb14a92f5b67ee9ce0eeab5805f76829bedd3735c0eec9b1f744`  
		Last Modified: Wed, 13 Sep 2023 05:38:29 GMT  
		Size: 1.7 MB (1687175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f520ac11e32bd8e755e12beaef19d397e709b5d8b007fb948658b974af6c7e2`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:e27807e1af059f2f978b562de306e9d021538db7c394f3838deb1d734efc29ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1970; amd64

### `caddy:2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1970; amd64

```console
$ docker pull caddy@sha256:0a56e01d98805d99f891740e4644f1afb62f725060c36ad3cdcad27f452c3952
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1934132962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f26855783f570cd07fa203aa143ae0ddab1ef24e3a100e66f3cac124f008c0e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 01:35:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 01:35:30 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Sep 2023 01:35:31 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Sep 2023 01:35:32 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Sep 2023 01:35:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Sep 2023 01:36:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:36:16 GMT
ENV GOPATH=C:\go
# Wed, 13 Sep 2023 01:36:38 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Sep 2023 01:36:39 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 13 Sep 2023 01:38:59 GMT
RUN $url = 'https://dl.google.com/go/go1.21.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '10a4f5b63215d11d1770453733dbcbf024f3f74872f84e28d7ea59f0250316c6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:39:01 GMT
WORKDIR C:\go
# Wed, 13 Sep 2023 05:36:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:36:35 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 13 Sep 2023 05:36:35 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:36:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Sep 2023 05:37:04 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Sep 2023 05:37:05 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f40969dbf1e035a6c49e7c40b216960e3ee98ec3b76f76f9fe4498d0110bee`  
		Last Modified: Wed, 13 Sep 2023 02:15:22 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a846e03791bc3a58cfed3f02e65f87e18a5f5f416405456368e8a0ec4f9364`  
		Last Modified: Wed, 13 Sep 2023 02:15:21 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bc2015fc36cda903dca8edfdc1c87b219753af24c4ff5a95db324fb0e1cc0c`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d1910b6e6c60b5b71a12c43af94e08cf0ba20718d9a6c16ad07734f4977311`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46353fb4c6176aee49921617b1cd3ac7dcbca49d4d7a734cb5ddef177b8354b2`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f70d11added5b27b9707831ac76b04e95d4fa92b406f09532472fa350df630`  
		Last Modified: Wed, 13 Sep 2023 02:15:25 GMT  
		Size: 25.6 MB (25551011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892bff3fc5428691c1922057d675611c2b50e50cf3c6d22c2054b270861bc53c`  
		Last Modified: Wed, 13 Sep 2023 02:15:17 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ee07c029ab53a292bbb7320390d24d86b21159530b1b77d968b2b5416e8f67`  
		Last Modified: Wed, 13 Sep 2023 02:15:18 GMT  
		Size: 277.5 KB (277484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02fba082f03e26936264b99820372415048914f7ffd7f2469a28d3c0edd9224d`  
		Last Modified: Wed, 13 Sep 2023 02:15:17 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5004044396790144a82fbe98df119c5d7ae1a9abaac51c4cf0813b0d43f3f58`  
		Last Modified: Wed, 13 Sep 2023 02:15:43 GMT  
		Size: 69.3 MB (69336704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d84e4497229ea334095327a0106b2812e1dd5261c636cb1461fd698efffc4b6`  
		Last Modified: Wed, 13 Sep 2023 02:15:17 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20bad1e33f8c7089f46cd563d46ed621e589ef95c6dd41ba7569e5649804f136`  
		Last Modified: Wed, 13 Sep 2023 05:38:48 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c872ac2c7792d27826114f417d42ecbf945599d2b446775726d828ee99aab2c0`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6aff62b7b35fb324b51b0049e8a19ba51736b4f6ba1bfd92511f117e51e794`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77347ece80c37436fa82eb033a03166eb1c797e7341a6b642bf3bb80c12e36d5`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d1c7afb782c38442247cae60bbf9b16689939a03c80d4394125a9ff0af783c`  
		Last Modified: Wed, 13 Sep 2023 05:38:47 GMT  
		Size: 1.7 MB (1675830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191cef90893a643b034d031ee3e41cd4daa1b59c1d2d0e2dc1640f7bedb6c55a`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:4e0879a2422f5309c4ed33c36438e076aa198dc89228e2dc8a56369b86fac7a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4851; amd64
	-	windows version 10.0.20348.1970; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.4851; amd64

```console
$ docker pull caddy@sha256:3f230e8c687c5611e74c84c3ec6f7ef7844b3cc3443d9302e9bb778e6210bfe2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2032252342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea189389e39a38d33c2124e3c02e0a9bc2f3168e5605fa8a909e749ac52fc3f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:30:52 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:30:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:32:00 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:32:02 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:32:04 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:32:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:32:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:32:08 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:32:09 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:33:07 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:33:07 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2bc90334de89082943edb24d5f52a3bb36ef134c17a417ba45cc4e122be3b2`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 465.0 KB (465015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba1c9fb8dedf070862eb0526393862bb5a0f2c87a87bc3864b9b24b11af5524`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5249ade277243b1b7f8c198de7d036f2e106b8a679d777b7bfc885af7b9b76`  
		Last Modified: Wed, 13 Sep 2023 05:37:46 GMT  
		Size: 15.2 MB (15176891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224a0aed4c02b4a48f633ac01c40e020d4e8fbc32fe8896d93032f9d72f50cda`  
		Last Modified: Wed, 13 Sep 2023 05:37:42 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fc1c10b7da22b1e9a26f059801a53ce4ce22e7d24ab14ec56d343a806f3bc2`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bd26e7302c16a8d83a8a6b5d9d263b804279f2b4c7d2fcea59a97c1e187648`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f69e667aa7c5e5a21f7d8a8cdd213b9d20a8a0c790dd18fe51d4df9e5b08a7`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e456b9da79a468c972d487e55e3628f8a8917f78948550c359afc891a5ad24a`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bc4af3e90793180c1ed8b8b9ac6866e24a5de16881f363dacf0ecf47396c8`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0289dff328d597d94fcd8612bd4a726573e13f780790744c5c6f4b40b49823`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52ff2438c88a58e8be33368f668557c92bcfdc503bd58025d081c7b88ec88b`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0f1c855afa9fd7bcf5ded632c161f2ff013f4b08f5c233fa3bdf3d13701467`  
		Last Modified: Wed, 13 Sep 2023 05:37:38 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2e0bf79eee4bbd609b5a111793e394f22ad86eb897cf85c6df2c45d9a8d777`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff797288117550c2b80f9a39dd5a04cb449defc2660cf6a7589618b8d3606464`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa0d1665270ae2e22844b2386842b1deab36f8936506db82df0ec69dc72fb84`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c867297eb9d01dfe100695ae10a0c67bd38f2124de0ee7446d1e66b6dede5c06`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee97f69cfbd31f5a098d45934b159384d8e986d860ad3007140beee338aa4533`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b741c4ffade19f3d712c3fb839c3ae7f1ae4e39e5f777a2b24917b5e630d0f86`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 256.7 KB (256675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a415b22709a225227fa7ce65d7767f3f820c7e9e445b0d718dfb68ae2249832`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.20348.1970; amd64

```console
$ docker pull caddy@sha256:76214fe6feb9f96f1c46334c01e1b9d310eb2e745bb08ba4130547b2147f3677
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1853253940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f0e585ea0797bdd13d148afed1e86161022e8cf2a79d11337f9d4dde0a8efe6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 01:35:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:33:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:33:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:34:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:34:25 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:34:26 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:34:27 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:34:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:34:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:34:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:34:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:34:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:34:33 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:34:34 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:34:35 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:34:36 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:34:56 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:34:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f40969dbf1e035a6c49e7c40b216960e3ee98ec3b76f76f9fe4498d0110bee`  
		Last Modified: Wed, 13 Sep 2023 02:15:22 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2d313a26784edb67b74292171891c0393ea119a53238e09150b5b7bc52371f`  
		Last Modified: Wed, 13 Sep 2023 05:38:08 GMT  
		Size: 483.0 KB (482985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb50376a60c42178e92d96a048b0e7f2dbc2cafe73274ab76722cda86fb32ee`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeecad99d9c5b378a623153b24130f8c36442e9a48ef6a48f878c5f585a66bd4`  
		Last Modified: Wed, 13 Sep 2023 05:38:11 GMT  
		Size: 15.2 MB (15183860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6b7a19981a71c15e39afbc3a52ed5f0c065f77c1ccd55a88e5f1b51af88753`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd7340889e9a6bfc8018c7709595b75ef962cf2608d14398ffbc90b90804a04`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7537acdfe48467d248afb6a69dad6bdb09c62617600305d2b2adb8a45ece2f`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf3cb277ba29189d90269123acd401fa787771fb095f2f2ec532be7bba2a025`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64eb5cc4069279b73a665e35bf526fa42558af1a3a71fc13d76913846d96818`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74348cf2ecbfe3a00df246034f9ab755418e8584b24113c9d327fc80cb134829`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa3fef62dce81d37fff2c621b94314d2aa9d0318523407b0a1d7d2b1e079234`  
		Last Modified: Wed, 13 Sep 2023 05:38:04 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d033d5a006e7fa969026194ef48446c840a891ad252f0316d32bc01843f0e4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbef09c0840262b42ba39068c868fc9b353bed78bb7de251e953289149e9a64e`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea46de371cf13fdb02566c79fc3a22c7123bd7c8903d20645b9cfe34f7ca85d4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63cdcd333c2c131733511c6750d4154ea7f097d981934d1dda8944bf2840860`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8259824bfebcdadd0448ccc0a815b7257636f6eb420e7e00216359908281e7b`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51874919dc1cfa2121d50499f839a702c4cd7340e8708e90b2af042e9debba9`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee3a41ffde2d883c73932756f176ba6901eaeb7a680a351a2b476398263cc8`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73e8028e6f79476106af6c347aa4765644a8ed828c5b6c117ee3dcc2e22e1ef`  
		Last Modified: Wed, 13 Sep 2023 05:38:02 GMT  
		Size: 289.2 KB (289194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd87253476a12fff6cbe718338261ef5ec78a1eb19d8e222838e7f96c3100a0`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:2869cf74555da33dba54fe0c70e1e7baf4d8535444766d27f78fdada2c7e8bb8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull caddy@sha256:3f230e8c687c5611e74c84c3ec6f7ef7844b3cc3443d9302e9bb778e6210bfe2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2032252342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea189389e39a38d33c2124e3c02e0a9bc2f3168e5605fa8a909e749ac52fc3f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:30:52 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:30:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:32:00 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:32:02 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:32:04 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:32:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:32:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:32:08 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:32:09 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:33:07 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:33:07 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2bc90334de89082943edb24d5f52a3bb36ef134c17a417ba45cc4e122be3b2`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 465.0 KB (465015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba1c9fb8dedf070862eb0526393862bb5a0f2c87a87bc3864b9b24b11af5524`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5249ade277243b1b7f8c198de7d036f2e106b8a679d777b7bfc885af7b9b76`  
		Last Modified: Wed, 13 Sep 2023 05:37:46 GMT  
		Size: 15.2 MB (15176891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224a0aed4c02b4a48f633ac01c40e020d4e8fbc32fe8896d93032f9d72f50cda`  
		Last Modified: Wed, 13 Sep 2023 05:37:42 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fc1c10b7da22b1e9a26f059801a53ce4ce22e7d24ab14ec56d343a806f3bc2`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bd26e7302c16a8d83a8a6b5d9d263b804279f2b4c7d2fcea59a97c1e187648`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f69e667aa7c5e5a21f7d8a8cdd213b9d20a8a0c790dd18fe51d4df9e5b08a7`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e456b9da79a468c972d487e55e3628f8a8917f78948550c359afc891a5ad24a`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bc4af3e90793180c1ed8b8b9ac6866e24a5de16881f363dacf0ecf47396c8`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0289dff328d597d94fcd8612bd4a726573e13f780790744c5c6f4b40b49823`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52ff2438c88a58e8be33368f668557c92bcfdc503bd58025d081c7b88ec88b`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0f1c855afa9fd7bcf5ded632c161f2ff013f4b08f5c233fa3bdf3d13701467`  
		Last Modified: Wed, 13 Sep 2023 05:37:38 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2e0bf79eee4bbd609b5a111793e394f22ad86eb897cf85c6df2c45d9a8d777`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff797288117550c2b80f9a39dd5a04cb449defc2660cf6a7589618b8d3606464`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa0d1665270ae2e22844b2386842b1deab36f8936506db82df0ec69dc72fb84`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c867297eb9d01dfe100695ae10a0c67bd38f2124de0ee7446d1e66b6dede5c06`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee97f69cfbd31f5a098d45934b159384d8e986d860ad3007140beee338aa4533`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b741c4ffade19f3d712c3fb839c3ae7f1ae4e39e5f777a2b24917b5e630d0f86`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 256.7 KB (256675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a415b22709a225227fa7ce65d7767f3f820c7e9e445b0d718dfb68ae2249832`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:1cf6f6aff1679190ae48af88d1f51c255c42ec58e320d967d97b39c0113fc8f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1970; amd64

### `caddy:2-windowsservercore-ltsc2022` - windows version 10.0.20348.1970; amd64

```console
$ docker pull caddy@sha256:76214fe6feb9f96f1c46334c01e1b9d310eb2e745bb08ba4130547b2147f3677
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1853253940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f0e585ea0797bdd13d148afed1e86161022e8cf2a79d11337f9d4dde0a8efe6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 01:35:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:33:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:33:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:34:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:34:25 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:34:26 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:34:27 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:34:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:34:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:34:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:34:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:34:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:34:33 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:34:34 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:34:35 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:34:36 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:34:56 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:34:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f40969dbf1e035a6c49e7c40b216960e3ee98ec3b76f76f9fe4498d0110bee`  
		Last Modified: Wed, 13 Sep 2023 02:15:22 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2d313a26784edb67b74292171891c0393ea119a53238e09150b5b7bc52371f`  
		Last Modified: Wed, 13 Sep 2023 05:38:08 GMT  
		Size: 483.0 KB (482985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb50376a60c42178e92d96a048b0e7f2dbc2cafe73274ab76722cda86fb32ee`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeecad99d9c5b378a623153b24130f8c36442e9a48ef6a48f878c5f585a66bd4`  
		Last Modified: Wed, 13 Sep 2023 05:38:11 GMT  
		Size: 15.2 MB (15183860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6b7a19981a71c15e39afbc3a52ed5f0c065f77c1ccd55a88e5f1b51af88753`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd7340889e9a6bfc8018c7709595b75ef962cf2608d14398ffbc90b90804a04`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7537acdfe48467d248afb6a69dad6bdb09c62617600305d2b2adb8a45ece2f`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf3cb277ba29189d90269123acd401fa787771fb095f2f2ec532be7bba2a025`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64eb5cc4069279b73a665e35bf526fa42558af1a3a71fc13d76913846d96818`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74348cf2ecbfe3a00df246034f9ab755418e8584b24113c9d327fc80cb134829`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa3fef62dce81d37fff2c621b94314d2aa9d0318523407b0a1d7d2b1e079234`  
		Last Modified: Wed, 13 Sep 2023 05:38:04 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d033d5a006e7fa969026194ef48446c840a891ad252f0316d32bc01843f0e4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbef09c0840262b42ba39068c868fc9b353bed78bb7de251e953289149e9a64e`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea46de371cf13fdb02566c79fc3a22c7123bd7c8903d20645b9cfe34f7ca85d4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63cdcd333c2c131733511c6750d4154ea7f097d981934d1dda8944bf2840860`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8259824bfebcdadd0448ccc0a815b7257636f6eb420e7e00216359908281e7b`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51874919dc1cfa2121d50499f839a702c4cd7340e8708e90b2af042e9debba9`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee3a41ffde2d883c73932756f176ba6901eaeb7a680a351a2b476398263cc8`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73e8028e6f79476106af6c347aa4765644a8ed828c5b6c117ee3dcc2e22e1ef`  
		Last Modified: Wed, 13 Sep 2023 05:38:02 GMT  
		Size: 289.2 KB (289194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd87253476a12fff6cbe718338261ef5ec78a1eb19d8e222838e7f96c3100a0`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7`

```console
$ docker pull caddy@sha256:df239ca80315c8271f9e87a981fb47124831f8b5a7c85970249d2dfd712479a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4851; amd64
	-	windows version 10.0.20348.1970; amd64

### `caddy:2.7` - linux; amd64

```console
$ docker pull caddy@sha256:3d1bf053476f2415b40e728c37e1112ee7551fa154a63d6f62b275c13fea8166
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18364247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a7b2e234b158c1e01eab04f851fc4b1a33296dbaa68c57d11815ee38a3cafaf`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:43:13 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 22:43:15 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 22:43:15 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 22:43:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 22:43:17 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 22:43:17 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 22:43:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 22:43:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 22:43:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 80
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 443
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 22:43:18 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 22:43:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37be51084fb891c6796079e693b73f6f882266a5e66211344173031e2b0c8ffd`  
		Last Modified: Thu, 28 Sep 2023 22:43:35 GMT  
		Size: 350.8 KB (350826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d867aa37ac50364bf4082dc48c7d4e1b88ead3164d47855e1bbc2ef3678cfc`  
		Last Modified: Thu, 28 Sep 2023 22:43:35 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147aa3899aa3307c28e185f5385015c7a5f15dfa42578a8a8eca88bf2f1e7e3e`  
		Last Modified: Thu, 28 Sep 2023 22:43:37 GMT  
		Size: 14.6 MB (14603949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - linux; arm variant v6

```console
$ docker pull caddy@sha256:239c4a78d1bd0540a44003332119cf019e6ff839f4d303cd9801b1cc9e755ec4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17314598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b41f754b4ebb826dde7fb5c0c3c6048823add70f27a7f9c8d9f8ff1a9636ed2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:59:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 21:59:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 21:59:13 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 21:59:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 21:59:16 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 21:59:16 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 21:59:16 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 21:59:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 21:59:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 80
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 443
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 21:59:17 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 21:59:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1018057a600163b1c1b92c21ade975c631b2f8ccde66d524cfe0ecdac8e1920d`  
		Last Modified: Thu, 28 Sep 2023 21:59:43 GMT  
		Size: 347.6 KB (347613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec54680cbf2cb1a25285c82a7888498ab47d03a68db200a160d7162325a5be19`  
		Last Modified: Thu, 28 Sep 2023 21:59:43 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d087db4282d622690fce98f1d8802151567e43bfdd884a3e2a4d084701229a1`  
		Last Modified: Thu, 28 Sep 2023 21:59:45 GMT  
		Size: 13.8 MB (13814189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - linux; arm variant v7

```console
$ docker pull caddy@sha256:85dd4fae9241ac3330e98e1d3b052d36b7ecbe1cd69b4c860454c84976426e70
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17043239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f78b426118e91fcb43786aa4c3003cd91ee86ab5f896516a885f964056b08cae`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:19:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 23:19:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 23:19:20 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 23:19:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 23:19:24 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 23:19:24 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 80
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 443
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 23:19:25 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 23:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66901ba48d0ee53cd827f4eb2cfd8b049cebba8c3d307b69760e1be917f69476`  
		Last Modified: Thu, 28 Sep 2023 23:19:46 GMT  
		Size: 344.4 KB (344448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dddeb3f6febb36993d8a51ad919784fd152aab5f6e17fe00d579916f32e42911`  
		Last Modified: Thu, 28 Sep 2023 23:19:46 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f936b2c0499a587b75385edfeb1d22b8f16ed05dca7dd0999ccc0635e1904a`  
		Last Modified: Thu, 28 Sep 2023 23:19:48 GMT  
		Size: 13.8 MB (13791383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:595e5490450c9ed29cc960149e2c265210e8444f3b3ea5ff2fab62d0da5ec3d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17163627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23f8ae4a1af151ac93d2945855095990774bc44f70af5c0e4b058dbb7e8b8c09`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:16:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 29 Sep 2023 01:16:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 29 Sep 2023 01:16:13 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 01:16:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 29 Sep 2023 01:16:15 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 29 Sep 2023 01:16:15 GMT
ENV XDG_DATA_HOME=/data
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 80
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 443
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 443/udp
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 2019
# Fri, 29 Sep 2023 01:16:16 GMT
WORKDIR /srv
# Fri, 29 Sep 2023 01:16:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f21cb0286edf1f5fefb4a859b414a446bb81baa9e8901fc8f4eca55a43aeeec`  
		Last Modified: Fri, 29 Sep 2023 01:16:34 GMT  
		Size: 360.6 KB (360643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5444b3f9419d06a4b77a65935a3b1c6e657c607bcfb9e3bd1abebe57eae36e6a`  
		Last Modified: Fri, 29 Sep 2023 01:16:34 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3485ef64f848b891981d59d52e0b092b261205ad787b38ae389e5ac39eed493f`  
		Last Modified: Fri, 29 Sep 2023 01:16:35 GMT  
		Size: 13.5 MB (13463646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - linux; ppc64le

```console
$ docker pull caddy@sha256:65084a14a1557b92af5b8ba6fcba9a7a710ed5caef1e2310f9622166608c9531
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16945195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73ba45deaa04c3feac6474c22204ac6f5ebc380b331ff7d585ecd196284459b3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:17:03 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 29 Sep 2023 02:17:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 29 Sep 2023 02:17:06 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 02:17:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 29 Sep 2023 02:17:13 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 29 Sep 2023 02:17:14 GMT
ENV XDG_DATA_HOME=/data
# Fri, 29 Sep 2023 02:17:15 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Fri, 29 Sep 2023 02:17:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 29 Sep 2023 02:17:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 29 Sep 2023 02:17:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 29 Sep 2023 02:17:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 29 Sep 2023 02:17:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 29 Sep 2023 02:17:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 29 Sep 2023 02:17:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 29 Sep 2023 02:17:21 GMT
EXPOSE 80
# Fri, 29 Sep 2023 02:17:21 GMT
EXPOSE 443
# Fri, 29 Sep 2023 02:17:22 GMT
EXPOSE 443/udp
# Fri, 29 Sep 2023 02:17:22 GMT
EXPOSE 2019
# Fri, 29 Sep 2023 02:17:24 GMT
WORKDIR /srv
# Fri, 29 Sep 2023 02:17:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa65cea7f5d70d1e203b851e43ad676e92f28c930ad32b6691e84ff9b5cda87`  
		Last Modified: Fri, 29 Sep 2023 02:18:03 GMT  
		Size: 362.2 KB (362182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7089a1d537371e29a65d106f43b45f2a0367d4d1db0eb7d6b7099f8ba05645`  
		Last Modified: Fri, 29 Sep 2023 02:18:01 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b93ab741fa6270144ea59d6a5fa3c4138286a569f246fdccd829b317b051f3a`  
		Last Modified: Fri, 29 Sep 2023 02:18:05 GMT  
		Size: 13.2 MB (13228998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - linux; s390x

```console
$ docker pull caddy@sha256:9e13bd2b56147eecc80f1fe1710e4350ea63d5edfb389fa89e2c6de06c08593a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17721238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2f0101e0f893afb763d99b2050dbf4d68a44aae29785af6c05af5a552b0c1a7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:19:38 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 22:19:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 22:19:39 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 22:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 22:19:42 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 22:19:42 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 80
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 443
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 22:19:44 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 22:19:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed3df874173df47ad0bd0ef67b8ee598c77921810d84a67fd2984c4f8151c91`  
		Last Modified: Thu, 28 Sep 2023 22:20:14 GMT  
		Size: 354.9 KB (354948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95a69c42a5c7fc6d73c00c7f6eb68522f3881aae55db4f85a8400e83b678b181`  
		Last Modified: Thu, 28 Sep 2023 22:20:14 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793016dc78c9794c627c07afcd2fb34af4ee470ee7fef1a1596eff0c59ba6659`  
		Last Modified: Thu, 28 Sep 2023 22:20:16 GMT  
		Size: 14.1 MB (14143684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - windows version 10.0.17763.4851; amd64

```console
$ docker pull caddy@sha256:3f230e8c687c5611e74c84c3ec6f7ef7844b3cc3443d9302e9bb778e6210bfe2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2032252342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea189389e39a38d33c2124e3c02e0a9bc2f3168e5605fa8a909e749ac52fc3f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:30:52 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:30:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:32:00 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:32:02 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:32:04 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:32:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:32:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:32:08 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:32:09 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:33:07 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:33:07 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2bc90334de89082943edb24d5f52a3bb36ef134c17a417ba45cc4e122be3b2`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 465.0 KB (465015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba1c9fb8dedf070862eb0526393862bb5a0f2c87a87bc3864b9b24b11af5524`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5249ade277243b1b7f8c198de7d036f2e106b8a679d777b7bfc885af7b9b76`  
		Last Modified: Wed, 13 Sep 2023 05:37:46 GMT  
		Size: 15.2 MB (15176891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224a0aed4c02b4a48f633ac01c40e020d4e8fbc32fe8896d93032f9d72f50cda`  
		Last Modified: Wed, 13 Sep 2023 05:37:42 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fc1c10b7da22b1e9a26f059801a53ce4ce22e7d24ab14ec56d343a806f3bc2`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bd26e7302c16a8d83a8a6b5d9d263b804279f2b4c7d2fcea59a97c1e187648`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f69e667aa7c5e5a21f7d8a8cdd213b9d20a8a0c790dd18fe51d4df9e5b08a7`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e456b9da79a468c972d487e55e3628f8a8917f78948550c359afc891a5ad24a`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bc4af3e90793180c1ed8b8b9ac6866e24a5de16881f363dacf0ecf47396c8`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0289dff328d597d94fcd8612bd4a726573e13f780790744c5c6f4b40b49823`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52ff2438c88a58e8be33368f668557c92bcfdc503bd58025d081c7b88ec88b`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0f1c855afa9fd7bcf5ded632c161f2ff013f4b08f5c233fa3bdf3d13701467`  
		Last Modified: Wed, 13 Sep 2023 05:37:38 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2e0bf79eee4bbd609b5a111793e394f22ad86eb897cf85c6df2c45d9a8d777`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff797288117550c2b80f9a39dd5a04cb449defc2660cf6a7589618b8d3606464`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa0d1665270ae2e22844b2386842b1deab36f8936506db82df0ec69dc72fb84`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c867297eb9d01dfe100695ae10a0c67bd38f2124de0ee7446d1e66b6dede5c06`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee97f69cfbd31f5a098d45934b159384d8e986d860ad3007140beee338aa4533`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b741c4ffade19f3d712c3fb839c3ae7f1ae4e39e5f777a2b24917b5e630d0f86`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 256.7 KB (256675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a415b22709a225227fa7ce65d7767f3f820c7e9e445b0d718dfb68ae2249832`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - windows version 10.0.20348.1970; amd64

```console
$ docker pull caddy@sha256:76214fe6feb9f96f1c46334c01e1b9d310eb2e745bb08ba4130547b2147f3677
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1853253940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f0e585ea0797bdd13d148afed1e86161022e8cf2a79d11337f9d4dde0a8efe6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 01:35:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:33:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:33:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:34:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:34:25 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:34:26 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:34:27 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:34:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:34:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:34:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:34:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:34:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:34:33 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:34:34 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:34:35 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:34:36 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:34:56 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:34:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f40969dbf1e035a6c49e7c40b216960e3ee98ec3b76f76f9fe4498d0110bee`  
		Last Modified: Wed, 13 Sep 2023 02:15:22 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2d313a26784edb67b74292171891c0393ea119a53238e09150b5b7bc52371f`  
		Last Modified: Wed, 13 Sep 2023 05:38:08 GMT  
		Size: 483.0 KB (482985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb50376a60c42178e92d96a048b0e7f2dbc2cafe73274ab76722cda86fb32ee`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeecad99d9c5b378a623153b24130f8c36442e9a48ef6a48f878c5f585a66bd4`  
		Last Modified: Wed, 13 Sep 2023 05:38:11 GMT  
		Size: 15.2 MB (15183860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6b7a19981a71c15e39afbc3a52ed5f0c065f77c1ccd55a88e5f1b51af88753`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd7340889e9a6bfc8018c7709595b75ef962cf2608d14398ffbc90b90804a04`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7537acdfe48467d248afb6a69dad6bdb09c62617600305d2b2adb8a45ece2f`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf3cb277ba29189d90269123acd401fa787771fb095f2f2ec532be7bba2a025`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64eb5cc4069279b73a665e35bf526fa42558af1a3a71fc13d76913846d96818`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74348cf2ecbfe3a00df246034f9ab755418e8584b24113c9d327fc80cb134829`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa3fef62dce81d37fff2c621b94314d2aa9d0318523407b0a1d7d2b1e079234`  
		Last Modified: Wed, 13 Sep 2023 05:38:04 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d033d5a006e7fa969026194ef48446c840a891ad252f0316d32bc01843f0e4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbef09c0840262b42ba39068c868fc9b353bed78bb7de251e953289149e9a64e`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea46de371cf13fdb02566c79fc3a22c7123bd7c8903d20645b9cfe34f7ca85d4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63cdcd333c2c131733511c6750d4154ea7f097d981934d1dda8944bf2840860`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8259824bfebcdadd0448ccc0a815b7257636f6eb420e7e00216359908281e7b`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51874919dc1cfa2121d50499f839a702c4cd7340e8708e90b2af042e9debba9`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee3a41ffde2d883c73932756f176ba6901eaeb7a680a351a2b476398263cc8`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73e8028e6f79476106af6c347aa4765644a8ed828c5b6c117ee3dcc2e22e1ef`  
		Last Modified: Wed, 13 Sep 2023 05:38:02 GMT  
		Size: 289.2 KB (289194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd87253476a12fff6cbe718338261ef5ec78a1eb19d8e222838e7f96c3100a0`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-alpine`

```console
$ docker pull caddy@sha256:11ae052d9015105757d19caf86dc51fc14403841f2b65e93fe320f4d0e197385
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
$ docker pull caddy@sha256:3d1bf053476f2415b40e728c37e1112ee7551fa154a63d6f62b275c13fea8166
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18364247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a7b2e234b158c1e01eab04f851fc4b1a33296dbaa68c57d11815ee38a3cafaf`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:43:13 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 22:43:15 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 22:43:15 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 22:43:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 22:43:17 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 22:43:17 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 22:43:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 22:43:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 22:43:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 80
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 443
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 22:43:18 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 22:43:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37be51084fb891c6796079e693b73f6f882266a5e66211344173031e2b0c8ffd`  
		Last Modified: Thu, 28 Sep 2023 22:43:35 GMT  
		Size: 350.8 KB (350826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d867aa37ac50364bf4082dc48c7d4e1b88ead3164d47855e1bbc2ef3678cfc`  
		Last Modified: Thu, 28 Sep 2023 22:43:35 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147aa3899aa3307c28e185f5385015c7a5f15dfa42578a8a8eca88bf2f1e7e3e`  
		Last Modified: Thu, 28 Sep 2023 22:43:37 GMT  
		Size: 14.6 MB (14603949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:239c4a78d1bd0540a44003332119cf019e6ff839f4d303cd9801b1cc9e755ec4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17314598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b41f754b4ebb826dde7fb5c0c3c6048823add70f27a7f9c8d9f8ff1a9636ed2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:59:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 21:59:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 21:59:13 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 21:59:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 21:59:16 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 21:59:16 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 21:59:16 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 21:59:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 21:59:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 80
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 443
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 21:59:17 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 21:59:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1018057a600163b1c1b92c21ade975c631b2f8ccde66d524cfe0ecdac8e1920d`  
		Last Modified: Thu, 28 Sep 2023 21:59:43 GMT  
		Size: 347.6 KB (347613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec54680cbf2cb1a25285c82a7888498ab47d03a68db200a160d7162325a5be19`  
		Last Modified: Thu, 28 Sep 2023 21:59:43 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d087db4282d622690fce98f1d8802151567e43bfdd884a3e2a4d084701229a1`  
		Last Modified: Thu, 28 Sep 2023 21:59:45 GMT  
		Size: 13.8 MB (13814189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:85dd4fae9241ac3330e98e1d3b052d36b7ecbe1cd69b4c860454c84976426e70
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17043239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f78b426118e91fcb43786aa4c3003cd91ee86ab5f896516a885f964056b08cae`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:19:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 23:19:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 23:19:20 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 23:19:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 23:19:24 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 23:19:24 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 80
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 443
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 23:19:25 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 23:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66901ba48d0ee53cd827f4eb2cfd8b049cebba8c3d307b69760e1be917f69476`  
		Last Modified: Thu, 28 Sep 2023 23:19:46 GMT  
		Size: 344.4 KB (344448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dddeb3f6febb36993d8a51ad919784fd152aab5f6e17fe00d579916f32e42911`  
		Last Modified: Thu, 28 Sep 2023 23:19:46 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f936b2c0499a587b75385edfeb1d22b8f16ed05dca7dd0999ccc0635e1904a`  
		Last Modified: Thu, 28 Sep 2023 23:19:48 GMT  
		Size: 13.8 MB (13791383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:595e5490450c9ed29cc960149e2c265210e8444f3b3ea5ff2fab62d0da5ec3d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17163627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23f8ae4a1af151ac93d2945855095990774bc44f70af5c0e4b058dbb7e8b8c09`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:16:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 29 Sep 2023 01:16:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 29 Sep 2023 01:16:13 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 01:16:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 29 Sep 2023 01:16:15 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 29 Sep 2023 01:16:15 GMT
ENV XDG_DATA_HOME=/data
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 80
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 443
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 443/udp
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 2019
# Fri, 29 Sep 2023 01:16:16 GMT
WORKDIR /srv
# Fri, 29 Sep 2023 01:16:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f21cb0286edf1f5fefb4a859b414a446bb81baa9e8901fc8f4eca55a43aeeec`  
		Last Modified: Fri, 29 Sep 2023 01:16:34 GMT  
		Size: 360.6 KB (360643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5444b3f9419d06a4b77a65935a3b1c6e657c607bcfb9e3bd1abebe57eae36e6a`  
		Last Modified: Fri, 29 Sep 2023 01:16:34 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3485ef64f848b891981d59d52e0b092b261205ad787b38ae389e5ac39eed493f`  
		Last Modified: Fri, 29 Sep 2023 01:16:35 GMT  
		Size: 13.5 MB (13463646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:65084a14a1557b92af5b8ba6fcba9a7a710ed5caef1e2310f9622166608c9531
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16945195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73ba45deaa04c3feac6474c22204ac6f5ebc380b331ff7d585ecd196284459b3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:17:03 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 29 Sep 2023 02:17:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 29 Sep 2023 02:17:06 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 02:17:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 29 Sep 2023 02:17:13 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 29 Sep 2023 02:17:14 GMT
ENV XDG_DATA_HOME=/data
# Fri, 29 Sep 2023 02:17:15 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Fri, 29 Sep 2023 02:17:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 29 Sep 2023 02:17:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 29 Sep 2023 02:17:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 29 Sep 2023 02:17:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 29 Sep 2023 02:17:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 29 Sep 2023 02:17:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 29 Sep 2023 02:17:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 29 Sep 2023 02:17:21 GMT
EXPOSE 80
# Fri, 29 Sep 2023 02:17:21 GMT
EXPOSE 443
# Fri, 29 Sep 2023 02:17:22 GMT
EXPOSE 443/udp
# Fri, 29 Sep 2023 02:17:22 GMT
EXPOSE 2019
# Fri, 29 Sep 2023 02:17:24 GMT
WORKDIR /srv
# Fri, 29 Sep 2023 02:17:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa65cea7f5d70d1e203b851e43ad676e92f28c930ad32b6691e84ff9b5cda87`  
		Last Modified: Fri, 29 Sep 2023 02:18:03 GMT  
		Size: 362.2 KB (362182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7089a1d537371e29a65d106f43b45f2a0367d4d1db0eb7d6b7099f8ba05645`  
		Last Modified: Fri, 29 Sep 2023 02:18:01 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b93ab741fa6270144ea59d6a5fa3c4138286a569f246fdccd829b317b051f3a`  
		Last Modified: Fri, 29 Sep 2023 02:18:05 GMT  
		Size: 13.2 MB (13228998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:9e13bd2b56147eecc80f1fe1710e4350ea63d5edfb389fa89e2c6de06c08593a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17721238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2f0101e0f893afb763d99b2050dbf4d68a44aae29785af6c05af5a552b0c1a7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:19:38 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 22:19:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 22:19:39 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 22:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 22:19:42 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 22:19:42 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 80
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 443
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 22:19:44 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 22:19:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed3df874173df47ad0bd0ef67b8ee598c77921810d84a67fd2984c4f8151c91`  
		Last Modified: Thu, 28 Sep 2023 22:20:14 GMT  
		Size: 354.9 KB (354948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95a69c42a5c7fc6d73c00c7f6eb68522f3881aae55db4f85a8400e83b678b181`  
		Last Modified: Thu, 28 Sep 2023 22:20:14 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793016dc78c9794c627c07afcd2fb34af4ee470ee7fef1a1596eff0c59ba6659`  
		Last Modified: Thu, 28 Sep 2023 22:20:16 GMT  
		Size: 14.1 MB (14143684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-builder`

```console
$ docker pull caddy@sha256:33050f2d060171a04ef015097c2c431bebbef8e878f3d53db4adf2b93862e11d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4851; amd64
	-	windows version 10.0.20348.1970; amd64

### `caddy:2.7-builder` - linux; amd64

```console
$ docker pull caddy@sha256:1feb6492b7349402a4e1183682415d3a06e2c50998e55e05a23a7ff54104f12e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76961764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b60574c0fd570f746bcbc19dbe40382acf64d8088c9ec08e4e3ffe8e45f1f41`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:54:30 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:54:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:54:31 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 22:54:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 22:54:41 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 22:54:41 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 22:54:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:54:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 22:54:42 GMT
WORKDIR /go
# Fri, 29 Sep 2023 03:34:26 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Fri, 29 Sep 2023 03:34:26 GMT
ENV XCADDY_VERSION=v0.3.5
# Fri, 29 Sep 2023 03:34:26 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 03:34:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 29 Sep 2023 03:34:26 GMT
ENV XCADDY_SETCAP=1
# Fri, 29 Sep 2023 03:34:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 29 Sep 2023 03:34:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 29 Sep 2023 03:34:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc37b24bb09971feb8bf4882e861bce9db0c985a16a900adb0dc9de3f854243b`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 284.7 KB (284690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94517ad51c70c15adb540d431b757078be8f6214a2f1d2181afc9454fa65d281`  
		Last Modified: Thu, 28 Sep 2023 22:57:25 GMT  
		Size: 67.0 MB (67001967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2087470b845b2224ab3a61dafcdf2abbf9540f77be63368c3346b85ad2969fa6`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2981d490d3f8070423e8c669473d70f16909bf20541abd01afb263f326ce67c2`  
		Last Modified: Fri, 29 Sep 2023 03:34:47 GMT  
		Size: 5.0 MB (4970347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5299a94e56556856e0899be99ae303524bf1ef797eb49e7a358611d2d2b3f2`  
		Last Modified: Fri, 29 Sep 2023 03:34:46 GMT  
		Size: 1.3 MB (1302233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965d515814f9dd3e22b51ab0a9ea4f92d693760133d5cf9835588e835635e33d`  
		Last Modified: Fri, 29 Sep 2023 03:34:46 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:de02c3655970e860e68fd2840e08fd9656cebb751cf677a0982e67d8fc5538a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75403016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:636f8b72fc8192d5a346042bbf7f4b91636efcd463c388b6789b3d107346d09d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:55:22 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:55:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:55:22 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 21:55:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 21:55:37 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 21:55:37 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 21:55:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:55:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 21:55:37 GMT
WORKDIR /go
# Thu, 28 Sep 2023 21:59:22 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 28 Sep 2023 21:59:22 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 28 Sep 2023 21:59:22 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 21:59:23 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Sep 2023 21:59:23 GMT
ENV XCADDY_SETCAP=1
# Thu, 28 Sep 2023 21:59:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Sep 2023 21:59:24 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Sep 2023 21:59:24 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3da3b9e7a12f6bb6b7f56e9240c2c92ce8c9f5fd5ef3b3063b9a93d454919e`  
		Last Modified: Thu, 28 Sep 2023 21:58:05 GMT  
		Size: 284.9 KB (284887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db471c20f6642596c4a4eeca4a9348dd5a897aa1c3c2383fdf2fe2c2d6f1628`  
		Last Modified: Thu, 28 Sep 2023 21:58:18 GMT  
		Size: 65.8 MB (65758212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037298c7b9748af97a3a2906d0ebb91f2dd588f633a9e8f94e2e2b2a571ead1f`  
		Last Modified: Thu, 28 Sep 2023 21:58:05 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc923fd6dd565567ed402508a7420812a84f61bbecfa0e1f988bd9b2d7b772b`  
		Last Modified: Thu, 28 Sep 2023 22:00:17 GMT  
		Size: 5.0 MB (4965415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b055d2dc5239a960f27dc6b7a7dcbe9455defa55bfb2f41d11678f8d56591668`  
		Last Modified: Thu, 28 Sep 2023 22:00:17 GMT  
		Size: 1.2 MB (1248652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513967d31b50a4e0f6dd90e6b95fe92f327bab78e463b9ed3a5ab386b0796a0e`  
		Last Modified: Thu, 28 Sep 2023 22:00:16 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0ad7a5fed30df59cfe78f87f33dd741fcf2f9588b879cf4a999db785e17ce566
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74701068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e079a52ac41cfb0c167d0940a0ed4a65fac94f7728283be07ef1f9a9661f0cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:15:15 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:15:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:15:15 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 22:15:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 22:15:32 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 22:15:32 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 22:15:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:15:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 22:15:33 GMT
WORKDIR /go
# Thu, 28 Sep 2023 23:19:29 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 28 Sep 2023 23:19:30 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 28 Sep 2023 23:19:30 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 23:19:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Sep 2023 23:19:30 GMT
ENV XCADDY_SETCAP=1
# Thu, 28 Sep 2023 23:19:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Sep 2023 23:19:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Sep 2023 23:19:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e0aec75477c9a2cf6993e068fa40a45f0684d622ece61f54e6e02f9adebeb8`  
		Last Modified: Thu, 28 Sep 2023 22:19:29 GMT  
		Size: 284.1 KB (284076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b5f8bc58ed201378ca797f82d516632d7a864a26eb9f29c4314f061c253a5d`  
		Last Modified: Thu, 28 Sep 2023 22:19:45 GMT  
		Size: 65.8 MB (65758178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f7cae270f0f74f4af87304330243fa68170426cfac2ed3042885f518bd97fb`  
		Last Modified: Thu, 28 Sep 2023 22:19:29 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eda060e9fe56bc05ae87a1f04e06d4aa8e1b59f3143db70491a8b212f53eceb`  
		Last Modified: Thu, 28 Sep 2023 23:20:02 GMT  
		Size: 4.5 MB (4512263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56d31be6b7b9ec4232229a322a3e283089e9524392a0c2317b6870571a1f366`  
		Last Modified: Thu, 28 Sep 2023 23:20:01 GMT  
		Size: 1.2 MB (1246086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a8990e3e6f77162545c3d58676a3cded2b3260baa61c1c27f8255bb9afb3ba`  
		Last Modified: Thu, 28 Sep 2023 23:20:01 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:af47b965d6c7ddd0a5c0691ee19821ebec47fd96c8ceeb01ad0d12b2024be158
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73995021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf00a9d5850ec2c2a9fb5239a41e1f452b6798d56f52c5dcf8063e9bb8685055`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:03:38 GMT
RUN apk add --no-cache ca-certificates
# Fri, 29 Sep 2023 01:40:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Sep 2023 01:40:17 GMT
ENV GOLANG_VERSION=1.21.1
# Fri, 29 Sep 2023 01:40:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 29 Sep 2023 01:40:27 GMT
ENV GOTOOLCHAIN=local
# Fri, 29 Sep 2023 01:40:27 GMT
ENV GOPATH=/go
# Fri, 29 Sep 2023 01:40:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Sep 2023 01:40:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Fri, 29 Sep 2023 01:40:28 GMT
WORKDIR /go
# Fri, 29 Sep 2023 04:34:55 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Fri, 29 Sep 2023 04:34:55 GMT
ENV XCADDY_VERSION=v0.3.5
# Fri, 29 Sep 2023 04:34:55 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 04:34:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 29 Sep 2023 04:34:56 GMT
ENV XCADDY_SETCAP=1
# Fri, 29 Sep 2023 04:34:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 29 Sep 2023 04:34:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 29 Sep 2023 04:34:57 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c21914ef412ef71f6092299b025bf4d504a49024701bf684bc9efd218155c63`  
		Last Modified: Fri, 29 Sep 2023 01:03:48 GMT  
		Size: 286.3 KB (286306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5340c63a94930ed08fa6eea6fd627bdb38f335952054831c49716a27a8c8dfa0`  
		Last Modified: Fri, 29 Sep 2023 01:42:20 GMT  
		Size: 64.1 MB (64108807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3ca664c3732429a52e8e77a07dc94297fce7c851529dd6a572983f0bf99ae1`  
		Last Modified: Fri, 29 Sep 2023 01:42:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63283848834a5104fc3043f65de33b90d451c46dfbb2fa91874f41c1f0fcbdf2`  
		Last Modified: Fri, 29 Sep 2023 04:35:13 GMT  
		Size: 5.1 MB (5069067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a59c9f8a01ff922ae6c69e34038c2eb56dcc3bf0e7bc786804f9cabda360ec`  
		Last Modified: Fri, 29 Sep 2023 04:35:12 GMT  
		Size: 1.2 MB (1198450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a52b5eedc76b0958663cbb9be6e5ac8eaa51dff9778a4b4cff667120ab6da12`  
		Last Modified: Fri, 29 Sep 2023 04:35:12 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:55d9b4418c520166c8863db2e2993557191bf9caf6e028f7b04a5b8ab1b63a73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74205796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a71360173a10dc6951ba63109fda1b23d9e5356b14225bf346845fa455513541`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:13:11 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:13:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:13:12 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 22:13:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 22:13:47 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 22:13:48 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 22:13:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:13:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 22:13:52 GMT
WORKDIR /go
# Fri, 29 Sep 2023 02:17:36 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Fri, 29 Sep 2023 02:17:37 GMT
ENV XCADDY_VERSION=v0.3.5
# Fri, 29 Sep 2023 02:17:37 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 02:17:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 29 Sep 2023 02:17:38 GMT
ENV XCADDY_SETCAP=1
# Fri, 29 Sep 2023 02:17:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 29 Sep 2023 02:17:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 29 Sep 2023 02:17:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc67971d1767eae5019ffeaf8f893e6d81dbba50bde347da0c0433c56e3f2a3`  
		Last Modified: Thu, 28 Sep 2023 22:18:17 GMT  
		Size: 286.7 KB (286659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a20f495e184de0c46bb781c57dd99e2cfc30deaa14db48a8f0cc95fc20ed28b`  
		Last Modified: Thu, 28 Sep 2023 22:18:37 GMT  
		Size: 64.1 MB (64116623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9a2fd37dab154ff5a7a7f14553c32641833c766ad5fb9ab737767a24048145`  
		Last Modified: Thu, 28 Sep 2023 22:18:16 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f689a2a610338f9a37a48fa810fa16f44dc7777786d0ed4b2df7e7e4e01cb38`  
		Last Modified: Fri, 29 Sep 2023 02:18:20 GMT  
		Size: 5.3 MB (5269263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322aacb09420bf02551659cc5b56c905f8fc7944553e6c3b1c85b5eb92547d7f`  
		Last Modified: Fri, 29 Sep 2023 02:18:20 GMT  
		Size: 1.2 MB (1186183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490b3f0289dc37c4f918f9f29f48774d57525c152a6ee4708b66c38798b2421c`  
		Last Modified: Fri, 29 Sep 2023 02:18:19 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; s390x

```console
$ docker pull caddy@sha256:b438b3cf1ad85b0cc2fe8f5319ac062a52640a6a231f4858917e081b1e773001
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76102753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1788e10f8a6f8ccdc56c8b2c4b5a6ebc9387eb3b66b2b9d2dd1f18b74223f3c2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:38:54 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:38:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:38:54 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 21:39:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 21:39:15 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 21:39:15 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 21:39:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:39:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 21:39:15 GMT
WORKDIR /go
# Thu, 28 Sep 2023 22:19:51 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 28 Sep 2023 22:19:51 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_SETCAP=1
# Thu, 28 Sep 2023 22:19:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Sep 2023 22:19:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Sep 2023 22:19:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0721f16693d4788a5add1bd0b22764c8887cdc62b24edf388ae895df440f4aa9`  
		Last Modified: Thu, 28 Sep 2023 21:46:22 GMT  
		Size: 285.1 KB (285095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40248878cac53fafdd0778844ffa03633e8f3cd73c5d5136e02da42557cb26f6`  
		Last Modified: Thu, 28 Sep 2023 21:46:16 GMT  
		Size: 66.2 MB (66224373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3d28e3790630932107b3adf42c8b1564c57d0ab97f15a759b1a8f835ee4101`  
		Last Modified: Thu, 28 Sep 2023 21:46:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d382e103bfc732fc0a4c2b972100a5426b9a8e99cd21d22eddb196e5bb029206`  
		Last Modified: Thu, 28 Sep 2023 22:20:30 GMT  
		Size: 5.1 MB (5115228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3232faabff7e982d010fd0c3775d8c4a6b80e55bc3acdb0af1e63077c07656`  
		Last Modified: Thu, 28 Sep 2023 22:20:30 GMT  
		Size: 1.3 MB (1262392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff69fb680d5cc18f0d5150ac6c2922176848b00c8456922df5843f6e1c993cc7`  
		Last Modified: Thu, 28 Sep 2023 22:20:29 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - windows version 10.0.17763.4851; amd64

```console
$ docker pull caddy@sha256:95c666eeefee6beeed59b530714de1ebdd28f2ba6ad0703b37f26b729f5e3793
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2113168904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9bf61498c4479dace7e2fa1c8c4c29a0a0722e06138f3d5fa9226287d83f2d6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 01:39:14 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Sep 2023 01:39:15 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Sep 2023 01:39:16 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Sep 2023 01:39:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Sep 2023 01:40:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:40:50 GMT
ENV GOPATH=C:\go
# Wed, 13 Sep 2023 01:41:53 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Sep 2023 01:41:54 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 13 Sep 2023 01:45:02 GMT
RUN $url = 'https://dl.google.com/go/go1.21.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '10a4f5b63215d11d1770453733dbcbf024f3f74872f84e28d7ea59f0250316c6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:45:04 GMT
WORKDIR C:\go
# Wed, 13 Sep 2023 05:35:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:35:07 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 13 Sep 2023 05:35:07 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:35:08 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Sep 2023 05:36:24 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Sep 2023 05:36:25 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cdfacf538899a08fcbb1c6b92df02725dbfcc05c593d6f310371baf9cc5c28b`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaa9f7bc4f06074cd41e4c8f38f9019d00b30116cc81e7e57bb201a2cddbe76`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa369f25c61f03e75b9090231c21b059562345a9aa5b4710c1d4bd043232a46`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1338c790efe798520cb633291aa3dbf3b37552cfbd91737d2539bad7bcac882c`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af230316f5f5bdfd37af05e436ffaadf28ac7a31d97f315dbfb2924c4d1ca3c`  
		Last Modified: Wed, 13 Sep 2023 02:16:54 GMT  
		Size: 25.6 MB (25567707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606d89c5df48922aee4ed7b88afc9f9fc270b462891c28d20b75199f2726201e`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f90ec51ca481c33d4e3887adf74f8b37c2f82af9e60290d2755f34c55b70e9c`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 220.5 KB (220461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9741d5460d3c8c14c62fd6990864968f75fbb895dfd099803a72c140739264b`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac37fd27ee4a5046c706042d53bb4a5b5e2e9ac0ec76a27142f42a55f09c31aa`  
		Last Modified: Wed, 13 Sep 2023 02:17:12 GMT  
		Size: 69.3 MB (69345076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4460c6474f9af5dc17adefba85607fa63b6072fc39250bcf433f458742fd0987`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 1.6 KB (1559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8840f55013cb306bc30661534c9618bdfda370c585b638deb791ba84fbceee9c`  
		Last Modified: Wed, 13 Sep 2023 05:38:30 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f45db9ea611a79882cee37d8b10da3ddf761d7f9ae24bf1fe0cfdb58497a6ae`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51195ebf7ad1d0ac3972b387896050e20749e6e0bb65d49a1907f49ab5cec5f2`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56989aaa5684bbc2d72ae4bb645d01d4dd0c63d35c8f4515b4c8587d6611d519`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae11f7d16342cb14a92f5b67ee9ce0eeab5805f76829bedd3735c0eec9b1f744`  
		Last Modified: Wed, 13 Sep 2023 05:38:29 GMT  
		Size: 1.7 MB (1687175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f520ac11e32bd8e755e12beaef19d397e709b5d8b007fb948658b974af6c7e2`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - windows version 10.0.20348.1970; amd64

```console
$ docker pull caddy@sha256:0a56e01d98805d99f891740e4644f1afb62f725060c36ad3cdcad27f452c3952
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1934132962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f26855783f570cd07fa203aa143ae0ddab1ef24e3a100e66f3cac124f008c0e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 01:35:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 01:35:30 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Sep 2023 01:35:31 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Sep 2023 01:35:32 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Sep 2023 01:35:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Sep 2023 01:36:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:36:16 GMT
ENV GOPATH=C:\go
# Wed, 13 Sep 2023 01:36:38 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Sep 2023 01:36:39 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 13 Sep 2023 01:38:59 GMT
RUN $url = 'https://dl.google.com/go/go1.21.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '10a4f5b63215d11d1770453733dbcbf024f3f74872f84e28d7ea59f0250316c6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:39:01 GMT
WORKDIR C:\go
# Wed, 13 Sep 2023 05:36:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:36:35 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 13 Sep 2023 05:36:35 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:36:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Sep 2023 05:37:04 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Sep 2023 05:37:05 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f40969dbf1e035a6c49e7c40b216960e3ee98ec3b76f76f9fe4498d0110bee`  
		Last Modified: Wed, 13 Sep 2023 02:15:22 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a846e03791bc3a58cfed3f02e65f87e18a5f5f416405456368e8a0ec4f9364`  
		Last Modified: Wed, 13 Sep 2023 02:15:21 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bc2015fc36cda903dca8edfdc1c87b219753af24c4ff5a95db324fb0e1cc0c`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d1910b6e6c60b5b71a12c43af94e08cf0ba20718d9a6c16ad07734f4977311`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46353fb4c6176aee49921617b1cd3ac7dcbca49d4d7a734cb5ddef177b8354b2`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f70d11added5b27b9707831ac76b04e95d4fa92b406f09532472fa350df630`  
		Last Modified: Wed, 13 Sep 2023 02:15:25 GMT  
		Size: 25.6 MB (25551011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892bff3fc5428691c1922057d675611c2b50e50cf3c6d22c2054b270861bc53c`  
		Last Modified: Wed, 13 Sep 2023 02:15:17 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ee07c029ab53a292bbb7320390d24d86b21159530b1b77d968b2b5416e8f67`  
		Last Modified: Wed, 13 Sep 2023 02:15:18 GMT  
		Size: 277.5 KB (277484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02fba082f03e26936264b99820372415048914f7ffd7f2469a28d3c0edd9224d`  
		Last Modified: Wed, 13 Sep 2023 02:15:17 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5004044396790144a82fbe98df119c5d7ae1a9abaac51c4cf0813b0d43f3f58`  
		Last Modified: Wed, 13 Sep 2023 02:15:43 GMT  
		Size: 69.3 MB (69336704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d84e4497229ea334095327a0106b2812e1dd5261c636cb1461fd698efffc4b6`  
		Last Modified: Wed, 13 Sep 2023 02:15:17 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20bad1e33f8c7089f46cd563d46ed621e589ef95c6dd41ba7569e5649804f136`  
		Last Modified: Wed, 13 Sep 2023 05:38:48 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c872ac2c7792d27826114f417d42ecbf945599d2b446775726d828ee99aab2c0`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6aff62b7b35fb324b51b0049e8a19ba51736b4f6ba1bfd92511f117e51e794`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77347ece80c37436fa82eb033a03166eb1c797e7341a6b642bf3bb80c12e36d5`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d1c7afb782c38442247cae60bbf9b16689939a03c80d4394125a9ff0af783c`  
		Last Modified: Wed, 13 Sep 2023 05:38:47 GMT  
		Size: 1.7 MB (1675830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191cef90893a643b034d031ee3e41cd4daa1b59c1d2d0e2dc1640f7bedb6c55a`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-builder-alpine`

```console
$ docker pull caddy@sha256:308ffbaa017c0bb533cfe7442c49460b33193a43192b2bb9744a0fa7080a50c3
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
$ docker pull caddy@sha256:1feb6492b7349402a4e1183682415d3a06e2c50998e55e05a23a7ff54104f12e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76961764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b60574c0fd570f746bcbc19dbe40382acf64d8088c9ec08e4e3ffe8e45f1f41`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:54:30 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:54:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:54:31 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 22:54:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 22:54:41 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 22:54:41 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 22:54:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:54:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 22:54:42 GMT
WORKDIR /go
# Fri, 29 Sep 2023 03:34:26 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Fri, 29 Sep 2023 03:34:26 GMT
ENV XCADDY_VERSION=v0.3.5
# Fri, 29 Sep 2023 03:34:26 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 03:34:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 29 Sep 2023 03:34:26 GMT
ENV XCADDY_SETCAP=1
# Fri, 29 Sep 2023 03:34:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 29 Sep 2023 03:34:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 29 Sep 2023 03:34:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc37b24bb09971feb8bf4882e861bce9db0c985a16a900adb0dc9de3f854243b`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 284.7 KB (284690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94517ad51c70c15adb540d431b757078be8f6214a2f1d2181afc9454fa65d281`  
		Last Modified: Thu, 28 Sep 2023 22:57:25 GMT  
		Size: 67.0 MB (67001967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2087470b845b2224ab3a61dafcdf2abbf9540f77be63368c3346b85ad2969fa6`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2981d490d3f8070423e8c669473d70f16909bf20541abd01afb263f326ce67c2`  
		Last Modified: Fri, 29 Sep 2023 03:34:47 GMT  
		Size: 5.0 MB (4970347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5299a94e56556856e0899be99ae303524bf1ef797eb49e7a358611d2d2b3f2`  
		Last Modified: Fri, 29 Sep 2023 03:34:46 GMT  
		Size: 1.3 MB (1302233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965d515814f9dd3e22b51ab0a9ea4f92d693760133d5cf9835588e835635e33d`  
		Last Modified: Fri, 29 Sep 2023 03:34:46 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:de02c3655970e860e68fd2840e08fd9656cebb751cf677a0982e67d8fc5538a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75403016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:636f8b72fc8192d5a346042bbf7f4b91636efcd463c388b6789b3d107346d09d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:55:22 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:55:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:55:22 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 21:55:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 21:55:37 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 21:55:37 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 21:55:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:55:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 21:55:37 GMT
WORKDIR /go
# Thu, 28 Sep 2023 21:59:22 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 28 Sep 2023 21:59:22 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 28 Sep 2023 21:59:22 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 21:59:23 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Sep 2023 21:59:23 GMT
ENV XCADDY_SETCAP=1
# Thu, 28 Sep 2023 21:59:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Sep 2023 21:59:24 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Sep 2023 21:59:24 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3da3b9e7a12f6bb6b7f56e9240c2c92ce8c9f5fd5ef3b3063b9a93d454919e`  
		Last Modified: Thu, 28 Sep 2023 21:58:05 GMT  
		Size: 284.9 KB (284887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db471c20f6642596c4a4eeca4a9348dd5a897aa1c3c2383fdf2fe2c2d6f1628`  
		Last Modified: Thu, 28 Sep 2023 21:58:18 GMT  
		Size: 65.8 MB (65758212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037298c7b9748af97a3a2906d0ebb91f2dd588f633a9e8f94e2e2b2a571ead1f`  
		Last Modified: Thu, 28 Sep 2023 21:58:05 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc923fd6dd565567ed402508a7420812a84f61bbecfa0e1f988bd9b2d7b772b`  
		Last Modified: Thu, 28 Sep 2023 22:00:17 GMT  
		Size: 5.0 MB (4965415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b055d2dc5239a960f27dc6b7a7dcbe9455defa55bfb2f41d11678f8d56591668`  
		Last Modified: Thu, 28 Sep 2023 22:00:17 GMT  
		Size: 1.2 MB (1248652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513967d31b50a4e0f6dd90e6b95fe92f327bab78e463b9ed3a5ab386b0796a0e`  
		Last Modified: Thu, 28 Sep 2023 22:00:16 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0ad7a5fed30df59cfe78f87f33dd741fcf2f9588b879cf4a999db785e17ce566
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74701068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e079a52ac41cfb0c167d0940a0ed4a65fac94f7728283be07ef1f9a9661f0cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:15:15 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:15:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:15:15 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 22:15:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 22:15:32 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 22:15:32 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 22:15:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:15:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 22:15:33 GMT
WORKDIR /go
# Thu, 28 Sep 2023 23:19:29 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 28 Sep 2023 23:19:30 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 28 Sep 2023 23:19:30 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 23:19:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Sep 2023 23:19:30 GMT
ENV XCADDY_SETCAP=1
# Thu, 28 Sep 2023 23:19:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Sep 2023 23:19:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Sep 2023 23:19:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e0aec75477c9a2cf6993e068fa40a45f0684d622ece61f54e6e02f9adebeb8`  
		Last Modified: Thu, 28 Sep 2023 22:19:29 GMT  
		Size: 284.1 KB (284076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b5f8bc58ed201378ca797f82d516632d7a864a26eb9f29c4314f061c253a5d`  
		Last Modified: Thu, 28 Sep 2023 22:19:45 GMT  
		Size: 65.8 MB (65758178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f7cae270f0f74f4af87304330243fa68170426cfac2ed3042885f518bd97fb`  
		Last Modified: Thu, 28 Sep 2023 22:19:29 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eda060e9fe56bc05ae87a1f04e06d4aa8e1b59f3143db70491a8b212f53eceb`  
		Last Modified: Thu, 28 Sep 2023 23:20:02 GMT  
		Size: 4.5 MB (4512263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56d31be6b7b9ec4232229a322a3e283089e9524392a0c2317b6870571a1f366`  
		Last Modified: Thu, 28 Sep 2023 23:20:01 GMT  
		Size: 1.2 MB (1246086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a8990e3e6f77162545c3d58676a3cded2b3260baa61c1c27f8255bb9afb3ba`  
		Last Modified: Thu, 28 Sep 2023 23:20:01 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:af47b965d6c7ddd0a5c0691ee19821ebec47fd96c8ceeb01ad0d12b2024be158
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73995021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf00a9d5850ec2c2a9fb5239a41e1f452b6798d56f52c5dcf8063e9bb8685055`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:03:38 GMT
RUN apk add --no-cache ca-certificates
# Fri, 29 Sep 2023 01:40:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Sep 2023 01:40:17 GMT
ENV GOLANG_VERSION=1.21.1
# Fri, 29 Sep 2023 01:40:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 29 Sep 2023 01:40:27 GMT
ENV GOTOOLCHAIN=local
# Fri, 29 Sep 2023 01:40:27 GMT
ENV GOPATH=/go
# Fri, 29 Sep 2023 01:40:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Sep 2023 01:40:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Fri, 29 Sep 2023 01:40:28 GMT
WORKDIR /go
# Fri, 29 Sep 2023 04:34:55 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Fri, 29 Sep 2023 04:34:55 GMT
ENV XCADDY_VERSION=v0.3.5
# Fri, 29 Sep 2023 04:34:55 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 04:34:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 29 Sep 2023 04:34:56 GMT
ENV XCADDY_SETCAP=1
# Fri, 29 Sep 2023 04:34:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 29 Sep 2023 04:34:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 29 Sep 2023 04:34:57 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c21914ef412ef71f6092299b025bf4d504a49024701bf684bc9efd218155c63`  
		Last Modified: Fri, 29 Sep 2023 01:03:48 GMT  
		Size: 286.3 KB (286306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5340c63a94930ed08fa6eea6fd627bdb38f335952054831c49716a27a8c8dfa0`  
		Last Modified: Fri, 29 Sep 2023 01:42:20 GMT  
		Size: 64.1 MB (64108807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3ca664c3732429a52e8e77a07dc94297fce7c851529dd6a572983f0bf99ae1`  
		Last Modified: Fri, 29 Sep 2023 01:42:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63283848834a5104fc3043f65de33b90d451c46dfbb2fa91874f41c1f0fcbdf2`  
		Last Modified: Fri, 29 Sep 2023 04:35:13 GMT  
		Size: 5.1 MB (5069067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a59c9f8a01ff922ae6c69e34038c2eb56dcc3bf0e7bc786804f9cabda360ec`  
		Last Modified: Fri, 29 Sep 2023 04:35:12 GMT  
		Size: 1.2 MB (1198450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a52b5eedc76b0958663cbb9be6e5ac8eaa51dff9778a4b4cff667120ab6da12`  
		Last Modified: Fri, 29 Sep 2023 04:35:12 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:55d9b4418c520166c8863db2e2993557191bf9caf6e028f7b04a5b8ab1b63a73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74205796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a71360173a10dc6951ba63109fda1b23d9e5356b14225bf346845fa455513541`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:13:11 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:13:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:13:12 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 22:13:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 22:13:47 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 22:13:48 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 22:13:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:13:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 22:13:52 GMT
WORKDIR /go
# Fri, 29 Sep 2023 02:17:36 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Fri, 29 Sep 2023 02:17:37 GMT
ENV XCADDY_VERSION=v0.3.5
# Fri, 29 Sep 2023 02:17:37 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 02:17:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 29 Sep 2023 02:17:38 GMT
ENV XCADDY_SETCAP=1
# Fri, 29 Sep 2023 02:17:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 29 Sep 2023 02:17:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 29 Sep 2023 02:17:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc67971d1767eae5019ffeaf8f893e6d81dbba50bde347da0c0433c56e3f2a3`  
		Last Modified: Thu, 28 Sep 2023 22:18:17 GMT  
		Size: 286.7 KB (286659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a20f495e184de0c46bb781c57dd99e2cfc30deaa14db48a8f0cc95fc20ed28b`  
		Last Modified: Thu, 28 Sep 2023 22:18:37 GMT  
		Size: 64.1 MB (64116623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9a2fd37dab154ff5a7a7f14553c32641833c766ad5fb9ab737767a24048145`  
		Last Modified: Thu, 28 Sep 2023 22:18:16 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f689a2a610338f9a37a48fa810fa16f44dc7777786d0ed4b2df7e7e4e01cb38`  
		Last Modified: Fri, 29 Sep 2023 02:18:20 GMT  
		Size: 5.3 MB (5269263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322aacb09420bf02551659cc5b56c905f8fc7944553e6c3b1c85b5eb92547d7f`  
		Last Modified: Fri, 29 Sep 2023 02:18:20 GMT  
		Size: 1.2 MB (1186183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490b3f0289dc37c4f918f9f29f48774d57525c152a6ee4708b66c38798b2421c`  
		Last Modified: Fri, 29 Sep 2023 02:18:19 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:b438b3cf1ad85b0cc2fe8f5319ac062a52640a6a231f4858917e081b1e773001
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76102753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1788e10f8a6f8ccdc56c8b2c4b5a6ebc9387eb3b66b2b9d2dd1f18b74223f3c2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:38:54 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:38:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:38:54 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 21:39:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 21:39:15 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 21:39:15 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 21:39:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:39:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 21:39:15 GMT
WORKDIR /go
# Thu, 28 Sep 2023 22:19:51 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 28 Sep 2023 22:19:51 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_SETCAP=1
# Thu, 28 Sep 2023 22:19:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Sep 2023 22:19:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Sep 2023 22:19:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0721f16693d4788a5add1bd0b22764c8887cdc62b24edf388ae895df440f4aa9`  
		Last Modified: Thu, 28 Sep 2023 21:46:22 GMT  
		Size: 285.1 KB (285095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40248878cac53fafdd0778844ffa03633e8f3cd73c5d5136e02da42557cb26f6`  
		Last Modified: Thu, 28 Sep 2023 21:46:16 GMT  
		Size: 66.2 MB (66224373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3d28e3790630932107b3adf42c8b1564c57d0ab97f15a759b1a8f835ee4101`  
		Last Modified: Thu, 28 Sep 2023 21:46:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d382e103bfc732fc0a4c2b972100a5426b9a8e99cd21d22eddb196e5bb029206`  
		Last Modified: Thu, 28 Sep 2023 22:20:30 GMT  
		Size: 5.1 MB (5115228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3232faabff7e982d010fd0c3775d8c4a6b80e55bc3acdb0af1e63077c07656`  
		Last Modified: Thu, 28 Sep 2023 22:20:30 GMT  
		Size: 1.3 MB (1262392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff69fb680d5cc18f0d5150ac6c2922176848b00c8456922df5843f6e1c993cc7`  
		Last Modified: Thu, 28 Sep 2023 22:20:29 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:1a9280c29c9c558a4f0870515605df3716ff711eeef8f648d8207f81f3577c8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `caddy:2.7-builder-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull caddy@sha256:95c666eeefee6beeed59b530714de1ebdd28f2ba6ad0703b37f26b729f5e3793
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2113168904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9bf61498c4479dace7e2fa1c8c4c29a0a0722e06138f3d5fa9226287d83f2d6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 01:39:14 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Sep 2023 01:39:15 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Sep 2023 01:39:16 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Sep 2023 01:39:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Sep 2023 01:40:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:40:50 GMT
ENV GOPATH=C:\go
# Wed, 13 Sep 2023 01:41:53 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Sep 2023 01:41:54 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 13 Sep 2023 01:45:02 GMT
RUN $url = 'https://dl.google.com/go/go1.21.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '10a4f5b63215d11d1770453733dbcbf024f3f74872f84e28d7ea59f0250316c6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:45:04 GMT
WORKDIR C:\go
# Wed, 13 Sep 2023 05:35:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:35:07 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 13 Sep 2023 05:35:07 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:35:08 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Sep 2023 05:36:24 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Sep 2023 05:36:25 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cdfacf538899a08fcbb1c6b92df02725dbfcc05c593d6f310371baf9cc5c28b`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaa9f7bc4f06074cd41e4c8f38f9019d00b30116cc81e7e57bb201a2cddbe76`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa369f25c61f03e75b9090231c21b059562345a9aa5b4710c1d4bd043232a46`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1338c790efe798520cb633291aa3dbf3b37552cfbd91737d2539bad7bcac882c`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af230316f5f5bdfd37af05e436ffaadf28ac7a31d97f315dbfb2924c4d1ca3c`  
		Last Modified: Wed, 13 Sep 2023 02:16:54 GMT  
		Size: 25.6 MB (25567707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606d89c5df48922aee4ed7b88afc9f9fc270b462891c28d20b75199f2726201e`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f90ec51ca481c33d4e3887adf74f8b37c2f82af9e60290d2755f34c55b70e9c`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 220.5 KB (220461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9741d5460d3c8c14c62fd6990864968f75fbb895dfd099803a72c140739264b`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac37fd27ee4a5046c706042d53bb4a5b5e2e9ac0ec76a27142f42a55f09c31aa`  
		Last Modified: Wed, 13 Sep 2023 02:17:12 GMT  
		Size: 69.3 MB (69345076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4460c6474f9af5dc17adefba85607fa63b6072fc39250bcf433f458742fd0987`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 1.6 KB (1559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8840f55013cb306bc30661534c9618bdfda370c585b638deb791ba84fbceee9c`  
		Last Modified: Wed, 13 Sep 2023 05:38:30 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f45db9ea611a79882cee37d8b10da3ddf761d7f9ae24bf1fe0cfdb58497a6ae`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51195ebf7ad1d0ac3972b387896050e20749e6e0bb65d49a1907f49ab5cec5f2`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56989aaa5684bbc2d72ae4bb645d01d4dd0c63d35c8f4515b4c8587d6611d519`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae11f7d16342cb14a92f5b67ee9ce0eeab5805f76829bedd3735c0eec9b1f744`  
		Last Modified: Wed, 13 Sep 2023 05:38:29 GMT  
		Size: 1.7 MB (1687175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f520ac11e32bd8e755e12beaef19d397e709b5d8b007fb948658b974af6c7e2`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:e27807e1af059f2f978b562de306e9d021538db7c394f3838deb1d734efc29ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1970; amd64

### `caddy:2.7-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1970; amd64

```console
$ docker pull caddy@sha256:0a56e01d98805d99f891740e4644f1afb62f725060c36ad3cdcad27f452c3952
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1934132962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f26855783f570cd07fa203aa143ae0ddab1ef24e3a100e66f3cac124f008c0e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 01:35:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 01:35:30 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Sep 2023 01:35:31 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Sep 2023 01:35:32 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Sep 2023 01:35:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Sep 2023 01:36:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:36:16 GMT
ENV GOPATH=C:\go
# Wed, 13 Sep 2023 01:36:38 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Sep 2023 01:36:39 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 13 Sep 2023 01:38:59 GMT
RUN $url = 'https://dl.google.com/go/go1.21.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '10a4f5b63215d11d1770453733dbcbf024f3f74872f84e28d7ea59f0250316c6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:39:01 GMT
WORKDIR C:\go
# Wed, 13 Sep 2023 05:36:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:36:35 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 13 Sep 2023 05:36:35 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:36:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Sep 2023 05:37:04 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Sep 2023 05:37:05 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f40969dbf1e035a6c49e7c40b216960e3ee98ec3b76f76f9fe4498d0110bee`  
		Last Modified: Wed, 13 Sep 2023 02:15:22 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a846e03791bc3a58cfed3f02e65f87e18a5f5f416405456368e8a0ec4f9364`  
		Last Modified: Wed, 13 Sep 2023 02:15:21 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bc2015fc36cda903dca8edfdc1c87b219753af24c4ff5a95db324fb0e1cc0c`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d1910b6e6c60b5b71a12c43af94e08cf0ba20718d9a6c16ad07734f4977311`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46353fb4c6176aee49921617b1cd3ac7dcbca49d4d7a734cb5ddef177b8354b2`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f70d11added5b27b9707831ac76b04e95d4fa92b406f09532472fa350df630`  
		Last Modified: Wed, 13 Sep 2023 02:15:25 GMT  
		Size: 25.6 MB (25551011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892bff3fc5428691c1922057d675611c2b50e50cf3c6d22c2054b270861bc53c`  
		Last Modified: Wed, 13 Sep 2023 02:15:17 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ee07c029ab53a292bbb7320390d24d86b21159530b1b77d968b2b5416e8f67`  
		Last Modified: Wed, 13 Sep 2023 02:15:18 GMT  
		Size: 277.5 KB (277484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02fba082f03e26936264b99820372415048914f7ffd7f2469a28d3c0edd9224d`  
		Last Modified: Wed, 13 Sep 2023 02:15:17 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5004044396790144a82fbe98df119c5d7ae1a9abaac51c4cf0813b0d43f3f58`  
		Last Modified: Wed, 13 Sep 2023 02:15:43 GMT  
		Size: 69.3 MB (69336704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d84e4497229ea334095327a0106b2812e1dd5261c636cb1461fd698efffc4b6`  
		Last Modified: Wed, 13 Sep 2023 02:15:17 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20bad1e33f8c7089f46cd563d46ed621e589ef95c6dd41ba7569e5649804f136`  
		Last Modified: Wed, 13 Sep 2023 05:38:48 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c872ac2c7792d27826114f417d42ecbf945599d2b446775726d828ee99aab2c0`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6aff62b7b35fb324b51b0049e8a19ba51736b4f6ba1bfd92511f117e51e794`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77347ece80c37436fa82eb033a03166eb1c797e7341a6b642bf3bb80c12e36d5`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d1c7afb782c38442247cae60bbf9b16689939a03c80d4394125a9ff0af783c`  
		Last Modified: Wed, 13 Sep 2023 05:38:47 GMT  
		Size: 1.7 MB (1675830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191cef90893a643b034d031ee3e41cd4daa1b59c1d2d0e2dc1640f7bedb6c55a`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-windowsservercore`

```console
$ docker pull caddy@sha256:4e0879a2422f5309c4ed33c36438e076aa198dc89228e2dc8a56369b86fac7a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4851; amd64
	-	windows version 10.0.20348.1970; amd64

### `caddy:2.7-windowsservercore` - windows version 10.0.17763.4851; amd64

```console
$ docker pull caddy@sha256:3f230e8c687c5611e74c84c3ec6f7ef7844b3cc3443d9302e9bb778e6210bfe2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2032252342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea189389e39a38d33c2124e3c02e0a9bc2f3168e5605fa8a909e749ac52fc3f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:30:52 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:30:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:32:00 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:32:02 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:32:04 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:32:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:32:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:32:08 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:32:09 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:33:07 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:33:07 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2bc90334de89082943edb24d5f52a3bb36ef134c17a417ba45cc4e122be3b2`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 465.0 KB (465015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba1c9fb8dedf070862eb0526393862bb5a0f2c87a87bc3864b9b24b11af5524`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5249ade277243b1b7f8c198de7d036f2e106b8a679d777b7bfc885af7b9b76`  
		Last Modified: Wed, 13 Sep 2023 05:37:46 GMT  
		Size: 15.2 MB (15176891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224a0aed4c02b4a48f633ac01c40e020d4e8fbc32fe8896d93032f9d72f50cda`  
		Last Modified: Wed, 13 Sep 2023 05:37:42 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fc1c10b7da22b1e9a26f059801a53ce4ce22e7d24ab14ec56d343a806f3bc2`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bd26e7302c16a8d83a8a6b5d9d263b804279f2b4c7d2fcea59a97c1e187648`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f69e667aa7c5e5a21f7d8a8cdd213b9d20a8a0c790dd18fe51d4df9e5b08a7`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e456b9da79a468c972d487e55e3628f8a8917f78948550c359afc891a5ad24a`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bc4af3e90793180c1ed8b8b9ac6866e24a5de16881f363dacf0ecf47396c8`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0289dff328d597d94fcd8612bd4a726573e13f780790744c5c6f4b40b49823`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52ff2438c88a58e8be33368f668557c92bcfdc503bd58025d081c7b88ec88b`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0f1c855afa9fd7bcf5ded632c161f2ff013f4b08f5c233fa3bdf3d13701467`  
		Last Modified: Wed, 13 Sep 2023 05:37:38 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2e0bf79eee4bbd609b5a111793e394f22ad86eb897cf85c6df2c45d9a8d777`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff797288117550c2b80f9a39dd5a04cb449defc2660cf6a7589618b8d3606464`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa0d1665270ae2e22844b2386842b1deab36f8936506db82df0ec69dc72fb84`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c867297eb9d01dfe100695ae10a0c67bd38f2124de0ee7446d1e66b6dede5c06`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee97f69cfbd31f5a098d45934b159384d8e986d860ad3007140beee338aa4533`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b741c4ffade19f3d712c3fb839c3ae7f1ae4e39e5f777a2b24917b5e630d0f86`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 256.7 KB (256675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a415b22709a225227fa7ce65d7767f3f820c7e9e445b0d718dfb68ae2249832`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-windowsservercore` - windows version 10.0.20348.1970; amd64

```console
$ docker pull caddy@sha256:76214fe6feb9f96f1c46334c01e1b9d310eb2e745bb08ba4130547b2147f3677
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1853253940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f0e585ea0797bdd13d148afed1e86161022e8cf2a79d11337f9d4dde0a8efe6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 01:35:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:33:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:33:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:34:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:34:25 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:34:26 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:34:27 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:34:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:34:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:34:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:34:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:34:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:34:33 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:34:34 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:34:35 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:34:36 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:34:56 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:34:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f40969dbf1e035a6c49e7c40b216960e3ee98ec3b76f76f9fe4498d0110bee`  
		Last Modified: Wed, 13 Sep 2023 02:15:22 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2d313a26784edb67b74292171891c0393ea119a53238e09150b5b7bc52371f`  
		Last Modified: Wed, 13 Sep 2023 05:38:08 GMT  
		Size: 483.0 KB (482985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb50376a60c42178e92d96a048b0e7f2dbc2cafe73274ab76722cda86fb32ee`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeecad99d9c5b378a623153b24130f8c36442e9a48ef6a48f878c5f585a66bd4`  
		Last Modified: Wed, 13 Sep 2023 05:38:11 GMT  
		Size: 15.2 MB (15183860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6b7a19981a71c15e39afbc3a52ed5f0c065f77c1ccd55a88e5f1b51af88753`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd7340889e9a6bfc8018c7709595b75ef962cf2608d14398ffbc90b90804a04`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7537acdfe48467d248afb6a69dad6bdb09c62617600305d2b2adb8a45ece2f`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf3cb277ba29189d90269123acd401fa787771fb095f2f2ec532be7bba2a025`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64eb5cc4069279b73a665e35bf526fa42558af1a3a71fc13d76913846d96818`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74348cf2ecbfe3a00df246034f9ab755418e8584b24113c9d327fc80cb134829`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa3fef62dce81d37fff2c621b94314d2aa9d0318523407b0a1d7d2b1e079234`  
		Last Modified: Wed, 13 Sep 2023 05:38:04 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d033d5a006e7fa969026194ef48446c840a891ad252f0316d32bc01843f0e4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbef09c0840262b42ba39068c868fc9b353bed78bb7de251e953289149e9a64e`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea46de371cf13fdb02566c79fc3a22c7123bd7c8903d20645b9cfe34f7ca85d4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63cdcd333c2c131733511c6750d4154ea7f097d981934d1dda8944bf2840860`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8259824bfebcdadd0448ccc0a815b7257636f6eb420e7e00216359908281e7b`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51874919dc1cfa2121d50499f839a702c4cd7340e8708e90b2af042e9debba9`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee3a41ffde2d883c73932756f176ba6901eaeb7a680a351a2b476398263cc8`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73e8028e6f79476106af6c347aa4765644a8ed828c5b6c117ee3dcc2e22e1ef`  
		Last Modified: Wed, 13 Sep 2023 05:38:02 GMT  
		Size: 289.2 KB (289194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd87253476a12fff6cbe718338261ef5ec78a1eb19d8e222838e7f96c3100a0`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-windowsservercore-1809`

```console
$ docker pull caddy@sha256:2869cf74555da33dba54fe0c70e1e7baf4d8535444766d27f78fdada2c7e8bb8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `caddy:2.7-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull caddy@sha256:3f230e8c687c5611e74c84c3ec6f7ef7844b3cc3443d9302e9bb778e6210bfe2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2032252342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea189389e39a38d33c2124e3c02e0a9bc2f3168e5605fa8a909e749ac52fc3f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:30:52 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:30:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:32:00 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:32:02 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:32:04 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:32:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:32:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:32:08 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:32:09 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:33:07 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:33:07 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2bc90334de89082943edb24d5f52a3bb36ef134c17a417ba45cc4e122be3b2`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 465.0 KB (465015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba1c9fb8dedf070862eb0526393862bb5a0f2c87a87bc3864b9b24b11af5524`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5249ade277243b1b7f8c198de7d036f2e106b8a679d777b7bfc885af7b9b76`  
		Last Modified: Wed, 13 Sep 2023 05:37:46 GMT  
		Size: 15.2 MB (15176891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224a0aed4c02b4a48f633ac01c40e020d4e8fbc32fe8896d93032f9d72f50cda`  
		Last Modified: Wed, 13 Sep 2023 05:37:42 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fc1c10b7da22b1e9a26f059801a53ce4ce22e7d24ab14ec56d343a806f3bc2`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bd26e7302c16a8d83a8a6b5d9d263b804279f2b4c7d2fcea59a97c1e187648`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f69e667aa7c5e5a21f7d8a8cdd213b9d20a8a0c790dd18fe51d4df9e5b08a7`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e456b9da79a468c972d487e55e3628f8a8917f78948550c359afc891a5ad24a`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bc4af3e90793180c1ed8b8b9ac6866e24a5de16881f363dacf0ecf47396c8`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0289dff328d597d94fcd8612bd4a726573e13f780790744c5c6f4b40b49823`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52ff2438c88a58e8be33368f668557c92bcfdc503bd58025d081c7b88ec88b`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0f1c855afa9fd7bcf5ded632c161f2ff013f4b08f5c233fa3bdf3d13701467`  
		Last Modified: Wed, 13 Sep 2023 05:37:38 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2e0bf79eee4bbd609b5a111793e394f22ad86eb897cf85c6df2c45d9a8d777`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff797288117550c2b80f9a39dd5a04cb449defc2660cf6a7589618b8d3606464`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa0d1665270ae2e22844b2386842b1deab36f8936506db82df0ec69dc72fb84`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c867297eb9d01dfe100695ae10a0c67bd38f2124de0ee7446d1e66b6dede5c06`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee97f69cfbd31f5a098d45934b159384d8e986d860ad3007140beee338aa4533`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b741c4ffade19f3d712c3fb839c3ae7f1ae4e39e5f777a2b24917b5e630d0f86`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 256.7 KB (256675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a415b22709a225227fa7ce65d7767f3f820c7e9e445b0d718dfb68ae2249832`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:1cf6f6aff1679190ae48af88d1f51c255c42ec58e320d967d97b39c0113fc8f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1970; amd64

### `caddy:2.7-windowsservercore-ltsc2022` - windows version 10.0.20348.1970; amd64

```console
$ docker pull caddy@sha256:76214fe6feb9f96f1c46334c01e1b9d310eb2e745bb08ba4130547b2147f3677
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1853253940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f0e585ea0797bdd13d148afed1e86161022e8cf2a79d11337f9d4dde0a8efe6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 01:35:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:33:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:33:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:34:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:34:25 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:34:26 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:34:27 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:34:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:34:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:34:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:34:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:34:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:34:33 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:34:34 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:34:35 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:34:36 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:34:56 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:34:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f40969dbf1e035a6c49e7c40b216960e3ee98ec3b76f76f9fe4498d0110bee`  
		Last Modified: Wed, 13 Sep 2023 02:15:22 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2d313a26784edb67b74292171891c0393ea119a53238e09150b5b7bc52371f`  
		Last Modified: Wed, 13 Sep 2023 05:38:08 GMT  
		Size: 483.0 KB (482985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb50376a60c42178e92d96a048b0e7f2dbc2cafe73274ab76722cda86fb32ee`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeecad99d9c5b378a623153b24130f8c36442e9a48ef6a48f878c5f585a66bd4`  
		Last Modified: Wed, 13 Sep 2023 05:38:11 GMT  
		Size: 15.2 MB (15183860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6b7a19981a71c15e39afbc3a52ed5f0c065f77c1ccd55a88e5f1b51af88753`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd7340889e9a6bfc8018c7709595b75ef962cf2608d14398ffbc90b90804a04`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7537acdfe48467d248afb6a69dad6bdb09c62617600305d2b2adb8a45ece2f`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf3cb277ba29189d90269123acd401fa787771fb095f2f2ec532be7bba2a025`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64eb5cc4069279b73a665e35bf526fa42558af1a3a71fc13d76913846d96818`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74348cf2ecbfe3a00df246034f9ab755418e8584b24113c9d327fc80cb134829`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa3fef62dce81d37fff2c621b94314d2aa9d0318523407b0a1d7d2b1e079234`  
		Last Modified: Wed, 13 Sep 2023 05:38:04 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d033d5a006e7fa969026194ef48446c840a891ad252f0316d32bc01843f0e4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbef09c0840262b42ba39068c868fc9b353bed78bb7de251e953289149e9a64e`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea46de371cf13fdb02566c79fc3a22c7123bd7c8903d20645b9cfe34f7ca85d4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63cdcd333c2c131733511c6750d4154ea7f097d981934d1dda8944bf2840860`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8259824bfebcdadd0448ccc0a815b7257636f6eb420e7e00216359908281e7b`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51874919dc1cfa2121d50499f839a702c4cd7340e8708e90b2af042e9debba9`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee3a41ffde2d883c73932756f176ba6901eaeb7a680a351a2b476398263cc8`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73e8028e6f79476106af6c347aa4765644a8ed828c5b6c117ee3dcc2e22e1ef`  
		Last Modified: Wed, 13 Sep 2023 05:38:02 GMT  
		Size: 289.2 KB (289194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd87253476a12fff6cbe718338261ef5ec78a1eb19d8e222838e7f96c3100a0`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.4`

```console
$ docker pull caddy@sha256:df239ca80315c8271f9e87a981fb47124831f8b5a7c85970249d2dfd712479a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4851; amd64
	-	windows version 10.0.20348.1970; amd64

### `caddy:2.7.4` - linux; amd64

```console
$ docker pull caddy@sha256:3d1bf053476f2415b40e728c37e1112ee7551fa154a63d6f62b275c13fea8166
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18364247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a7b2e234b158c1e01eab04f851fc4b1a33296dbaa68c57d11815ee38a3cafaf`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:43:13 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 22:43:15 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 22:43:15 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 22:43:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 22:43:17 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 22:43:17 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 22:43:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 22:43:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 22:43:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 80
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 443
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 22:43:18 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 22:43:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37be51084fb891c6796079e693b73f6f882266a5e66211344173031e2b0c8ffd`  
		Last Modified: Thu, 28 Sep 2023 22:43:35 GMT  
		Size: 350.8 KB (350826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d867aa37ac50364bf4082dc48c7d4e1b88ead3164d47855e1bbc2ef3678cfc`  
		Last Modified: Thu, 28 Sep 2023 22:43:35 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147aa3899aa3307c28e185f5385015c7a5f15dfa42578a8a8eca88bf2f1e7e3e`  
		Last Modified: Thu, 28 Sep 2023 22:43:37 GMT  
		Size: 14.6 MB (14603949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4` - linux; arm variant v6

```console
$ docker pull caddy@sha256:239c4a78d1bd0540a44003332119cf019e6ff839f4d303cd9801b1cc9e755ec4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17314598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b41f754b4ebb826dde7fb5c0c3c6048823add70f27a7f9c8d9f8ff1a9636ed2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:59:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 21:59:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 21:59:13 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 21:59:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 21:59:16 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 21:59:16 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 21:59:16 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 21:59:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 21:59:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 80
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 443
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 21:59:17 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 21:59:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1018057a600163b1c1b92c21ade975c631b2f8ccde66d524cfe0ecdac8e1920d`  
		Last Modified: Thu, 28 Sep 2023 21:59:43 GMT  
		Size: 347.6 KB (347613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec54680cbf2cb1a25285c82a7888498ab47d03a68db200a160d7162325a5be19`  
		Last Modified: Thu, 28 Sep 2023 21:59:43 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d087db4282d622690fce98f1d8802151567e43bfdd884a3e2a4d084701229a1`  
		Last Modified: Thu, 28 Sep 2023 21:59:45 GMT  
		Size: 13.8 MB (13814189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4` - linux; arm variant v7

```console
$ docker pull caddy@sha256:85dd4fae9241ac3330e98e1d3b052d36b7ecbe1cd69b4c860454c84976426e70
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17043239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f78b426118e91fcb43786aa4c3003cd91ee86ab5f896516a885f964056b08cae`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:19:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 23:19:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 23:19:20 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 23:19:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 23:19:24 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 23:19:24 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 80
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 443
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 23:19:25 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 23:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66901ba48d0ee53cd827f4eb2cfd8b049cebba8c3d307b69760e1be917f69476`  
		Last Modified: Thu, 28 Sep 2023 23:19:46 GMT  
		Size: 344.4 KB (344448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dddeb3f6febb36993d8a51ad919784fd152aab5f6e17fe00d579916f32e42911`  
		Last Modified: Thu, 28 Sep 2023 23:19:46 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f936b2c0499a587b75385edfeb1d22b8f16ed05dca7dd0999ccc0635e1904a`  
		Last Modified: Thu, 28 Sep 2023 23:19:48 GMT  
		Size: 13.8 MB (13791383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:595e5490450c9ed29cc960149e2c265210e8444f3b3ea5ff2fab62d0da5ec3d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17163627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23f8ae4a1af151ac93d2945855095990774bc44f70af5c0e4b058dbb7e8b8c09`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:16:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 29 Sep 2023 01:16:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 29 Sep 2023 01:16:13 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 01:16:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 29 Sep 2023 01:16:15 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 29 Sep 2023 01:16:15 GMT
ENV XDG_DATA_HOME=/data
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 80
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 443
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 443/udp
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 2019
# Fri, 29 Sep 2023 01:16:16 GMT
WORKDIR /srv
# Fri, 29 Sep 2023 01:16:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f21cb0286edf1f5fefb4a859b414a446bb81baa9e8901fc8f4eca55a43aeeec`  
		Last Modified: Fri, 29 Sep 2023 01:16:34 GMT  
		Size: 360.6 KB (360643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5444b3f9419d06a4b77a65935a3b1c6e657c607bcfb9e3bd1abebe57eae36e6a`  
		Last Modified: Fri, 29 Sep 2023 01:16:34 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3485ef64f848b891981d59d52e0b092b261205ad787b38ae389e5ac39eed493f`  
		Last Modified: Fri, 29 Sep 2023 01:16:35 GMT  
		Size: 13.5 MB (13463646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4` - linux; ppc64le

```console
$ docker pull caddy@sha256:65084a14a1557b92af5b8ba6fcba9a7a710ed5caef1e2310f9622166608c9531
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16945195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73ba45deaa04c3feac6474c22204ac6f5ebc380b331ff7d585ecd196284459b3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:17:03 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 29 Sep 2023 02:17:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 29 Sep 2023 02:17:06 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 02:17:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 29 Sep 2023 02:17:13 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 29 Sep 2023 02:17:14 GMT
ENV XDG_DATA_HOME=/data
# Fri, 29 Sep 2023 02:17:15 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Fri, 29 Sep 2023 02:17:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 29 Sep 2023 02:17:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 29 Sep 2023 02:17:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 29 Sep 2023 02:17:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 29 Sep 2023 02:17:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 29 Sep 2023 02:17:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 29 Sep 2023 02:17:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 29 Sep 2023 02:17:21 GMT
EXPOSE 80
# Fri, 29 Sep 2023 02:17:21 GMT
EXPOSE 443
# Fri, 29 Sep 2023 02:17:22 GMT
EXPOSE 443/udp
# Fri, 29 Sep 2023 02:17:22 GMT
EXPOSE 2019
# Fri, 29 Sep 2023 02:17:24 GMT
WORKDIR /srv
# Fri, 29 Sep 2023 02:17:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa65cea7f5d70d1e203b851e43ad676e92f28c930ad32b6691e84ff9b5cda87`  
		Last Modified: Fri, 29 Sep 2023 02:18:03 GMT  
		Size: 362.2 KB (362182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7089a1d537371e29a65d106f43b45f2a0367d4d1db0eb7d6b7099f8ba05645`  
		Last Modified: Fri, 29 Sep 2023 02:18:01 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b93ab741fa6270144ea59d6a5fa3c4138286a569f246fdccd829b317b051f3a`  
		Last Modified: Fri, 29 Sep 2023 02:18:05 GMT  
		Size: 13.2 MB (13228998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4` - linux; s390x

```console
$ docker pull caddy@sha256:9e13bd2b56147eecc80f1fe1710e4350ea63d5edfb389fa89e2c6de06c08593a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17721238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2f0101e0f893afb763d99b2050dbf4d68a44aae29785af6c05af5a552b0c1a7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:19:38 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 22:19:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 22:19:39 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 22:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 22:19:42 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 22:19:42 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 80
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 443
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 22:19:44 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 22:19:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed3df874173df47ad0bd0ef67b8ee598c77921810d84a67fd2984c4f8151c91`  
		Last Modified: Thu, 28 Sep 2023 22:20:14 GMT  
		Size: 354.9 KB (354948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95a69c42a5c7fc6d73c00c7f6eb68522f3881aae55db4f85a8400e83b678b181`  
		Last Modified: Thu, 28 Sep 2023 22:20:14 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793016dc78c9794c627c07afcd2fb34af4ee470ee7fef1a1596eff0c59ba6659`  
		Last Modified: Thu, 28 Sep 2023 22:20:16 GMT  
		Size: 14.1 MB (14143684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4` - windows version 10.0.17763.4851; amd64

```console
$ docker pull caddy@sha256:3f230e8c687c5611e74c84c3ec6f7ef7844b3cc3443d9302e9bb778e6210bfe2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2032252342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea189389e39a38d33c2124e3c02e0a9bc2f3168e5605fa8a909e749ac52fc3f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:30:52 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:30:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:32:00 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:32:02 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:32:04 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:32:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:32:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:32:08 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:32:09 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:33:07 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:33:07 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2bc90334de89082943edb24d5f52a3bb36ef134c17a417ba45cc4e122be3b2`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 465.0 KB (465015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba1c9fb8dedf070862eb0526393862bb5a0f2c87a87bc3864b9b24b11af5524`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5249ade277243b1b7f8c198de7d036f2e106b8a679d777b7bfc885af7b9b76`  
		Last Modified: Wed, 13 Sep 2023 05:37:46 GMT  
		Size: 15.2 MB (15176891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224a0aed4c02b4a48f633ac01c40e020d4e8fbc32fe8896d93032f9d72f50cda`  
		Last Modified: Wed, 13 Sep 2023 05:37:42 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fc1c10b7da22b1e9a26f059801a53ce4ce22e7d24ab14ec56d343a806f3bc2`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bd26e7302c16a8d83a8a6b5d9d263b804279f2b4c7d2fcea59a97c1e187648`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f69e667aa7c5e5a21f7d8a8cdd213b9d20a8a0c790dd18fe51d4df9e5b08a7`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e456b9da79a468c972d487e55e3628f8a8917f78948550c359afc891a5ad24a`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bc4af3e90793180c1ed8b8b9ac6866e24a5de16881f363dacf0ecf47396c8`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0289dff328d597d94fcd8612bd4a726573e13f780790744c5c6f4b40b49823`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52ff2438c88a58e8be33368f668557c92bcfdc503bd58025d081c7b88ec88b`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0f1c855afa9fd7bcf5ded632c161f2ff013f4b08f5c233fa3bdf3d13701467`  
		Last Modified: Wed, 13 Sep 2023 05:37:38 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2e0bf79eee4bbd609b5a111793e394f22ad86eb897cf85c6df2c45d9a8d777`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff797288117550c2b80f9a39dd5a04cb449defc2660cf6a7589618b8d3606464`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa0d1665270ae2e22844b2386842b1deab36f8936506db82df0ec69dc72fb84`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c867297eb9d01dfe100695ae10a0c67bd38f2124de0ee7446d1e66b6dede5c06`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee97f69cfbd31f5a098d45934b159384d8e986d860ad3007140beee338aa4533`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b741c4ffade19f3d712c3fb839c3ae7f1ae4e39e5f777a2b24917b5e630d0f86`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 256.7 KB (256675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a415b22709a225227fa7ce65d7767f3f820c7e9e445b0d718dfb68ae2249832`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4` - windows version 10.0.20348.1970; amd64

```console
$ docker pull caddy@sha256:76214fe6feb9f96f1c46334c01e1b9d310eb2e745bb08ba4130547b2147f3677
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1853253940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f0e585ea0797bdd13d148afed1e86161022e8cf2a79d11337f9d4dde0a8efe6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 01:35:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:33:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:33:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:34:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:34:25 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:34:26 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:34:27 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:34:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:34:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:34:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:34:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:34:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:34:33 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:34:34 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:34:35 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:34:36 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:34:56 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:34:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f40969dbf1e035a6c49e7c40b216960e3ee98ec3b76f76f9fe4498d0110bee`  
		Last Modified: Wed, 13 Sep 2023 02:15:22 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2d313a26784edb67b74292171891c0393ea119a53238e09150b5b7bc52371f`  
		Last Modified: Wed, 13 Sep 2023 05:38:08 GMT  
		Size: 483.0 KB (482985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb50376a60c42178e92d96a048b0e7f2dbc2cafe73274ab76722cda86fb32ee`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeecad99d9c5b378a623153b24130f8c36442e9a48ef6a48f878c5f585a66bd4`  
		Last Modified: Wed, 13 Sep 2023 05:38:11 GMT  
		Size: 15.2 MB (15183860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6b7a19981a71c15e39afbc3a52ed5f0c065f77c1ccd55a88e5f1b51af88753`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd7340889e9a6bfc8018c7709595b75ef962cf2608d14398ffbc90b90804a04`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7537acdfe48467d248afb6a69dad6bdb09c62617600305d2b2adb8a45ece2f`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf3cb277ba29189d90269123acd401fa787771fb095f2f2ec532be7bba2a025`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64eb5cc4069279b73a665e35bf526fa42558af1a3a71fc13d76913846d96818`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74348cf2ecbfe3a00df246034f9ab755418e8584b24113c9d327fc80cb134829`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa3fef62dce81d37fff2c621b94314d2aa9d0318523407b0a1d7d2b1e079234`  
		Last Modified: Wed, 13 Sep 2023 05:38:04 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d033d5a006e7fa969026194ef48446c840a891ad252f0316d32bc01843f0e4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbef09c0840262b42ba39068c868fc9b353bed78bb7de251e953289149e9a64e`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea46de371cf13fdb02566c79fc3a22c7123bd7c8903d20645b9cfe34f7ca85d4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63cdcd333c2c131733511c6750d4154ea7f097d981934d1dda8944bf2840860`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8259824bfebcdadd0448ccc0a815b7257636f6eb420e7e00216359908281e7b`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51874919dc1cfa2121d50499f839a702c4cd7340e8708e90b2af042e9debba9`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee3a41ffde2d883c73932756f176ba6901eaeb7a680a351a2b476398263cc8`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73e8028e6f79476106af6c347aa4765644a8ed828c5b6c117ee3dcc2e22e1ef`  
		Last Modified: Wed, 13 Sep 2023 05:38:02 GMT  
		Size: 289.2 KB (289194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd87253476a12fff6cbe718338261ef5ec78a1eb19d8e222838e7f96c3100a0`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.4-alpine`

```console
$ docker pull caddy@sha256:11ae052d9015105757d19caf86dc51fc14403841f2b65e93fe320f4d0e197385
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
$ docker pull caddy@sha256:3d1bf053476f2415b40e728c37e1112ee7551fa154a63d6f62b275c13fea8166
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18364247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a7b2e234b158c1e01eab04f851fc4b1a33296dbaa68c57d11815ee38a3cafaf`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:43:13 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 22:43:15 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 22:43:15 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 22:43:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 22:43:17 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 22:43:17 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 22:43:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 22:43:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 22:43:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 80
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 443
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 22:43:18 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 22:43:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37be51084fb891c6796079e693b73f6f882266a5e66211344173031e2b0c8ffd`  
		Last Modified: Thu, 28 Sep 2023 22:43:35 GMT  
		Size: 350.8 KB (350826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d867aa37ac50364bf4082dc48c7d4e1b88ead3164d47855e1bbc2ef3678cfc`  
		Last Modified: Thu, 28 Sep 2023 22:43:35 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147aa3899aa3307c28e185f5385015c7a5f15dfa42578a8a8eca88bf2f1e7e3e`  
		Last Modified: Thu, 28 Sep 2023 22:43:37 GMT  
		Size: 14.6 MB (14603949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:239c4a78d1bd0540a44003332119cf019e6ff839f4d303cd9801b1cc9e755ec4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17314598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b41f754b4ebb826dde7fb5c0c3c6048823add70f27a7f9c8d9f8ff1a9636ed2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:59:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 21:59:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 21:59:13 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 21:59:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 21:59:16 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 21:59:16 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 21:59:16 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 21:59:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 21:59:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 80
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 443
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 21:59:17 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 21:59:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1018057a600163b1c1b92c21ade975c631b2f8ccde66d524cfe0ecdac8e1920d`  
		Last Modified: Thu, 28 Sep 2023 21:59:43 GMT  
		Size: 347.6 KB (347613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec54680cbf2cb1a25285c82a7888498ab47d03a68db200a160d7162325a5be19`  
		Last Modified: Thu, 28 Sep 2023 21:59:43 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d087db4282d622690fce98f1d8802151567e43bfdd884a3e2a4d084701229a1`  
		Last Modified: Thu, 28 Sep 2023 21:59:45 GMT  
		Size: 13.8 MB (13814189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:85dd4fae9241ac3330e98e1d3b052d36b7ecbe1cd69b4c860454c84976426e70
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17043239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f78b426118e91fcb43786aa4c3003cd91ee86ab5f896516a885f964056b08cae`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:19:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 23:19:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 23:19:20 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 23:19:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 23:19:24 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 23:19:24 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 80
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 443
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 23:19:25 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 23:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66901ba48d0ee53cd827f4eb2cfd8b049cebba8c3d307b69760e1be917f69476`  
		Last Modified: Thu, 28 Sep 2023 23:19:46 GMT  
		Size: 344.4 KB (344448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dddeb3f6febb36993d8a51ad919784fd152aab5f6e17fe00d579916f32e42911`  
		Last Modified: Thu, 28 Sep 2023 23:19:46 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f936b2c0499a587b75385edfeb1d22b8f16ed05dca7dd0999ccc0635e1904a`  
		Last Modified: Thu, 28 Sep 2023 23:19:48 GMT  
		Size: 13.8 MB (13791383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:595e5490450c9ed29cc960149e2c265210e8444f3b3ea5ff2fab62d0da5ec3d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17163627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23f8ae4a1af151ac93d2945855095990774bc44f70af5c0e4b058dbb7e8b8c09`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:16:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 29 Sep 2023 01:16:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 29 Sep 2023 01:16:13 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 01:16:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 29 Sep 2023 01:16:15 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 29 Sep 2023 01:16:15 GMT
ENV XDG_DATA_HOME=/data
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 80
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 443
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 443/udp
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 2019
# Fri, 29 Sep 2023 01:16:16 GMT
WORKDIR /srv
# Fri, 29 Sep 2023 01:16:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f21cb0286edf1f5fefb4a859b414a446bb81baa9e8901fc8f4eca55a43aeeec`  
		Last Modified: Fri, 29 Sep 2023 01:16:34 GMT  
		Size: 360.6 KB (360643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5444b3f9419d06a4b77a65935a3b1c6e657c607bcfb9e3bd1abebe57eae36e6a`  
		Last Modified: Fri, 29 Sep 2023 01:16:34 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3485ef64f848b891981d59d52e0b092b261205ad787b38ae389e5ac39eed493f`  
		Last Modified: Fri, 29 Sep 2023 01:16:35 GMT  
		Size: 13.5 MB (13463646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:65084a14a1557b92af5b8ba6fcba9a7a710ed5caef1e2310f9622166608c9531
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16945195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73ba45deaa04c3feac6474c22204ac6f5ebc380b331ff7d585ecd196284459b3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:17:03 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 29 Sep 2023 02:17:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 29 Sep 2023 02:17:06 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 02:17:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 29 Sep 2023 02:17:13 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 29 Sep 2023 02:17:14 GMT
ENV XDG_DATA_HOME=/data
# Fri, 29 Sep 2023 02:17:15 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Fri, 29 Sep 2023 02:17:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 29 Sep 2023 02:17:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 29 Sep 2023 02:17:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 29 Sep 2023 02:17:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 29 Sep 2023 02:17:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 29 Sep 2023 02:17:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 29 Sep 2023 02:17:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 29 Sep 2023 02:17:21 GMT
EXPOSE 80
# Fri, 29 Sep 2023 02:17:21 GMT
EXPOSE 443
# Fri, 29 Sep 2023 02:17:22 GMT
EXPOSE 443/udp
# Fri, 29 Sep 2023 02:17:22 GMT
EXPOSE 2019
# Fri, 29 Sep 2023 02:17:24 GMT
WORKDIR /srv
# Fri, 29 Sep 2023 02:17:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa65cea7f5d70d1e203b851e43ad676e92f28c930ad32b6691e84ff9b5cda87`  
		Last Modified: Fri, 29 Sep 2023 02:18:03 GMT  
		Size: 362.2 KB (362182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7089a1d537371e29a65d106f43b45f2a0367d4d1db0eb7d6b7099f8ba05645`  
		Last Modified: Fri, 29 Sep 2023 02:18:01 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b93ab741fa6270144ea59d6a5fa3c4138286a569f246fdccd829b317b051f3a`  
		Last Modified: Fri, 29 Sep 2023 02:18:05 GMT  
		Size: 13.2 MB (13228998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:9e13bd2b56147eecc80f1fe1710e4350ea63d5edfb389fa89e2c6de06c08593a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17721238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2f0101e0f893afb763d99b2050dbf4d68a44aae29785af6c05af5a552b0c1a7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:19:38 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 22:19:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 22:19:39 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 22:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 22:19:42 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 22:19:42 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 80
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 443
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 22:19:44 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 22:19:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed3df874173df47ad0bd0ef67b8ee598c77921810d84a67fd2984c4f8151c91`  
		Last Modified: Thu, 28 Sep 2023 22:20:14 GMT  
		Size: 354.9 KB (354948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95a69c42a5c7fc6d73c00c7f6eb68522f3881aae55db4f85a8400e83b678b181`  
		Last Modified: Thu, 28 Sep 2023 22:20:14 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793016dc78c9794c627c07afcd2fb34af4ee470ee7fef1a1596eff0c59ba6659`  
		Last Modified: Thu, 28 Sep 2023 22:20:16 GMT  
		Size: 14.1 MB (14143684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.4-builder`

```console
$ docker pull caddy@sha256:33050f2d060171a04ef015097c2c431bebbef8e878f3d53db4adf2b93862e11d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4851; amd64
	-	windows version 10.0.20348.1970; amd64

### `caddy:2.7.4-builder` - linux; amd64

```console
$ docker pull caddy@sha256:1feb6492b7349402a4e1183682415d3a06e2c50998e55e05a23a7ff54104f12e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76961764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b60574c0fd570f746bcbc19dbe40382acf64d8088c9ec08e4e3ffe8e45f1f41`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:54:30 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:54:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:54:31 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 22:54:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 22:54:41 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 22:54:41 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 22:54:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:54:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 22:54:42 GMT
WORKDIR /go
# Fri, 29 Sep 2023 03:34:26 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Fri, 29 Sep 2023 03:34:26 GMT
ENV XCADDY_VERSION=v0.3.5
# Fri, 29 Sep 2023 03:34:26 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 03:34:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 29 Sep 2023 03:34:26 GMT
ENV XCADDY_SETCAP=1
# Fri, 29 Sep 2023 03:34:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 29 Sep 2023 03:34:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 29 Sep 2023 03:34:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc37b24bb09971feb8bf4882e861bce9db0c985a16a900adb0dc9de3f854243b`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 284.7 KB (284690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94517ad51c70c15adb540d431b757078be8f6214a2f1d2181afc9454fa65d281`  
		Last Modified: Thu, 28 Sep 2023 22:57:25 GMT  
		Size: 67.0 MB (67001967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2087470b845b2224ab3a61dafcdf2abbf9540f77be63368c3346b85ad2969fa6`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2981d490d3f8070423e8c669473d70f16909bf20541abd01afb263f326ce67c2`  
		Last Modified: Fri, 29 Sep 2023 03:34:47 GMT  
		Size: 5.0 MB (4970347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5299a94e56556856e0899be99ae303524bf1ef797eb49e7a358611d2d2b3f2`  
		Last Modified: Fri, 29 Sep 2023 03:34:46 GMT  
		Size: 1.3 MB (1302233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965d515814f9dd3e22b51ab0a9ea4f92d693760133d5cf9835588e835635e33d`  
		Last Modified: Fri, 29 Sep 2023 03:34:46 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:de02c3655970e860e68fd2840e08fd9656cebb751cf677a0982e67d8fc5538a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75403016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:636f8b72fc8192d5a346042bbf7f4b91636efcd463c388b6789b3d107346d09d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:55:22 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:55:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:55:22 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 21:55:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 21:55:37 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 21:55:37 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 21:55:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:55:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 21:55:37 GMT
WORKDIR /go
# Thu, 28 Sep 2023 21:59:22 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 28 Sep 2023 21:59:22 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 28 Sep 2023 21:59:22 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 21:59:23 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Sep 2023 21:59:23 GMT
ENV XCADDY_SETCAP=1
# Thu, 28 Sep 2023 21:59:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Sep 2023 21:59:24 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Sep 2023 21:59:24 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3da3b9e7a12f6bb6b7f56e9240c2c92ce8c9f5fd5ef3b3063b9a93d454919e`  
		Last Modified: Thu, 28 Sep 2023 21:58:05 GMT  
		Size: 284.9 KB (284887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db471c20f6642596c4a4eeca4a9348dd5a897aa1c3c2383fdf2fe2c2d6f1628`  
		Last Modified: Thu, 28 Sep 2023 21:58:18 GMT  
		Size: 65.8 MB (65758212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037298c7b9748af97a3a2906d0ebb91f2dd588f633a9e8f94e2e2b2a571ead1f`  
		Last Modified: Thu, 28 Sep 2023 21:58:05 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc923fd6dd565567ed402508a7420812a84f61bbecfa0e1f988bd9b2d7b772b`  
		Last Modified: Thu, 28 Sep 2023 22:00:17 GMT  
		Size: 5.0 MB (4965415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b055d2dc5239a960f27dc6b7a7dcbe9455defa55bfb2f41d11678f8d56591668`  
		Last Modified: Thu, 28 Sep 2023 22:00:17 GMT  
		Size: 1.2 MB (1248652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513967d31b50a4e0f6dd90e6b95fe92f327bab78e463b9ed3a5ab386b0796a0e`  
		Last Modified: Thu, 28 Sep 2023 22:00:16 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0ad7a5fed30df59cfe78f87f33dd741fcf2f9588b879cf4a999db785e17ce566
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74701068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e079a52ac41cfb0c167d0940a0ed4a65fac94f7728283be07ef1f9a9661f0cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:15:15 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:15:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:15:15 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 22:15:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 22:15:32 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 22:15:32 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 22:15:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:15:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 22:15:33 GMT
WORKDIR /go
# Thu, 28 Sep 2023 23:19:29 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 28 Sep 2023 23:19:30 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 28 Sep 2023 23:19:30 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 23:19:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Sep 2023 23:19:30 GMT
ENV XCADDY_SETCAP=1
# Thu, 28 Sep 2023 23:19:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Sep 2023 23:19:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Sep 2023 23:19:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e0aec75477c9a2cf6993e068fa40a45f0684d622ece61f54e6e02f9adebeb8`  
		Last Modified: Thu, 28 Sep 2023 22:19:29 GMT  
		Size: 284.1 KB (284076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b5f8bc58ed201378ca797f82d516632d7a864a26eb9f29c4314f061c253a5d`  
		Last Modified: Thu, 28 Sep 2023 22:19:45 GMT  
		Size: 65.8 MB (65758178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f7cae270f0f74f4af87304330243fa68170426cfac2ed3042885f518bd97fb`  
		Last Modified: Thu, 28 Sep 2023 22:19:29 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eda060e9fe56bc05ae87a1f04e06d4aa8e1b59f3143db70491a8b212f53eceb`  
		Last Modified: Thu, 28 Sep 2023 23:20:02 GMT  
		Size: 4.5 MB (4512263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56d31be6b7b9ec4232229a322a3e283089e9524392a0c2317b6870571a1f366`  
		Last Modified: Thu, 28 Sep 2023 23:20:01 GMT  
		Size: 1.2 MB (1246086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a8990e3e6f77162545c3d58676a3cded2b3260baa61c1c27f8255bb9afb3ba`  
		Last Modified: Thu, 28 Sep 2023 23:20:01 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:af47b965d6c7ddd0a5c0691ee19821ebec47fd96c8ceeb01ad0d12b2024be158
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73995021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf00a9d5850ec2c2a9fb5239a41e1f452b6798d56f52c5dcf8063e9bb8685055`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:03:38 GMT
RUN apk add --no-cache ca-certificates
# Fri, 29 Sep 2023 01:40:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Sep 2023 01:40:17 GMT
ENV GOLANG_VERSION=1.21.1
# Fri, 29 Sep 2023 01:40:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 29 Sep 2023 01:40:27 GMT
ENV GOTOOLCHAIN=local
# Fri, 29 Sep 2023 01:40:27 GMT
ENV GOPATH=/go
# Fri, 29 Sep 2023 01:40:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Sep 2023 01:40:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Fri, 29 Sep 2023 01:40:28 GMT
WORKDIR /go
# Fri, 29 Sep 2023 04:34:55 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Fri, 29 Sep 2023 04:34:55 GMT
ENV XCADDY_VERSION=v0.3.5
# Fri, 29 Sep 2023 04:34:55 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 04:34:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 29 Sep 2023 04:34:56 GMT
ENV XCADDY_SETCAP=1
# Fri, 29 Sep 2023 04:34:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 29 Sep 2023 04:34:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 29 Sep 2023 04:34:57 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c21914ef412ef71f6092299b025bf4d504a49024701bf684bc9efd218155c63`  
		Last Modified: Fri, 29 Sep 2023 01:03:48 GMT  
		Size: 286.3 KB (286306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5340c63a94930ed08fa6eea6fd627bdb38f335952054831c49716a27a8c8dfa0`  
		Last Modified: Fri, 29 Sep 2023 01:42:20 GMT  
		Size: 64.1 MB (64108807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3ca664c3732429a52e8e77a07dc94297fce7c851529dd6a572983f0bf99ae1`  
		Last Modified: Fri, 29 Sep 2023 01:42:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63283848834a5104fc3043f65de33b90d451c46dfbb2fa91874f41c1f0fcbdf2`  
		Last Modified: Fri, 29 Sep 2023 04:35:13 GMT  
		Size: 5.1 MB (5069067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a59c9f8a01ff922ae6c69e34038c2eb56dcc3bf0e7bc786804f9cabda360ec`  
		Last Modified: Fri, 29 Sep 2023 04:35:12 GMT  
		Size: 1.2 MB (1198450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a52b5eedc76b0958663cbb9be6e5ac8eaa51dff9778a4b4cff667120ab6da12`  
		Last Modified: Fri, 29 Sep 2023 04:35:12 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:55d9b4418c520166c8863db2e2993557191bf9caf6e028f7b04a5b8ab1b63a73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74205796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a71360173a10dc6951ba63109fda1b23d9e5356b14225bf346845fa455513541`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:13:11 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:13:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:13:12 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 22:13:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 22:13:47 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 22:13:48 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 22:13:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:13:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 22:13:52 GMT
WORKDIR /go
# Fri, 29 Sep 2023 02:17:36 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Fri, 29 Sep 2023 02:17:37 GMT
ENV XCADDY_VERSION=v0.3.5
# Fri, 29 Sep 2023 02:17:37 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 02:17:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 29 Sep 2023 02:17:38 GMT
ENV XCADDY_SETCAP=1
# Fri, 29 Sep 2023 02:17:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 29 Sep 2023 02:17:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 29 Sep 2023 02:17:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc67971d1767eae5019ffeaf8f893e6d81dbba50bde347da0c0433c56e3f2a3`  
		Last Modified: Thu, 28 Sep 2023 22:18:17 GMT  
		Size: 286.7 KB (286659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a20f495e184de0c46bb781c57dd99e2cfc30deaa14db48a8f0cc95fc20ed28b`  
		Last Modified: Thu, 28 Sep 2023 22:18:37 GMT  
		Size: 64.1 MB (64116623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9a2fd37dab154ff5a7a7f14553c32641833c766ad5fb9ab737767a24048145`  
		Last Modified: Thu, 28 Sep 2023 22:18:16 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f689a2a610338f9a37a48fa810fa16f44dc7777786d0ed4b2df7e7e4e01cb38`  
		Last Modified: Fri, 29 Sep 2023 02:18:20 GMT  
		Size: 5.3 MB (5269263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322aacb09420bf02551659cc5b56c905f8fc7944553e6c3b1c85b5eb92547d7f`  
		Last Modified: Fri, 29 Sep 2023 02:18:20 GMT  
		Size: 1.2 MB (1186183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490b3f0289dc37c4f918f9f29f48774d57525c152a6ee4708b66c38798b2421c`  
		Last Modified: Fri, 29 Sep 2023 02:18:19 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-builder` - linux; s390x

```console
$ docker pull caddy@sha256:b438b3cf1ad85b0cc2fe8f5319ac062a52640a6a231f4858917e081b1e773001
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76102753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1788e10f8a6f8ccdc56c8b2c4b5a6ebc9387eb3b66b2b9d2dd1f18b74223f3c2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:38:54 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:38:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:38:54 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 21:39:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 21:39:15 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 21:39:15 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 21:39:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:39:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 21:39:15 GMT
WORKDIR /go
# Thu, 28 Sep 2023 22:19:51 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 28 Sep 2023 22:19:51 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_SETCAP=1
# Thu, 28 Sep 2023 22:19:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Sep 2023 22:19:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Sep 2023 22:19:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0721f16693d4788a5add1bd0b22764c8887cdc62b24edf388ae895df440f4aa9`  
		Last Modified: Thu, 28 Sep 2023 21:46:22 GMT  
		Size: 285.1 KB (285095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40248878cac53fafdd0778844ffa03633e8f3cd73c5d5136e02da42557cb26f6`  
		Last Modified: Thu, 28 Sep 2023 21:46:16 GMT  
		Size: 66.2 MB (66224373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3d28e3790630932107b3adf42c8b1564c57d0ab97f15a759b1a8f835ee4101`  
		Last Modified: Thu, 28 Sep 2023 21:46:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d382e103bfc732fc0a4c2b972100a5426b9a8e99cd21d22eddb196e5bb029206`  
		Last Modified: Thu, 28 Sep 2023 22:20:30 GMT  
		Size: 5.1 MB (5115228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3232faabff7e982d010fd0c3775d8c4a6b80e55bc3acdb0af1e63077c07656`  
		Last Modified: Thu, 28 Sep 2023 22:20:30 GMT  
		Size: 1.3 MB (1262392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff69fb680d5cc18f0d5150ac6c2922176848b00c8456922df5843f6e1c993cc7`  
		Last Modified: Thu, 28 Sep 2023 22:20:29 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-builder` - windows version 10.0.17763.4851; amd64

```console
$ docker pull caddy@sha256:95c666eeefee6beeed59b530714de1ebdd28f2ba6ad0703b37f26b729f5e3793
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2113168904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9bf61498c4479dace7e2fa1c8c4c29a0a0722e06138f3d5fa9226287d83f2d6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 01:39:14 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Sep 2023 01:39:15 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Sep 2023 01:39:16 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Sep 2023 01:39:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Sep 2023 01:40:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:40:50 GMT
ENV GOPATH=C:\go
# Wed, 13 Sep 2023 01:41:53 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Sep 2023 01:41:54 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 13 Sep 2023 01:45:02 GMT
RUN $url = 'https://dl.google.com/go/go1.21.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '10a4f5b63215d11d1770453733dbcbf024f3f74872f84e28d7ea59f0250316c6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:45:04 GMT
WORKDIR C:\go
# Wed, 13 Sep 2023 05:35:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:35:07 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 13 Sep 2023 05:35:07 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:35:08 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Sep 2023 05:36:24 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Sep 2023 05:36:25 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cdfacf538899a08fcbb1c6b92df02725dbfcc05c593d6f310371baf9cc5c28b`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaa9f7bc4f06074cd41e4c8f38f9019d00b30116cc81e7e57bb201a2cddbe76`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa369f25c61f03e75b9090231c21b059562345a9aa5b4710c1d4bd043232a46`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1338c790efe798520cb633291aa3dbf3b37552cfbd91737d2539bad7bcac882c`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af230316f5f5bdfd37af05e436ffaadf28ac7a31d97f315dbfb2924c4d1ca3c`  
		Last Modified: Wed, 13 Sep 2023 02:16:54 GMT  
		Size: 25.6 MB (25567707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606d89c5df48922aee4ed7b88afc9f9fc270b462891c28d20b75199f2726201e`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f90ec51ca481c33d4e3887adf74f8b37c2f82af9e60290d2755f34c55b70e9c`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 220.5 KB (220461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9741d5460d3c8c14c62fd6990864968f75fbb895dfd099803a72c140739264b`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac37fd27ee4a5046c706042d53bb4a5b5e2e9ac0ec76a27142f42a55f09c31aa`  
		Last Modified: Wed, 13 Sep 2023 02:17:12 GMT  
		Size: 69.3 MB (69345076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4460c6474f9af5dc17adefba85607fa63b6072fc39250bcf433f458742fd0987`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 1.6 KB (1559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8840f55013cb306bc30661534c9618bdfda370c585b638deb791ba84fbceee9c`  
		Last Modified: Wed, 13 Sep 2023 05:38:30 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f45db9ea611a79882cee37d8b10da3ddf761d7f9ae24bf1fe0cfdb58497a6ae`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51195ebf7ad1d0ac3972b387896050e20749e6e0bb65d49a1907f49ab5cec5f2`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56989aaa5684bbc2d72ae4bb645d01d4dd0c63d35c8f4515b4c8587d6611d519`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae11f7d16342cb14a92f5b67ee9ce0eeab5805f76829bedd3735c0eec9b1f744`  
		Last Modified: Wed, 13 Sep 2023 05:38:29 GMT  
		Size: 1.7 MB (1687175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f520ac11e32bd8e755e12beaef19d397e709b5d8b007fb948658b974af6c7e2`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-builder` - windows version 10.0.20348.1970; amd64

```console
$ docker pull caddy@sha256:0a56e01d98805d99f891740e4644f1afb62f725060c36ad3cdcad27f452c3952
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1934132962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f26855783f570cd07fa203aa143ae0ddab1ef24e3a100e66f3cac124f008c0e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 01:35:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 01:35:30 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Sep 2023 01:35:31 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Sep 2023 01:35:32 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Sep 2023 01:35:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Sep 2023 01:36:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:36:16 GMT
ENV GOPATH=C:\go
# Wed, 13 Sep 2023 01:36:38 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Sep 2023 01:36:39 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 13 Sep 2023 01:38:59 GMT
RUN $url = 'https://dl.google.com/go/go1.21.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '10a4f5b63215d11d1770453733dbcbf024f3f74872f84e28d7ea59f0250316c6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:39:01 GMT
WORKDIR C:\go
# Wed, 13 Sep 2023 05:36:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:36:35 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 13 Sep 2023 05:36:35 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:36:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Sep 2023 05:37:04 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Sep 2023 05:37:05 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f40969dbf1e035a6c49e7c40b216960e3ee98ec3b76f76f9fe4498d0110bee`  
		Last Modified: Wed, 13 Sep 2023 02:15:22 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a846e03791bc3a58cfed3f02e65f87e18a5f5f416405456368e8a0ec4f9364`  
		Last Modified: Wed, 13 Sep 2023 02:15:21 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bc2015fc36cda903dca8edfdc1c87b219753af24c4ff5a95db324fb0e1cc0c`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d1910b6e6c60b5b71a12c43af94e08cf0ba20718d9a6c16ad07734f4977311`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46353fb4c6176aee49921617b1cd3ac7dcbca49d4d7a734cb5ddef177b8354b2`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f70d11added5b27b9707831ac76b04e95d4fa92b406f09532472fa350df630`  
		Last Modified: Wed, 13 Sep 2023 02:15:25 GMT  
		Size: 25.6 MB (25551011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892bff3fc5428691c1922057d675611c2b50e50cf3c6d22c2054b270861bc53c`  
		Last Modified: Wed, 13 Sep 2023 02:15:17 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ee07c029ab53a292bbb7320390d24d86b21159530b1b77d968b2b5416e8f67`  
		Last Modified: Wed, 13 Sep 2023 02:15:18 GMT  
		Size: 277.5 KB (277484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02fba082f03e26936264b99820372415048914f7ffd7f2469a28d3c0edd9224d`  
		Last Modified: Wed, 13 Sep 2023 02:15:17 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5004044396790144a82fbe98df119c5d7ae1a9abaac51c4cf0813b0d43f3f58`  
		Last Modified: Wed, 13 Sep 2023 02:15:43 GMT  
		Size: 69.3 MB (69336704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d84e4497229ea334095327a0106b2812e1dd5261c636cb1461fd698efffc4b6`  
		Last Modified: Wed, 13 Sep 2023 02:15:17 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20bad1e33f8c7089f46cd563d46ed621e589ef95c6dd41ba7569e5649804f136`  
		Last Modified: Wed, 13 Sep 2023 05:38:48 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c872ac2c7792d27826114f417d42ecbf945599d2b446775726d828ee99aab2c0`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6aff62b7b35fb324b51b0049e8a19ba51736b4f6ba1bfd92511f117e51e794`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77347ece80c37436fa82eb033a03166eb1c797e7341a6b642bf3bb80c12e36d5`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d1c7afb782c38442247cae60bbf9b16689939a03c80d4394125a9ff0af783c`  
		Last Modified: Wed, 13 Sep 2023 05:38:47 GMT  
		Size: 1.7 MB (1675830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191cef90893a643b034d031ee3e41cd4daa1b59c1d2d0e2dc1640f7bedb6c55a`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.4-builder-alpine`

```console
$ docker pull caddy@sha256:308ffbaa017c0bb533cfe7442c49460b33193a43192b2bb9744a0fa7080a50c3
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
$ docker pull caddy@sha256:1feb6492b7349402a4e1183682415d3a06e2c50998e55e05a23a7ff54104f12e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76961764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b60574c0fd570f746bcbc19dbe40382acf64d8088c9ec08e4e3ffe8e45f1f41`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:54:30 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:54:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:54:31 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 22:54:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 22:54:41 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 22:54:41 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 22:54:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:54:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 22:54:42 GMT
WORKDIR /go
# Fri, 29 Sep 2023 03:34:26 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Fri, 29 Sep 2023 03:34:26 GMT
ENV XCADDY_VERSION=v0.3.5
# Fri, 29 Sep 2023 03:34:26 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 03:34:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 29 Sep 2023 03:34:26 GMT
ENV XCADDY_SETCAP=1
# Fri, 29 Sep 2023 03:34:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 29 Sep 2023 03:34:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 29 Sep 2023 03:34:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc37b24bb09971feb8bf4882e861bce9db0c985a16a900adb0dc9de3f854243b`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 284.7 KB (284690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94517ad51c70c15adb540d431b757078be8f6214a2f1d2181afc9454fa65d281`  
		Last Modified: Thu, 28 Sep 2023 22:57:25 GMT  
		Size: 67.0 MB (67001967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2087470b845b2224ab3a61dafcdf2abbf9540f77be63368c3346b85ad2969fa6`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2981d490d3f8070423e8c669473d70f16909bf20541abd01afb263f326ce67c2`  
		Last Modified: Fri, 29 Sep 2023 03:34:47 GMT  
		Size: 5.0 MB (4970347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5299a94e56556856e0899be99ae303524bf1ef797eb49e7a358611d2d2b3f2`  
		Last Modified: Fri, 29 Sep 2023 03:34:46 GMT  
		Size: 1.3 MB (1302233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965d515814f9dd3e22b51ab0a9ea4f92d693760133d5cf9835588e835635e33d`  
		Last Modified: Fri, 29 Sep 2023 03:34:46 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:de02c3655970e860e68fd2840e08fd9656cebb751cf677a0982e67d8fc5538a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75403016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:636f8b72fc8192d5a346042bbf7f4b91636efcd463c388b6789b3d107346d09d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:55:22 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:55:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:55:22 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 21:55:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 21:55:37 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 21:55:37 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 21:55:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:55:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 21:55:37 GMT
WORKDIR /go
# Thu, 28 Sep 2023 21:59:22 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 28 Sep 2023 21:59:22 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 28 Sep 2023 21:59:22 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 21:59:23 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Sep 2023 21:59:23 GMT
ENV XCADDY_SETCAP=1
# Thu, 28 Sep 2023 21:59:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Sep 2023 21:59:24 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Sep 2023 21:59:24 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3da3b9e7a12f6bb6b7f56e9240c2c92ce8c9f5fd5ef3b3063b9a93d454919e`  
		Last Modified: Thu, 28 Sep 2023 21:58:05 GMT  
		Size: 284.9 KB (284887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db471c20f6642596c4a4eeca4a9348dd5a897aa1c3c2383fdf2fe2c2d6f1628`  
		Last Modified: Thu, 28 Sep 2023 21:58:18 GMT  
		Size: 65.8 MB (65758212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037298c7b9748af97a3a2906d0ebb91f2dd588f633a9e8f94e2e2b2a571ead1f`  
		Last Modified: Thu, 28 Sep 2023 21:58:05 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc923fd6dd565567ed402508a7420812a84f61bbecfa0e1f988bd9b2d7b772b`  
		Last Modified: Thu, 28 Sep 2023 22:00:17 GMT  
		Size: 5.0 MB (4965415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b055d2dc5239a960f27dc6b7a7dcbe9455defa55bfb2f41d11678f8d56591668`  
		Last Modified: Thu, 28 Sep 2023 22:00:17 GMT  
		Size: 1.2 MB (1248652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513967d31b50a4e0f6dd90e6b95fe92f327bab78e463b9ed3a5ab386b0796a0e`  
		Last Modified: Thu, 28 Sep 2023 22:00:16 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0ad7a5fed30df59cfe78f87f33dd741fcf2f9588b879cf4a999db785e17ce566
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74701068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e079a52ac41cfb0c167d0940a0ed4a65fac94f7728283be07ef1f9a9661f0cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:15:15 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:15:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:15:15 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 22:15:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 22:15:32 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 22:15:32 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 22:15:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:15:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 22:15:33 GMT
WORKDIR /go
# Thu, 28 Sep 2023 23:19:29 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 28 Sep 2023 23:19:30 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 28 Sep 2023 23:19:30 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 23:19:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Sep 2023 23:19:30 GMT
ENV XCADDY_SETCAP=1
# Thu, 28 Sep 2023 23:19:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Sep 2023 23:19:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Sep 2023 23:19:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e0aec75477c9a2cf6993e068fa40a45f0684d622ece61f54e6e02f9adebeb8`  
		Last Modified: Thu, 28 Sep 2023 22:19:29 GMT  
		Size: 284.1 KB (284076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b5f8bc58ed201378ca797f82d516632d7a864a26eb9f29c4314f061c253a5d`  
		Last Modified: Thu, 28 Sep 2023 22:19:45 GMT  
		Size: 65.8 MB (65758178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f7cae270f0f74f4af87304330243fa68170426cfac2ed3042885f518bd97fb`  
		Last Modified: Thu, 28 Sep 2023 22:19:29 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eda060e9fe56bc05ae87a1f04e06d4aa8e1b59f3143db70491a8b212f53eceb`  
		Last Modified: Thu, 28 Sep 2023 23:20:02 GMT  
		Size: 4.5 MB (4512263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56d31be6b7b9ec4232229a322a3e283089e9524392a0c2317b6870571a1f366`  
		Last Modified: Thu, 28 Sep 2023 23:20:01 GMT  
		Size: 1.2 MB (1246086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a8990e3e6f77162545c3d58676a3cded2b3260baa61c1c27f8255bb9afb3ba`  
		Last Modified: Thu, 28 Sep 2023 23:20:01 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:af47b965d6c7ddd0a5c0691ee19821ebec47fd96c8ceeb01ad0d12b2024be158
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73995021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf00a9d5850ec2c2a9fb5239a41e1f452b6798d56f52c5dcf8063e9bb8685055`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:03:38 GMT
RUN apk add --no-cache ca-certificates
# Fri, 29 Sep 2023 01:40:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Sep 2023 01:40:17 GMT
ENV GOLANG_VERSION=1.21.1
# Fri, 29 Sep 2023 01:40:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 29 Sep 2023 01:40:27 GMT
ENV GOTOOLCHAIN=local
# Fri, 29 Sep 2023 01:40:27 GMT
ENV GOPATH=/go
# Fri, 29 Sep 2023 01:40:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Sep 2023 01:40:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Fri, 29 Sep 2023 01:40:28 GMT
WORKDIR /go
# Fri, 29 Sep 2023 04:34:55 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Fri, 29 Sep 2023 04:34:55 GMT
ENV XCADDY_VERSION=v0.3.5
# Fri, 29 Sep 2023 04:34:55 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 04:34:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 29 Sep 2023 04:34:56 GMT
ENV XCADDY_SETCAP=1
# Fri, 29 Sep 2023 04:34:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 29 Sep 2023 04:34:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 29 Sep 2023 04:34:57 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c21914ef412ef71f6092299b025bf4d504a49024701bf684bc9efd218155c63`  
		Last Modified: Fri, 29 Sep 2023 01:03:48 GMT  
		Size: 286.3 KB (286306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5340c63a94930ed08fa6eea6fd627bdb38f335952054831c49716a27a8c8dfa0`  
		Last Modified: Fri, 29 Sep 2023 01:42:20 GMT  
		Size: 64.1 MB (64108807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3ca664c3732429a52e8e77a07dc94297fce7c851529dd6a572983f0bf99ae1`  
		Last Modified: Fri, 29 Sep 2023 01:42:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63283848834a5104fc3043f65de33b90d451c46dfbb2fa91874f41c1f0fcbdf2`  
		Last Modified: Fri, 29 Sep 2023 04:35:13 GMT  
		Size: 5.1 MB (5069067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a59c9f8a01ff922ae6c69e34038c2eb56dcc3bf0e7bc786804f9cabda360ec`  
		Last Modified: Fri, 29 Sep 2023 04:35:12 GMT  
		Size: 1.2 MB (1198450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a52b5eedc76b0958663cbb9be6e5ac8eaa51dff9778a4b4cff667120ab6da12`  
		Last Modified: Fri, 29 Sep 2023 04:35:12 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:55d9b4418c520166c8863db2e2993557191bf9caf6e028f7b04a5b8ab1b63a73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74205796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a71360173a10dc6951ba63109fda1b23d9e5356b14225bf346845fa455513541`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:13:11 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:13:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:13:12 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 22:13:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 22:13:47 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 22:13:48 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 22:13:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:13:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 22:13:52 GMT
WORKDIR /go
# Fri, 29 Sep 2023 02:17:36 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Fri, 29 Sep 2023 02:17:37 GMT
ENV XCADDY_VERSION=v0.3.5
# Fri, 29 Sep 2023 02:17:37 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 02:17:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 29 Sep 2023 02:17:38 GMT
ENV XCADDY_SETCAP=1
# Fri, 29 Sep 2023 02:17:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 29 Sep 2023 02:17:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 29 Sep 2023 02:17:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc67971d1767eae5019ffeaf8f893e6d81dbba50bde347da0c0433c56e3f2a3`  
		Last Modified: Thu, 28 Sep 2023 22:18:17 GMT  
		Size: 286.7 KB (286659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a20f495e184de0c46bb781c57dd99e2cfc30deaa14db48a8f0cc95fc20ed28b`  
		Last Modified: Thu, 28 Sep 2023 22:18:37 GMT  
		Size: 64.1 MB (64116623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9a2fd37dab154ff5a7a7f14553c32641833c766ad5fb9ab737767a24048145`  
		Last Modified: Thu, 28 Sep 2023 22:18:16 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f689a2a610338f9a37a48fa810fa16f44dc7777786d0ed4b2df7e7e4e01cb38`  
		Last Modified: Fri, 29 Sep 2023 02:18:20 GMT  
		Size: 5.3 MB (5269263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322aacb09420bf02551659cc5b56c905f8fc7944553e6c3b1c85b5eb92547d7f`  
		Last Modified: Fri, 29 Sep 2023 02:18:20 GMT  
		Size: 1.2 MB (1186183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490b3f0289dc37c4f918f9f29f48774d57525c152a6ee4708b66c38798b2421c`  
		Last Modified: Fri, 29 Sep 2023 02:18:19 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:b438b3cf1ad85b0cc2fe8f5319ac062a52640a6a231f4858917e081b1e773001
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76102753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1788e10f8a6f8ccdc56c8b2c4b5a6ebc9387eb3b66b2b9d2dd1f18b74223f3c2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:38:54 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:38:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:38:54 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 21:39:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 21:39:15 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 21:39:15 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 21:39:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:39:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 21:39:15 GMT
WORKDIR /go
# Thu, 28 Sep 2023 22:19:51 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 28 Sep 2023 22:19:51 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_SETCAP=1
# Thu, 28 Sep 2023 22:19:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Sep 2023 22:19:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Sep 2023 22:19:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0721f16693d4788a5add1bd0b22764c8887cdc62b24edf388ae895df440f4aa9`  
		Last Modified: Thu, 28 Sep 2023 21:46:22 GMT  
		Size: 285.1 KB (285095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40248878cac53fafdd0778844ffa03633e8f3cd73c5d5136e02da42557cb26f6`  
		Last Modified: Thu, 28 Sep 2023 21:46:16 GMT  
		Size: 66.2 MB (66224373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3d28e3790630932107b3adf42c8b1564c57d0ab97f15a759b1a8f835ee4101`  
		Last Modified: Thu, 28 Sep 2023 21:46:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d382e103bfc732fc0a4c2b972100a5426b9a8e99cd21d22eddb196e5bb029206`  
		Last Modified: Thu, 28 Sep 2023 22:20:30 GMT  
		Size: 5.1 MB (5115228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3232faabff7e982d010fd0c3775d8c4a6b80e55bc3acdb0af1e63077c07656`  
		Last Modified: Thu, 28 Sep 2023 22:20:30 GMT  
		Size: 1.3 MB (1262392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff69fb680d5cc18f0d5150ac6c2922176848b00c8456922df5843f6e1c993cc7`  
		Last Modified: Thu, 28 Sep 2023 22:20:29 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.4-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:1a9280c29c9c558a4f0870515605df3716ff711eeef8f648d8207f81f3577c8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `caddy:2.7.4-builder-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull caddy@sha256:95c666eeefee6beeed59b530714de1ebdd28f2ba6ad0703b37f26b729f5e3793
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2113168904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9bf61498c4479dace7e2fa1c8c4c29a0a0722e06138f3d5fa9226287d83f2d6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 01:39:14 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Sep 2023 01:39:15 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Sep 2023 01:39:16 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Sep 2023 01:39:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Sep 2023 01:40:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:40:50 GMT
ENV GOPATH=C:\go
# Wed, 13 Sep 2023 01:41:53 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Sep 2023 01:41:54 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 13 Sep 2023 01:45:02 GMT
RUN $url = 'https://dl.google.com/go/go1.21.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '10a4f5b63215d11d1770453733dbcbf024f3f74872f84e28d7ea59f0250316c6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:45:04 GMT
WORKDIR C:\go
# Wed, 13 Sep 2023 05:35:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:35:07 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 13 Sep 2023 05:35:07 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:35:08 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Sep 2023 05:36:24 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Sep 2023 05:36:25 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cdfacf538899a08fcbb1c6b92df02725dbfcc05c593d6f310371baf9cc5c28b`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaa9f7bc4f06074cd41e4c8f38f9019d00b30116cc81e7e57bb201a2cddbe76`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa369f25c61f03e75b9090231c21b059562345a9aa5b4710c1d4bd043232a46`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1338c790efe798520cb633291aa3dbf3b37552cfbd91737d2539bad7bcac882c`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af230316f5f5bdfd37af05e436ffaadf28ac7a31d97f315dbfb2924c4d1ca3c`  
		Last Modified: Wed, 13 Sep 2023 02:16:54 GMT  
		Size: 25.6 MB (25567707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606d89c5df48922aee4ed7b88afc9f9fc270b462891c28d20b75199f2726201e`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f90ec51ca481c33d4e3887adf74f8b37c2f82af9e60290d2755f34c55b70e9c`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 220.5 KB (220461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9741d5460d3c8c14c62fd6990864968f75fbb895dfd099803a72c140739264b`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac37fd27ee4a5046c706042d53bb4a5b5e2e9ac0ec76a27142f42a55f09c31aa`  
		Last Modified: Wed, 13 Sep 2023 02:17:12 GMT  
		Size: 69.3 MB (69345076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4460c6474f9af5dc17adefba85607fa63b6072fc39250bcf433f458742fd0987`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 1.6 KB (1559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8840f55013cb306bc30661534c9618bdfda370c585b638deb791ba84fbceee9c`  
		Last Modified: Wed, 13 Sep 2023 05:38:30 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f45db9ea611a79882cee37d8b10da3ddf761d7f9ae24bf1fe0cfdb58497a6ae`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51195ebf7ad1d0ac3972b387896050e20749e6e0bb65d49a1907f49ab5cec5f2`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56989aaa5684bbc2d72ae4bb645d01d4dd0c63d35c8f4515b4c8587d6611d519`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae11f7d16342cb14a92f5b67ee9ce0eeab5805f76829bedd3735c0eec9b1f744`  
		Last Modified: Wed, 13 Sep 2023 05:38:29 GMT  
		Size: 1.7 MB (1687175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f520ac11e32bd8e755e12beaef19d397e709b5d8b007fb948658b974af6c7e2`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.4-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:e27807e1af059f2f978b562de306e9d021538db7c394f3838deb1d734efc29ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1970; amd64

### `caddy:2.7.4-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1970; amd64

```console
$ docker pull caddy@sha256:0a56e01d98805d99f891740e4644f1afb62f725060c36ad3cdcad27f452c3952
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1934132962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f26855783f570cd07fa203aa143ae0ddab1ef24e3a100e66f3cac124f008c0e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 01:35:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 01:35:30 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Sep 2023 01:35:31 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Sep 2023 01:35:32 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Sep 2023 01:35:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Sep 2023 01:36:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:36:16 GMT
ENV GOPATH=C:\go
# Wed, 13 Sep 2023 01:36:38 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Sep 2023 01:36:39 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 13 Sep 2023 01:38:59 GMT
RUN $url = 'https://dl.google.com/go/go1.21.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '10a4f5b63215d11d1770453733dbcbf024f3f74872f84e28d7ea59f0250316c6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:39:01 GMT
WORKDIR C:\go
# Wed, 13 Sep 2023 05:36:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:36:35 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 13 Sep 2023 05:36:35 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:36:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Sep 2023 05:37:04 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Sep 2023 05:37:05 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f40969dbf1e035a6c49e7c40b216960e3ee98ec3b76f76f9fe4498d0110bee`  
		Last Modified: Wed, 13 Sep 2023 02:15:22 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a846e03791bc3a58cfed3f02e65f87e18a5f5f416405456368e8a0ec4f9364`  
		Last Modified: Wed, 13 Sep 2023 02:15:21 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bc2015fc36cda903dca8edfdc1c87b219753af24c4ff5a95db324fb0e1cc0c`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d1910b6e6c60b5b71a12c43af94e08cf0ba20718d9a6c16ad07734f4977311`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46353fb4c6176aee49921617b1cd3ac7dcbca49d4d7a734cb5ddef177b8354b2`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f70d11added5b27b9707831ac76b04e95d4fa92b406f09532472fa350df630`  
		Last Modified: Wed, 13 Sep 2023 02:15:25 GMT  
		Size: 25.6 MB (25551011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892bff3fc5428691c1922057d675611c2b50e50cf3c6d22c2054b270861bc53c`  
		Last Modified: Wed, 13 Sep 2023 02:15:17 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ee07c029ab53a292bbb7320390d24d86b21159530b1b77d968b2b5416e8f67`  
		Last Modified: Wed, 13 Sep 2023 02:15:18 GMT  
		Size: 277.5 KB (277484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02fba082f03e26936264b99820372415048914f7ffd7f2469a28d3c0edd9224d`  
		Last Modified: Wed, 13 Sep 2023 02:15:17 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5004044396790144a82fbe98df119c5d7ae1a9abaac51c4cf0813b0d43f3f58`  
		Last Modified: Wed, 13 Sep 2023 02:15:43 GMT  
		Size: 69.3 MB (69336704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d84e4497229ea334095327a0106b2812e1dd5261c636cb1461fd698efffc4b6`  
		Last Modified: Wed, 13 Sep 2023 02:15:17 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20bad1e33f8c7089f46cd563d46ed621e589ef95c6dd41ba7569e5649804f136`  
		Last Modified: Wed, 13 Sep 2023 05:38:48 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c872ac2c7792d27826114f417d42ecbf945599d2b446775726d828ee99aab2c0`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6aff62b7b35fb324b51b0049e8a19ba51736b4f6ba1bfd92511f117e51e794`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77347ece80c37436fa82eb033a03166eb1c797e7341a6b642bf3bb80c12e36d5`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d1c7afb782c38442247cae60bbf9b16689939a03c80d4394125a9ff0af783c`  
		Last Modified: Wed, 13 Sep 2023 05:38:47 GMT  
		Size: 1.7 MB (1675830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191cef90893a643b034d031ee3e41cd4daa1b59c1d2d0e2dc1640f7bedb6c55a`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.4-windowsservercore`

```console
$ docker pull caddy@sha256:4e0879a2422f5309c4ed33c36438e076aa198dc89228e2dc8a56369b86fac7a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4851; amd64
	-	windows version 10.0.20348.1970; amd64

### `caddy:2.7.4-windowsservercore` - windows version 10.0.17763.4851; amd64

```console
$ docker pull caddy@sha256:3f230e8c687c5611e74c84c3ec6f7ef7844b3cc3443d9302e9bb778e6210bfe2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2032252342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea189389e39a38d33c2124e3c02e0a9bc2f3168e5605fa8a909e749ac52fc3f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:30:52 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:30:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:32:00 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:32:02 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:32:04 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:32:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:32:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:32:08 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:32:09 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:33:07 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:33:07 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2bc90334de89082943edb24d5f52a3bb36ef134c17a417ba45cc4e122be3b2`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 465.0 KB (465015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba1c9fb8dedf070862eb0526393862bb5a0f2c87a87bc3864b9b24b11af5524`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5249ade277243b1b7f8c198de7d036f2e106b8a679d777b7bfc885af7b9b76`  
		Last Modified: Wed, 13 Sep 2023 05:37:46 GMT  
		Size: 15.2 MB (15176891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224a0aed4c02b4a48f633ac01c40e020d4e8fbc32fe8896d93032f9d72f50cda`  
		Last Modified: Wed, 13 Sep 2023 05:37:42 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fc1c10b7da22b1e9a26f059801a53ce4ce22e7d24ab14ec56d343a806f3bc2`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bd26e7302c16a8d83a8a6b5d9d263b804279f2b4c7d2fcea59a97c1e187648`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f69e667aa7c5e5a21f7d8a8cdd213b9d20a8a0c790dd18fe51d4df9e5b08a7`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e456b9da79a468c972d487e55e3628f8a8917f78948550c359afc891a5ad24a`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bc4af3e90793180c1ed8b8b9ac6866e24a5de16881f363dacf0ecf47396c8`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0289dff328d597d94fcd8612bd4a726573e13f780790744c5c6f4b40b49823`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52ff2438c88a58e8be33368f668557c92bcfdc503bd58025d081c7b88ec88b`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0f1c855afa9fd7bcf5ded632c161f2ff013f4b08f5c233fa3bdf3d13701467`  
		Last Modified: Wed, 13 Sep 2023 05:37:38 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2e0bf79eee4bbd609b5a111793e394f22ad86eb897cf85c6df2c45d9a8d777`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff797288117550c2b80f9a39dd5a04cb449defc2660cf6a7589618b8d3606464`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa0d1665270ae2e22844b2386842b1deab36f8936506db82df0ec69dc72fb84`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c867297eb9d01dfe100695ae10a0c67bd38f2124de0ee7446d1e66b6dede5c06`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee97f69cfbd31f5a098d45934b159384d8e986d860ad3007140beee338aa4533`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b741c4ffade19f3d712c3fb839c3ae7f1ae4e39e5f777a2b24917b5e630d0f86`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 256.7 KB (256675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a415b22709a225227fa7ce65d7767f3f820c7e9e445b0d718dfb68ae2249832`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.4-windowsservercore` - windows version 10.0.20348.1970; amd64

```console
$ docker pull caddy@sha256:76214fe6feb9f96f1c46334c01e1b9d310eb2e745bb08ba4130547b2147f3677
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1853253940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f0e585ea0797bdd13d148afed1e86161022e8cf2a79d11337f9d4dde0a8efe6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 01:35:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:33:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:33:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:34:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:34:25 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:34:26 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:34:27 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:34:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:34:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:34:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:34:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:34:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:34:33 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:34:34 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:34:35 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:34:36 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:34:56 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:34:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f40969dbf1e035a6c49e7c40b216960e3ee98ec3b76f76f9fe4498d0110bee`  
		Last Modified: Wed, 13 Sep 2023 02:15:22 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2d313a26784edb67b74292171891c0393ea119a53238e09150b5b7bc52371f`  
		Last Modified: Wed, 13 Sep 2023 05:38:08 GMT  
		Size: 483.0 KB (482985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb50376a60c42178e92d96a048b0e7f2dbc2cafe73274ab76722cda86fb32ee`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeecad99d9c5b378a623153b24130f8c36442e9a48ef6a48f878c5f585a66bd4`  
		Last Modified: Wed, 13 Sep 2023 05:38:11 GMT  
		Size: 15.2 MB (15183860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6b7a19981a71c15e39afbc3a52ed5f0c065f77c1ccd55a88e5f1b51af88753`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd7340889e9a6bfc8018c7709595b75ef962cf2608d14398ffbc90b90804a04`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7537acdfe48467d248afb6a69dad6bdb09c62617600305d2b2adb8a45ece2f`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf3cb277ba29189d90269123acd401fa787771fb095f2f2ec532be7bba2a025`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64eb5cc4069279b73a665e35bf526fa42558af1a3a71fc13d76913846d96818`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74348cf2ecbfe3a00df246034f9ab755418e8584b24113c9d327fc80cb134829`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa3fef62dce81d37fff2c621b94314d2aa9d0318523407b0a1d7d2b1e079234`  
		Last Modified: Wed, 13 Sep 2023 05:38:04 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d033d5a006e7fa969026194ef48446c840a891ad252f0316d32bc01843f0e4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbef09c0840262b42ba39068c868fc9b353bed78bb7de251e953289149e9a64e`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea46de371cf13fdb02566c79fc3a22c7123bd7c8903d20645b9cfe34f7ca85d4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63cdcd333c2c131733511c6750d4154ea7f097d981934d1dda8944bf2840860`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8259824bfebcdadd0448ccc0a815b7257636f6eb420e7e00216359908281e7b`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51874919dc1cfa2121d50499f839a702c4cd7340e8708e90b2af042e9debba9`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee3a41ffde2d883c73932756f176ba6901eaeb7a680a351a2b476398263cc8`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73e8028e6f79476106af6c347aa4765644a8ed828c5b6c117ee3dcc2e22e1ef`  
		Last Modified: Wed, 13 Sep 2023 05:38:02 GMT  
		Size: 289.2 KB (289194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd87253476a12fff6cbe718338261ef5ec78a1eb19d8e222838e7f96c3100a0`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.4-windowsservercore-1809`

```console
$ docker pull caddy@sha256:2869cf74555da33dba54fe0c70e1e7baf4d8535444766d27f78fdada2c7e8bb8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `caddy:2.7.4-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull caddy@sha256:3f230e8c687c5611e74c84c3ec6f7ef7844b3cc3443d9302e9bb778e6210bfe2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2032252342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea189389e39a38d33c2124e3c02e0a9bc2f3168e5605fa8a909e749ac52fc3f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:30:52 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:30:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:32:00 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:32:02 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:32:04 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:32:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:32:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:32:08 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:32:09 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:33:07 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:33:07 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2bc90334de89082943edb24d5f52a3bb36ef134c17a417ba45cc4e122be3b2`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 465.0 KB (465015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba1c9fb8dedf070862eb0526393862bb5a0f2c87a87bc3864b9b24b11af5524`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5249ade277243b1b7f8c198de7d036f2e106b8a679d777b7bfc885af7b9b76`  
		Last Modified: Wed, 13 Sep 2023 05:37:46 GMT  
		Size: 15.2 MB (15176891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224a0aed4c02b4a48f633ac01c40e020d4e8fbc32fe8896d93032f9d72f50cda`  
		Last Modified: Wed, 13 Sep 2023 05:37:42 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fc1c10b7da22b1e9a26f059801a53ce4ce22e7d24ab14ec56d343a806f3bc2`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bd26e7302c16a8d83a8a6b5d9d263b804279f2b4c7d2fcea59a97c1e187648`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f69e667aa7c5e5a21f7d8a8cdd213b9d20a8a0c790dd18fe51d4df9e5b08a7`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e456b9da79a468c972d487e55e3628f8a8917f78948550c359afc891a5ad24a`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bc4af3e90793180c1ed8b8b9ac6866e24a5de16881f363dacf0ecf47396c8`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0289dff328d597d94fcd8612bd4a726573e13f780790744c5c6f4b40b49823`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52ff2438c88a58e8be33368f668557c92bcfdc503bd58025d081c7b88ec88b`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0f1c855afa9fd7bcf5ded632c161f2ff013f4b08f5c233fa3bdf3d13701467`  
		Last Modified: Wed, 13 Sep 2023 05:37:38 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2e0bf79eee4bbd609b5a111793e394f22ad86eb897cf85c6df2c45d9a8d777`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff797288117550c2b80f9a39dd5a04cb449defc2660cf6a7589618b8d3606464`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa0d1665270ae2e22844b2386842b1deab36f8936506db82df0ec69dc72fb84`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c867297eb9d01dfe100695ae10a0c67bd38f2124de0ee7446d1e66b6dede5c06`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee97f69cfbd31f5a098d45934b159384d8e986d860ad3007140beee338aa4533`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b741c4ffade19f3d712c3fb839c3ae7f1ae4e39e5f777a2b24917b5e630d0f86`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 256.7 KB (256675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a415b22709a225227fa7ce65d7767f3f820c7e9e445b0d718dfb68ae2249832`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.4-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:1cf6f6aff1679190ae48af88d1f51c255c42ec58e320d967d97b39c0113fc8f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1970; amd64

### `caddy:2.7.4-windowsservercore-ltsc2022` - windows version 10.0.20348.1970; amd64

```console
$ docker pull caddy@sha256:76214fe6feb9f96f1c46334c01e1b9d310eb2e745bb08ba4130547b2147f3677
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1853253940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f0e585ea0797bdd13d148afed1e86161022e8cf2a79d11337f9d4dde0a8efe6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 01:35:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:33:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:33:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:34:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:34:25 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:34:26 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:34:27 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:34:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:34:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:34:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:34:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:34:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:34:33 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:34:34 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:34:35 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:34:36 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:34:56 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:34:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f40969dbf1e035a6c49e7c40b216960e3ee98ec3b76f76f9fe4498d0110bee`  
		Last Modified: Wed, 13 Sep 2023 02:15:22 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2d313a26784edb67b74292171891c0393ea119a53238e09150b5b7bc52371f`  
		Last Modified: Wed, 13 Sep 2023 05:38:08 GMT  
		Size: 483.0 KB (482985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb50376a60c42178e92d96a048b0e7f2dbc2cafe73274ab76722cda86fb32ee`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeecad99d9c5b378a623153b24130f8c36442e9a48ef6a48f878c5f585a66bd4`  
		Last Modified: Wed, 13 Sep 2023 05:38:11 GMT  
		Size: 15.2 MB (15183860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6b7a19981a71c15e39afbc3a52ed5f0c065f77c1ccd55a88e5f1b51af88753`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd7340889e9a6bfc8018c7709595b75ef962cf2608d14398ffbc90b90804a04`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7537acdfe48467d248afb6a69dad6bdb09c62617600305d2b2adb8a45ece2f`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf3cb277ba29189d90269123acd401fa787771fb095f2f2ec532be7bba2a025`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64eb5cc4069279b73a665e35bf526fa42558af1a3a71fc13d76913846d96818`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74348cf2ecbfe3a00df246034f9ab755418e8584b24113c9d327fc80cb134829`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa3fef62dce81d37fff2c621b94314d2aa9d0318523407b0a1d7d2b1e079234`  
		Last Modified: Wed, 13 Sep 2023 05:38:04 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d033d5a006e7fa969026194ef48446c840a891ad252f0316d32bc01843f0e4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbef09c0840262b42ba39068c868fc9b353bed78bb7de251e953289149e9a64e`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea46de371cf13fdb02566c79fc3a22c7123bd7c8903d20645b9cfe34f7ca85d4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63cdcd333c2c131733511c6750d4154ea7f097d981934d1dda8944bf2840860`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8259824bfebcdadd0448ccc0a815b7257636f6eb420e7e00216359908281e7b`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51874919dc1cfa2121d50499f839a702c4cd7340e8708e90b2af042e9debba9`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee3a41ffde2d883c73932756f176ba6901eaeb7a680a351a2b476398263cc8`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73e8028e6f79476106af6c347aa4765644a8ed828c5b6c117ee3dcc2e22e1ef`  
		Last Modified: Wed, 13 Sep 2023 05:38:02 GMT  
		Size: 289.2 KB (289194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd87253476a12fff6cbe718338261ef5ec78a1eb19d8e222838e7f96c3100a0`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:11ae052d9015105757d19caf86dc51fc14403841f2b65e93fe320f4d0e197385
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
$ docker pull caddy@sha256:3d1bf053476f2415b40e728c37e1112ee7551fa154a63d6f62b275c13fea8166
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18364247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a7b2e234b158c1e01eab04f851fc4b1a33296dbaa68c57d11815ee38a3cafaf`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:43:13 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 22:43:15 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 22:43:15 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 22:43:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 22:43:17 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 22:43:17 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 22:43:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 22:43:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 22:43:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 80
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 443
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 22:43:18 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 22:43:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37be51084fb891c6796079e693b73f6f882266a5e66211344173031e2b0c8ffd`  
		Last Modified: Thu, 28 Sep 2023 22:43:35 GMT  
		Size: 350.8 KB (350826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d867aa37ac50364bf4082dc48c7d4e1b88ead3164d47855e1bbc2ef3678cfc`  
		Last Modified: Thu, 28 Sep 2023 22:43:35 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147aa3899aa3307c28e185f5385015c7a5f15dfa42578a8a8eca88bf2f1e7e3e`  
		Last Modified: Thu, 28 Sep 2023 22:43:37 GMT  
		Size: 14.6 MB (14603949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:239c4a78d1bd0540a44003332119cf019e6ff839f4d303cd9801b1cc9e755ec4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17314598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b41f754b4ebb826dde7fb5c0c3c6048823add70f27a7f9c8d9f8ff1a9636ed2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:59:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 21:59:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 21:59:13 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 21:59:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 21:59:16 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 21:59:16 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 21:59:16 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 21:59:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 21:59:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 80
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 443
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 21:59:17 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 21:59:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1018057a600163b1c1b92c21ade975c631b2f8ccde66d524cfe0ecdac8e1920d`  
		Last Modified: Thu, 28 Sep 2023 21:59:43 GMT  
		Size: 347.6 KB (347613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec54680cbf2cb1a25285c82a7888498ab47d03a68db200a160d7162325a5be19`  
		Last Modified: Thu, 28 Sep 2023 21:59:43 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d087db4282d622690fce98f1d8802151567e43bfdd884a3e2a4d084701229a1`  
		Last Modified: Thu, 28 Sep 2023 21:59:45 GMT  
		Size: 13.8 MB (13814189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:85dd4fae9241ac3330e98e1d3b052d36b7ecbe1cd69b4c860454c84976426e70
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17043239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f78b426118e91fcb43786aa4c3003cd91ee86ab5f896516a885f964056b08cae`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:19:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 23:19:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 23:19:20 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 23:19:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 23:19:24 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 23:19:24 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 80
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 443
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 23:19:25 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 23:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66901ba48d0ee53cd827f4eb2cfd8b049cebba8c3d307b69760e1be917f69476`  
		Last Modified: Thu, 28 Sep 2023 23:19:46 GMT  
		Size: 344.4 KB (344448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dddeb3f6febb36993d8a51ad919784fd152aab5f6e17fe00d579916f32e42911`  
		Last Modified: Thu, 28 Sep 2023 23:19:46 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f936b2c0499a587b75385edfeb1d22b8f16ed05dca7dd0999ccc0635e1904a`  
		Last Modified: Thu, 28 Sep 2023 23:19:48 GMT  
		Size: 13.8 MB (13791383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:595e5490450c9ed29cc960149e2c265210e8444f3b3ea5ff2fab62d0da5ec3d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17163627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23f8ae4a1af151ac93d2945855095990774bc44f70af5c0e4b058dbb7e8b8c09`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:16:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 29 Sep 2023 01:16:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 29 Sep 2023 01:16:13 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 01:16:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 29 Sep 2023 01:16:15 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 29 Sep 2023 01:16:15 GMT
ENV XDG_DATA_HOME=/data
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 80
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 443
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 443/udp
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 2019
# Fri, 29 Sep 2023 01:16:16 GMT
WORKDIR /srv
# Fri, 29 Sep 2023 01:16:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f21cb0286edf1f5fefb4a859b414a446bb81baa9e8901fc8f4eca55a43aeeec`  
		Last Modified: Fri, 29 Sep 2023 01:16:34 GMT  
		Size: 360.6 KB (360643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5444b3f9419d06a4b77a65935a3b1c6e657c607bcfb9e3bd1abebe57eae36e6a`  
		Last Modified: Fri, 29 Sep 2023 01:16:34 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3485ef64f848b891981d59d52e0b092b261205ad787b38ae389e5ac39eed493f`  
		Last Modified: Fri, 29 Sep 2023 01:16:35 GMT  
		Size: 13.5 MB (13463646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:65084a14a1557b92af5b8ba6fcba9a7a710ed5caef1e2310f9622166608c9531
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16945195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73ba45deaa04c3feac6474c22204ac6f5ebc380b331ff7d585ecd196284459b3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:17:03 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 29 Sep 2023 02:17:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 29 Sep 2023 02:17:06 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 02:17:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 29 Sep 2023 02:17:13 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 29 Sep 2023 02:17:14 GMT
ENV XDG_DATA_HOME=/data
# Fri, 29 Sep 2023 02:17:15 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Fri, 29 Sep 2023 02:17:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 29 Sep 2023 02:17:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 29 Sep 2023 02:17:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 29 Sep 2023 02:17:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 29 Sep 2023 02:17:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 29 Sep 2023 02:17:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 29 Sep 2023 02:17:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 29 Sep 2023 02:17:21 GMT
EXPOSE 80
# Fri, 29 Sep 2023 02:17:21 GMT
EXPOSE 443
# Fri, 29 Sep 2023 02:17:22 GMT
EXPOSE 443/udp
# Fri, 29 Sep 2023 02:17:22 GMT
EXPOSE 2019
# Fri, 29 Sep 2023 02:17:24 GMT
WORKDIR /srv
# Fri, 29 Sep 2023 02:17:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa65cea7f5d70d1e203b851e43ad676e92f28c930ad32b6691e84ff9b5cda87`  
		Last Modified: Fri, 29 Sep 2023 02:18:03 GMT  
		Size: 362.2 KB (362182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7089a1d537371e29a65d106f43b45f2a0367d4d1db0eb7d6b7099f8ba05645`  
		Last Modified: Fri, 29 Sep 2023 02:18:01 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b93ab741fa6270144ea59d6a5fa3c4138286a569f246fdccd829b317b051f3a`  
		Last Modified: Fri, 29 Sep 2023 02:18:05 GMT  
		Size: 13.2 MB (13228998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:9e13bd2b56147eecc80f1fe1710e4350ea63d5edfb389fa89e2c6de06c08593a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17721238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2f0101e0f893afb763d99b2050dbf4d68a44aae29785af6c05af5a552b0c1a7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:19:38 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 22:19:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 22:19:39 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 22:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 22:19:42 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 22:19:42 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 80
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 443
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 22:19:44 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 22:19:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed3df874173df47ad0bd0ef67b8ee598c77921810d84a67fd2984c4f8151c91`  
		Last Modified: Thu, 28 Sep 2023 22:20:14 GMT  
		Size: 354.9 KB (354948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95a69c42a5c7fc6d73c00c7f6eb68522f3881aae55db4f85a8400e83b678b181`  
		Last Modified: Thu, 28 Sep 2023 22:20:14 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793016dc78c9794c627c07afcd2fb34af4ee470ee7fef1a1596eff0c59ba6659`  
		Last Modified: Thu, 28 Sep 2023 22:20:16 GMT  
		Size: 14.1 MB (14143684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:33050f2d060171a04ef015097c2c431bebbef8e878f3d53db4adf2b93862e11d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4851; amd64
	-	windows version 10.0.20348.1970; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:1feb6492b7349402a4e1183682415d3a06e2c50998e55e05a23a7ff54104f12e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76961764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b60574c0fd570f746bcbc19dbe40382acf64d8088c9ec08e4e3ffe8e45f1f41`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:54:30 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:54:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:54:31 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 22:54:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 22:54:41 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 22:54:41 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 22:54:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:54:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 22:54:42 GMT
WORKDIR /go
# Fri, 29 Sep 2023 03:34:26 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Fri, 29 Sep 2023 03:34:26 GMT
ENV XCADDY_VERSION=v0.3.5
# Fri, 29 Sep 2023 03:34:26 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 03:34:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 29 Sep 2023 03:34:26 GMT
ENV XCADDY_SETCAP=1
# Fri, 29 Sep 2023 03:34:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 29 Sep 2023 03:34:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 29 Sep 2023 03:34:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc37b24bb09971feb8bf4882e861bce9db0c985a16a900adb0dc9de3f854243b`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 284.7 KB (284690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94517ad51c70c15adb540d431b757078be8f6214a2f1d2181afc9454fa65d281`  
		Last Modified: Thu, 28 Sep 2023 22:57:25 GMT  
		Size: 67.0 MB (67001967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2087470b845b2224ab3a61dafcdf2abbf9540f77be63368c3346b85ad2969fa6`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2981d490d3f8070423e8c669473d70f16909bf20541abd01afb263f326ce67c2`  
		Last Modified: Fri, 29 Sep 2023 03:34:47 GMT  
		Size: 5.0 MB (4970347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5299a94e56556856e0899be99ae303524bf1ef797eb49e7a358611d2d2b3f2`  
		Last Modified: Fri, 29 Sep 2023 03:34:46 GMT  
		Size: 1.3 MB (1302233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965d515814f9dd3e22b51ab0a9ea4f92d693760133d5cf9835588e835635e33d`  
		Last Modified: Fri, 29 Sep 2023 03:34:46 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:de02c3655970e860e68fd2840e08fd9656cebb751cf677a0982e67d8fc5538a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75403016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:636f8b72fc8192d5a346042bbf7f4b91636efcd463c388b6789b3d107346d09d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:55:22 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:55:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:55:22 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 21:55:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 21:55:37 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 21:55:37 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 21:55:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:55:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 21:55:37 GMT
WORKDIR /go
# Thu, 28 Sep 2023 21:59:22 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 28 Sep 2023 21:59:22 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 28 Sep 2023 21:59:22 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 21:59:23 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Sep 2023 21:59:23 GMT
ENV XCADDY_SETCAP=1
# Thu, 28 Sep 2023 21:59:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Sep 2023 21:59:24 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Sep 2023 21:59:24 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3da3b9e7a12f6bb6b7f56e9240c2c92ce8c9f5fd5ef3b3063b9a93d454919e`  
		Last Modified: Thu, 28 Sep 2023 21:58:05 GMT  
		Size: 284.9 KB (284887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db471c20f6642596c4a4eeca4a9348dd5a897aa1c3c2383fdf2fe2c2d6f1628`  
		Last Modified: Thu, 28 Sep 2023 21:58:18 GMT  
		Size: 65.8 MB (65758212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037298c7b9748af97a3a2906d0ebb91f2dd588f633a9e8f94e2e2b2a571ead1f`  
		Last Modified: Thu, 28 Sep 2023 21:58:05 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc923fd6dd565567ed402508a7420812a84f61bbecfa0e1f988bd9b2d7b772b`  
		Last Modified: Thu, 28 Sep 2023 22:00:17 GMT  
		Size: 5.0 MB (4965415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b055d2dc5239a960f27dc6b7a7dcbe9455defa55bfb2f41d11678f8d56591668`  
		Last Modified: Thu, 28 Sep 2023 22:00:17 GMT  
		Size: 1.2 MB (1248652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513967d31b50a4e0f6dd90e6b95fe92f327bab78e463b9ed3a5ab386b0796a0e`  
		Last Modified: Thu, 28 Sep 2023 22:00:16 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0ad7a5fed30df59cfe78f87f33dd741fcf2f9588b879cf4a999db785e17ce566
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74701068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e079a52ac41cfb0c167d0940a0ed4a65fac94f7728283be07ef1f9a9661f0cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:15:15 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:15:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:15:15 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 22:15:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 22:15:32 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 22:15:32 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 22:15:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:15:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 22:15:33 GMT
WORKDIR /go
# Thu, 28 Sep 2023 23:19:29 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 28 Sep 2023 23:19:30 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 28 Sep 2023 23:19:30 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 23:19:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Sep 2023 23:19:30 GMT
ENV XCADDY_SETCAP=1
# Thu, 28 Sep 2023 23:19:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Sep 2023 23:19:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Sep 2023 23:19:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e0aec75477c9a2cf6993e068fa40a45f0684d622ece61f54e6e02f9adebeb8`  
		Last Modified: Thu, 28 Sep 2023 22:19:29 GMT  
		Size: 284.1 KB (284076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b5f8bc58ed201378ca797f82d516632d7a864a26eb9f29c4314f061c253a5d`  
		Last Modified: Thu, 28 Sep 2023 22:19:45 GMT  
		Size: 65.8 MB (65758178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f7cae270f0f74f4af87304330243fa68170426cfac2ed3042885f518bd97fb`  
		Last Modified: Thu, 28 Sep 2023 22:19:29 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eda060e9fe56bc05ae87a1f04e06d4aa8e1b59f3143db70491a8b212f53eceb`  
		Last Modified: Thu, 28 Sep 2023 23:20:02 GMT  
		Size: 4.5 MB (4512263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56d31be6b7b9ec4232229a322a3e283089e9524392a0c2317b6870571a1f366`  
		Last Modified: Thu, 28 Sep 2023 23:20:01 GMT  
		Size: 1.2 MB (1246086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a8990e3e6f77162545c3d58676a3cded2b3260baa61c1c27f8255bb9afb3ba`  
		Last Modified: Thu, 28 Sep 2023 23:20:01 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:af47b965d6c7ddd0a5c0691ee19821ebec47fd96c8ceeb01ad0d12b2024be158
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73995021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf00a9d5850ec2c2a9fb5239a41e1f452b6798d56f52c5dcf8063e9bb8685055`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:03:38 GMT
RUN apk add --no-cache ca-certificates
# Fri, 29 Sep 2023 01:40:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Sep 2023 01:40:17 GMT
ENV GOLANG_VERSION=1.21.1
# Fri, 29 Sep 2023 01:40:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 29 Sep 2023 01:40:27 GMT
ENV GOTOOLCHAIN=local
# Fri, 29 Sep 2023 01:40:27 GMT
ENV GOPATH=/go
# Fri, 29 Sep 2023 01:40:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Sep 2023 01:40:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Fri, 29 Sep 2023 01:40:28 GMT
WORKDIR /go
# Fri, 29 Sep 2023 04:34:55 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Fri, 29 Sep 2023 04:34:55 GMT
ENV XCADDY_VERSION=v0.3.5
# Fri, 29 Sep 2023 04:34:55 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 04:34:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 29 Sep 2023 04:34:56 GMT
ENV XCADDY_SETCAP=1
# Fri, 29 Sep 2023 04:34:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 29 Sep 2023 04:34:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 29 Sep 2023 04:34:57 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c21914ef412ef71f6092299b025bf4d504a49024701bf684bc9efd218155c63`  
		Last Modified: Fri, 29 Sep 2023 01:03:48 GMT  
		Size: 286.3 KB (286306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5340c63a94930ed08fa6eea6fd627bdb38f335952054831c49716a27a8c8dfa0`  
		Last Modified: Fri, 29 Sep 2023 01:42:20 GMT  
		Size: 64.1 MB (64108807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3ca664c3732429a52e8e77a07dc94297fce7c851529dd6a572983f0bf99ae1`  
		Last Modified: Fri, 29 Sep 2023 01:42:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63283848834a5104fc3043f65de33b90d451c46dfbb2fa91874f41c1f0fcbdf2`  
		Last Modified: Fri, 29 Sep 2023 04:35:13 GMT  
		Size: 5.1 MB (5069067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a59c9f8a01ff922ae6c69e34038c2eb56dcc3bf0e7bc786804f9cabda360ec`  
		Last Modified: Fri, 29 Sep 2023 04:35:12 GMT  
		Size: 1.2 MB (1198450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a52b5eedc76b0958663cbb9be6e5ac8eaa51dff9778a4b4cff667120ab6da12`  
		Last Modified: Fri, 29 Sep 2023 04:35:12 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:55d9b4418c520166c8863db2e2993557191bf9caf6e028f7b04a5b8ab1b63a73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74205796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a71360173a10dc6951ba63109fda1b23d9e5356b14225bf346845fa455513541`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:13:11 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:13:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:13:12 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 22:13:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 22:13:47 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 22:13:48 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 22:13:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:13:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 22:13:52 GMT
WORKDIR /go
# Fri, 29 Sep 2023 02:17:36 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Fri, 29 Sep 2023 02:17:37 GMT
ENV XCADDY_VERSION=v0.3.5
# Fri, 29 Sep 2023 02:17:37 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 02:17:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 29 Sep 2023 02:17:38 GMT
ENV XCADDY_SETCAP=1
# Fri, 29 Sep 2023 02:17:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 29 Sep 2023 02:17:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 29 Sep 2023 02:17:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc67971d1767eae5019ffeaf8f893e6d81dbba50bde347da0c0433c56e3f2a3`  
		Last Modified: Thu, 28 Sep 2023 22:18:17 GMT  
		Size: 286.7 KB (286659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a20f495e184de0c46bb781c57dd99e2cfc30deaa14db48a8f0cc95fc20ed28b`  
		Last Modified: Thu, 28 Sep 2023 22:18:37 GMT  
		Size: 64.1 MB (64116623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9a2fd37dab154ff5a7a7f14553c32641833c766ad5fb9ab737767a24048145`  
		Last Modified: Thu, 28 Sep 2023 22:18:16 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f689a2a610338f9a37a48fa810fa16f44dc7777786d0ed4b2df7e7e4e01cb38`  
		Last Modified: Fri, 29 Sep 2023 02:18:20 GMT  
		Size: 5.3 MB (5269263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322aacb09420bf02551659cc5b56c905f8fc7944553e6c3b1c85b5eb92547d7f`  
		Last Modified: Fri, 29 Sep 2023 02:18:20 GMT  
		Size: 1.2 MB (1186183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490b3f0289dc37c4f918f9f29f48774d57525c152a6ee4708b66c38798b2421c`  
		Last Modified: Fri, 29 Sep 2023 02:18:19 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:b438b3cf1ad85b0cc2fe8f5319ac062a52640a6a231f4858917e081b1e773001
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76102753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1788e10f8a6f8ccdc56c8b2c4b5a6ebc9387eb3b66b2b9d2dd1f18b74223f3c2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:38:54 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:38:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:38:54 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 21:39:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 21:39:15 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 21:39:15 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 21:39:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:39:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 21:39:15 GMT
WORKDIR /go
# Thu, 28 Sep 2023 22:19:51 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 28 Sep 2023 22:19:51 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_SETCAP=1
# Thu, 28 Sep 2023 22:19:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Sep 2023 22:19:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Sep 2023 22:19:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0721f16693d4788a5add1bd0b22764c8887cdc62b24edf388ae895df440f4aa9`  
		Last Modified: Thu, 28 Sep 2023 21:46:22 GMT  
		Size: 285.1 KB (285095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40248878cac53fafdd0778844ffa03633e8f3cd73c5d5136e02da42557cb26f6`  
		Last Modified: Thu, 28 Sep 2023 21:46:16 GMT  
		Size: 66.2 MB (66224373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3d28e3790630932107b3adf42c8b1564c57d0ab97f15a759b1a8f835ee4101`  
		Last Modified: Thu, 28 Sep 2023 21:46:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d382e103bfc732fc0a4c2b972100a5426b9a8e99cd21d22eddb196e5bb029206`  
		Last Modified: Thu, 28 Sep 2023 22:20:30 GMT  
		Size: 5.1 MB (5115228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3232faabff7e982d010fd0c3775d8c4a6b80e55bc3acdb0af1e63077c07656`  
		Last Modified: Thu, 28 Sep 2023 22:20:30 GMT  
		Size: 1.3 MB (1262392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff69fb680d5cc18f0d5150ac6c2922176848b00c8456922df5843f6e1c993cc7`  
		Last Modified: Thu, 28 Sep 2023 22:20:29 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.4851; amd64

```console
$ docker pull caddy@sha256:95c666eeefee6beeed59b530714de1ebdd28f2ba6ad0703b37f26b729f5e3793
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2113168904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9bf61498c4479dace7e2fa1c8c4c29a0a0722e06138f3d5fa9226287d83f2d6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 01:39:14 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Sep 2023 01:39:15 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Sep 2023 01:39:16 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Sep 2023 01:39:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Sep 2023 01:40:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:40:50 GMT
ENV GOPATH=C:\go
# Wed, 13 Sep 2023 01:41:53 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Sep 2023 01:41:54 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 13 Sep 2023 01:45:02 GMT
RUN $url = 'https://dl.google.com/go/go1.21.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '10a4f5b63215d11d1770453733dbcbf024f3f74872f84e28d7ea59f0250316c6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:45:04 GMT
WORKDIR C:\go
# Wed, 13 Sep 2023 05:35:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:35:07 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 13 Sep 2023 05:35:07 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:35:08 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Sep 2023 05:36:24 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Sep 2023 05:36:25 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cdfacf538899a08fcbb1c6b92df02725dbfcc05c593d6f310371baf9cc5c28b`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaa9f7bc4f06074cd41e4c8f38f9019d00b30116cc81e7e57bb201a2cddbe76`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa369f25c61f03e75b9090231c21b059562345a9aa5b4710c1d4bd043232a46`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1338c790efe798520cb633291aa3dbf3b37552cfbd91737d2539bad7bcac882c`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af230316f5f5bdfd37af05e436ffaadf28ac7a31d97f315dbfb2924c4d1ca3c`  
		Last Modified: Wed, 13 Sep 2023 02:16:54 GMT  
		Size: 25.6 MB (25567707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606d89c5df48922aee4ed7b88afc9f9fc270b462891c28d20b75199f2726201e`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f90ec51ca481c33d4e3887adf74f8b37c2f82af9e60290d2755f34c55b70e9c`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 220.5 KB (220461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9741d5460d3c8c14c62fd6990864968f75fbb895dfd099803a72c140739264b`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac37fd27ee4a5046c706042d53bb4a5b5e2e9ac0ec76a27142f42a55f09c31aa`  
		Last Modified: Wed, 13 Sep 2023 02:17:12 GMT  
		Size: 69.3 MB (69345076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4460c6474f9af5dc17adefba85607fa63b6072fc39250bcf433f458742fd0987`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 1.6 KB (1559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8840f55013cb306bc30661534c9618bdfda370c585b638deb791ba84fbceee9c`  
		Last Modified: Wed, 13 Sep 2023 05:38:30 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f45db9ea611a79882cee37d8b10da3ddf761d7f9ae24bf1fe0cfdb58497a6ae`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51195ebf7ad1d0ac3972b387896050e20749e6e0bb65d49a1907f49ab5cec5f2`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56989aaa5684bbc2d72ae4bb645d01d4dd0c63d35c8f4515b4c8587d6611d519`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae11f7d16342cb14a92f5b67ee9ce0eeab5805f76829bedd3735c0eec9b1f744`  
		Last Modified: Wed, 13 Sep 2023 05:38:29 GMT  
		Size: 1.7 MB (1687175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f520ac11e32bd8e755e12beaef19d397e709b5d8b007fb948658b974af6c7e2`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.20348.1970; amd64

```console
$ docker pull caddy@sha256:0a56e01d98805d99f891740e4644f1afb62f725060c36ad3cdcad27f452c3952
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1934132962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f26855783f570cd07fa203aa143ae0ddab1ef24e3a100e66f3cac124f008c0e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 01:35:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 01:35:30 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Sep 2023 01:35:31 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Sep 2023 01:35:32 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Sep 2023 01:35:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Sep 2023 01:36:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:36:16 GMT
ENV GOPATH=C:\go
# Wed, 13 Sep 2023 01:36:38 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Sep 2023 01:36:39 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 13 Sep 2023 01:38:59 GMT
RUN $url = 'https://dl.google.com/go/go1.21.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '10a4f5b63215d11d1770453733dbcbf024f3f74872f84e28d7ea59f0250316c6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:39:01 GMT
WORKDIR C:\go
# Wed, 13 Sep 2023 05:36:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:36:35 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 13 Sep 2023 05:36:35 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:36:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Sep 2023 05:37:04 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Sep 2023 05:37:05 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f40969dbf1e035a6c49e7c40b216960e3ee98ec3b76f76f9fe4498d0110bee`  
		Last Modified: Wed, 13 Sep 2023 02:15:22 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a846e03791bc3a58cfed3f02e65f87e18a5f5f416405456368e8a0ec4f9364`  
		Last Modified: Wed, 13 Sep 2023 02:15:21 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bc2015fc36cda903dca8edfdc1c87b219753af24c4ff5a95db324fb0e1cc0c`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d1910b6e6c60b5b71a12c43af94e08cf0ba20718d9a6c16ad07734f4977311`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46353fb4c6176aee49921617b1cd3ac7dcbca49d4d7a734cb5ddef177b8354b2`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f70d11added5b27b9707831ac76b04e95d4fa92b406f09532472fa350df630`  
		Last Modified: Wed, 13 Sep 2023 02:15:25 GMT  
		Size: 25.6 MB (25551011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892bff3fc5428691c1922057d675611c2b50e50cf3c6d22c2054b270861bc53c`  
		Last Modified: Wed, 13 Sep 2023 02:15:17 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ee07c029ab53a292bbb7320390d24d86b21159530b1b77d968b2b5416e8f67`  
		Last Modified: Wed, 13 Sep 2023 02:15:18 GMT  
		Size: 277.5 KB (277484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02fba082f03e26936264b99820372415048914f7ffd7f2469a28d3c0edd9224d`  
		Last Modified: Wed, 13 Sep 2023 02:15:17 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5004044396790144a82fbe98df119c5d7ae1a9abaac51c4cf0813b0d43f3f58`  
		Last Modified: Wed, 13 Sep 2023 02:15:43 GMT  
		Size: 69.3 MB (69336704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d84e4497229ea334095327a0106b2812e1dd5261c636cb1461fd698efffc4b6`  
		Last Modified: Wed, 13 Sep 2023 02:15:17 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20bad1e33f8c7089f46cd563d46ed621e589ef95c6dd41ba7569e5649804f136`  
		Last Modified: Wed, 13 Sep 2023 05:38:48 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c872ac2c7792d27826114f417d42ecbf945599d2b446775726d828ee99aab2c0`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6aff62b7b35fb324b51b0049e8a19ba51736b4f6ba1bfd92511f117e51e794`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77347ece80c37436fa82eb033a03166eb1c797e7341a6b642bf3bb80c12e36d5`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d1c7afb782c38442247cae60bbf9b16689939a03c80d4394125a9ff0af783c`  
		Last Modified: Wed, 13 Sep 2023 05:38:47 GMT  
		Size: 1.7 MB (1675830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191cef90893a643b034d031ee3e41cd4daa1b59c1d2d0e2dc1640f7bedb6c55a`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:308ffbaa017c0bb533cfe7442c49460b33193a43192b2bb9744a0fa7080a50c3
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
$ docker pull caddy@sha256:1feb6492b7349402a4e1183682415d3a06e2c50998e55e05a23a7ff54104f12e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76961764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b60574c0fd570f746bcbc19dbe40382acf64d8088c9ec08e4e3ffe8e45f1f41`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:54:30 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:54:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:54:31 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 22:54:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 22:54:41 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 22:54:41 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 22:54:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:54:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 22:54:42 GMT
WORKDIR /go
# Fri, 29 Sep 2023 03:34:26 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Fri, 29 Sep 2023 03:34:26 GMT
ENV XCADDY_VERSION=v0.3.5
# Fri, 29 Sep 2023 03:34:26 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 03:34:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 29 Sep 2023 03:34:26 GMT
ENV XCADDY_SETCAP=1
# Fri, 29 Sep 2023 03:34:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 29 Sep 2023 03:34:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 29 Sep 2023 03:34:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc37b24bb09971feb8bf4882e861bce9db0c985a16a900adb0dc9de3f854243b`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 284.7 KB (284690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94517ad51c70c15adb540d431b757078be8f6214a2f1d2181afc9454fa65d281`  
		Last Modified: Thu, 28 Sep 2023 22:57:25 GMT  
		Size: 67.0 MB (67001967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2087470b845b2224ab3a61dafcdf2abbf9540f77be63368c3346b85ad2969fa6`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2981d490d3f8070423e8c669473d70f16909bf20541abd01afb263f326ce67c2`  
		Last Modified: Fri, 29 Sep 2023 03:34:47 GMT  
		Size: 5.0 MB (4970347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5299a94e56556856e0899be99ae303524bf1ef797eb49e7a358611d2d2b3f2`  
		Last Modified: Fri, 29 Sep 2023 03:34:46 GMT  
		Size: 1.3 MB (1302233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965d515814f9dd3e22b51ab0a9ea4f92d693760133d5cf9835588e835635e33d`  
		Last Modified: Fri, 29 Sep 2023 03:34:46 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:de02c3655970e860e68fd2840e08fd9656cebb751cf677a0982e67d8fc5538a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75403016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:636f8b72fc8192d5a346042bbf7f4b91636efcd463c388b6789b3d107346d09d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:55:22 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:55:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:55:22 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 21:55:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 21:55:37 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 21:55:37 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 21:55:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:55:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 21:55:37 GMT
WORKDIR /go
# Thu, 28 Sep 2023 21:59:22 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 28 Sep 2023 21:59:22 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 28 Sep 2023 21:59:22 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 21:59:23 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Sep 2023 21:59:23 GMT
ENV XCADDY_SETCAP=1
# Thu, 28 Sep 2023 21:59:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Sep 2023 21:59:24 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Sep 2023 21:59:24 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3da3b9e7a12f6bb6b7f56e9240c2c92ce8c9f5fd5ef3b3063b9a93d454919e`  
		Last Modified: Thu, 28 Sep 2023 21:58:05 GMT  
		Size: 284.9 KB (284887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db471c20f6642596c4a4eeca4a9348dd5a897aa1c3c2383fdf2fe2c2d6f1628`  
		Last Modified: Thu, 28 Sep 2023 21:58:18 GMT  
		Size: 65.8 MB (65758212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037298c7b9748af97a3a2906d0ebb91f2dd588f633a9e8f94e2e2b2a571ead1f`  
		Last Modified: Thu, 28 Sep 2023 21:58:05 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc923fd6dd565567ed402508a7420812a84f61bbecfa0e1f988bd9b2d7b772b`  
		Last Modified: Thu, 28 Sep 2023 22:00:17 GMT  
		Size: 5.0 MB (4965415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b055d2dc5239a960f27dc6b7a7dcbe9455defa55bfb2f41d11678f8d56591668`  
		Last Modified: Thu, 28 Sep 2023 22:00:17 GMT  
		Size: 1.2 MB (1248652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513967d31b50a4e0f6dd90e6b95fe92f327bab78e463b9ed3a5ab386b0796a0e`  
		Last Modified: Thu, 28 Sep 2023 22:00:16 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0ad7a5fed30df59cfe78f87f33dd741fcf2f9588b879cf4a999db785e17ce566
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74701068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e079a52ac41cfb0c167d0940a0ed4a65fac94f7728283be07ef1f9a9661f0cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:15:15 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:15:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:15:15 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 22:15:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 22:15:32 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 22:15:32 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 22:15:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:15:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 22:15:33 GMT
WORKDIR /go
# Thu, 28 Sep 2023 23:19:29 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 28 Sep 2023 23:19:30 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 28 Sep 2023 23:19:30 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 23:19:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Sep 2023 23:19:30 GMT
ENV XCADDY_SETCAP=1
# Thu, 28 Sep 2023 23:19:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Sep 2023 23:19:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Sep 2023 23:19:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e0aec75477c9a2cf6993e068fa40a45f0684d622ece61f54e6e02f9adebeb8`  
		Last Modified: Thu, 28 Sep 2023 22:19:29 GMT  
		Size: 284.1 KB (284076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b5f8bc58ed201378ca797f82d516632d7a864a26eb9f29c4314f061c253a5d`  
		Last Modified: Thu, 28 Sep 2023 22:19:45 GMT  
		Size: 65.8 MB (65758178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f7cae270f0f74f4af87304330243fa68170426cfac2ed3042885f518bd97fb`  
		Last Modified: Thu, 28 Sep 2023 22:19:29 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eda060e9fe56bc05ae87a1f04e06d4aa8e1b59f3143db70491a8b212f53eceb`  
		Last Modified: Thu, 28 Sep 2023 23:20:02 GMT  
		Size: 4.5 MB (4512263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56d31be6b7b9ec4232229a322a3e283089e9524392a0c2317b6870571a1f366`  
		Last Modified: Thu, 28 Sep 2023 23:20:01 GMT  
		Size: 1.2 MB (1246086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a8990e3e6f77162545c3d58676a3cded2b3260baa61c1c27f8255bb9afb3ba`  
		Last Modified: Thu, 28 Sep 2023 23:20:01 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:af47b965d6c7ddd0a5c0691ee19821ebec47fd96c8ceeb01ad0d12b2024be158
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73995021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf00a9d5850ec2c2a9fb5239a41e1f452b6798d56f52c5dcf8063e9bb8685055`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:03:38 GMT
RUN apk add --no-cache ca-certificates
# Fri, 29 Sep 2023 01:40:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Sep 2023 01:40:17 GMT
ENV GOLANG_VERSION=1.21.1
# Fri, 29 Sep 2023 01:40:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 29 Sep 2023 01:40:27 GMT
ENV GOTOOLCHAIN=local
# Fri, 29 Sep 2023 01:40:27 GMT
ENV GOPATH=/go
# Fri, 29 Sep 2023 01:40:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Sep 2023 01:40:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Fri, 29 Sep 2023 01:40:28 GMT
WORKDIR /go
# Fri, 29 Sep 2023 04:34:55 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Fri, 29 Sep 2023 04:34:55 GMT
ENV XCADDY_VERSION=v0.3.5
# Fri, 29 Sep 2023 04:34:55 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 04:34:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 29 Sep 2023 04:34:56 GMT
ENV XCADDY_SETCAP=1
# Fri, 29 Sep 2023 04:34:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 29 Sep 2023 04:34:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 29 Sep 2023 04:34:57 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c21914ef412ef71f6092299b025bf4d504a49024701bf684bc9efd218155c63`  
		Last Modified: Fri, 29 Sep 2023 01:03:48 GMT  
		Size: 286.3 KB (286306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5340c63a94930ed08fa6eea6fd627bdb38f335952054831c49716a27a8c8dfa0`  
		Last Modified: Fri, 29 Sep 2023 01:42:20 GMT  
		Size: 64.1 MB (64108807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3ca664c3732429a52e8e77a07dc94297fce7c851529dd6a572983f0bf99ae1`  
		Last Modified: Fri, 29 Sep 2023 01:42:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63283848834a5104fc3043f65de33b90d451c46dfbb2fa91874f41c1f0fcbdf2`  
		Last Modified: Fri, 29 Sep 2023 04:35:13 GMT  
		Size: 5.1 MB (5069067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a59c9f8a01ff922ae6c69e34038c2eb56dcc3bf0e7bc786804f9cabda360ec`  
		Last Modified: Fri, 29 Sep 2023 04:35:12 GMT  
		Size: 1.2 MB (1198450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a52b5eedc76b0958663cbb9be6e5ac8eaa51dff9778a4b4cff667120ab6da12`  
		Last Modified: Fri, 29 Sep 2023 04:35:12 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:55d9b4418c520166c8863db2e2993557191bf9caf6e028f7b04a5b8ab1b63a73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74205796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a71360173a10dc6951ba63109fda1b23d9e5356b14225bf346845fa455513541`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:13:11 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:13:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:13:12 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 22:13:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 22:13:47 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 22:13:48 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 22:13:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 22:13:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 22:13:52 GMT
WORKDIR /go
# Fri, 29 Sep 2023 02:17:36 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Fri, 29 Sep 2023 02:17:37 GMT
ENV XCADDY_VERSION=v0.3.5
# Fri, 29 Sep 2023 02:17:37 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 02:17:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 29 Sep 2023 02:17:38 GMT
ENV XCADDY_SETCAP=1
# Fri, 29 Sep 2023 02:17:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 29 Sep 2023 02:17:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 29 Sep 2023 02:17:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc67971d1767eae5019ffeaf8f893e6d81dbba50bde347da0c0433c56e3f2a3`  
		Last Modified: Thu, 28 Sep 2023 22:18:17 GMT  
		Size: 286.7 KB (286659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a20f495e184de0c46bb781c57dd99e2cfc30deaa14db48a8f0cc95fc20ed28b`  
		Last Modified: Thu, 28 Sep 2023 22:18:37 GMT  
		Size: 64.1 MB (64116623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9a2fd37dab154ff5a7a7f14553c32641833c766ad5fb9ab737767a24048145`  
		Last Modified: Thu, 28 Sep 2023 22:18:16 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f689a2a610338f9a37a48fa810fa16f44dc7777786d0ed4b2df7e7e4e01cb38`  
		Last Modified: Fri, 29 Sep 2023 02:18:20 GMT  
		Size: 5.3 MB (5269263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322aacb09420bf02551659cc5b56c905f8fc7944553e6c3b1c85b5eb92547d7f`  
		Last Modified: Fri, 29 Sep 2023 02:18:20 GMT  
		Size: 1.2 MB (1186183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490b3f0289dc37c4f918f9f29f48774d57525c152a6ee4708b66c38798b2421c`  
		Last Modified: Fri, 29 Sep 2023 02:18:19 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:b438b3cf1ad85b0cc2fe8f5319ac062a52640a6a231f4858917e081b1e773001
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76102753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1788e10f8a6f8ccdc56c8b2c4b5a6ebc9387eb3b66b2b9d2dd1f18b74223f3c2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:38:54 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:38:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:38:54 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 21:39:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 21:39:15 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 21:39:15 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 21:39:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:39:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 21:39:15 GMT
WORKDIR /go
# Thu, 28 Sep 2023 22:19:51 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 28 Sep 2023 22:19:51 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_SETCAP=1
# Thu, 28 Sep 2023 22:19:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Sep 2023 22:19:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Sep 2023 22:19:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0721f16693d4788a5add1bd0b22764c8887cdc62b24edf388ae895df440f4aa9`  
		Last Modified: Thu, 28 Sep 2023 21:46:22 GMT  
		Size: 285.1 KB (285095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40248878cac53fafdd0778844ffa03633e8f3cd73c5d5136e02da42557cb26f6`  
		Last Modified: Thu, 28 Sep 2023 21:46:16 GMT  
		Size: 66.2 MB (66224373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3d28e3790630932107b3adf42c8b1564c57d0ab97f15a759b1a8f835ee4101`  
		Last Modified: Thu, 28 Sep 2023 21:46:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d382e103bfc732fc0a4c2b972100a5426b9a8e99cd21d22eddb196e5bb029206`  
		Last Modified: Thu, 28 Sep 2023 22:20:30 GMT  
		Size: 5.1 MB (5115228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3232faabff7e982d010fd0c3775d8c4a6b80e55bc3acdb0af1e63077c07656`  
		Last Modified: Thu, 28 Sep 2023 22:20:30 GMT  
		Size: 1.3 MB (1262392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff69fb680d5cc18f0d5150ac6c2922176848b00c8456922df5843f6e1c993cc7`  
		Last Modified: Thu, 28 Sep 2023 22:20:29 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:1a9280c29c9c558a4f0870515605df3716ff711eeef8f648d8207f81f3577c8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull caddy@sha256:95c666eeefee6beeed59b530714de1ebdd28f2ba6ad0703b37f26b729f5e3793
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2113168904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9bf61498c4479dace7e2fa1c8c4c29a0a0722e06138f3d5fa9226287d83f2d6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 01:39:14 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Sep 2023 01:39:15 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Sep 2023 01:39:16 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Sep 2023 01:39:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Sep 2023 01:40:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:40:50 GMT
ENV GOPATH=C:\go
# Wed, 13 Sep 2023 01:41:53 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Sep 2023 01:41:54 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 13 Sep 2023 01:45:02 GMT
RUN $url = 'https://dl.google.com/go/go1.21.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '10a4f5b63215d11d1770453733dbcbf024f3f74872f84e28d7ea59f0250316c6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:45:04 GMT
WORKDIR C:\go
# Wed, 13 Sep 2023 05:35:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:35:07 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 13 Sep 2023 05:35:07 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:35:08 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Sep 2023 05:36:24 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Sep 2023 05:36:25 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cdfacf538899a08fcbb1c6b92df02725dbfcc05c593d6f310371baf9cc5c28b`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaa9f7bc4f06074cd41e4c8f38f9019d00b30116cc81e7e57bb201a2cddbe76`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa369f25c61f03e75b9090231c21b059562345a9aa5b4710c1d4bd043232a46`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1338c790efe798520cb633291aa3dbf3b37552cfbd91737d2539bad7bcac882c`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af230316f5f5bdfd37af05e436ffaadf28ac7a31d97f315dbfb2924c4d1ca3c`  
		Last Modified: Wed, 13 Sep 2023 02:16:54 GMT  
		Size: 25.6 MB (25567707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606d89c5df48922aee4ed7b88afc9f9fc270b462891c28d20b75199f2726201e`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f90ec51ca481c33d4e3887adf74f8b37c2f82af9e60290d2755f34c55b70e9c`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 220.5 KB (220461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9741d5460d3c8c14c62fd6990864968f75fbb895dfd099803a72c140739264b`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac37fd27ee4a5046c706042d53bb4a5b5e2e9ac0ec76a27142f42a55f09c31aa`  
		Last Modified: Wed, 13 Sep 2023 02:17:12 GMT  
		Size: 69.3 MB (69345076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4460c6474f9af5dc17adefba85607fa63b6072fc39250bcf433f458742fd0987`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 1.6 KB (1559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8840f55013cb306bc30661534c9618bdfda370c585b638deb791ba84fbceee9c`  
		Last Modified: Wed, 13 Sep 2023 05:38:30 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f45db9ea611a79882cee37d8b10da3ddf761d7f9ae24bf1fe0cfdb58497a6ae`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51195ebf7ad1d0ac3972b387896050e20749e6e0bb65d49a1907f49ab5cec5f2`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56989aaa5684bbc2d72ae4bb645d01d4dd0c63d35c8f4515b4c8587d6611d519`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae11f7d16342cb14a92f5b67ee9ce0eeab5805f76829bedd3735c0eec9b1f744`  
		Last Modified: Wed, 13 Sep 2023 05:38:29 GMT  
		Size: 1.7 MB (1687175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f520ac11e32bd8e755e12beaef19d397e709b5d8b007fb948658b974af6c7e2`  
		Last Modified: Wed, 13 Sep 2023 05:38:28 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:e27807e1af059f2f978b562de306e9d021538db7c394f3838deb1d734efc29ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1970; amd64

### `caddy:builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1970; amd64

```console
$ docker pull caddy@sha256:0a56e01d98805d99f891740e4644f1afb62f725060c36ad3cdcad27f452c3952
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1934132962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f26855783f570cd07fa203aa143ae0ddab1ef24e3a100e66f3cac124f008c0e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 01:35:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 01:35:30 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Sep 2023 01:35:31 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Sep 2023 01:35:32 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Sep 2023 01:35:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Sep 2023 01:36:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:36:16 GMT
ENV GOPATH=C:\go
# Wed, 13 Sep 2023 01:36:38 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Sep 2023 01:36:39 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 13 Sep 2023 01:38:59 GMT
RUN $url = 'https://dl.google.com/go/go1.21.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '10a4f5b63215d11d1770453733dbcbf024f3f74872f84e28d7ea59f0250316c6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:39:01 GMT
WORKDIR C:\go
# Wed, 13 Sep 2023 05:36:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:36:35 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 13 Sep 2023 05:36:35 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:36:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Sep 2023 05:37:04 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Sep 2023 05:37:05 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f40969dbf1e035a6c49e7c40b216960e3ee98ec3b76f76f9fe4498d0110bee`  
		Last Modified: Wed, 13 Sep 2023 02:15:22 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a846e03791bc3a58cfed3f02e65f87e18a5f5f416405456368e8a0ec4f9364`  
		Last Modified: Wed, 13 Sep 2023 02:15:21 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bc2015fc36cda903dca8edfdc1c87b219753af24c4ff5a95db324fb0e1cc0c`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d1910b6e6c60b5b71a12c43af94e08cf0ba20718d9a6c16ad07734f4977311`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46353fb4c6176aee49921617b1cd3ac7dcbca49d4d7a734cb5ddef177b8354b2`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f70d11added5b27b9707831ac76b04e95d4fa92b406f09532472fa350df630`  
		Last Modified: Wed, 13 Sep 2023 02:15:25 GMT  
		Size: 25.6 MB (25551011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892bff3fc5428691c1922057d675611c2b50e50cf3c6d22c2054b270861bc53c`  
		Last Modified: Wed, 13 Sep 2023 02:15:17 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ee07c029ab53a292bbb7320390d24d86b21159530b1b77d968b2b5416e8f67`  
		Last Modified: Wed, 13 Sep 2023 02:15:18 GMT  
		Size: 277.5 KB (277484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02fba082f03e26936264b99820372415048914f7ffd7f2469a28d3c0edd9224d`  
		Last Modified: Wed, 13 Sep 2023 02:15:17 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5004044396790144a82fbe98df119c5d7ae1a9abaac51c4cf0813b0d43f3f58`  
		Last Modified: Wed, 13 Sep 2023 02:15:43 GMT  
		Size: 69.3 MB (69336704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d84e4497229ea334095327a0106b2812e1dd5261c636cb1461fd698efffc4b6`  
		Last Modified: Wed, 13 Sep 2023 02:15:17 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20bad1e33f8c7089f46cd563d46ed621e589ef95c6dd41ba7569e5649804f136`  
		Last Modified: Wed, 13 Sep 2023 05:38:48 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c872ac2c7792d27826114f417d42ecbf945599d2b446775726d828ee99aab2c0`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6aff62b7b35fb324b51b0049e8a19ba51736b4f6ba1bfd92511f117e51e794`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77347ece80c37436fa82eb033a03166eb1c797e7341a6b642bf3bb80c12e36d5`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d1c7afb782c38442247cae60bbf9b16689939a03c80d4394125a9ff0af783c`  
		Last Modified: Wed, 13 Sep 2023 05:38:47 GMT  
		Size: 1.7 MB (1675830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191cef90893a643b034d031ee3e41cd4daa1b59c1d2d0e2dc1640f7bedb6c55a`  
		Last Modified: Wed, 13 Sep 2023 05:38:46 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:df239ca80315c8271f9e87a981fb47124831f8b5a7c85970249d2dfd712479a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4851; amd64
	-	windows version 10.0.20348.1970; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:3d1bf053476f2415b40e728c37e1112ee7551fa154a63d6f62b275c13fea8166
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18364247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a7b2e234b158c1e01eab04f851fc4b1a33296dbaa68c57d11815ee38a3cafaf`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:43:13 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 22:43:15 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 22:43:15 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 22:43:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 22:43:17 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 22:43:17 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 22:43:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 22:43:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 22:43:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 22:43:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 80
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 443
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 22:43:18 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 22:43:18 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 22:43:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37be51084fb891c6796079e693b73f6f882266a5e66211344173031e2b0c8ffd`  
		Last Modified: Thu, 28 Sep 2023 22:43:35 GMT  
		Size: 350.8 KB (350826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d867aa37ac50364bf4082dc48c7d4e1b88ead3164d47855e1bbc2ef3678cfc`  
		Last Modified: Thu, 28 Sep 2023 22:43:35 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147aa3899aa3307c28e185f5385015c7a5f15dfa42578a8a8eca88bf2f1e7e3e`  
		Last Modified: Thu, 28 Sep 2023 22:43:37 GMT  
		Size: 14.6 MB (14603949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:239c4a78d1bd0540a44003332119cf019e6ff839f4d303cd9801b1cc9e755ec4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17314598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b41f754b4ebb826dde7fb5c0c3c6048823add70f27a7f9c8d9f8ff1a9636ed2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:59:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 21:59:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 21:59:13 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 21:59:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 21:59:16 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 21:59:16 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 21:59:16 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 21:59:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 21:59:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 21:59:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 80
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 443
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 21:59:17 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 21:59:17 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 21:59:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1018057a600163b1c1b92c21ade975c631b2f8ccde66d524cfe0ecdac8e1920d`  
		Last Modified: Thu, 28 Sep 2023 21:59:43 GMT  
		Size: 347.6 KB (347613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec54680cbf2cb1a25285c82a7888498ab47d03a68db200a160d7162325a5be19`  
		Last Modified: Thu, 28 Sep 2023 21:59:43 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d087db4282d622690fce98f1d8802151567e43bfdd884a3e2a4d084701229a1`  
		Last Modified: Thu, 28 Sep 2023 21:59:45 GMT  
		Size: 13.8 MB (13814189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:85dd4fae9241ac3330e98e1d3b052d36b7ecbe1cd69b4c860454c84976426e70
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17043239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f78b426118e91fcb43786aa4c3003cd91ee86ab5f896516a885f964056b08cae`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:19:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 23:19:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 23:19:20 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 23:19:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 23:19:24 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 23:19:24 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 23:19:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 23:19:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 80
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 443
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 23:19:25 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 23:19:25 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 23:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66901ba48d0ee53cd827f4eb2cfd8b049cebba8c3d307b69760e1be917f69476`  
		Last Modified: Thu, 28 Sep 2023 23:19:46 GMT  
		Size: 344.4 KB (344448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dddeb3f6febb36993d8a51ad919784fd152aab5f6e17fe00d579916f32e42911`  
		Last Modified: Thu, 28 Sep 2023 23:19:46 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f936b2c0499a587b75385edfeb1d22b8f16ed05dca7dd0999ccc0635e1904a`  
		Last Modified: Thu, 28 Sep 2023 23:19:48 GMT  
		Size: 13.8 MB (13791383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:595e5490450c9ed29cc960149e2c265210e8444f3b3ea5ff2fab62d0da5ec3d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17163627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23f8ae4a1af151ac93d2945855095990774bc44f70af5c0e4b058dbb7e8b8c09`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:16:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 29 Sep 2023 01:16:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 29 Sep 2023 01:16:13 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 01:16:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 29 Sep 2023 01:16:15 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 29 Sep 2023 01:16:15 GMT
ENV XDG_DATA_HOME=/data
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 29 Sep 2023 01:16:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 80
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 443
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 443/udp
# Fri, 29 Sep 2023 01:16:16 GMT
EXPOSE 2019
# Fri, 29 Sep 2023 01:16:16 GMT
WORKDIR /srv
# Fri, 29 Sep 2023 01:16:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f21cb0286edf1f5fefb4a859b414a446bb81baa9e8901fc8f4eca55a43aeeec`  
		Last Modified: Fri, 29 Sep 2023 01:16:34 GMT  
		Size: 360.6 KB (360643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5444b3f9419d06a4b77a65935a3b1c6e657c607bcfb9e3bd1abebe57eae36e6a`  
		Last Modified: Fri, 29 Sep 2023 01:16:34 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3485ef64f848b891981d59d52e0b092b261205ad787b38ae389e5ac39eed493f`  
		Last Modified: Fri, 29 Sep 2023 01:16:35 GMT  
		Size: 13.5 MB (13463646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:65084a14a1557b92af5b8ba6fcba9a7a710ed5caef1e2310f9622166608c9531
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16945195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73ba45deaa04c3feac6474c22204ac6f5ebc380b331ff7d585ecd196284459b3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:17:03 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 29 Sep 2023 02:17:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 29 Sep 2023 02:17:06 GMT
ENV CADDY_VERSION=v2.7.4
# Fri, 29 Sep 2023 02:17:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 29 Sep 2023 02:17:13 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 29 Sep 2023 02:17:14 GMT
ENV XDG_DATA_HOME=/data
# Fri, 29 Sep 2023 02:17:15 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Fri, 29 Sep 2023 02:17:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 29 Sep 2023 02:17:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 29 Sep 2023 02:17:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 29 Sep 2023 02:17:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 29 Sep 2023 02:17:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 29 Sep 2023 02:17:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 29 Sep 2023 02:17:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 29 Sep 2023 02:17:21 GMT
EXPOSE 80
# Fri, 29 Sep 2023 02:17:21 GMT
EXPOSE 443
# Fri, 29 Sep 2023 02:17:22 GMT
EXPOSE 443/udp
# Fri, 29 Sep 2023 02:17:22 GMT
EXPOSE 2019
# Fri, 29 Sep 2023 02:17:24 GMT
WORKDIR /srv
# Fri, 29 Sep 2023 02:17:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa65cea7f5d70d1e203b851e43ad676e92f28c930ad32b6691e84ff9b5cda87`  
		Last Modified: Fri, 29 Sep 2023 02:18:03 GMT  
		Size: 362.2 KB (362182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7089a1d537371e29a65d106f43b45f2a0367d4d1db0eb7d6b7099f8ba05645`  
		Last Modified: Fri, 29 Sep 2023 02:18:01 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b93ab741fa6270144ea59d6a5fa3c4138286a569f246fdccd829b317b051f3a`  
		Last Modified: Fri, 29 Sep 2023 02:18:05 GMT  
		Size: 13.2 MB (13228998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:9e13bd2b56147eecc80f1fe1710e4350ea63d5edfb389fa89e2c6de06c08593a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17721238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2f0101e0f893afb763d99b2050dbf4d68a44aae29785af6c05af5a552b0c1a7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:19:38 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 28 Sep 2023 22:19:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 28 Sep 2023 22:19:39 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 22:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Sep 2023 22:19:42 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Sep 2023 22:19:42 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Sep 2023 22:19:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Sep 2023 22:19:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 80
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 443
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 443/udp
# Thu, 28 Sep 2023 22:19:43 GMT
EXPOSE 2019
# Thu, 28 Sep 2023 22:19:44 GMT
WORKDIR /srv
# Thu, 28 Sep 2023 22:19:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed3df874173df47ad0bd0ef67b8ee598c77921810d84a67fd2984c4f8151c91`  
		Last Modified: Thu, 28 Sep 2023 22:20:14 GMT  
		Size: 354.9 KB (354948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95a69c42a5c7fc6d73c00c7f6eb68522f3881aae55db4f85a8400e83b678b181`  
		Last Modified: Thu, 28 Sep 2023 22:20:14 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793016dc78c9794c627c07afcd2fb34af4ee470ee7fef1a1596eff0c59ba6659`  
		Last Modified: Thu, 28 Sep 2023 22:20:16 GMT  
		Size: 14.1 MB (14143684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.4851; amd64

```console
$ docker pull caddy@sha256:3f230e8c687c5611e74c84c3ec6f7ef7844b3cc3443d9302e9bb778e6210bfe2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2032252342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea189389e39a38d33c2124e3c02e0a9bc2f3168e5605fa8a909e749ac52fc3f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:30:52 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:30:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:32:00 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:32:02 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:32:04 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:32:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:32:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:32:08 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:32:09 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:33:07 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:33:07 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2bc90334de89082943edb24d5f52a3bb36ef134c17a417ba45cc4e122be3b2`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 465.0 KB (465015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba1c9fb8dedf070862eb0526393862bb5a0f2c87a87bc3864b9b24b11af5524`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5249ade277243b1b7f8c198de7d036f2e106b8a679d777b7bfc885af7b9b76`  
		Last Modified: Wed, 13 Sep 2023 05:37:46 GMT  
		Size: 15.2 MB (15176891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224a0aed4c02b4a48f633ac01c40e020d4e8fbc32fe8896d93032f9d72f50cda`  
		Last Modified: Wed, 13 Sep 2023 05:37:42 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fc1c10b7da22b1e9a26f059801a53ce4ce22e7d24ab14ec56d343a806f3bc2`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bd26e7302c16a8d83a8a6b5d9d263b804279f2b4c7d2fcea59a97c1e187648`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f69e667aa7c5e5a21f7d8a8cdd213b9d20a8a0c790dd18fe51d4df9e5b08a7`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e456b9da79a468c972d487e55e3628f8a8917f78948550c359afc891a5ad24a`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bc4af3e90793180c1ed8b8b9ac6866e24a5de16881f363dacf0ecf47396c8`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0289dff328d597d94fcd8612bd4a726573e13f780790744c5c6f4b40b49823`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52ff2438c88a58e8be33368f668557c92bcfdc503bd58025d081c7b88ec88b`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0f1c855afa9fd7bcf5ded632c161f2ff013f4b08f5c233fa3bdf3d13701467`  
		Last Modified: Wed, 13 Sep 2023 05:37:38 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2e0bf79eee4bbd609b5a111793e394f22ad86eb897cf85c6df2c45d9a8d777`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff797288117550c2b80f9a39dd5a04cb449defc2660cf6a7589618b8d3606464`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa0d1665270ae2e22844b2386842b1deab36f8936506db82df0ec69dc72fb84`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c867297eb9d01dfe100695ae10a0c67bd38f2124de0ee7446d1e66b6dede5c06`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee97f69cfbd31f5a098d45934b159384d8e986d860ad3007140beee338aa4533`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b741c4ffade19f3d712c3fb839c3ae7f1ae4e39e5f777a2b24917b5e630d0f86`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 256.7 KB (256675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a415b22709a225227fa7ce65d7767f3f820c7e9e445b0d718dfb68ae2249832`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.20348.1970; amd64

```console
$ docker pull caddy@sha256:76214fe6feb9f96f1c46334c01e1b9d310eb2e745bb08ba4130547b2147f3677
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1853253940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f0e585ea0797bdd13d148afed1e86161022e8cf2a79d11337f9d4dde0a8efe6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 01:35:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:33:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:33:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:34:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:34:25 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:34:26 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:34:27 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:34:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:34:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:34:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:34:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:34:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:34:33 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:34:34 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:34:35 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:34:36 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:34:56 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:34:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f40969dbf1e035a6c49e7c40b216960e3ee98ec3b76f76f9fe4498d0110bee`  
		Last Modified: Wed, 13 Sep 2023 02:15:22 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2d313a26784edb67b74292171891c0393ea119a53238e09150b5b7bc52371f`  
		Last Modified: Wed, 13 Sep 2023 05:38:08 GMT  
		Size: 483.0 KB (482985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb50376a60c42178e92d96a048b0e7f2dbc2cafe73274ab76722cda86fb32ee`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeecad99d9c5b378a623153b24130f8c36442e9a48ef6a48f878c5f585a66bd4`  
		Last Modified: Wed, 13 Sep 2023 05:38:11 GMT  
		Size: 15.2 MB (15183860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6b7a19981a71c15e39afbc3a52ed5f0c065f77c1ccd55a88e5f1b51af88753`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd7340889e9a6bfc8018c7709595b75ef962cf2608d14398ffbc90b90804a04`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7537acdfe48467d248afb6a69dad6bdb09c62617600305d2b2adb8a45ece2f`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf3cb277ba29189d90269123acd401fa787771fb095f2f2ec532be7bba2a025`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64eb5cc4069279b73a665e35bf526fa42558af1a3a71fc13d76913846d96818`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74348cf2ecbfe3a00df246034f9ab755418e8584b24113c9d327fc80cb134829`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa3fef62dce81d37fff2c621b94314d2aa9d0318523407b0a1d7d2b1e079234`  
		Last Modified: Wed, 13 Sep 2023 05:38:04 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d033d5a006e7fa969026194ef48446c840a891ad252f0316d32bc01843f0e4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbef09c0840262b42ba39068c868fc9b353bed78bb7de251e953289149e9a64e`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea46de371cf13fdb02566c79fc3a22c7123bd7c8903d20645b9cfe34f7ca85d4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63cdcd333c2c131733511c6750d4154ea7f097d981934d1dda8944bf2840860`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8259824bfebcdadd0448ccc0a815b7257636f6eb420e7e00216359908281e7b`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51874919dc1cfa2121d50499f839a702c4cd7340e8708e90b2af042e9debba9`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee3a41ffde2d883c73932756f176ba6901eaeb7a680a351a2b476398263cc8`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73e8028e6f79476106af6c347aa4765644a8ed828c5b6c117ee3dcc2e22e1ef`  
		Last Modified: Wed, 13 Sep 2023 05:38:02 GMT  
		Size: 289.2 KB (289194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd87253476a12fff6cbe718338261ef5ec78a1eb19d8e222838e7f96c3100a0`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:4e0879a2422f5309c4ed33c36438e076aa198dc89228e2dc8a56369b86fac7a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4851; amd64
	-	windows version 10.0.20348.1970; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.4851; amd64

```console
$ docker pull caddy@sha256:3f230e8c687c5611e74c84c3ec6f7ef7844b3cc3443d9302e9bb778e6210bfe2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2032252342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea189389e39a38d33c2124e3c02e0a9bc2f3168e5605fa8a909e749ac52fc3f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:30:52 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:30:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:32:00 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:32:02 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:32:04 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:32:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:32:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:32:08 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:32:09 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:33:07 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:33:07 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2bc90334de89082943edb24d5f52a3bb36ef134c17a417ba45cc4e122be3b2`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 465.0 KB (465015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba1c9fb8dedf070862eb0526393862bb5a0f2c87a87bc3864b9b24b11af5524`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5249ade277243b1b7f8c198de7d036f2e106b8a679d777b7bfc885af7b9b76`  
		Last Modified: Wed, 13 Sep 2023 05:37:46 GMT  
		Size: 15.2 MB (15176891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224a0aed4c02b4a48f633ac01c40e020d4e8fbc32fe8896d93032f9d72f50cda`  
		Last Modified: Wed, 13 Sep 2023 05:37:42 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fc1c10b7da22b1e9a26f059801a53ce4ce22e7d24ab14ec56d343a806f3bc2`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bd26e7302c16a8d83a8a6b5d9d263b804279f2b4c7d2fcea59a97c1e187648`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f69e667aa7c5e5a21f7d8a8cdd213b9d20a8a0c790dd18fe51d4df9e5b08a7`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e456b9da79a468c972d487e55e3628f8a8917f78948550c359afc891a5ad24a`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bc4af3e90793180c1ed8b8b9ac6866e24a5de16881f363dacf0ecf47396c8`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0289dff328d597d94fcd8612bd4a726573e13f780790744c5c6f4b40b49823`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52ff2438c88a58e8be33368f668557c92bcfdc503bd58025d081c7b88ec88b`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0f1c855afa9fd7bcf5ded632c161f2ff013f4b08f5c233fa3bdf3d13701467`  
		Last Modified: Wed, 13 Sep 2023 05:37:38 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2e0bf79eee4bbd609b5a111793e394f22ad86eb897cf85c6df2c45d9a8d777`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff797288117550c2b80f9a39dd5a04cb449defc2660cf6a7589618b8d3606464`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa0d1665270ae2e22844b2386842b1deab36f8936506db82df0ec69dc72fb84`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c867297eb9d01dfe100695ae10a0c67bd38f2124de0ee7446d1e66b6dede5c06`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee97f69cfbd31f5a098d45934b159384d8e986d860ad3007140beee338aa4533`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b741c4ffade19f3d712c3fb839c3ae7f1ae4e39e5f777a2b24917b5e630d0f86`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 256.7 KB (256675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a415b22709a225227fa7ce65d7767f3f820c7e9e445b0d718dfb68ae2249832`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.20348.1970; amd64

```console
$ docker pull caddy@sha256:76214fe6feb9f96f1c46334c01e1b9d310eb2e745bb08ba4130547b2147f3677
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1853253940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f0e585ea0797bdd13d148afed1e86161022e8cf2a79d11337f9d4dde0a8efe6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 01:35:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:33:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:33:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:34:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:34:25 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:34:26 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:34:27 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:34:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:34:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:34:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:34:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:34:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:34:33 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:34:34 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:34:35 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:34:36 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:34:56 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:34:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f40969dbf1e035a6c49e7c40b216960e3ee98ec3b76f76f9fe4498d0110bee`  
		Last Modified: Wed, 13 Sep 2023 02:15:22 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2d313a26784edb67b74292171891c0393ea119a53238e09150b5b7bc52371f`  
		Last Modified: Wed, 13 Sep 2023 05:38:08 GMT  
		Size: 483.0 KB (482985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb50376a60c42178e92d96a048b0e7f2dbc2cafe73274ab76722cda86fb32ee`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeecad99d9c5b378a623153b24130f8c36442e9a48ef6a48f878c5f585a66bd4`  
		Last Modified: Wed, 13 Sep 2023 05:38:11 GMT  
		Size: 15.2 MB (15183860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6b7a19981a71c15e39afbc3a52ed5f0c065f77c1ccd55a88e5f1b51af88753`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd7340889e9a6bfc8018c7709595b75ef962cf2608d14398ffbc90b90804a04`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7537acdfe48467d248afb6a69dad6bdb09c62617600305d2b2adb8a45ece2f`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf3cb277ba29189d90269123acd401fa787771fb095f2f2ec532be7bba2a025`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64eb5cc4069279b73a665e35bf526fa42558af1a3a71fc13d76913846d96818`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74348cf2ecbfe3a00df246034f9ab755418e8584b24113c9d327fc80cb134829`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa3fef62dce81d37fff2c621b94314d2aa9d0318523407b0a1d7d2b1e079234`  
		Last Modified: Wed, 13 Sep 2023 05:38:04 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d033d5a006e7fa969026194ef48446c840a891ad252f0316d32bc01843f0e4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbef09c0840262b42ba39068c868fc9b353bed78bb7de251e953289149e9a64e`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea46de371cf13fdb02566c79fc3a22c7123bd7c8903d20645b9cfe34f7ca85d4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63cdcd333c2c131733511c6750d4154ea7f097d981934d1dda8944bf2840860`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8259824bfebcdadd0448ccc0a815b7257636f6eb420e7e00216359908281e7b`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51874919dc1cfa2121d50499f839a702c4cd7340e8708e90b2af042e9debba9`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee3a41ffde2d883c73932756f176ba6901eaeb7a680a351a2b476398263cc8`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73e8028e6f79476106af6c347aa4765644a8ed828c5b6c117ee3dcc2e22e1ef`  
		Last Modified: Wed, 13 Sep 2023 05:38:02 GMT  
		Size: 289.2 KB (289194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd87253476a12fff6cbe718338261ef5ec78a1eb19d8e222838e7f96c3100a0`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:2869cf74555da33dba54fe0c70e1e7baf4d8535444766d27f78fdada2c7e8bb8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull caddy@sha256:3f230e8c687c5611e74c84c3ec6f7ef7844b3cc3443d9302e9bb778e6210bfe2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2032252342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea189389e39a38d33c2124e3c02e0a9bc2f3168e5605fa8a909e749ac52fc3f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:30:52 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:30:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:32:00 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:32:02 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:32:04 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:32:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:32:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:32:08 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:32:09 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:33:07 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:33:07 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2bc90334de89082943edb24d5f52a3bb36ef134c17a417ba45cc4e122be3b2`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 465.0 KB (465015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba1c9fb8dedf070862eb0526393862bb5a0f2c87a87bc3864b9b24b11af5524`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5249ade277243b1b7f8c198de7d036f2e106b8a679d777b7bfc885af7b9b76`  
		Last Modified: Wed, 13 Sep 2023 05:37:46 GMT  
		Size: 15.2 MB (15176891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224a0aed4c02b4a48f633ac01c40e020d4e8fbc32fe8896d93032f9d72f50cda`  
		Last Modified: Wed, 13 Sep 2023 05:37:42 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fc1c10b7da22b1e9a26f059801a53ce4ce22e7d24ab14ec56d343a806f3bc2`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bd26e7302c16a8d83a8a6b5d9d263b804279f2b4c7d2fcea59a97c1e187648`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f69e667aa7c5e5a21f7d8a8cdd213b9d20a8a0c790dd18fe51d4df9e5b08a7`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e456b9da79a468c972d487e55e3628f8a8917f78948550c359afc891a5ad24a`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bc4af3e90793180c1ed8b8b9ac6866e24a5de16881f363dacf0ecf47396c8`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0289dff328d597d94fcd8612bd4a726573e13f780790744c5c6f4b40b49823`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52ff2438c88a58e8be33368f668557c92bcfdc503bd58025d081c7b88ec88b`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0f1c855afa9fd7bcf5ded632c161f2ff013f4b08f5c233fa3bdf3d13701467`  
		Last Modified: Wed, 13 Sep 2023 05:37:38 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2e0bf79eee4bbd609b5a111793e394f22ad86eb897cf85c6df2c45d9a8d777`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff797288117550c2b80f9a39dd5a04cb449defc2660cf6a7589618b8d3606464`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa0d1665270ae2e22844b2386842b1deab36f8936506db82df0ec69dc72fb84`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c867297eb9d01dfe100695ae10a0c67bd38f2124de0ee7446d1e66b6dede5c06`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee97f69cfbd31f5a098d45934b159384d8e986d860ad3007140beee338aa4533`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b741c4ffade19f3d712c3fb839c3ae7f1ae4e39e5f777a2b24917b5e630d0f86`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 256.7 KB (256675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a415b22709a225227fa7ce65d7767f3f820c7e9e445b0d718dfb68ae2249832`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:1cf6f6aff1679190ae48af88d1f51c255c42ec58e320d967d97b39c0113fc8f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1970; amd64

### `caddy:windowsservercore-ltsc2022` - windows version 10.0.20348.1970; amd64

```console
$ docker pull caddy@sha256:76214fe6feb9f96f1c46334c01e1b9d310eb2e745bb08ba4130547b2147f3677
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1853253940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f0e585ea0797bdd13d148afed1e86161022e8cf2a79d11337f9d4dde0a8efe6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 01:35:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:33:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:33:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:34:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:34:25 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:34:26 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:34:27 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:34:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:34:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:34:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:34:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:34:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:34:33 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:34:34 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:34:35 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:34:36 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:34:56 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:34:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f40969dbf1e035a6c49e7c40b216960e3ee98ec3b76f76f9fe4498d0110bee`  
		Last Modified: Wed, 13 Sep 2023 02:15:22 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2d313a26784edb67b74292171891c0393ea119a53238e09150b5b7bc52371f`  
		Last Modified: Wed, 13 Sep 2023 05:38:08 GMT  
		Size: 483.0 KB (482985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb50376a60c42178e92d96a048b0e7f2dbc2cafe73274ab76722cda86fb32ee`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeecad99d9c5b378a623153b24130f8c36442e9a48ef6a48f878c5f585a66bd4`  
		Last Modified: Wed, 13 Sep 2023 05:38:11 GMT  
		Size: 15.2 MB (15183860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6b7a19981a71c15e39afbc3a52ed5f0c065f77c1ccd55a88e5f1b51af88753`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd7340889e9a6bfc8018c7709595b75ef962cf2608d14398ffbc90b90804a04`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7537acdfe48467d248afb6a69dad6bdb09c62617600305d2b2adb8a45ece2f`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf3cb277ba29189d90269123acd401fa787771fb095f2f2ec532be7bba2a025`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64eb5cc4069279b73a665e35bf526fa42558af1a3a71fc13d76913846d96818`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74348cf2ecbfe3a00df246034f9ab755418e8584b24113c9d327fc80cb134829`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa3fef62dce81d37fff2c621b94314d2aa9d0318523407b0a1d7d2b1e079234`  
		Last Modified: Wed, 13 Sep 2023 05:38:04 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d033d5a006e7fa969026194ef48446c840a891ad252f0316d32bc01843f0e4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbef09c0840262b42ba39068c868fc9b353bed78bb7de251e953289149e9a64e`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea46de371cf13fdb02566c79fc3a22c7123bd7c8903d20645b9cfe34f7ca85d4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63cdcd333c2c131733511c6750d4154ea7f097d981934d1dda8944bf2840860`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8259824bfebcdadd0448ccc0a815b7257636f6eb420e7e00216359908281e7b`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51874919dc1cfa2121d50499f839a702c4cd7340e8708e90b2af042e9debba9`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee3a41ffde2d883c73932756f176ba6901eaeb7a680a351a2b476398263cc8`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73e8028e6f79476106af6c347aa4765644a8ed828c5b6c117ee3dcc2e22e1ef`  
		Last Modified: Wed, 13 Sep 2023 05:38:02 GMT  
		Size: 289.2 KB (289194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd87253476a12fff6cbe718338261ef5ec78a1eb19d8e222838e7f96c3100a0`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
