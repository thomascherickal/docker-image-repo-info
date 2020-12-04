<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `caddy`

-	[`caddy:2`](#caddy2)
-	[`caddy:2.1.1`](#caddy211)
-	[`caddy:2.1.1-alpine`](#caddy211-alpine)
-	[`caddy:2.1.1-builder`](#caddy211-builder)
-	[`caddy:2.1.1-builder-alpine`](#caddy211-builder-alpine)
-	[`caddy:2.1.1-builder-windowsservercore-1809`](#caddy211-builder-windowsservercore-1809)
-	[`caddy:2.1.1-builder-windowsservercore-ltsc2016`](#caddy211-builder-windowsservercore-ltsc2016)
-	[`caddy:2.1.1-windowsservercore`](#caddy211-windowsservercore)
-	[`caddy:2.1.1-windowsservercore-1809`](#caddy211-windowsservercore-1809)
-	[`caddy:2.1.1-windowsservercore-ltsc2016`](#caddy211-windowsservercore-ltsc2016)
-	[`caddy:2.2.1`](#caddy221)
-	[`caddy:2.2.1-alpine`](#caddy221-alpine)
-	[`caddy:2.2.1-builder`](#caddy221-builder)
-	[`caddy:2.2.1-builder-alpine`](#caddy221-builder-alpine)
-	[`caddy:2.2.1-builder-windowsservercore-1809`](#caddy221-builder-windowsservercore-1809)
-	[`caddy:2.2.1-builder-windowsservercore-ltsc2016`](#caddy221-builder-windowsservercore-ltsc2016)
-	[`caddy:2.2.1-windowsservercore`](#caddy221-windowsservercore)
-	[`caddy:2.2.1-windowsservercore-1809`](#caddy221-windowsservercore-1809)
-	[`caddy:2.2.1-windowsservercore-ltsc2016`](#caddy221-windowsservercore-ltsc2016)
-	[`caddy:2-alpine`](#caddy2-alpine)
-	[`caddy:2-builder`](#caddy2-builder)
-	[`caddy:2-builder-alpine`](#caddy2-builder-alpine)
-	[`caddy:2-builder-windowsservercore-1809`](#caddy2-builder-windowsservercore-1809)
-	[`caddy:2-builder-windowsservercore-ltsc2016`](#caddy2-builder-windowsservercore-ltsc2016)
-	[`caddy:2-windowsservercore`](#caddy2-windowsservercore)
-	[`caddy:2-windowsservercore-1809`](#caddy2-windowsservercore-1809)
-	[`caddy:2-windowsservercore-ltsc2016`](#caddy2-windowsservercore-ltsc2016)
-	[`caddy:alpine`](#caddyalpine)
-	[`caddy:builder`](#caddybuilder)
-	[`caddy:builder-alpine`](#caddybuilder-alpine)
-	[`caddy:builder-windowsservercore-1809`](#caddybuilder-windowsservercore-1809)
-	[`caddy:builder-windowsservercore-ltsc2016`](#caddybuilder-windowsservercore-ltsc2016)
-	[`caddy:latest`](#caddylatest)
-	[`caddy:windowsservercore`](#caddywindowsservercore)
-	[`caddy:windowsservercore-1809`](#caddywindowsservercore-1809)
-	[`caddy:windowsservercore-ltsc2016`](#caddywindowsservercore-ltsc2016)

## `caddy:2`

```console
$ docker pull caddy@sha256:e46050590a9ac1a411b5da0349f735b5977e9dcbe6ab91e9a95c9a731533aba8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1577; amd64
	-	windows version 10.0.14393.4046; amd64

### `caddy:2` - linux; amd64

```console
$ docker pull caddy@sha256:4ebad49f78a3f98164d89431978046ee6e94f1e8a70454abc7f49ce1a5ee7826
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14635232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bb0137bab0e21a92b0bc9ec1cc22c259b097d5bf239b161ae1eac0de1833e67`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:33:22 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 04:33:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 04:33:55 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 04:33:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 04:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 04:34:01 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 04:34:01 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 04:34:01 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 04:34:02 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 04:34:02 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 04:34:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 04:34:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 04:34:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 04:34:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 04:34:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 04:34:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 04:34:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 04:34:05 GMT
EXPOSE 80
# Thu, 22 Oct 2020 04:34:05 GMT
EXPOSE 443
# Thu, 22 Oct 2020 04:34:06 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 04:34:06 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 04:34:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2e2d825895b6421ca5dbd63db0d99f790ef84a84c7bcaff51e60b654397858`  
		Last Modified: Thu, 22 Oct 2020 04:34:47 GMT  
		Size: 300.0 KB (299956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaf2e3dee2e74b401fce928bf9502e48df68da4e8c1933bfd6b00b1137529fc`  
		Last Modified: Thu, 22 Oct 2020 04:35:02 GMT  
		Size: 5.8 KB (5754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2215cf93250599c5db984cee0fddd5d0cd59ef035ab5a317387b67211bde86d`  
		Last Modified: Thu, 22 Oct 2020 04:35:06 GMT  
		Size: 11.5 MB (11532508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060365e49ba5ee96a2859e269b366f5a5c9f386e5bdbf07d2ef31b1fc6934baa`  
		Last Modified: Thu, 22 Oct 2020 04:35:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:abba73dc860b2f35703cb7d27f08baf5bfc084e18e627b94661d01a8e2befdaf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13784259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f0aad5a281913821dd39ffed5e144daae22ac81ac4314731395ab65eedde72a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:58:10 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 02:58:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 02:58:46 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 02:58:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 02:58:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:59:00 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 02:59:01 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 02:59:01 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 02:59:03 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 02:59:08 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 02:59:09 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 02:59:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 02:59:11 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 02:59:11 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 02:59:12 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 02:59:13 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 02:59:14 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 02:59:15 GMT
EXPOSE 80
# Thu, 22 Oct 2020 02:59:19 GMT
EXPOSE 443
# Thu, 22 Oct 2020 02:59:20 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 02:59:21 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 02:59:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7369c3ac4b39c55c74e96dd3eb61ac2fa65e5671b1c2acca9697a7c9d20c3cf`  
		Last Modified: Thu, 22 Oct 2020 02:59:49 GMT  
		Size: 300.1 KB (300086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8f4045920069dff3382a5993783c5d846d9e28d0f5a63c475ed298fce0abb7`  
		Last Modified: Thu, 22 Oct 2020 03:00:03 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db6bde4735da15e5db23ad62f3d64d78aed8713a40d12547f5538c15c90f9da`  
		Last Modified: Thu, 22 Oct 2020 03:00:06 GMT  
		Size: 10.9 MB (10876280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a95efd7a14ed98a53a238da45faa7e3b0fdd2a93529b83bfe9d0823dafac67c`  
		Last Modified: Thu, 22 Oct 2020 03:00:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:8cf66cbe3c03273ca54bdab908092a6a9b9f02d39595ed15b1111f1465430426
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13565251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b20723dea614fc40d9f3cb59eddd33bf0e89dfda3f8ed4a7b404ef334632a4b9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:04:57 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 03:05:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 03:05:45 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 03:05:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 03:05:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:05:53 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 03:05:53 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 03:05:54 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 03:05:55 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 03:05:56 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 03:05:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 03:05:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 03:05:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 03:05:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 03:05:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 03:06:00 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 03:06:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 03:06:01 GMT
EXPOSE 80
# Thu, 22 Oct 2020 03:06:02 GMT
EXPOSE 443
# Thu, 22 Oct 2020 03:06:02 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 03:06:03 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 03:06:04 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a8e7fe5034ac502626b0a921d79be80c092890176e33b236c489d6f00710a2`  
		Last Modified: Thu, 22 Oct 2020 03:06:32 GMT  
		Size: 299.2 KB (299211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14db75acdaca15b1e81890f29b3b757fcc73e7a69a55f5ed659bf800f6340108`  
		Last Modified: Thu, 22 Oct 2020 03:06:43 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2197c38adf245bca8f229a4cd718c4d0f619a87bae5786572ccdac1a286882c`  
		Last Modified: Thu, 22 Oct 2020 03:06:46 GMT  
		Size: 10.9 MB (10854384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0104bc6a595940856019d00d9ff8e04365338a7964d948b64cc44bf73cc59e`  
		Last Modified: Thu, 22 Oct 2020 03:06:42 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:da121cf42d1759ed03af3130533d365c365af1d738d550744ad863e05e64cf46
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13540356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89b4aa38988ab2442575062d99c3cb44976de6c227256c118f35340e7c21c303`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:40:04 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 02:40:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 02:40:57 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 02:41:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 02:41:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:41:07 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 02:41:08 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 02:41:09 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 02:41:10 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 02:41:10 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 02:41:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 02:41:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 02:41:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 02:41:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 02:41:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 02:41:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 02:41:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 02:41:19 GMT
EXPOSE 80
# Thu, 22 Oct 2020 02:41:20 GMT
EXPOSE 443
# Thu, 22 Oct 2020 02:41:20 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 02:41:21 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 02:41:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dbde357077a97c0f831033bf03c9828203cb7e3e6cb33217ce4d7cfd71c931`  
		Last Modified: Thu, 22 Oct 2020 02:41:47 GMT  
		Size: 300.3 KB (300348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a5ab0aa923ce1fe233b904008bbf932c4787f48bcd59f07a85616147b7cbc3`  
		Last Modified: Thu, 22 Oct 2020 02:41:56 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc398339860cf826624c9c22b5de9b45a193260e2ff24826d210b493483398f`  
		Last Modified: Thu, 22 Oct 2020 02:41:59 GMT  
		Size: 10.5 MB (10527465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6e7d61d1d4a00550447ea1f67edc0463cc527e49356e98959edfafba0df879`  
		Last Modified: Thu, 22 Oct 2020 02:41:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:09208042b4d19d7ed87b51b99dc20b390dab20d9ae7e235a62a3af3aaf472bd5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13291756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe5c77284adc35481d13003d31a866f637b6eaf9f5764f667e536db79ce23129`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 13:39:52 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 13:44:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 13:44:04 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 13:44:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 13:44:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 13:44:33 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 13:44:37 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 13:44:40 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 13:44:44 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 13:44:48 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 13:44:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 13:44:56 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 13:45:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 13:45:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 13:45:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 13:45:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 13:45:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 13:45:23 GMT
EXPOSE 80
# Thu, 22 Oct 2020 13:45:26 GMT
EXPOSE 443
# Thu, 22 Oct 2020 13:45:30 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 13:45:35 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 13:45:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649a4964211b7ce86541a0c1dad8ef3800ec38a3ca90aff94b76759b4cb8e279`  
		Last Modified: Thu, 22 Oct 2020 13:47:22 GMT  
		Size: 302.3 KB (302327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58dd938ef3e3eae8509deda8fab9ab5f9344169d912e35a802633e799feed1bb`  
		Last Modified: Thu, 22 Oct 2020 13:47:52 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe23c296ee12ee12ef84dbabbb4f7bf0362a9a12b684782ebd3f44a97c8fcf8e`  
		Last Modified: Thu, 22 Oct 2020 13:47:55 GMT  
		Size: 10.2 MB (10180223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d2f3c084745fecafaa9ff33626a81124f2d70267ceee705da555714238bfa1`  
		Last Modified: Thu, 22 Oct 2020 13:47:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:3e18b421d651721239cb3422bc890d1211535681219b7696816f487b4cebc4ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14074857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4d5562f1d148d3d67ff7f5995be8f860553ad0f3d07091335643306b83385e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:41:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 02:41:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 02:41:31 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 02:41:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 02:41:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:41:36 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 02:41:36 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 02:41:37 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 02:41:37 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 02:41:37 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 02:41:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 02:41:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 02:41:38 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 02:41:38 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 02:41:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 02:41:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 02:41:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 02:41:40 GMT
EXPOSE 80
# Thu, 22 Oct 2020 02:41:40 GMT
EXPOSE 443
# Thu, 22 Oct 2020 02:41:40 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 02:41:41 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 02:41:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f988ff23f3cbb35bfed69e33f3b7ee69403bfae4f46363a08eea4830053e9c`  
		Last Modified: Thu, 22 Oct 2020 02:42:01 GMT  
		Size: 300.5 KB (300481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd6a4e0db99510879c5dfceabd1e629a0692c4544bb0da34971f8722b881e92`  
		Last Modified: Thu, 22 Oct 2020 02:42:09 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e13b938aa802e74610585cabba77d625db4baf219f577a81195c272408c7d3`  
		Last Modified: Thu, 22 Oct 2020 02:42:16 GMT  
		Size: 11.2 MB (11202559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a221fff082950a8a98db12eb99f532a39008f0d6e21684bc1aed06fa1ed2a764`  
		Last Modified: Thu, 22 Oct 2020 02:42:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.1577; amd64

```console
$ docker pull caddy@sha256:dad45b6df45cf6f4c45f010c391544a830a6372847bb2504a23a870eb9e96638
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2413941176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61f3df5163746a4530d03a8bc80f3b1318d935f9f1b3e26f00a31af891a9ba86`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 20:53:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Nov 2020 20:53:31 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 11 Nov 2020 20:54:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Nov 2020 20:54:04 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Nov 2020 20:54:04 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Nov 2020 20:54:05 GMT
VOLUME [c:/config]
# Wed, 11 Nov 2020 20:54:06 GMT
VOLUME [c:/data]
# Wed, 11 Nov 2020 20:54:07 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 11 Nov 2020 20:54:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Nov 2020 20:54:09 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Nov 2020 20:54:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Nov 2020 20:54:11 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Nov 2020 20:54:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Nov 2020 20:54:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Nov 2020 20:54:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Nov 2020 20:54:13 GMT
EXPOSE 80
# Wed, 11 Nov 2020 20:54:14 GMT
EXPOSE 443
# Wed, 11 Nov 2020 20:54:14 GMT
EXPOSE 2019
# Wed, 11 Nov 2020 20:54:30 GMT
RUN caddy version
# Wed, 11 Nov 2020 20:54:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01dcdd0030882c54a82d0a279a4099081c604810ccccb17d3d7c04a2057bf657`  
		Last Modified: Wed, 11 Nov 2020 21:02:39 GMT  
		Size: 9.2 MB (9248045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3be730f5a5cc9d1dd7080908242b9ed33ba6541e7120addf14e416b944b577`  
		Last Modified: Wed, 11 Nov 2020 21:02:36 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d70ac9fb0285fe6670a558e9c1da67b5594dd483872376ac91425a3058f95b9`  
		Last Modified: Wed, 11 Nov 2020 21:02:54 GMT  
		Size: 16.3 MB (16343997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72340d1f03d76debdf2a014ab06bbd3bc5cb1e8358520912f0c9f71f2b4a6ea`  
		Last Modified: Wed, 11 Nov 2020 21:02:34 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ae7bc4f9eb3af2fa576dd096f9992ad2cfc8a2e9aad0af79e1ebf11c95065d`  
		Last Modified: Wed, 11 Nov 2020 21:02:33 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46832c7bcb0b053968836644798024f37cfede18aaac00abed0c1571fbeeca4c`  
		Last Modified: Wed, 11 Nov 2020 21:02:33 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdafb0d35a00870fdb93efde60b2d5c002b5ec117bb07526ec1d744787529f58`  
		Last Modified: Wed, 11 Nov 2020 21:02:31 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af235cb3a2a159b44c6b773e30cbd6f7931055fb7cfed2aee403c9197e0defc`  
		Last Modified: Wed, 11 Nov 2020 21:02:32 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493ee2907458eb7d47b217b59e2f23b4dd4a6974a36a70462fa54e5b9201f26b`  
		Last Modified: Wed, 11 Nov 2020 21:02:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2f8b9a7de64bd747e2afbc20e6ca964b00d3b48ccdb9245e162300a5ef9b44`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc59b5cb8ee3554d8e4971222e0208e7b6dd831b33894abeba76400bbcb7d56`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c88104f4e1fc6125880b248f3e1edcc5cbf3daf73aaf26bf3782972f11203c3`  
		Last Modified: Wed, 11 Nov 2020 21:02:30 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7cb21eb1cd8ca039940f462fdfe3348c877262adbbc5891cdbc3601ffa2649`  
		Last Modified: Wed, 11 Nov 2020 21:02:27 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef21802812d7f9ad5dcebb2efbf8d4831fcdf5b024bac00c22d04e7406a420b`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed806482965bf605e395b83f00ba44639cc1c88b1b8ec7c75bb708d9c031610`  
		Last Modified: Wed, 11 Nov 2020 21:02:24 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee097b51db8b06f6e93d48da3e914d6a598b32681fdf27785279f3f5dbb5796`  
		Last Modified: Wed, 11 Nov 2020 21:02:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf5349d69a690d25aa14a10fab1fc6e7a82ec345bae9e1a01a4dfd95f09cd1b`  
		Last Modified: Wed, 11 Nov 2020 21:02:22 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0b5aa8db0e75c1ef349905a29ef299882814b7937d14753d2e6a972f7b13b1`  
		Last Modified: Wed, 11 Nov 2020 21:02:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cac55d84f022bb91b78bfb339492198e3fa96a7d1e25c1f8e09ad648376d45d`  
		Last Modified: Wed, 11 Nov 2020 21:02:21 GMT  
		Size: 299.3 KB (299301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7476d855c257a4a27ce525860567dd9bd67e74abb01c0fd1b334444ffaa8504c`  
		Last Modified: Wed, 11 Nov 2020 21:02:24 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.14393.4046; amd64

```console
$ docker pull caddy@sha256:405a17b713c3f1517124a2506ac9b4ed33285819013417e6b90fb2aa07cb0bd6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5802615067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:371225d0afbf64a113a3745e99535e2e17239829f4e36d99aa36e7aee3be9efc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 13:23:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 20:56:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Nov 2020 20:56:05 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 11 Nov 2020 20:57:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Nov 2020 20:57:25 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Nov 2020 20:57:26 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Nov 2020 20:57:28 GMT
VOLUME [c:/config]
# Wed, 11 Nov 2020 20:57:29 GMT
VOLUME [c:/data]
# Wed, 11 Nov 2020 20:57:30 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 11 Nov 2020 20:57:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Nov 2020 20:57:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Nov 2020 20:57:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Nov 2020 20:57:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Nov 2020 20:57:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Nov 2020 20:57:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Nov 2020 20:57:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Nov 2020 20:57:35 GMT
EXPOSE 80
# Wed, 11 Nov 2020 20:57:36 GMT
EXPOSE 443
# Wed, 11 Nov 2020 20:57:37 GMT
EXPOSE 2019
# Wed, 11 Nov 2020 20:58:18 GMT
RUN caddy version
# Wed, 11 Nov 2020 20:58:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:126d9a92c0cb7b68c56dec2dd5ba118de9dde3ec6368db734c5135fdf1528a33`  
		Last Modified: Wed, 11 Nov 2020 13:34:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5595cf12db880fdffb7bc7e0ceef81a68e0766ff34fdc357635566a05b60085`  
		Last Modified: Wed, 11 Nov 2020 21:03:35 GMT  
		Size: 10.1 MB (10089893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47fc9d917c611e97ffa642af414764e4712d012a3b2c10700a357a771d58bf3`  
		Last Modified: Wed, 11 Nov 2020 21:03:24 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2b332d20177fb217e2744454885bba6eb94e9c7512c35bef53cf1222f10b3a`  
		Last Modified: Wed, 11 Nov 2020 21:03:50 GMT  
		Size: 21.7 MB (21694741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061740784584c807be44f52e632b6fcafa7893cab07ca93723103ca41e759cd2`  
		Last Modified: Wed, 11 Nov 2020 21:03:23 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a051df7f978fd750beb5e55b7a7da2d50550a52c97baf897cd3452347196147`  
		Last Modified: Wed, 11 Nov 2020 21:03:23 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94db8d6fb716d4c43b34e09a05176f94701accb480ce613c231d70ef23c649b`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eeb5cfdcdca36082954b3510135aea31966da19679b9cc7d8d4e43a3892f2f5`  
		Last Modified: Wed, 11 Nov 2020 21:03:19 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50cc11877f41dad7cb21c9e61379268e564a03b044ec4cfb124cccd267ef551c`  
		Last Modified: Wed, 11 Nov 2020 21:03:21 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9914893b848ce6d71a6f99575e794219e1603afe1dcee2bcbf69f3a41451ab05`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab52b473d299810d7e49b3d9d98db42e6aa57e5426b79f4cd7f68fd766a8a9b`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3333f590132f229c9979af102fd15c4a5958d9e3d94d50632eeb045c14028ac1`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12c4e6df6d5faa8f29b56e44eb52dc65c9d6795322a0e6d743a9d373f97adf9`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a015ed900b4c4b4d23631449b68473b1e31eda520fa22c7c19a845ac6f133f31`  
		Last Modified: Wed, 11 Nov 2020 21:03:16 GMT  
		Size: 1.1 KB (1069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f354d2a4fb61ae55364b2ae298552e22165583c076c39e05707e906633b8a2`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc11e1af39f958f492359f3242aa5205230791b166e14ab2f94067e9999464e`  
		Last Modified: Wed, 11 Nov 2020 21:03:16 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a4e622ed285e795cc2fd731f38022c2e6ca478f2223fb9fcafe0a61b5e969`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f936683e767d2733a4a898519ce7c8bc6a608fede4e7cc04c41b5fed180287`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b4fbe6665c83c229d90ec42acce959b356dbf1a97ca281604625a29d8437133`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6966c1a2733b248361e0fbafefb3b58805b223ef954ced160cb1ca7f239c25`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 251.9 KB (251913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3d08972458dc80b8c379340207e2cfeee9ea33d9e9e405ebbf52421ef16dd5`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1`

```console
$ docker pull caddy@sha256:f025e013ef93b4c17260e11bece06003b90c55a9ac3933bc75e97055ddea1792
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1577; amd64
	-	windows version 10.0.14393.4046; amd64

### `caddy:2.1.1` - linux; amd64

```console
$ docker pull caddy@sha256:94aab32108ee277eca3476c03eb3cd0c791581ccceef288e4021b4658b6e14e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16160083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:813d26d5b5f80df7e1a12968331cc52103ef347206fdfe404f095db39538745f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:33:22 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 04:33:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Thu, 22 Oct 2020 04:33:24 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 22 Oct 2020 04:33:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 04:33:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 04:33:30 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 04:33:30 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 04:33:31 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 04:33:31 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 04:33:31 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Thu, 22 Oct 2020 04:33:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 04:33:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 04:33:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 04:33:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 04:33:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 04:33:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 04:33:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 04:33:34 GMT
EXPOSE 80
# Thu, 22 Oct 2020 04:33:34 GMT
EXPOSE 443
# Thu, 22 Oct 2020 04:33:35 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 04:33:35 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 04:33:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2e2d825895b6421ca5dbd63db0d99f790ef84a84c7bcaff51e60b654397858`  
		Last Modified: Thu, 22 Oct 2020 04:34:47 GMT  
		Size: 300.0 KB (299956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792a8e39706390221a8cc5927203b39027a0bce4149c60137a8a68c14124a188`  
		Last Modified: Thu, 22 Oct 2020 04:34:47 GMT  
		Size: 5.8 KB (5753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e121fa2dd673519fd0bbbe8acae3339d2c242a0d454569905d45fcae45cbd210`  
		Last Modified: Thu, 22 Oct 2020 04:34:50 GMT  
		Size: 13.1 MB (13057360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02cabd94ff7acf4922fc1f955d07f4c8a22e63a2cb69ca77d49d20629759e6d7`  
		Last Modified: Thu, 22 Oct 2020 04:34:46 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - linux; arm variant v6

```console
$ docker pull caddy@sha256:3dcf641ed85190e11d4d2aeee30ce6fd5e12acaf14764d0ecc9c2d43cc5c52f2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15322911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55dc188cdeb883fd020df45c6c2e4274e437337e1820e0db79e0b0ff14295b34`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:58:10 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 02:58:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Thu, 22 Oct 2020 02:58:13 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 22 Oct 2020 02:58:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 02:58:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:58:22 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 02:58:23 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 02:58:23 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 02:58:24 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 02:58:25 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Thu, 22 Oct 2020 02:58:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 02:58:26 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 02:58:27 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 02:58:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 02:58:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 02:58:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 02:58:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 02:58:30 GMT
EXPOSE 80
# Thu, 22 Oct 2020 02:58:31 GMT
EXPOSE 443
# Thu, 22 Oct 2020 02:58:32 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 02:58:32 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 02:58:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7369c3ac4b39c55c74e96dd3eb61ac2fa65e5671b1c2acca9697a7c9d20c3cf`  
		Last Modified: Thu, 22 Oct 2020 02:59:49 GMT  
		Size: 300.1 KB (300086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0affadb729cb104658a545e4b2cd1eb71a6f4ca473a7576bb6a65d97de2003ff`  
		Last Modified: Thu, 22 Oct 2020 02:59:49 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a834360c16db0f4578fa61b1bb8e51d39cfdfa7616b763a7f9080b5f3fd337`  
		Last Modified: Thu, 22 Oct 2020 02:59:55 GMT  
		Size: 12.4 MB (12414928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1dea75e2b66ab3649bf01ef2e7accd82012104cf4bc9dd180b75298b9335941`  
		Last Modified: Thu, 22 Oct 2020 02:59:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - linux; arm variant v7

```console
$ docker pull caddy@sha256:3ad6c0a0783ba264b9258c26ecd947b8c1ddd9ce0eedf47bf50e0d92ce26b253
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15106906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baa5aceec9b3b914788468802d025e1d1f3551a181c58365d22efa3fe8dfb9f3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:04:57 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 03:05:00 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Thu, 22 Oct 2020 03:05:01 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 22 Oct 2020 03:05:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 03:05:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:05:11 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 03:05:12 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 03:05:13 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 03:05:13 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 03:05:14 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Thu, 22 Oct 2020 03:05:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 03:05:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 03:05:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 03:05:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 03:05:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 03:05:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 03:05:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 03:05:22 GMT
EXPOSE 80
# Thu, 22 Oct 2020 03:05:23 GMT
EXPOSE 443
# Thu, 22 Oct 2020 03:05:24 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 03:05:26 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 03:05:27 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a8e7fe5034ac502626b0a921d79be80c092890176e33b236c489d6f00710a2`  
		Last Modified: Thu, 22 Oct 2020 03:06:32 GMT  
		Size: 299.2 KB (299211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eac4e817bcf2c7b80f6f6341ad2e45a1a984b272460858c08c1a39ca8acddbe`  
		Last Modified: Thu, 22 Oct 2020 03:06:32 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4916ca18103e521657f386ae15b838945f507f4e71e7ffb9ae6146a207fc98e4`  
		Last Modified: Thu, 22 Oct 2020 03:06:36 GMT  
		Size: 12.4 MB (12396037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516dbda4db0089c1377a5f56e371ecf8ebada5ddedf4eb445b7b5a00b35837a0`  
		Last Modified: Thu, 22 Oct 2020 03:06:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:bed04cea05f8703919db1411fa43db3caf2c5feee4604e432ca3fbb39ba4e9e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.0 MB (15025979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d3072bf9e0127310f4d1cc1237287c7562fe9fe90f9e7084ef33d8ebd97fb70`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:40:04 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 02:40:08 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Thu, 22 Oct 2020 02:40:09 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 22 Oct 2020 02:40:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 02:40:18 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:40:22 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 02:40:22 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 02:40:24 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 02:40:25 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 02:40:26 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Thu, 22 Oct 2020 02:40:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 02:40:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 02:40:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 02:40:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 02:40:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 02:40:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 02:40:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 02:40:33 GMT
EXPOSE 80
# Thu, 22 Oct 2020 02:40:33 GMT
EXPOSE 443
# Thu, 22 Oct 2020 02:40:35 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 02:40:36 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 02:40:37 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dbde357077a97c0f831033bf03c9828203cb7e3e6cb33217ce4d7cfd71c931`  
		Last Modified: Thu, 22 Oct 2020 02:41:47 GMT  
		Size: 300.3 KB (300348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede963cf3892bef49a806e2b2b6cd351a073839746d3ba0040c807c9ede34282`  
		Last Modified: Thu, 22 Oct 2020 02:41:47 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30dd5666b9cb9cb79f2931d16947dff6632df90edde47a765a9abb46d21a7f8e`  
		Last Modified: Thu, 22 Oct 2020 02:41:50 GMT  
		Size: 12.0 MB (12013098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac0780379a69d70077155f92bdaf6679c77647156daf6c6b61784db51baf0b`  
		Last Modified: Thu, 22 Oct 2020 02:41:47 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - linux; ppc64le

```console
$ docker pull caddy@sha256:013e8f3007f8464b73d523c0620524d183067549b162c35f7c34a104b2e03c19
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14896989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a7eb13196205b2269a7eba953f625b2a6cb717e66971db551bcc960cd917cc2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 13:39:52 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 13:40:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Thu, 22 Oct 2020 13:40:25 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 22 Oct 2020 13:40:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 13:41:03 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 13:41:08 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 13:41:13 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 13:41:19 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 13:41:26 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 13:41:32 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Thu, 22 Oct 2020 13:41:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 13:41:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 13:41:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 13:42:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 13:42:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 13:42:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 13:42:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 13:42:18 GMT
EXPOSE 80
# Thu, 22 Oct 2020 13:42:23 GMT
EXPOSE 443
# Thu, 22 Oct 2020 13:42:29 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 13:42:34 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 13:42:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649a4964211b7ce86541a0c1dad8ef3800ec38a3ca90aff94b76759b4cb8e279`  
		Last Modified: Thu, 22 Oct 2020 13:47:22 GMT  
		Size: 302.3 KB (302327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d796f3d42ae827c5c6abc4f1d86eb2c77d579b52d88f20195c3480d66f3e0af`  
		Last Modified: Thu, 22 Oct 2020 13:47:22 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b45c60413a5845a6a452dfc06bfecd19bdcb7111f4c5011c9c273914f54284`  
		Last Modified: Thu, 22 Oct 2020 13:47:26 GMT  
		Size: 11.8 MB (11785457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae3c1c0668096c5f9942efa1b8694a27b599f3996495b052f5cd7f6e0188781`  
		Last Modified: Thu, 22 Oct 2020 13:47:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - linux; s390x

```console
$ docker pull caddy@sha256:937db8998b02f140f7b1dc4d9b6a14ff40db24dfdc22d4b1d1f5d0d0509e67ba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15709107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:007a65f150c3943695dbf4e3018205572467467599ba7ea5010e044f5fced62d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:41:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 02:41:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Thu, 22 Oct 2020 02:41:10 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 22 Oct 2020 02:41:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 02:41:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:41:15 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 02:41:15 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 02:41:16 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 02:41:16 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 02:41:16 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Thu, 22 Oct 2020 02:41:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 02:41:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 02:41:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 02:41:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 02:41:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 02:41:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 02:41:19 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 02:41:19 GMT
EXPOSE 80
# Thu, 22 Oct 2020 02:41:19 GMT
EXPOSE 443
# Thu, 22 Oct 2020 02:41:20 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 02:41:20 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 02:41:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f988ff23f3cbb35bfed69e33f3b7ee69403bfae4f46363a08eea4830053e9c`  
		Last Modified: Thu, 22 Oct 2020 02:42:01 GMT  
		Size: 300.5 KB (300481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb33c2548f9314af36267dc9e886d94ad83d75881e0c93b6931ed52734b7f451`  
		Last Modified: Thu, 22 Oct 2020 02:42:01 GMT  
		Size: 5.8 KB (5835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad254f130346e29cbf490913417f35cf7473184bba1b7ff8d90579f3b2809a29`  
		Last Modified: Thu, 22 Oct 2020 02:42:03 GMT  
		Size: 12.8 MB (12836808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf01317e485bb835fdf7067969a86d9fa9679bdd0a1c214931b788e4b8e9388f`  
		Last Modified: Thu, 22 Oct 2020 02:42:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - windows version 10.0.17763.1577; amd64

```console
$ docker pull caddy@sha256:e2d41115b10e26568979fd99964d79319400d1008733bd29b0ad270cd446041a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2415318960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca72587c4cf96e2aed3533eac5415b8b05f1282ae904b914b42a5267aa5aac29`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 20:45:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Nov 2020 20:45:21 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 11 Nov 2020 20:45:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Nov 2020 20:45:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Nov 2020 20:45:56 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Nov 2020 20:45:57 GMT
VOLUME [c:/config]
# Wed, 11 Nov 2020 20:45:57 GMT
VOLUME [c:/data]
# Wed, 11 Nov 2020 20:45:58 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 11 Nov 2020 20:45:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Nov 2020 20:46:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Nov 2020 20:46:01 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Nov 2020 20:46:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Nov 2020 20:46:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Nov 2020 20:46:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Nov 2020 20:46:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Nov 2020 20:46:04 GMT
EXPOSE 80
# Wed, 11 Nov 2020 20:46:05 GMT
EXPOSE 443
# Wed, 11 Nov 2020 20:46:05 GMT
EXPOSE 2019
# Wed, 11 Nov 2020 20:46:22 GMT
RUN caddy version
# Wed, 11 Nov 2020 20:46:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9241b8447db6ee01486692864d501d1b85cc8e28b6ba12477da3ccb91ac6fb80`  
		Last Modified: Wed, 11 Nov 2020 21:01:08 GMT  
		Size: 9.2 MB (9248091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140d2864a3ecf900ddcbb7825de568deed4368848546c6f5b33b1031d0d2785c`  
		Last Modified: Wed, 11 Nov 2020 21:01:04 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773bfe60fc2adaea22a607f2ef04801f3a1fe4d1d2742fffd1b3708b9cc2616e`  
		Last Modified: Wed, 11 Nov 2020 21:01:08 GMT  
		Size: 17.7 MB (17722401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6ac34c199b688dcea4ee50fdd427343360897f7b879c92f58e54730a2c7813`  
		Last Modified: Wed, 11 Nov 2020 21:01:03 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37ba66c494cd95e08bddfe1439674935321d50cc6619659859d447d225b9345`  
		Last Modified: Wed, 11 Nov 2020 21:01:03 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa9619dc6858361d1cc3c3459f509b1af176afab3951a8b46ff7cd4065ad56e`  
		Last Modified: Wed, 11 Nov 2020 21:01:00 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d5c4e2731ec2cf1a69fecede53c0cfc076d1c7a3031d9d2f16695b82280856`  
		Last Modified: Wed, 11 Nov 2020 21:01:00 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f78932772adde20a5b82826a3aeca1f6cbea5205a042134ccffb88993a8cbf`  
		Last Modified: Wed, 11 Nov 2020 21:01:00 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6bb7af2868628d7e417e249d60572cb1c53508861a07aa3dcbe601b698fc054`  
		Last Modified: Wed, 11 Nov 2020 21:00:59 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4046f61372cfde3727e85e91767d4eda8547125814b7cc7ace12ea083cf4741b`  
		Last Modified: Wed, 11 Nov 2020 21:00:59 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dfe0ab7ccd8016d0fb2f185efbc294841b8e43d77509a4478fa4cc6edaa4ff`  
		Last Modified: Wed, 11 Nov 2020 21:00:56 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8012fd5e700acdf295c51de57a059928e395cd4654aa5c8fcc6743961b4adf70`  
		Last Modified: Wed, 11 Nov 2020 21:00:56 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298316ad3edcfa6e02b2ed6ad0795b0167fb20254f79c4eb19ad3253c903adb1`  
		Last Modified: Wed, 11 Nov 2020 21:00:57 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451c72395cd914723ccd8dd337a0ca840c0dd00d829d6ce3d9dba4c6462102c9`  
		Last Modified: Wed, 11 Nov 2020 21:00:56 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a43113a9d7534b3a4fbeca6ad58f5ef8e1a6fa5b8d6a488f3d8edda1d7cdd61`  
		Last Modified: Wed, 11 Nov 2020 21:00:56 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369cba41c19fe5008c5dfe0b88cd8f0ef77b138d68c7eca3374c7fbf18d5afcd`  
		Last Modified: Wed, 11 Nov 2020 21:00:53 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0479adc0c263c2e9eab3e3e8fcb7b9d933a95b0f26c04c4c900c5f3804011eb3`  
		Last Modified: Wed, 11 Nov 2020 21:00:53 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea0e70171ceaae4ac02e06588b5aa7f97be0a7e82af15000c7dc8d75dd91c44`  
		Last Modified: Wed, 11 Nov 2020 21:00:53 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b2ec7137cc7d53728109e434d551d89f4694290199f60dfbdfcd4709d8a58f`  
		Last Modified: Wed, 11 Nov 2020 21:00:53 GMT  
		Size: 298.7 KB (298665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e6d60b9c57f55e542ddd3aefdcdbd16da124a2a8142c961c0dab1635429b6c`  
		Last Modified: Wed, 11 Nov 2020 21:00:53 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - windows version 10.0.14393.4046; amd64

```console
$ docker pull caddy@sha256:dede9ad27fd496b1102d3530355b3d007bca80608739b3f1beebd3474ce96575
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5803984357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f16f2509b06ce8b2e9d98af30d2ac226c0e89e30a4f81ae6ee79176655906a8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 13:23:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 20:47:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Nov 2020 20:47:53 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 11 Nov 2020 20:49:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Nov 2020 20:49:22 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Nov 2020 20:49:23 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Nov 2020 20:49:24 GMT
VOLUME [c:/config]
# Wed, 11 Nov 2020 20:49:26 GMT
VOLUME [c:/data]
# Wed, 11 Nov 2020 20:49:27 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 11 Nov 2020 20:49:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Nov 2020 20:49:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Nov 2020 20:49:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Nov 2020 20:49:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Nov 2020 20:49:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Nov 2020 20:49:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Nov 2020 20:49:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Nov 2020 20:49:32 GMT
EXPOSE 80
# Wed, 11 Nov 2020 20:49:33 GMT
EXPOSE 443
# Wed, 11 Nov 2020 20:49:34 GMT
EXPOSE 2019
# Wed, 11 Nov 2020 20:50:16 GMT
RUN caddy version
# Wed, 11 Nov 2020 20:50:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:126d9a92c0cb7b68c56dec2dd5ba118de9dde3ec6368db734c5135fdf1528a33`  
		Last Modified: Wed, 11 Nov 2020 13:34:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8209753221a853170a05478f1dcd98e0e053e700619c6ef12dc177c4e55a57ff`  
		Last Modified: Wed, 11 Nov 2020 21:01:31 GMT  
		Size: 10.1 MB (10089052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6dfd50db08ec5e748cacc844bf84f012344731801c87ab92146b9194059acf`  
		Last Modified: Wed, 11 Nov 2020 21:01:28 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac9ba3c4948efa385a4a66354591ee0f151329021799ccc9e27ddf072a22445`  
		Last Modified: Wed, 11 Nov 2020 21:01:36 GMT  
		Size: 23.1 MB (23065071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df648d1a9f54d00470e5427e4f248c99f895b4149a403ce2cd781a02a2af95e`  
		Last Modified: Wed, 11 Nov 2020 21:01:27 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a0f1dc2f6df109fbeffb6befe78cbfa1789dc66a40f841ad3f52bf99cacdc`  
		Last Modified: Wed, 11 Nov 2020 21:01:27 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87f1d0037fbb238614a6c0fdb80467c72928f95e1fef04508b7ef20fb50f7cc`  
		Last Modified: Wed, 11 Nov 2020 21:01:25 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338c2c27df684d482250c1eb4fcdf8d82e46d70adbd1c9ec145d62ae7de422f9`  
		Last Modified: Wed, 11 Nov 2020 21:01:25 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f589f2f83fd1d8a0ed928b717bf4730b00dae2cf1a930a40fa139e2b2d651f`  
		Last Modified: Wed, 11 Nov 2020 21:01:24 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f29aa9fa439221c221fc981284a1ef76ca26a80e9e32007cd2245b9a1ca8c0`  
		Last Modified: Wed, 11 Nov 2020 21:01:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c98142e163981917efb57c375062ebe8a063c074a5e687fee3f024f33c65133`  
		Last Modified: Wed, 11 Nov 2020 21:01:25 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e33dd735daeae3d313fee34288454b0ff1cd20d5184bc4e37f4065274ab8a53`  
		Last Modified: Wed, 11 Nov 2020 21:01:21 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adcac5351e0ac5818f5fed08a87a3c9b4af5c2f654e3f6cc9ffbbe3124f22730`  
		Last Modified: Wed, 11 Nov 2020 21:01:20 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd52cb52dc571effe896fddd8e45cb3a31b369c12cf66b15dedbc957b780445`  
		Last Modified: Wed, 11 Nov 2020 21:01:20 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6f2ce7819480f8698aa11ed1cc180152b229b83d84055b23302d5333a3a01c`  
		Last Modified: Wed, 11 Nov 2020 21:01:20 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312140622316dd22301893e44b627d8ecf2ecf21886f0679078f40af80c4dad0`  
		Last Modified: Wed, 11 Nov 2020 21:01:19 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae32cf038a6af4af39597ba603771fb0b2688d5115f90e3e0a8f478638496431`  
		Last Modified: Wed, 11 Nov 2020 21:01:16 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544b2275c156b747ed298cc1d4fa2c7ea9963fdcc008cfcc9cabc428c8e62db3`  
		Last Modified: Wed, 11 Nov 2020 21:01:17 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b208564e0dfb1a5f3a2cfb06f0781056ccd741d16aa35a666c9098566f731881`  
		Last Modified: Wed, 11 Nov 2020 21:01:16 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bb9ee1a8500dc7fff16801c4258123a3437964735ba1e97521d0c58cbe9394`  
		Last Modified: Wed, 11 Nov 2020 21:01:17 GMT  
		Size: 250.9 KB (250895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5647190d14b3b4a098f47097beb01bd57348258c58a82b4031d028fc431a5a8`  
		Last Modified: Wed, 11 Nov 2020 21:01:16 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-alpine`

```console
$ docker pull caddy@sha256:acf4730fd996e56a713b99d6f1892b87bf9f95af4ebc5fed53e942986ffbc2cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.1.1-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:94aab32108ee277eca3476c03eb3cd0c791581ccceef288e4021b4658b6e14e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16160083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:813d26d5b5f80df7e1a12968331cc52103ef347206fdfe404f095db39538745f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:33:22 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 04:33:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Thu, 22 Oct 2020 04:33:24 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 22 Oct 2020 04:33:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 04:33:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 04:33:30 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 04:33:30 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 04:33:31 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 04:33:31 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 04:33:31 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Thu, 22 Oct 2020 04:33:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 04:33:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 04:33:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 04:33:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 04:33:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 04:33:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 04:33:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 04:33:34 GMT
EXPOSE 80
# Thu, 22 Oct 2020 04:33:34 GMT
EXPOSE 443
# Thu, 22 Oct 2020 04:33:35 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 04:33:35 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 04:33:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2e2d825895b6421ca5dbd63db0d99f790ef84a84c7bcaff51e60b654397858`  
		Last Modified: Thu, 22 Oct 2020 04:34:47 GMT  
		Size: 300.0 KB (299956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792a8e39706390221a8cc5927203b39027a0bce4149c60137a8a68c14124a188`  
		Last Modified: Thu, 22 Oct 2020 04:34:47 GMT  
		Size: 5.8 KB (5753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e121fa2dd673519fd0bbbe8acae3339d2c242a0d454569905d45fcae45cbd210`  
		Last Modified: Thu, 22 Oct 2020 04:34:50 GMT  
		Size: 13.1 MB (13057360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02cabd94ff7acf4922fc1f955d07f4c8a22e63a2cb69ca77d49d20629759e6d7`  
		Last Modified: Thu, 22 Oct 2020 04:34:46 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:3dcf641ed85190e11d4d2aeee30ce6fd5e12acaf14764d0ecc9c2d43cc5c52f2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15322911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55dc188cdeb883fd020df45c6c2e4274e437337e1820e0db79e0b0ff14295b34`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:58:10 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 02:58:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Thu, 22 Oct 2020 02:58:13 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 22 Oct 2020 02:58:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 02:58:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:58:22 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 02:58:23 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 02:58:23 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 02:58:24 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 02:58:25 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Thu, 22 Oct 2020 02:58:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 02:58:26 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 02:58:27 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 02:58:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 02:58:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 02:58:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 02:58:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 02:58:30 GMT
EXPOSE 80
# Thu, 22 Oct 2020 02:58:31 GMT
EXPOSE 443
# Thu, 22 Oct 2020 02:58:32 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 02:58:32 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 02:58:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7369c3ac4b39c55c74e96dd3eb61ac2fa65e5671b1c2acca9697a7c9d20c3cf`  
		Last Modified: Thu, 22 Oct 2020 02:59:49 GMT  
		Size: 300.1 KB (300086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0affadb729cb104658a545e4b2cd1eb71a6f4ca473a7576bb6a65d97de2003ff`  
		Last Modified: Thu, 22 Oct 2020 02:59:49 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a834360c16db0f4578fa61b1bb8e51d39cfdfa7616b763a7f9080b5f3fd337`  
		Last Modified: Thu, 22 Oct 2020 02:59:55 GMT  
		Size: 12.4 MB (12414928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1dea75e2b66ab3649bf01ef2e7accd82012104cf4bc9dd180b75298b9335941`  
		Last Modified: Thu, 22 Oct 2020 02:59:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:3ad6c0a0783ba264b9258c26ecd947b8c1ddd9ce0eedf47bf50e0d92ce26b253
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15106906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baa5aceec9b3b914788468802d025e1d1f3551a181c58365d22efa3fe8dfb9f3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:04:57 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 03:05:00 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Thu, 22 Oct 2020 03:05:01 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 22 Oct 2020 03:05:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 03:05:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:05:11 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 03:05:12 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 03:05:13 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 03:05:13 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 03:05:14 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Thu, 22 Oct 2020 03:05:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 03:05:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 03:05:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 03:05:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 03:05:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 03:05:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 03:05:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 03:05:22 GMT
EXPOSE 80
# Thu, 22 Oct 2020 03:05:23 GMT
EXPOSE 443
# Thu, 22 Oct 2020 03:05:24 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 03:05:26 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 03:05:27 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a8e7fe5034ac502626b0a921d79be80c092890176e33b236c489d6f00710a2`  
		Last Modified: Thu, 22 Oct 2020 03:06:32 GMT  
		Size: 299.2 KB (299211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eac4e817bcf2c7b80f6f6341ad2e45a1a984b272460858c08c1a39ca8acddbe`  
		Last Modified: Thu, 22 Oct 2020 03:06:32 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4916ca18103e521657f386ae15b838945f507f4e71e7ffb9ae6146a207fc98e4`  
		Last Modified: Thu, 22 Oct 2020 03:06:36 GMT  
		Size: 12.4 MB (12396037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516dbda4db0089c1377a5f56e371ecf8ebada5ddedf4eb445b7b5a00b35837a0`  
		Last Modified: Thu, 22 Oct 2020 03:06:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:bed04cea05f8703919db1411fa43db3caf2c5feee4604e432ca3fbb39ba4e9e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.0 MB (15025979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d3072bf9e0127310f4d1cc1237287c7562fe9fe90f9e7084ef33d8ebd97fb70`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:40:04 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 02:40:08 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Thu, 22 Oct 2020 02:40:09 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 22 Oct 2020 02:40:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 02:40:18 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:40:22 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 02:40:22 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 02:40:24 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 02:40:25 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 02:40:26 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Thu, 22 Oct 2020 02:40:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 02:40:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 02:40:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 02:40:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 02:40:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 02:40:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 02:40:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 02:40:33 GMT
EXPOSE 80
# Thu, 22 Oct 2020 02:40:33 GMT
EXPOSE 443
# Thu, 22 Oct 2020 02:40:35 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 02:40:36 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 02:40:37 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dbde357077a97c0f831033bf03c9828203cb7e3e6cb33217ce4d7cfd71c931`  
		Last Modified: Thu, 22 Oct 2020 02:41:47 GMT  
		Size: 300.3 KB (300348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede963cf3892bef49a806e2b2b6cd351a073839746d3ba0040c807c9ede34282`  
		Last Modified: Thu, 22 Oct 2020 02:41:47 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30dd5666b9cb9cb79f2931d16947dff6632df90edde47a765a9abb46d21a7f8e`  
		Last Modified: Thu, 22 Oct 2020 02:41:50 GMT  
		Size: 12.0 MB (12013098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac0780379a69d70077155f92bdaf6679c77647156daf6c6b61784db51baf0b`  
		Last Modified: Thu, 22 Oct 2020 02:41:47 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:013e8f3007f8464b73d523c0620524d183067549b162c35f7c34a104b2e03c19
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14896989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a7eb13196205b2269a7eba953f625b2a6cb717e66971db551bcc960cd917cc2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 13:39:52 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 13:40:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Thu, 22 Oct 2020 13:40:25 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 22 Oct 2020 13:40:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 13:41:03 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 13:41:08 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 13:41:13 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 13:41:19 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 13:41:26 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 13:41:32 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Thu, 22 Oct 2020 13:41:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 13:41:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 13:41:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 13:42:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 13:42:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 13:42:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 13:42:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 13:42:18 GMT
EXPOSE 80
# Thu, 22 Oct 2020 13:42:23 GMT
EXPOSE 443
# Thu, 22 Oct 2020 13:42:29 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 13:42:34 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 13:42:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649a4964211b7ce86541a0c1dad8ef3800ec38a3ca90aff94b76759b4cb8e279`  
		Last Modified: Thu, 22 Oct 2020 13:47:22 GMT  
		Size: 302.3 KB (302327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d796f3d42ae827c5c6abc4f1d86eb2c77d579b52d88f20195c3480d66f3e0af`  
		Last Modified: Thu, 22 Oct 2020 13:47:22 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b45c60413a5845a6a452dfc06bfecd19bdcb7111f4c5011c9c273914f54284`  
		Last Modified: Thu, 22 Oct 2020 13:47:26 GMT  
		Size: 11.8 MB (11785457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae3c1c0668096c5f9942efa1b8694a27b599f3996495b052f5cd7f6e0188781`  
		Last Modified: Thu, 22 Oct 2020 13:47:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:937db8998b02f140f7b1dc4d9b6a14ff40db24dfdc22d4b1d1f5d0d0509e67ba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15709107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:007a65f150c3943695dbf4e3018205572467467599ba7ea5010e044f5fced62d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:41:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 02:41:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Thu, 22 Oct 2020 02:41:10 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 22 Oct 2020 02:41:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 02:41:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:41:15 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 02:41:15 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 02:41:16 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 02:41:16 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 02:41:16 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Thu, 22 Oct 2020 02:41:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 02:41:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 02:41:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 02:41:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 02:41:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 02:41:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 02:41:19 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 02:41:19 GMT
EXPOSE 80
# Thu, 22 Oct 2020 02:41:19 GMT
EXPOSE 443
# Thu, 22 Oct 2020 02:41:20 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 02:41:20 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 02:41:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f988ff23f3cbb35bfed69e33f3b7ee69403bfae4f46363a08eea4830053e9c`  
		Last Modified: Thu, 22 Oct 2020 02:42:01 GMT  
		Size: 300.5 KB (300481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb33c2548f9314af36267dc9e886d94ad83d75881e0c93b6931ed52734b7f451`  
		Last Modified: Thu, 22 Oct 2020 02:42:01 GMT  
		Size: 5.8 KB (5835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad254f130346e29cbf490913417f35cf7473184bba1b7ff8d90579f3b2809a29`  
		Last Modified: Thu, 22 Oct 2020 02:42:03 GMT  
		Size: 12.8 MB (12836808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf01317e485bb835fdf7067969a86d9fa9679bdd0a1c214931b788e4b8e9388f`  
		Last Modified: Thu, 22 Oct 2020 02:42:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-builder`

```console
$ docker pull caddy@sha256:95e1fe51712d93a8fd5da1d8e49c09ac5d923aaa5dff1e0a68f0e9b78a093f1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1577; amd64
	-	windows version 10.0.14393.4046; amd64

### `caddy:2.1.1-builder` - linux; amd64

```console
$ docker pull caddy@sha256:37c634e75d14fc942393b95a9ca1803bc2e6eb39276cdbcb41f04653eb1aca3d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120346515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b3c25baf9316333b4308baa85ff5c4f5bdcdd0f2b43f480277a2427e10d43c6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:34:56 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:34:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:34:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:25:03 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 04 Dec 2020 00:27:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.13.src.tar.gz'; 	sha256='ba1d244c6b5c0ed04aa0d7856d06aceb89ed31b895de6ff783efb1cc8ab6b177'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:27:20 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:27:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:27:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:27:22 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:48:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:48:55 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:48:55 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 04 Dec 2020 00:48:55 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:48:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:48:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:48:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef7d3d256c8367c41c431143c63d083a25dd62ec9ee9d9773dd9e6c7b70ec9e`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 280.8 KB (280812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9db76c5a1d06710ed4f3073476b2d883ff8e911f8e47c558bc4a8d1d8663fa`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff250548074e76394d085b3a57acccc88c05cbde1dbb4b27f7a7d3f752d1df0`  
		Last Modified: Fri, 04 Dec 2020 00:32:49 GMT  
		Size: 107.6 MB (107550990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c86fa391e3d32b3d1db825e61ae70f87831992751d5971c62c587526b7909cb`  
		Last Modified: Fri, 04 Dec 2020 00:32:32 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1f309d33d760b2353f1b3cb1949ec8696c5076f42b245ae14aa1a1976fb8ab`  
		Last Modified: Fri, 04 Dec 2020 00:49:38 GMT  
		Size: 8.3 MB (8309953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a78bef7d8825ad6c9b092e9a9151f84af560335cd3492c3cd800bcf829eabda`  
		Last Modified: Fri, 04 Dec 2020 00:49:36 GMT  
		Size: 1.4 MB (1407215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0ee2ac4bf7c1c60fccb631b07fc1371698f356b1bf848be393ead9c77914e1`  
		Last Modified: Fri, 04 Dec 2020 00:49:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:874395176d58c742c946cc8f61eaa731193fe214db4df70fedea0f3f960b50c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116049846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f047b5860fd0f2aaa22d3e99a7374a5d9cd7f6b9fb0cfaa13745c68dc93cc4bf`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:07:24 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:07:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:07:27 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:57:43 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 04 Dec 2020 01:00:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.13.src.tar.gz'; 	sha256='ba1d244c6b5c0ed04aa0d7856d06aceb89ed31b895de6ff783efb1cc8ab6b177'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:00:31 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:00:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:00:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:00:41 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:23:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:23:33 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:23:34 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 04 Dec 2020 01:23:35 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:23:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:23:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:23:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20cc27a60e8ac1bf56dec787d3d52ba856e657179cfd56050036db79abb4267`  
		Last Modified: Thu, 22 Oct 2020 05:34:55 GMT  
		Size: 281.0 KB (280971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ecce92c3d2de40638d73e682dec26c2b79a055e85c8d70b88f4ccb9485bb9c9`  
		Last Modified: Thu, 22 Oct 2020 05:34:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c6a5805555088ebcf57777ba09456d944209f651c7ecc238ae7c72d5267696`  
		Last Modified: Fri, 04 Dec 2020 01:06:46 GMT  
		Size: 103.9 MB (103910059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0faa1fe22738eddfa05316081c07537fadf4d98d8fd03ef17c20e1b9279d3a5`  
		Last Modified: Fri, 04 Dec 2020 01:05:42 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ec764486071731ef492a5289711adf9fd4b962821f8ce65f4e89f29b7e1246`  
		Last Modified: Fri, 04 Dec 2020 01:24:16 GMT  
		Size: 7.9 MB (7928839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acdffbbadb25c98c1e272b050823d5715b8c59f9fca8eee71195a51c1a4029ce`  
		Last Modified: Fri, 04 Dec 2020 01:24:14 GMT  
		Size: 1.3 MB (1327351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475cfeba331857a969f00590b366cd2171462f79606fc9deff1065ff1c719607`  
		Last Modified: Fri, 04 Dec 2020 01:24:13 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:e03abef2fec55f201484597a22643a5f555b17f5bebdc057334bd7a301f424b7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114812725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c2dfdfc3751b3030414e6c70bc516989641ccce757579869a633b3b31862af8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:21:35 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:23:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:23:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:07:09 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 04 Dec 2020 00:09:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.13.src.tar.gz'; 	sha256='ba1d244c6b5c0ed04aa0d7856d06aceb89ed31b895de6ff783efb1cc8ab6b177'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:09:40 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:09:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:09:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:09:44 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:33:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:33:05 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:33:05 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 04 Dec 2020 00:33:08 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:33:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:33:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:33:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b753cfc04fdce9640aac1e7a4b3e7ce15fa60b8e357376e42f294f463a6e890`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 280.1 KB (280084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e90c422e5e4668cb4140aadb622d734faa93c81cc1e283da9b08bbbc65c45c5`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc832c4959c984d61cbf9ca04945922a7ac84d32c9a7dbfc4000f56b593f8fe`  
		Last Modified: Fri, 04 Dec 2020 00:16:33 GMT  
		Size: 103.7 MB (103655540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75782af3feb5c44682b68de6dbe1678c0028b8316b235c6bb325c9b96d47466f`  
		Last Modified: Fri, 04 Dec 2020 00:15:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3103923df4c137961411ee9beb2163bb0fceb96024cab996b338fff9dec323cb`  
		Last Modified: Fri, 04 Dec 2020 00:33:59 GMT  
		Size: 7.1 MB (7144867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4267c9a980b43f5e19848c54b902901643b512e49bca7eeb2694d6395d58d9e5`  
		Last Modified: Fri, 04 Dec 2020 00:33:59 GMT  
		Size: 1.3 MB (1325844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95b1cb145016023a360ff49d799308bb9a33fdaa990f076ead6e8454424856e`  
		Last Modified: Fri, 04 Dec 2020 00:33:58 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:c342415c2eacab2e75ff361dc7a30271d8693f36dfa5812bc9a73b45fb7650e8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115766627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e26fb7973448a7a127743363016ea1407c9372ff89327d196152ccb285a64d74`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:08:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 04:09:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 04:09:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:02:52 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 04 Dec 2020 01:04:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.13.src.tar.gz'; 	sha256='ba1d244c6b5c0ed04aa0d7856d06aceb89ed31b895de6ff783efb1cc8ab6b177'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:04:52 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:04:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:04:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:04:56 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:28:06 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:28:07 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:28:08 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 04 Dec 2020 01:28:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:28:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:28:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:28:13 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4357932f1b6fb010e1461cc5c673712fb832ac44ee627c691db0b64adf95d13`  
		Last Modified: Thu, 22 Oct 2020 04:28:32 GMT  
		Size: 281.2 KB (281230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c013af1878066e59b688e31fd962e7267430963de27c5257241e3c223aa1d6`  
		Last Modified: Thu, 22 Oct 2020 04:28:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f038c27fba9771a10e2d17f066f31884e1d64e9d50f996d4e1f98c7d9eca6df5`  
		Last Modified: Fri, 04 Dec 2020 01:11:44 GMT  
		Size: 103.0 MB (102968080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb141fcf8afeddffe403b798e502235e8746a2bbcecb5325ae2067d6e64aedc`  
		Last Modified: Fri, 04 Dec 2020 01:11:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237402524d7a7d687e3e2866ec83f21ad5a498ed7f26f1a8236cda6b5f560929`  
		Last Modified: Fri, 04 Dec 2020 01:28:54 GMT  
		Size: 8.5 MB (8499866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8c71374c7630456a387209dca122b16a8038192403356b827b0dfa2ab77eff`  
		Last Modified: Fri, 04 Dec 2020 01:28:52 GMT  
		Size: 1.3 MB (1310182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b6da552cad766345c3058306ad61d20a6f02651f46d71ce40583fc9f18762f7`  
		Last Modified: Fri, 04 Dec 2020 01:28:52 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:a3966dfa7df24217bd14943995fc0e4d6d8084992a5c389ccbca4f4118804b22
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115150516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ef65b689756199e63647a98cebfe48993694a73b122f91d3be33a2d69ce7c56`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 13:27:26 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 13:27:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 13:27:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:59:55 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 04 Dec 2020 02:01:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.13.src.tar.gz'; 	sha256='ba1d244c6b5c0ed04aa0d7856d06aceb89ed31b895de6ff783efb1cc8ab6b177'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 02:02:08 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 02:02:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 02:02:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 02:02:24 GMT
WORKDIR /go
# Fri, 04 Dec 2020 03:12:29 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 03:12:32 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 03:12:34 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 04 Dec 2020 03:12:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 03:12:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 03:12:53 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 03:12:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9900411dc7c8c88618743573bf89478d726007403bd002d8b00d21b7fecd40a`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 283.2 KB (283205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbd106374e3baf7eb8e3d8f7ffd4c364a35e57dcb3a89f8a153327a4c3fa3f9`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f63d5e2daabbfe6e2070563b812f7d8cedf414d153c493cd60bfc611e364dc9`  
		Last Modified: Fri, 04 Dec 2020 02:08:29 GMT  
		Size: 101.9 MB (101855605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07277d6b2e6785d1fc5318d4c63b413a76cb86a9d7beeb0d20bdd835d34eea19`  
		Last Modified: Fri, 04 Dec 2020 02:08:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6e1068327176aa38aa1e6a20aa01eeeb3b9427cbc0f41fbe367cc06474325b`  
		Last Modified: Fri, 04 Dec 2020 03:14:31 GMT  
		Size: 8.9 MB (8919981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86508b35ca9f1a8e0db3f8fc347a62e1e17b591a7785c85705169631d0df17d1`  
		Last Modified: Fri, 04 Dec 2020 03:14:28 GMT  
		Size: 1.3 MB (1287791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50938474f3e06598b1f0264f5bc734dde207d35f09f032ddae0bcf66fe7252e2`  
		Last Modified: Fri, 04 Dec 2020 03:14:28 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; s390x

```console
$ docker pull caddy@sha256:bf8caa0f019fb0999c392266cf4e3a264fd4c0f3685bee59d8a965ad6305193e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (120039213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:398dee0be71a224156b351a0adc7bc90512ff969cdc7837e637456cfb9531d55`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:53:28 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 02:53:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:53:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:46:14 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 04 Dec 2020 00:47:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.13.src.tar.gz'; 	sha256='ba1d244c6b5c0ed04aa0d7856d06aceb89ed31b895de6ff783efb1cc8ab6b177'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:47:41 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:47:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:47:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:47:43 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:07:42 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:07:42 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:07:43 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 04 Dec 2020 01:07:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:07:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:07:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:07:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5139d7663b8674a989574c2161166fb137f26ef16b2f701159c126628be75101`  
		Last Modified: Thu, 22 Oct 2020 02:58:32 GMT  
		Size: 281.4 KB (281363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d31a06258ad66efe2dedbf67809ebc107a55757b8a4543af77982f55ff6c067`  
		Last Modified: Thu, 22 Oct 2020 02:58:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4af143192364283094ca6d9b924b285fd263d85c957e8773636fc1ab14921ef`  
		Last Modified: Fri, 04 Dec 2020 00:51:33 GMT  
		Size: 107.5 MB (107450340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25cd2600cf17527ed939778c1110c5123d270458bd9de2bdfab8ceca3a203f9`  
		Last Modified: Fri, 04 Dec 2020 00:51:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f76e8753616ace4e8255edb836ebcea36a2048b3f956d592b6bbc5d2d608894`  
		Last Modified: Fri, 04 Dec 2020 01:08:14 GMT  
		Size: 8.4 MB (8352215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc5acda2876b28737fe05138b35bfeb675b33a36bfa7bd50f2d0e7b85084ef6`  
		Last Modified: Fri, 04 Dec 2020 01:08:12 GMT  
		Size: 1.4 MB (1388750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e1eee272ccb1c907dc426c8f9b4e95a2045ae34aacaacf633857db7757f269`  
		Last Modified: Fri, 04 Dec 2020 01:08:12 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - windows version 10.0.17763.1577; amd64

```console
$ docker pull caddy@sha256:f4ff8952c10616f52af89dc23dc7efa343fa7a747ad539fce189352ad01d260d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2562528759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b72c51baf7e34b3c543e7120ae03f5c4488a93741d5ec109d82633a358ddbb45`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 13:43:36 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Nov 2020 13:43:37 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Nov 2020 13:43:38 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Nov 2020 13:43:38 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Nov 2020 13:44:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 13:44:33 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Nov 2020 13:44:55 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Dec 2020 00:24:14 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 04 Dec 2020 00:26:40 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.14.13.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '18c5597d7648ce3872f4a0a7bc73a70c01b56b77feac5e5f80b2ecba0d231473'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Dec 2020 00:26:42 GMT
WORKDIR C:\gopath
# Fri, 04 Dec 2020 00:55:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Dec 2020 00:55:12 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:55:13 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 04 Dec 2020 00:55:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:55:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Dec 2020 00:55:38 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19e00ae033e023d5973e57402eb3f05fe0908fa3f40cd0a36ae20bc72df3927`  
		Last Modified: Wed, 11 Nov 2020 14:08:35 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7f2350f21c33479862fe11c4c46ef7fc8054cb8e0acb2581b663d9e71d37f4`  
		Last Modified: Wed, 11 Nov 2020 14:08:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b816110035a14bde6916267f7e5f008617773d19d8f23f77597d10b021b787c`  
		Last Modified: Wed, 11 Nov 2020 14:08:30 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7a389242a4449d1ca90994817f199ce0b9ec502e46035e6ea9c78c29282ce8`  
		Last Modified: Wed, 11 Nov 2020 14:08:29 GMT  
		Size: 1.1 KB (1098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c993585709f02af194d96f01fb74b3158a083cac1cbf2036662bd0abab75e3bf`  
		Last Modified: Wed, 11 Nov 2020 14:08:38 GMT  
		Size: 34.3 MB (34333277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822a63153155fc14ab856f02664a39a3dbf45ef8601277d161d64e9475748111`  
		Last Modified: Wed, 11 Nov 2020 14:08:26 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758771af484f25fbbe9ef11107e3680d525f6bfc5a1666db73f0eb9d84be3ef1`  
		Last Modified: Wed, 11 Nov 2020 14:08:26 GMT  
		Size: 311.3 KB (311320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0deb38ac5fb082b9321af2d974d10b3ce922ac605d17f979b6105118f00603`  
		Last Modified: Fri, 04 Dec 2020 00:35:37 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a3d529dbd6fc062c0dedc7422de9f5720cb9fad234e62499143181db538a613`  
		Last Modified: Fri, 04 Dec 2020 00:36:16 GMT  
		Size: 138.1 MB (138071680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb4540380ae74470f6b36b8d8d9dd14b7920813785e538bb6bdfab798cf0f22`  
		Last Modified: Fri, 04 Dec 2020 00:35:37 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:432d3805408bf37025204b16134a4357d9506daea4e89a0ac431bf6b16f71b35`  
		Last Modified: Fri, 04 Dec 2020 01:00:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702c8cf3fb19edf3f5ebda7a34576b7eae2fcf4ef38781205636a5a5337476d8`  
		Last Modified: Fri, 04 Dec 2020 00:59:58 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6da90c4051ad7cef8bfcb1e9aa2f3ff759afe51099b95c33151720102407914`  
		Last Modified: Fri, 04 Dec 2020 00:59:59 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e203f1b0bc2f9559d70a48c0beb32ec59f38abd6bea166e0e66645e3c472c5db`  
		Last Modified: Fri, 04 Dec 2020 00:59:58 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30015a8bc9570d30132e3ceedcb131736a1bbd8fbaa10fe50ec2bed40288493b`  
		Last Modified: Fri, 04 Dec 2020 00:59:59 GMT  
		Size: 1.8 MB (1768229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d683e4f27a110473c64683f2d522957b376300e9f51a94a581ce023669faf621`  
		Last Modified: Fri, 04 Dec 2020 00:59:58 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - windows version 10.0.14393.4046; amd64

```console
$ docker pull caddy@sha256:e83ec0fac89209a280261c91bd831afbd7728537b8fedd475b84a0e53e7edea1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5966171444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca04e2a22b05db16222e1cd7d820df601df419f73083f47e7439b10c15ab77e0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 13:23:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 13:47:33 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Nov 2020 13:47:34 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Nov 2020 13:47:34 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Nov 2020 13:47:35 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Nov 2020 13:49:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 13:49:05 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Nov 2020 13:51:21 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Dec 2020 00:26:56 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 04 Dec 2020 00:30:14 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.14.13.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '18c5597d7648ce3872f4a0a7bc73a70c01b56b77feac5e5f80b2ecba0d231473'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Dec 2020 00:30:16 GMT
WORKDIR C:\gopath
# Fri, 04 Dec 2020 00:55:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Dec 2020 00:55:43 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:55:44 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 04 Dec 2020 00:55:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:57:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Dec 2020 00:57:06 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:126d9a92c0cb7b68c56dec2dd5ba118de9dde3ec6368db734c5135fdf1528a33`  
		Last Modified: Wed, 11 Nov 2020 13:34:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48cdfe7c39f0358056c4c821593e466beab0dd18e49c8fae5aead3044dc4fcc`  
		Last Modified: Wed, 11 Nov 2020 14:09:26 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725a072d8cce622c524652fc146ce1398a73435bfe34b503ce6df7c2ba1954c5`  
		Last Modified: Wed, 11 Nov 2020 14:09:26 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff5342fb3e45a27028014ad657c3d05414fac6d9ea2e1213ac67ebd51c174f5`  
		Last Modified: Wed, 11 Nov 2020 14:09:23 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada6bdd6092185cd48a4b7a37d2fccf12a0598e2793361256a3658393e27de45`  
		Last Modified: Wed, 11 Nov 2020 14:09:22 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcaf43c793d08d3feb1cb8666a774e8709fd62cf468af1fcf7c3470bb777e5bc`  
		Last Modified: Wed, 11 Nov 2020 14:10:05 GMT  
		Size: 35.2 MB (35173627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e19e3e1a800738fb7127bdfaabdc86eb626a4b1ea386389bcc158ee6afcf2e8`  
		Last Modified: Wed, 11 Nov 2020 14:09:19 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8d4839ac80d0d8b637b35572732039f3c4bc755fbfa2ca871d32cf344c0032`  
		Last Modified: Wed, 11 Nov 2020 14:09:25 GMT  
		Size: 5.5 MB (5520399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48107a5c25f5d16a079d6bf63be2c5ae5cc551d3eec171da0546cd30e55ca338`  
		Last Modified: Fri, 04 Dec 2020 00:36:28 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1164832aabf2b2c477feadd272f6cab2f4d13a099314cb39700a1c15489865b9`  
		Last Modified: Fri, 04 Dec 2020 00:36:56 GMT  
		Size: 143.4 MB (143408851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56ca390d4244fa6ba37b42b4cc2a0ef8af88a1da0600f8c8058d68ef8f2c663`  
		Last Modified: Fri, 04 Dec 2020 00:36:28 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ee859d6ec81f6f1bcbbdf41b5f24e22a0c202ae7db85a512ade9227e0cc6db`  
		Last Modified: Fri, 04 Dec 2020 01:00:24 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69acca1f38dc5ecbe8e5b77d24a213f4fd113a6de353474b2cd472da5323da00`  
		Last Modified: Fri, 04 Dec 2020 01:00:20 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0922e22528306a039315e51dafb5290c8ec59e0699dbb0dab2e1092d0ae45a`  
		Last Modified: Fri, 04 Dec 2020 01:00:21 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc2647968a29567396d04d7ca91082120cabfa06c3fdea8b8d24711ddbfce38`  
		Last Modified: Fri, 04 Dec 2020 01:00:21 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c12526e6d6b37fa344dfda15400d6d543b1f93ba344645c0666cf79e76efd5`  
		Last Modified: Fri, 04 Dec 2020 01:00:24 GMT  
		Size: 11.5 MB (11494818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4060a5bbf9cd583d07592707493f6f140bb54291340b96443b4d9a7b801a5cdf`  
		Last Modified: Fri, 04 Dec 2020 01:00:21 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-builder-alpine`

```console
$ docker pull caddy@sha256:737e51762dc709a0cf2fc4aa7db7628cbbef829011fde8be43fa2135dfabfb64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.1.1-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:37c634e75d14fc942393b95a9ca1803bc2e6eb39276cdbcb41f04653eb1aca3d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120346515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b3c25baf9316333b4308baa85ff5c4f5bdcdd0f2b43f480277a2427e10d43c6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:34:56 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:34:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:34:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:25:03 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 04 Dec 2020 00:27:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.13.src.tar.gz'; 	sha256='ba1d244c6b5c0ed04aa0d7856d06aceb89ed31b895de6ff783efb1cc8ab6b177'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:27:20 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:27:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:27:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:27:22 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:48:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:48:55 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:48:55 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 04 Dec 2020 00:48:55 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:48:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:48:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:48:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef7d3d256c8367c41c431143c63d083a25dd62ec9ee9d9773dd9e6c7b70ec9e`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 280.8 KB (280812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9db76c5a1d06710ed4f3073476b2d883ff8e911f8e47c558bc4a8d1d8663fa`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff250548074e76394d085b3a57acccc88c05cbde1dbb4b27f7a7d3f752d1df0`  
		Last Modified: Fri, 04 Dec 2020 00:32:49 GMT  
		Size: 107.6 MB (107550990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c86fa391e3d32b3d1db825e61ae70f87831992751d5971c62c587526b7909cb`  
		Last Modified: Fri, 04 Dec 2020 00:32:32 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1f309d33d760b2353f1b3cb1949ec8696c5076f42b245ae14aa1a1976fb8ab`  
		Last Modified: Fri, 04 Dec 2020 00:49:38 GMT  
		Size: 8.3 MB (8309953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a78bef7d8825ad6c9b092e9a9151f84af560335cd3492c3cd800bcf829eabda`  
		Last Modified: Fri, 04 Dec 2020 00:49:36 GMT  
		Size: 1.4 MB (1407215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0ee2ac4bf7c1c60fccb631b07fc1371698f356b1bf848be393ead9c77914e1`  
		Last Modified: Fri, 04 Dec 2020 00:49:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:874395176d58c742c946cc8f61eaa731193fe214db4df70fedea0f3f960b50c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116049846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f047b5860fd0f2aaa22d3e99a7374a5d9cd7f6b9fb0cfaa13745c68dc93cc4bf`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:07:24 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:07:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:07:27 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:57:43 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 04 Dec 2020 01:00:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.13.src.tar.gz'; 	sha256='ba1d244c6b5c0ed04aa0d7856d06aceb89ed31b895de6ff783efb1cc8ab6b177'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:00:31 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:00:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:00:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:00:41 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:23:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:23:33 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:23:34 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 04 Dec 2020 01:23:35 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:23:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:23:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:23:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20cc27a60e8ac1bf56dec787d3d52ba856e657179cfd56050036db79abb4267`  
		Last Modified: Thu, 22 Oct 2020 05:34:55 GMT  
		Size: 281.0 KB (280971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ecce92c3d2de40638d73e682dec26c2b79a055e85c8d70b88f4ccb9485bb9c9`  
		Last Modified: Thu, 22 Oct 2020 05:34:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c6a5805555088ebcf57777ba09456d944209f651c7ecc238ae7c72d5267696`  
		Last Modified: Fri, 04 Dec 2020 01:06:46 GMT  
		Size: 103.9 MB (103910059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0faa1fe22738eddfa05316081c07537fadf4d98d8fd03ef17c20e1b9279d3a5`  
		Last Modified: Fri, 04 Dec 2020 01:05:42 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ec764486071731ef492a5289711adf9fd4b962821f8ce65f4e89f29b7e1246`  
		Last Modified: Fri, 04 Dec 2020 01:24:16 GMT  
		Size: 7.9 MB (7928839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acdffbbadb25c98c1e272b050823d5715b8c59f9fca8eee71195a51c1a4029ce`  
		Last Modified: Fri, 04 Dec 2020 01:24:14 GMT  
		Size: 1.3 MB (1327351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475cfeba331857a969f00590b366cd2171462f79606fc9deff1065ff1c719607`  
		Last Modified: Fri, 04 Dec 2020 01:24:13 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:e03abef2fec55f201484597a22643a5f555b17f5bebdc057334bd7a301f424b7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114812725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c2dfdfc3751b3030414e6c70bc516989641ccce757579869a633b3b31862af8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:21:35 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:23:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:23:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:07:09 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 04 Dec 2020 00:09:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.13.src.tar.gz'; 	sha256='ba1d244c6b5c0ed04aa0d7856d06aceb89ed31b895de6ff783efb1cc8ab6b177'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:09:40 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:09:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:09:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:09:44 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:33:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:33:05 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:33:05 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 04 Dec 2020 00:33:08 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:33:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:33:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:33:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b753cfc04fdce9640aac1e7a4b3e7ce15fa60b8e357376e42f294f463a6e890`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 280.1 KB (280084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e90c422e5e4668cb4140aadb622d734faa93c81cc1e283da9b08bbbc65c45c5`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc832c4959c984d61cbf9ca04945922a7ac84d32c9a7dbfc4000f56b593f8fe`  
		Last Modified: Fri, 04 Dec 2020 00:16:33 GMT  
		Size: 103.7 MB (103655540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75782af3feb5c44682b68de6dbe1678c0028b8316b235c6bb325c9b96d47466f`  
		Last Modified: Fri, 04 Dec 2020 00:15:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3103923df4c137961411ee9beb2163bb0fceb96024cab996b338fff9dec323cb`  
		Last Modified: Fri, 04 Dec 2020 00:33:59 GMT  
		Size: 7.1 MB (7144867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4267c9a980b43f5e19848c54b902901643b512e49bca7eeb2694d6395d58d9e5`  
		Last Modified: Fri, 04 Dec 2020 00:33:59 GMT  
		Size: 1.3 MB (1325844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95b1cb145016023a360ff49d799308bb9a33fdaa990f076ead6e8454424856e`  
		Last Modified: Fri, 04 Dec 2020 00:33:58 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:c342415c2eacab2e75ff361dc7a30271d8693f36dfa5812bc9a73b45fb7650e8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115766627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e26fb7973448a7a127743363016ea1407c9372ff89327d196152ccb285a64d74`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:08:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 04:09:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 04:09:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:02:52 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 04 Dec 2020 01:04:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.13.src.tar.gz'; 	sha256='ba1d244c6b5c0ed04aa0d7856d06aceb89ed31b895de6ff783efb1cc8ab6b177'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:04:52 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:04:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:04:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:04:56 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:28:06 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:28:07 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:28:08 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 04 Dec 2020 01:28:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:28:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:28:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:28:13 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4357932f1b6fb010e1461cc5c673712fb832ac44ee627c691db0b64adf95d13`  
		Last Modified: Thu, 22 Oct 2020 04:28:32 GMT  
		Size: 281.2 KB (281230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c013af1878066e59b688e31fd962e7267430963de27c5257241e3c223aa1d6`  
		Last Modified: Thu, 22 Oct 2020 04:28:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f038c27fba9771a10e2d17f066f31884e1d64e9d50f996d4e1f98c7d9eca6df5`  
		Last Modified: Fri, 04 Dec 2020 01:11:44 GMT  
		Size: 103.0 MB (102968080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb141fcf8afeddffe403b798e502235e8746a2bbcecb5325ae2067d6e64aedc`  
		Last Modified: Fri, 04 Dec 2020 01:11:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237402524d7a7d687e3e2866ec83f21ad5a498ed7f26f1a8236cda6b5f560929`  
		Last Modified: Fri, 04 Dec 2020 01:28:54 GMT  
		Size: 8.5 MB (8499866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8c71374c7630456a387209dca122b16a8038192403356b827b0dfa2ab77eff`  
		Last Modified: Fri, 04 Dec 2020 01:28:52 GMT  
		Size: 1.3 MB (1310182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b6da552cad766345c3058306ad61d20a6f02651f46d71ce40583fc9f18762f7`  
		Last Modified: Fri, 04 Dec 2020 01:28:52 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:a3966dfa7df24217bd14943995fc0e4d6d8084992a5c389ccbca4f4118804b22
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115150516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ef65b689756199e63647a98cebfe48993694a73b122f91d3be33a2d69ce7c56`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 13:27:26 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 13:27:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 13:27:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:59:55 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 04 Dec 2020 02:01:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.13.src.tar.gz'; 	sha256='ba1d244c6b5c0ed04aa0d7856d06aceb89ed31b895de6ff783efb1cc8ab6b177'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 02:02:08 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 02:02:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 02:02:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 02:02:24 GMT
WORKDIR /go
# Fri, 04 Dec 2020 03:12:29 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 03:12:32 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 03:12:34 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 04 Dec 2020 03:12:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 03:12:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 03:12:53 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 03:12:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9900411dc7c8c88618743573bf89478d726007403bd002d8b00d21b7fecd40a`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 283.2 KB (283205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbd106374e3baf7eb8e3d8f7ffd4c364a35e57dcb3a89f8a153327a4c3fa3f9`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f63d5e2daabbfe6e2070563b812f7d8cedf414d153c493cd60bfc611e364dc9`  
		Last Modified: Fri, 04 Dec 2020 02:08:29 GMT  
		Size: 101.9 MB (101855605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07277d6b2e6785d1fc5318d4c63b413a76cb86a9d7beeb0d20bdd835d34eea19`  
		Last Modified: Fri, 04 Dec 2020 02:08:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6e1068327176aa38aa1e6a20aa01eeeb3b9427cbc0f41fbe367cc06474325b`  
		Last Modified: Fri, 04 Dec 2020 03:14:31 GMT  
		Size: 8.9 MB (8919981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86508b35ca9f1a8e0db3f8fc347a62e1e17b591a7785c85705169631d0df17d1`  
		Last Modified: Fri, 04 Dec 2020 03:14:28 GMT  
		Size: 1.3 MB (1287791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50938474f3e06598b1f0264f5bc734dde207d35f09f032ddae0bcf66fe7252e2`  
		Last Modified: Fri, 04 Dec 2020 03:14:28 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:bf8caa0f019fb0999c392266cf4e3a264fd4c0f3685bee59d8a965ad6305193e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (120039213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:398dee0be71a224156b351a0adc7bc90512ff969cdc7837e637456cfb9531d55`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:53:28 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 02:53:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:53:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:46:14 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 04 Dec 2020 00:47:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.13.src.tar.gz'; 	sha256='ba1d244c6b5c0ed04aa0d7856d06aceb89ed31b895de6ff783efb1cc8ab6b177'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:47:41 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:47:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:47:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:47:43 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:07:42 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:07:42 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:07:43 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 04 Dec 2020 01:07:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:07:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:07:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:07:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5139d7663b8674a989574c2161166fb137f26ef16b2f701159c126628be75101`  
		Last Modified: Thu, 22 Oct 2020 02:58:32 GMT  
		Size: 281.4 KB (281363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d31a06258ad66efe2dedbf67809ebc107a55757b8a4543af77982f55ff6c067`  
		Last Modified: Thu, 22 Oct 2020 02:58:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4af143192364283094ca6d9b924b285fd263d85c957e8773636fc1ab14921ef`  
		Last Modified: Fri, 04 Dec 2020 00:51:33 GMT  
		Size: 107.5 MB (107450340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25cd2600cf17527ed939778c1110c5123d270458bd9de2bdfab8ceca3a203f9`  
		Last Modified: Fri, 04 Dec 2020 00:51:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f76e8753616ace4e8255edb836ebcea36a2048b3f956d592b6bbc5d2d608894`  
		Last Modified: Fri, 04 Dec 2020 01:08:14 GMT  
		Size: 8.4 MB (8352215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc5acda2876b28737fe05138b35bfeb675b33a36bfa7bd50f2d0e7b85084ef6`  
		Last Modified: Fri, 04 Dec 2020 01:08:12 GMT  
		Size: 1.4 MB (1388750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e1eee272ccb1c907dc426c8f9b4e95a2045ae34aacaacf633857db7757f269`  
		Last Modified: Fri, 04 Dec 2020 01:08:12 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:8d15c638f449bfadb74d0dac3005ad4c3f9dd8b216e2eb08abedd8bb4c085c9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `caddy:2.1.1-builder-windowsservercore-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull caddy@sha256:f4ff8952c10616f52af89dc23dc7efa343fa7a747ad539fce189352ad01d260d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2562528759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b72c51baf7e34b3c543e7120ae03f5c4488a93741d5ec109d82633a358ddbb45`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 13:43:36 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Nov 2020 13:43:37 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Nov 2020 13:43:38 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Nov 2020 13:43:38 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Nov 2020 13:44:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 13:44:33 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Nov 2020 13:44:55 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Dec 2020 00:24:14 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 04 Dec 2020 00:26:40 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.14.13.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '18c5597d7648ce3872f4a0a7bc73a70c01b56b77feac5e5f80b2ecba0d231473'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Dec 2020 00:26:42 GMT
WORKDIR C:\gopath
# Fri, 04 Dec 2020 00:55:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Dec 2020 00:55:12 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:55:13 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 04 Dec 2020 00:55:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:55:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Dec 2020 00:55:38 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19e00ae033e023d5973e57402eb3f05fe0908fa3f40cd0a36ae20bc72df3927`  
		Last Modified: Wed, 11 Nov 2020 14:08:35 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7f2350f21c33479862fe11c4c46ef7fc8054cb8e0acb2581b663d9e71d37f4`  
		Last Modified: Wed, 11 Nov 2020 14:08:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b816110035a14bde6916267f7e5f008617773d19d8f23f77597d10b021b787c`  
		Last Modified: Wed, 11 Nov 2020 14:08:30 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7a389242a4449d1ca90994817f199ce0b9ec502e46035e6ea9c78c29282ce8`  
		Last Modified: Wed, 11 Nov 2020 14:08:29 GMT  
		Size: 1.1 KB (1098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c993585709f02af194d96f01fb74b3158a083cac1cbf2036662bd0abab75e3bf`  
		Last Modified: Wed, 11 Nov 2020 14:08:38 GMT  
		Size: 34.3 MB (34333277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822a63153155fc14ab856f02664a39a3dbf45ef8601277d161d64e9475748111`  
		Last Modified: Wed, 11 Nov 2020 14:08:26 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758771af484f25fbbe9ef11107e3680d525f6bfc5a1666db73f0eb9d84be3ef1`  
		Last Modified: Wed, 11 Nov 2020 14:08:26 GMT  
		Size: 311.3 KB (311320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0deb38ac5fb082b9321af2d974d10b3ce922ac605d17f979b6105118f00603`  
		Last Modified: Fri, 04 Dec 2020 00:35:37 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a3d529dbd6fc062c0dedc7422de9f5720cb9fad234e62499143181db538a613`  
		Last Modified: Fri, 04 Dec 2020 00:36:16 GMT  
		Size: 138.1 MB (138071680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb4540380ae74470f6b36b8d8d9dd14b7920813785e538bb6bdfab798cf0f22`  
		Last Modified: Fri, 04 Dec 2020 00:35:37 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:432d3805408bf37025204b16134a4357d9506daea4e89a0ac431bf6b16f71b35`  
		Last Modified: Fri, 04 Dec 2020 01:00:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702c8cf3fb19edf3f5ebda7a34576b7eae2fcf4ef38781205636a5a5337476d8`  
		Last Modified: Fri, 04 Dec 2020 00:59:58 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6da90c4051ad7cef8bfcb1e9aa2f3ff759afe51099b95c33151720102407914`  
		Last Modified: Fri, 04 Dec 2020 00:59:59 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e203f1b0bc2f9559d70a48c0beb32ec59f38abd6bea166e0e66645e3c472c5db`  
		Last Modified: Fri, 04 Dec 2020 00:59:58 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30015a8bc9570d30132e3ceedcb131736a1bbd8fbaa10fe50ec2bed40288493b`  
		Last Modified: Fri, 04 Dec 2020 00:59:59 GMT  
		Size: 1.8 MB (1768229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d683e4f27a110473c64683f2d522957b376300e9f51a94a581ce023669faf621`  
		Last Modified: Fri, 04 Dec 2020 00:59:58 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:7bc295008a3ad00603b75d5681dd62164f5a00cf72bf3e61cf581a43ed01984c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64

### `caddy:2.1.1-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4046; amd64

```console
$ docker pull caddy@sha256:e83ec0fac89209a280261c91bd831afbd7728537b8fedd475b84a0e53e7edea1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5966171444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca04e2a22b05db16222e1cd7d820df601df419f73083f47e7439b10c15ab77e0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 13:23:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 13:47:33 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Nov 2020 13:47:34 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Nov 2020 13:47:34 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Nov 2020 13:47:35 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Nov 2020 13:49:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 13:49:05 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Nov 2020 13:51:21 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Dec 2020 00:26:56 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 04 Dec 2020 00:30:14 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.14.13.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '18c5597d7648ce3872f4a0a7bc73a70c01b56b77feac5e5f80b2ecba0d231473'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Dec 2020 00:30:16 GMT
WORKDIR C:\gopath
# Fri, 04 Dec 2020 00:55:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Dec 2020 00:55:43 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:55:44 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 04 Dec 2020 00:55:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:57:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Dec 2020 00:57:06 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:126d9a92c0cb7b68c56dec2dd5ba118de9dde3ec6368db734c5135fdf1528a33`  
		Last Modified: Wed, 11 Nov 2020 13:34:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48cdfe7c39f0358056c4c821593e466beab0dd18e49c8fae5aead3044dc4fcc`  
		Last Modified: Wed, 11 Nov 2020 14:09:26 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725a072d8cce622c524652fc146ce1398a73435bfe34b503ce6df7c2ba1954c5`  
		Last Modified: Wed, 11 Nov 2020 14:09:26 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff5342fb3e45a27028014ad657c3d05414fac6d9ea2e1213ac67ebd51c174f5`  
		Last Modified: Wed, 11 Nov 2020 14:09:23 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada6bdd6092185cd48a4b7a37d2fccf12a0598e2793361256a3658393e27de45`  
		Last Modified: Wed, 11 Nov 2020 14:09:22 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcaf43c793d08d3feb1cb8666a774e8709fd62cf468af1fcf7c3470bb777e5bc`  
		Last Modified: Wed, 11 Nov 2020 14:10:05 GMT  
		Size: 35.2 MB (35173627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e19e3e1a800738fb7127bdfaabdc86eb626a4b1ea386389bcc158ee6afcf2e8`  
		Last Modified: Wed, 11 Nov 2020 14:09:19 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8d4839ac80d0d8b637b35572732039f3c4bc755fbfa2ca871d32cf344c0032`  
		Last Modified: Wed, 11 Nov 2020 14:09:25 GMT  
		Size: 5.5 MB (5520399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48107a5c25f5d16a079d6bf63be2c5ae5cc551d3eec171da0546cd30e55ca338`  
		Last Modified: Fri, 04 Dec 2020 00:36:28 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1164832aabf2b2c477feadd272f6cab2f4d13a099314cb39700a1c15489865b9`  
		Last Modified: Fri, 04 Dec 2020 00:36:56 GMT  
		Size: 143.4 MB (143408851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56ca390d4244fa6ba37b42b4cc2a0ef8af88a1da0600f8c8058d68ef8f2c663`  
		Last Modified: Fri, 04 Dec 2020 00:36:28 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ee859d6ec81f6f1bcbbdf41b5f24e22a0c202ae7db85a512ade9227e0cc6db`  
		Last Modified: Fri, 04 Dec 2020 01:00:24 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69acca1f38dc5ecbe8e5b77d24a213f4fd113a6de353474b2cd472da5323da00`  
		Last Modified: Fri, 04 Dec 2020 01:00:20 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0922e22528306a039315e51dafb5290c8ec59e0699dbb0dab2e1092d0ae45a`  
		Last Modified: Fri, 04 Dec 2020 01:00:21 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc2647968a29567396d04d7ca91082120cabfa06c3fdea8b8d24711ddbfce38`  
		Last Modified: Fri, 04 Dec 2020 01:00:21 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c12526e6d6b37fa344dfda15400d6d543b1f93ba344645c0666cf79e76efd5`  
		Last Modified: Fri, 04 Dec 2020 01:00:24 GMT  
		Size: 11.5 MB (11494818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4060a5bbf9cd583d07592707493f6f140bb54291340b96443b4d9a7b801a5cdf`  
		Last Modified: Fri, 04 Dec 2020 01:00:21 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-windowsservercore`

```console
$ docker pull caddy@sha256:60f96c725ef75833f8a230e32dc0a59093dd88a38bfaaaafd76777dbdd605f27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64
	-	windows version 10.0.14393.4046; amd64

### `caddy:2.1.1-windowsservercore` - windows version 10.0.17763.1577; amd64

```console
$ docker pull caddy@sha256:e2d41115b10e26568979fd99964d79319400d1008733bd29b0ad270cd446041a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2415318960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca72587c4cf96e2aed3533eac5415b8b05f1282ae904b914b42a5267aa5aac29`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 20:45:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Nov 2020 20:45:21 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 11 Nov 2020 20:45:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Nov 2020 20:45:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Nov 2020 20:45:56 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Nov 2020 20:45:57 GMT
VOLUME [c:/config]
# Wed, 11 Nov 2020 20:45:57 GMT
VOLUME [c:/data]
# Wed, 11 Nov 2020 20:45:58 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 11 Nov 2020 20:45:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Nov 2020 20:46:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Nov 2020 20:46:01 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Nov 2020 20:46:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Nov 2020 20:46:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Nov 2020 20:46:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Nov 2020 20:46:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Nov 2020 20:46:04 GMT
EXPOSE 80
# Wed, 11 Nov 2020 20:46:05 GMT
EXPOSE 443
# Wed, 11 Nov 2020 20:46:05 GMT
EXPOSE 2019
# Wed, 11 Nov 2020 20:46:22 GMT
RUN caddy version
# Wed, 11 Nov 2020 20:46:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9241b8447db6ee01486692864d501d1b85cc8e28b6ba12477da3ccb91ac6fb80`  
		Last Modified: Wed, 11 Nov 2020 21:01:08 GMT  
		Size: 9.2 MB (9248091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140d2864a3ecf900ddcbb7825de568deed4368848546c6f5b33b1031d0d2785c`  
		Last Modified: Wed, 11 Nov 2020 21:01:04 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773bfe60fc2adaea22a607f2ef04801f3a1fe4d1d2742fffd1b3708b9cc2616e`  
		Last Modified: Wed, 11 Nov 2020 21:01:08 GMT  
		Size: 17.7 MB (17722401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6ac34c199b688dcea4ee50fdd427343360897f7b879c92f58e54730a2c7813`  
		Last Modified: Wed, 11 Nov 2020 21:01:03 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37ba66c494cd95e08bddfe1439674935321d50cc6619659859d447d225b9345`  
		Last Modified: Wed, 11 Nov 2020 21:01:03 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa9619dc6858361d1cc3c3459f509b1af176afab3951a8b46ff7cd4065ad56e`  
		Last Modified: Wed, 11 Nov 2020 21:01:00 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d5c4e2731ec2cf1a69fecede53c0cfc076d1c7a3031d9d2f16695b82280856`  
		Last Modified: Wed, 11 Nov 2020 21:01:00 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f78932772adde20a5b82826a3aeca1f6cbea5205a042134ccffb88993a8cbf`  
		Last Modified: Wed, 11 Nov 2020 21:01:00 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6bb7af2868628d7e417e249d60572cb1c53508861a07aa3dcbe601b698fc054`  
		Last Modified: Wed, 11 Nov 2020 21:00:59 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4046f61372cfde3727e85e91767d4eda8547125814b7cc7ace12ea083cf4741b`  
		Last Modified: Wed, 11 Nov 2020 21:00:59 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dfe0ab7ccd8016d0fb2f185efbc294841b8e43d77509a4478fa4cc6edaa4ff`  
		Last Modified: Wed, 11 Nov 2020 21:00:56 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8012fd5e700acdf295c51de57a059928e395cd4654aa5c8fcc6743961b4adf70`  
		Last Modified: Wed, 11 Nov 2020 21:00:56 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298316ad3edcfa6e02b2ed6ad0795b0167fb20254f79c4eb19ad3253c903adb1`  
		Last Modified: Wed, 11 Nov 2020 21:00:57 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451c72395cd914723ccd8dd337a0ca840c0dd00d829d6ce3d9dba4c6462102c9`  
		Last Modified: Wed, 11 Nov 2020 21:00:56 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a43113a9d7534b3a4fbeca6ad58f5ef8e1a6fa5b8d6a488f3d8edda1d7cdd61`  
		Last Modified: Wed, 11 Nov 2020 21:00:56 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369cba41c19fe5008c5dfe0b88cd8f0ef77b138d68c7eca3374c7fbf18d5afcd`  
		Last Modified: Wed, 11 Nov 2020 21:00:53 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0479adc0c263c2e9eab3e3e8fcb7b9d933a95b0f26c04c4c900c5f3804011eb3`  
		Last Modified: Wed, 11 Nov 2020 21:00:53 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea0e70171ceaae4ac02e06588b5aa7f97be0a7e82af15000c7dc8d75dd91c44`  
		Last Modified: Wed, 11 Nov 2020 21:00:53 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b2ec7137cc7d53728109e434d551d89f4694290199f60dfbdfcd4709d8a58f`  
		Last Modified: Wed, 11 Nov 2020 21:00:53 GMT  
		Size: 298.7 KB (298665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e6d60b9c57f55e542ddd3aefdcdbd16da124a2a8142c961c0dab1635429b6c`  
		Last Modified: Wed, 11 Nov 2020 21:00:53 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-windowsservercore` - windows version 10.0.14393.4046; amd64

```console
$ docker pull caddy@sha256:dede9ad27fd496b1102d3530355b3d007bca80608739b3f1beebd3474ce96575
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5803984357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f16f2509b06ce8b2e9d98af30d2ac226c0e89e30a4f81ae6ee79176655906a8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 13:23:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 20:47:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Nov 2020 20:47:53 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 11 Nov 2020 20:49:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Nov 2020 20:49:22 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Nov 2020 20:49:23 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Nov 2020 20:49:24 GMT
VOLUME [c:/config]
# Wed, 11 Nov 2020 20:49:26 GMT
VOLUME [c:/data]
# Wed, 11 Nov 2020 20:49:27 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 11 Nov 2020 20:49:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Nov 2020 20:49:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Nov 2020 20:49:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Nov 2020 20:49:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Nov 2020 20:49:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Nov 2020 20:49:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Nov 2020 20:49:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Nov 2020 20:49:32 GMT
EXPOSE 80
# Wed, 11 Nov 2020 20:49:33 GMT
EXPOSE 443
# Wed, 11 Nov 2020 20:49:34 GMT
EXPOSE 2019
# Wed, 11 Nov 2020 20:50:16 GMT
RUN caddy version
# Wed, 11 Nov 2020 20:50:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:126d9a92c0cb7b68c56dec2dd5ba118de9dde3ec6368db734c5135fdf1528a33`  
		Last Modified: Wed, 11 Nov 2020 13:34:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8209753221a853170a05478f1dcd98e0e053e700619c6ef12dc177c4e55a57ff`  
		Last Modified: Wed, 11 Nov 2020 21:01:31 GMT  
		Size: 10.1 MB (10089052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6dfd50db08ec5e748cacc844bf84f012344731801c87ab92146b9194059acf`  
		Last Modified: Wed, 11 Nov 2020 21:01:28 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac9ba3c4948efa385a4a66354591ee0f151329021799ccc9e27ddf072a22445`  
		Last Modified: Wed, 11 Nov 2020 21:01:36 GMT  
		Size: 23.1 MB (23065071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df648d1a9f54d00470e5427e4f248c99f895b4149a403ce2cd781a02a2af95e`  
		Last Modified: Wed, 11 Nov 2020 21:01:27 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a0f1dc2f6df109fbeffb6befe78cbfa1789dc66a40f841ad3f52bf99cacdc`  
		Last Modified: Wed, 11 Nov 2020 21:01:27 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87f1d0037fbb238614a6c0fdb80467c72928f95e1fef04508b7ef20fb50f7cc`  
		Last Modified: Wed, 11 Nov 2020 21:01:25 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338c2c27df684d482250c1eb4fcdf8d82e46d70adbd1c9ec145d62ae7de422f9`  
		Last Modified: Wed, 11 Nov 2020 21:01:25 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f589f2f83fd1d8a0ed928b717bf4730b00dae2cf1a930a40fa139e2b2d651f`  
		Last Modified: Wed, 11 Nov 2020 21:01:24 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f29aa9fa439221c221fc981284a1ef76ca26a80e9e32007cd2245b9a1ca8c0`  
		Last Modified: Wed, 11 Nov 2020 21:01:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c98142e163981917efb57c375062ebe8a063c074a5e687fee3f024f33c65133`  
		Last Modified: Wed, 11 Nov 2020 21:01:25 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e33dd735daeae3d313fee34288454b0ff1cd20d5184bc4e37f4065274ab8a53`  
		Last Modified: Wed, 11 Nov 2020 21:01:21 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adcac5351e0ac5818f5fed08a87a3c9b4af5c2f654e3f6cc9ffbbe3124f22730`  
		Last Modified: Wed, 11 Nov 2020 21:01:20 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd52cb52dc571effe896fddd8e45cb3a31b369c12cf66b15dedbc957b780445`  
		Last Modified: Wed, 11 Nov 2020 21:01:20 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6f2ce7819480f8698aa11ed1cc180152b229b83d84055b23302d5333a3a01c`  
		Last Modified: Wed, 11 Nov 2020 21:01:20 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312140622316dd22301893e44b627d8ecf2ecf21886f0679078f40af80c4dad0`  
		Last Modified: Wed, 11 Nov 2020 21:01:19 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae32cf038a6af4af39597ba603771fb0b2688d5115f90e3e0a8f478638496431`  
		Last Modified: Wed, 11 Nov 2020 21:01:16 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544b2275c156b747ed298cc1d4fa2c7ea9963fdcc008cfcc9cabc428c8e62db3`  
		Last Modified: Wed, 11 Nov 2020 21:01:17 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b208564e0dfb1a5f3a2cfb06f0781056ccd741d16aa35a666c9098566f731881`  
		Last Modified: Wed, 11 Nov 2020 21:01:16 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bb9ee1a8500dc7fff16801c4258123a3437964735ba1e97521d0c58cbe9394`  
		Last Modified: Wed, 11 Nov 2020 21:01:17 GMT  
		Size: 250.9 KB (250895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5647190d14b3b4a098f47097beb01bd57348258c58a82b4031d028fc431a5a8`  
		Last Modified: Wed, 11 Nov 2020 21:01:16 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-windowsservercore-1809`

```console
$ docker pull caddy@sha256:b1e4c0b55b3c293d7183cdae642cf4fdd58799d0d87bec7a77e9ee63724aa5af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `caddy:2.1.1-windowsservercore-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull caddy@sha256:e2d41115b10e26568979fd99964d79319400d1008733bd29b0ad270cd446041a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2415318960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca72587c4cf96e2aed3533eac5415b8b05f1282ae904b914b42a5267aa5aac29`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 20:45:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Nov 2020 20:45:21 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 11 Nov 2020 20:45:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Nov 2020 20:45:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Nov 2020 20:45:56 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Nov 2020 20:45:57 GMT
VOLUME [c:/config]
# Wed, 11 Nov 2020 20:45:57 GMT
VOLUME [c:/data]
# Wed, 11 Nov 2020 20:45:58 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 11 Nov 2020 20:45:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Nov 2020 20:46:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Nov 2020 20:46:01 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Nov 2020 20:46:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Nov 2020 20:46:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Nov 2020 20:46:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Nov 2020 20:46:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Nov 2020 20:46:04 GMT
EXPOSE 80
# Wed, 11 Nov 2020 20:46:05 GMT
EXPOSE 443
# Wed, 11 Nov 2020 20:46:05 GMT
EXPOSE 2019
# Wed, 11 Nov 2020 20:46:22 GMT
RUN caddy version
# Wed, 11 Nov 2020 20:46:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9241b8447db6ee01486692864d501d1b85cc8e28b6ba12477da3ccb91ac6fb80`  
		Last Modified: Wed, 11 Nov 2020 21:01:08 GMT  
		Size: 9.2 MB (9248091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140d2864a3ecf900ddcbb7825de568deed4368848546c6f5b33b1031d0d2785c`  
		Last Modified: Wed, 11 Nov 2020 21:01:04 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773bfe60fc2adaea22a607f2ef04801f3a1fe4d1d2742fffd1b3708b9cc2616e`  
		Last Modified: Wed, 11 Nov 2020 21:01:08 GMT  
		Size: 17.7 MB (17722401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6ac34c199b688dcea4ee50fdd427343360897f7b879c92f58e54730a2c7813`  
		Last Modified: Wed, 11 Nov 2020 21:01:03 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37ba66c494cd95e08bddfe1439674935321d50cc6619659859d447d225b9345`  
		Last Modified: Wed, 11 Nov 2020 21:01:03 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa9619dc6858361d1cc3c3459f509b1af176afab3951a8b46ff7cd4065ad56e`  
		Last Modified: Wed, 11 Nov 2020 21:01:00 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d5c4e2731ec2cf1a69fecede53c0cfc076d1c7a3031d9d2f16695b82280856`  
		Last Modified: Wed, 11 Nov 2020 21:01:00 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f78932772adde20a5b82826a3aeca1f6cbea5205a042134ccffb88993a8cbf`  
		Last Modified: Wed, 11 Nov 2020 21:01:00 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6bb7af2868628d7e417e249d60572cb1c53508861a07aa3dcbe601b698fc054`  
		Last Modified: Wed, 11 Nov 2020 21:00:59 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4046f61372cfde3727e85e91767d4eda8547125814b7cc7ace12ea083cf4741b`  
		Last Modified: Wed, 11 Nov 2020 21:00:59 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dfe0ab7ccd8016d0fb2f185efbc294841b8e43d77509a4478fa4cc6edaa4ff`  
		Last Modified: Wed, 11 Nov 2020 21:00:56 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8012fd5e700acdf295c51de57a059928e395cd4654aa5c8fcc6743961b4adf70`  
		Last Modified: Wed, 11 Nov 2020 21:00:56 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298316ad3edcfa6e02b2ed6ad0795b0167fb20254f79c4eb19ad3253c903adb1`  
		Last Modified: Wed, 11 Nov 2020 21:00:57 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451c72395cd914723ccd8dd337a0ca840c0dd00d829d6ce3d9dba4c6462102c9`  
		Last Modified: Wed, 11 Nov 2020 21:00:56 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a43113a9d7534b3a4fbeca6ad58f5ef8e1a6fa5b8d6a488f3d8edda1d7cdd61`  
		Last Modified: Wed, 11 Nov 2020 21:00:56 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369cba41c19fe5008c5dfe0b88cd8f0ef77b138d68c7eca3374c7fbf18d5afcd`  
		Last Modified: Wed, 11 Nov 2020 21:00:53 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0479adc0c263c2e9eab3e3e8fcb7b9d933a95b0f26c04c4c900c5f3804011eb3`  
		Last Modified: Wed, 11 Nov 2020 21:00:53 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea0e70171ceaae4ac02e06588b5aa7f97be0a7e82af15000c7dc8d75dd91c44`  
		Last Modified: Wed, 11 Nov 2020 21:00:53 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b2ec7137cc7d53728109e434d551d89f4694290199f60dfbdfcd4709d8a58f`  
		Last Modified: Wed, 11 Nov 2020 21:00:53 GMT  
		Size: 298.7 KB (298665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e6d60b9c57f55e542ddd3aefdcdbd16da124a2a8142c961c0dab1635429b6c`  
		Last Modified: Wed, 11 Nov 2020 21:00:53 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:e56336e2b1f136a1a3be08f829c7745d1d987af27ab488138a9472e1de0e7c07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64

### `caddy:2.1.1-windowsservercore-ltsc2016` - windows version 10.0.14393.4046; amd64

```console
$ docker pull caddy@sha256:dede9ad27fd496b1102d3530355b3d007bca80608739b3f1beebd3474ce96575
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5803984357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f16f2509b06ce8b2e9d98af30d2ac226c0e89e30a4f81ae6ee79176655906a8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 13:23:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 20:47:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Nov 2020 20:47:53 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 11 Nov 2020 20:49:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Nov 2020 20:49:22 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Nov 2020 20:49:23 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Nov 2020 20:49:24 GMT
VOLUME [c:/config]
# Wed, 11 Nov 2020 20:49:26 GMT
VOLUME [c:/data]
# Wed, 11 Nov 2020 20:49:27 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 11 Nov 2020 20:49:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Nov 2020 20:49:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Nov 2020 20:49:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Nov 2020 20:49:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Nov 2020 20:49:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Nov 2020 20:49:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Nov 2020 20:49:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Nov 2020 20:49:32 GMT
EXPOSE 80
# Wed, 11 Nov 2020 20:49:33 GMT
EXPOSE 443
# Wed, 11 Nov 2020 20:49:34 GMT
EXPOSE 2019
# Wed, 11 Nov 2020 20:50:16 GMT
RUN caddy version
# Wed, 11 Nov 2020 20:50:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:126d9a92c0cb7b68c56dec2dd5ba118de9dde3ec6368db734c5135fdf1528a33`  
		Last Modified: Wed, 11 Nov 2020 13:34:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8209753221a853170a05478f1dcd98e0e053e700619c6ef12dc177c4e55a57ff`  
		Last Modified: Wed, 11 Nov 2020 21:01:31 GMT  
		Size: 10.1 MB (10089052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6dfd50db08ec5e748cacc844bf84f012344731801c87ab92146b9194059acf`  
		Last Modified: Wed, 11 Nov 2020 21:01:28 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac9ba3c4948efa385a4a66354591ee0f151329021799ccc9e27ddf072a22445`  
		Last Modified: Wed, 11 Nov 2020 21:01:36 GMT  
		Size: 23.1 MB (23065071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df648d1a9f54d00470e5427e4f248c99f895b4149a403ce2cd781a02a2af95e`  
		Last Modified: Wed, 11 Nov 2020 21:01:27 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a0f1dc2f6df109fbeffb6befe78cbfa1789dc66a40f841ad3f52bf99cacdc`  
		Last Modified: Wed, 11 Nov 2020 21:01:27 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87f1d0037fbb238614a6c0fdb80467c72928f95e1fef04508b7ef20fb50f7cc`  
		Last Modified: Wed, 11 Nov 2020 21:01:25 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338c2c27df684d482250c1eb4fcdf8d82e46d70adbd1c9ec145d62ae7de422f9`  
		Last Modified: Wed, 11 Nov 2020 21:01:25 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f589f2f83fd1d8a0ed928b717bf4730b00dae2cf1a930a40fa139e2b2d651f`  
		Last Modified: Wed, 11 Nov 2020 21:01:24 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f29aa9fa439221c221fc981284a1ef76ca26a80e9e32007cd2245b9a1ca8c0`  
		Last Modified: Wed, 11 Nov 2020 21:01:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c98142e163981917efb57c375062ebe8a063c074a5e687fee3f024f33c65133`  
		Last Modified: Wed, 11 Nov 2020 21:01:25 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e33dd735daeae3d313fee34288454b0ff1cd20d5184bc4e37f4065274ab8a53`  
		Last Modified: Wed, 11 Nov 2020 21:01:21 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adcac5351e0ac5818f5fed08a87a3c9b4af5c2f654e3f6cc9ffbbe3124f22730`  
		Last Modified: Wed, 11 Nov 2020 21:01:20 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd52cb52dc571effe896fddd8e45cb3a31b369c12cf66b15dedbc957b780445`  
		Last Modified: Wed, 11 Nov 2020 21:01:20 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6f2ce7819480f8698aa11ed1cc180152b229b83d84055b23302d5333a3a01c`  
		Last Modified: Wed, 11 Nov 2020 21:01:20 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312140622316dd22301893e44b627d8ecf2ecf21886f0679078f40af80c4dad0`  
		Last Modified: Wed, 11 Nov 2020 21:01:19 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae32cf038a6af4af39597ba603771fb0b2688d5115f90e3e0a8f478638496431`  
		Last Modified: Wed, 11 Nov 2020 21:01:16 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544b2275c156b747ed298cc1d4fa2c7ea9963fdcc008cfcc9cabc428c8e62db3`  
		Last Modified: Wed, 11 Nov 2020 21:01:17 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b208564e0dfb1a5f3a2cfb06f0781056ccd741d16aa35a666c9098566f731881`  
		Last Modified: Wed, 11 Nov 2020 21:01:16 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bb9ee1a8500dc7fff16801c4258123a3437964735ba1e97521d0c58cbe9394`  
		Last Modified: Wed, 11 Nov 2020 21:01:17 GMT  
		Size: 250.9 KB (250895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5647190d14b3b4a098f47097beb01bd57348258c58a82b4031d028fc431a5a8`  
		Last Modified: Wed, 11 Nov 2020 21:01:16 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1`

```console
$ docker pull caddy@sha256:e46050590a9ac1a411b5da0349f735b5977e9dcbe6ab91e9a95c9a731533aba8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1577; amd64
	-	windows version 10.0.14393.4046; amd64

### `caddy:2.2.1` - linux; amd64

```console
$ docker pull caddy@sha256:4ebad49f78a3f98164d89431978046ee6e94f1e8a70454abc7f49ce1a5ee7826
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14635232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bb0137bab0e21a92b0bc9ec1cc22c259b097d5bf239b161ae1eac0de1833e67`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:33:22 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 04:33:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 04:33:55 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 04:33:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 04:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 04:34:01 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 04:34:01 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 04:34:01 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 04:34:02 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 04:34:02 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 04:34:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 04:34:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 04:34:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 04:34:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 04:34:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 04:34:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 04:34:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 04:34:05 GMT
EXPOSE 80
# Thu, 22 Oct 2020 04:34:05 GMT
EXPOSE 443
# Thu, 22 Oct 2020 04:34:06 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 04:34:06 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 04:34:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2e2d825895b6421ca5dbd63db0d99f790ef84a84c7bcaff51e60b654397858`  
		Last Modified: Thu, 22 Oct 2020 04:34:47 GMT  
		Size: 300.0 KB (299956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaf2e3dee2e74b401fce928bf9502e48df68da4e8c1933bfd6b00b1137529fc`  
		Last Modified: Thu, 22 Oct 2020 04:35:02 GMT  
		Size: 5.8 KB (5754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2215cf93250599c5db984cee0fddd5d0cd59ef035ab5a317387b67211bde86d`  
		Last Modified: Thu, 22 Oct 2020 04:35:06 GMT  
		Size: 11.5 MB (11532508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060365e49ba5ee96a2859e269b366f5a5c9f386e5bdbf07d2ef31b1fc6934baa`  
		Last Modified: Thu, 22 Oct 2020 04:35:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1` - linux; arm variant v6

```console
$ docker pull caddy@sha256:abba73dc860b2f35703cb7d27f08baf5bfc084e18e627b94661d01a8e2befdaf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13784259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f0aad5a281913821dd39ffed5e144daae22ac81ac4314731395ab65eedde72a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:58:10 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 02:58:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 02:58:46 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 02:58:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 02:58:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:59:00 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 02:59:01 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 02:59:01 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 02:59:03 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 02:59:08 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 02:59:09 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 02:59:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 02:59:11 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 02:59:11 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 02:59:12 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 02:59:13 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 02:59:14 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 02:59:15 GMT
EXPOSE 80
# Thu, 22 Oct 2020 02:59:19 GMT
EXPOSE 443
# Thu, 22 Oct 2020 02:59:20 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 02:59:21 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 02:59:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7369c3ac4b39c55c74e96dd3eb61ac2fa65e5671b1c2acca9697a7c9d20c3cf`  
		Last Modified: Thu, 22 Oct 2020 02:59:49 GMT  
		Size: 300.1 KB (300086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8f4045920069dff3382a5993783c5d846d9e28d0f5a63c475ed298fce0abb7`  
		Last Modified: Thu, 22 Oct 2020 03:00:03 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db6bde4735da15e5db23ad62f3d64d78aed8713a40d12547f5538c15c90f9da`  
		Last Modified: Thu, 22 Oct 2020 03:00:06 GMT  
		Size: 10.9 MB (10876280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a95efd7a14ed98a53a238da45faa7e3b0fdd2a93529b83bfe9d0823dafac67c`  
		Last Modified: Thu, 22 Oct 2020 03:00:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1` - linux; arm variant v7

```console
$ docker pull caddy@sha256:8cf66cbe3c03273ca54bdab908092a6a9b9f02d39595ed15b1111f1465430426
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13565251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b20723dea614fc40d9f3cb59eddd33bf0e89dfda3f8ed4a7b404ef334632a4b9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:04:57 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 03:05:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 03:05:45 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 03:05:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 03:05:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:05:53 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 03:05:53 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 03:05:54 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 03:05:55 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 03:05:56 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 03:05:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 03:05:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 03:05:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 03:05:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 03:05:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 03:06:00 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 03:06:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 03:06:01 GMT
EXPOSE 80
# Thu, 22 Oct 2020 03:06:02 GMT
EXPOSE 443
# Thu, 22 Oct 2020 03:06:02 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 03:06:03 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 03:06:04 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a8e7fe5034ac502626b0a921d79be80c092890176e33b236c489d6f00710a2`  
		Last Modified: Thu, 22 Oct 2020 03:06:32 GMT  
		Size: 299.2 KB (299211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14db75acdaca15b1e81890f29b3b757fcc73e7a69a55f5ed659bf800f6340108`  
		Last Modified: Thu, 22 Oct 2020 03:06:43 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2197c38adf245bca8f229a4cd718c4d0f619a87bae5786572ccdac1a286882c`  
		Last Modified: Thu, 22 Oct 2020 03:06:46 GMT  
		Size: 10.9 MB (10854384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0104bc6a595940856019d00d9ff8e04365338a7964d948b64cc44bf73cc59e`  
		Last Modified: Thu, 22 Oct 2020 03:06:42 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:da121cf42d1759ed03af3130533d365c365af1d738d550744ad863e05e64cf46
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13540356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89b4aa38988ab2442575062d99c3cb44976de6c227256c118f35340e7c21c303`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:40:04 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 02:40:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 02:40:57 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 02:41:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 02:41:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:41:07 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 02:41:08 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 02:41:09 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 02:41:10 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 02:41:10 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 02:41:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 02:41:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 02:41:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 02:41:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 02:41:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 02:41:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 02:41:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 02:41:19 GMT
EXPOSE 80
# Thu, 22 Oct 2020 02:41:20 GMT
EXPOSE 443
# Thu, 22 Oct 2020 02:41:20 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 02:41:21 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 02:41:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dbde357077a97c0f831033bf03c9828203cb7e3e6cb33217ce4d7cfd71c931`  
		Last Modified: Thu, 22 Oct 2020 02:41:47 GMT  
		Size: 300.3 KB (300348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a5ab0aa923ce1fe233b904008bbf932c4787f48bcd59f07a85616147b7cbc3`  
		Last Modified: Thu, 22 Oct 2020 02:41:56 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc398339860cf826624c9c22b5de9b45a193260e2ff24826d210b493483398f`  
		Last Modified: Thu, 22 Oct 2020 02:41:59 GMT  
		Size: 10.5 MB (10527465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6e7d61d1d4a00550447ea1f67edc0463cc527e49356e98959edfafba0df879`  
		Last Modified: Thu, 22 Oct 2020 02:41:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1` - linux; ppc64le

```console
$ docker pull caddy@sha256:09208042b4d19d7ed87b51b99dc20b390dab20d9ae7e235a62a3af3aaf472bd5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13291756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe5c77284adc35481d13003d31a866f637b6eaf9f5764f667e536db79ce23129`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 13:39:52 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 13:44:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 13:44:04 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 13:44:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 13:44:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 13:44:33 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 13:44:37 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 13:44:40 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 13:44:44 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 13:44:48 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 13:44:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 13:44:56 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 13:45:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 13:45:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 13:45:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 13:45:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 13:45:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 13:45:23 GMT
EXPOSE 80
# Thu, 22 Oct 2020 13:45:26 GMT
EXPOSE 443
# Thu, 22 Oct 2020 13:45:30 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 13:45:35 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 13:45:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649a4964211b7ce86541a0c1dad8ef3800ec38a3ca90aff94b76759b4cb8e279`  
		Last Modified: Thu, 22 Oct 2020 13:47:22 GMT  
		Size: 302.3 KB (302327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58dd938ef3e3eae8509deda8fab9ab5f9344169d912e35a802633e799feed1bb`  
		Last Modified: Thu, 22 Oct 2020 13:47:52 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe23c296ee12ee12ef84dbabbb4f7bf0362a9a12b684782ebd3f44a97c8fcf8e`  
		Last Modified: Thu, 22 Oct 2020 13:47:55 GMT  
		Size: 10.2 MB (10180223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d2f3c084745fecafaa9ff33626a81124f2d70267ceee705da555714238bfa1`  
		Last Modified: Thu, 22 Oct 2020 13:47:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1` - linux; s390x

```console
$ docker pull caddy@sha256:3e18b421d651721239cb3422bc890d1211535681219b7696816f487b4cebc4ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14074857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4d5562f1d148d3d67ff7f5995be8f860553ad0f3d07091335643306b83385e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:41:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 02:41:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 02:41:31 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 02:41:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 02:41:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:41:36 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 02:41:36 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 02:41:37 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 02:41:37 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 02:41:37 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 02:41:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 02:41:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 02:41:38 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 02:41:38 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 02:41:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 02:41:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 02:41:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 02:41:40 GMT
EXPOSE 80
# Thu, 22 Oct 2020 02:41:40 GMT
EXPOSE 443
# Thu, 22 Oct 2020 02:41:40 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 02:41:41 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 02:41:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f988ff23f3cbb35bfed69e33f3b7ee69403bfae4f46363a08eea4830053e9c`  
		Last Modified: Thu, 22 Oct 2020 02:42:01 GMT  
		Size: 300.5 KB (300481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd6a4e0db99510879c5dfceabd1e629a0692c4544bb0da34971f8722b881e92`  
		Last Modified: Thu, 22 Oct 2020 02:42:09 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e13b938aa802e74610585cabba77d625db4baf219f577a81195c272408c7d3`  
		Last Modified: Thu, 22 Oct 2020 02:42:16 GMT  
		Size: 11.2 MB (11202559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a221fff082950a8a98db12eb99f532a39008f0d6e21684bc1aed06fa1ed2a764`  
		Last Modified: Thu, 22 Oct 2020 02:42:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1` - windows version 10.0.17763.1577; amd64

```console
$ docker pull caddy@sha256:dad45b6df45cf6f4c45f010c391544a830a6372847bb2504a23a870eb9e96638
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2413941176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61f3df5163746a4530d03a8bc80f3b1318d935f9f1b3e26f00a31af891a9ba86`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 20:53:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Nov 2020 20:53:31 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 11 Nov 2020 20:54:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Nov 2020 20:54:04 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Nov 2020 20:54:04 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Nov 2020 20:54:05 GMT
VOLUME [c:/config]
# Wed, 11 Nov 2020 20:54:06 GMT
VOLUME [c:/data]
# Wed, 11 Nov 2020 20:54:07 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 11 Nov 2020 20:54:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Nov 2020 20:54:09 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Nov 2020 20:54:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Nov 2020 20:54:11 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Nov 2020 20:54:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Nov 2020 20:54:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Nov 2020 20:54:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Nov 2020 20:54:13 GMT
EXPOSE 80
# Wed, 11 Nov 2020 20:54:14 GMT
EXPOSE 443
# Wed, 11 Nov 2020 20:54:14 GMT
EXPOSE 2019
# Wed, 11 Nov 2020 20:54:30 GMT
RUN caddy version
# Wed, 11 Nov 2020 20:54:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01dcdd0030882c54a82d0a279a4099081c604810ccccb17d3d7c04a2057bf657`  
		Last Modified: Wed, 11 Nov 2020 21:02:39 GMT  
		Size: 9.2 MB (9248045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3be730f5a5cc9d1dd7080908242b9ed33ba6541e7120addf14e416b944b577`  
		Last Modified: Wed, 11 Nov 2020 21:02:36 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d70ac9fb0285fe6670a558e9c1da67b5594dd483872376ac91425a3058f95b9`  
		Last Modified: Wed, 11 Nov 2020 21:02:54 GMT  
		Size: 16.3 MB (16343997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72340d1f03d76debdf2a014ab06bbd3bc5cb1e8358520912f0c9f71f2b4a6ea`  
		Last Modified: Wed, 11 Nov 2020 21:02:34 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ae7bc4f9eb3af2fa576dd096f9992ad2cfc8a2e9aad0af79e1ebf11c95065d`  
		Last Modified: Wed, 11 Nov 2020 21:02:33 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46832c7bcb0b053968836644798024f37cfede18aaac00abed0c1571fbeeca4c`  
		Last Modified: Wed, 11 Nov 2020 21:02:33 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdafb0d35a00870fdb93efde60b2d5c002b5ec117bb07526ec1d744787529f58`  
		Last Modified: Wed, 11 Nov 2020 21:02:31 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af235cb3a2a159b44c6b773e30cbd6f7931055fb7cfed2aee403c9197e0defc`  
		Last Modified: Wed, 11 Nov 2020 21:02:32 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493ee2907458eb7d47b217b59e2f23b4dd4a6974a36a70462fa54e5b9201f26b`  
		Last Modified: Wed, 11 Nov 2020 21:02:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2f8b9a7de64bd747e2afbc20e6ca964b00d3b48ccdb9245e162300a5ef9b44`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc59b5cb8ee3554d8e4971222e0208e7b6dd831b33894abeba76400bbcb7d56`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c88104f4e1fc6125880b248f3e1edcc5cbf3daf73aaf26bf3782972f11203c3`  
		Last Modified: Wed, 11 Nov 2020 21:02:30 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7cb21eb1cd8ca039940f462fdfe3348c877262adbbc5891cdbc3601ffa2649`  
		Last Modified: Wed, 11 Nov 2020 21:02:27 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef21802812d7f9ad5dcebb2efbf8d4831fcdf5b024bac00c22d04e7406a420b`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed806482965bf605e395b83f00ba44639cc1c88b1b8ec7c75bb708d9c031610`  
		Last Modified: Wed, 11 Nov 2020 21:02:24 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee097b51db8b06f6e93d48da3e914d6a598b32681fdf27785279f3f5dbb5796`  
		Last Modified: Wed, 11 Nov 2020 21:02:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf5349d69a690d25aa14a10fab1fc6e7a82ec345bae9e1a01a4dfd95f09cd1b`  
		Last Modified: Wed, 11 Nov 2020 21:02:22 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0b5aa8db0e75c1ef349905a29ef299882814b7937d14753d2e6a972f7b13b1`  
		Last Modified: Wed, 11 Nov 2020 21:02:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cac55d84f022bb91b78bfb339492198e3fa96a7d1e25c1f8e09ad648376d45d`  
		Last Modified: Wed, 11 Nov 2020 21:02:21 GMT  
		Size: 299.3 KB (299301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7476d855c257a4a27ce525860567dd9bd67e74abb01c0fd1b334444ffaa8504c`  
		Last Modified: Wed, 11 Nov 2020 21:02:24 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1` - windows version 10.0.14393.4046; amd64

```console
$ docker pull caddy@sha256:405a17b713c3f1517124a2506ac9b4ed33285819013417e6b90fb2aa07cb0bd6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5802615067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:371225d0afbf64a113a3745e99535e2e17239829f4e36d99aa36e7aee3be9efc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 13:23:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 20:56:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Nov 2020 20:56:05 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 11 Nov 2020 20:57:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Nov 2020 20:57:25 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Nov 2020 20:57:26 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Nov 2020 20:57:28 GMT
VOLUME [c:/config]
# Wed, 11 Nov 2020 20:57:29 GMT
VOLUME [c:/data]
# Wed, 11 Nov 2020 20:57:30 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 11 Nov 2020 20:57:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Nov 2020 20:57:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Nov 2020 20:57:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Nov 2020 20:57:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Nov 2020 20:57:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Nov 2020 20:57:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Nov 2020 20:57:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Nov 2020 20:57:35 GMT
EXPOSE 80
# Wed, 11 Nov 2020 20:57:36 GMT
EXPOSE 443
# Wed, 11 Nov 2020 20:57:37 GMT
EXPOSE 2019
# Wed, 11 Nov 2020 20:58:18 GMT
RUN caddy version
# Wed, 11 Nov 2020 20:58:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:126d9a92c0cb7b68c56dec2dd5ba118de9dde3ec6368db734c5135fdf1528a33`  
		Last Modified: Wed, 11 Nov 2020 13:34:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5595cf12db880fdffb7bc7e0ceef81a68e0766ff34fdc357635566a05b60085`  
		Last Modified: Wed, 11 Nov 2020 21:03:35 GMT  
		Size: 10.1 MB (10089893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47fc9d917c611e97ffa642af414764e4712d012a3b2c10700a357a771d58bf3`  
		Last Modified: Wed, 11 Nov 2020 21:03:24 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2b332d20177fb217e2744454885bba6eb94e9c7512c35bef53cf1222f10b3a`  
		Last Modified: Wed, 11 Nov 2020 21:03:50 GMT  
		Size: 21.7 MB (21694741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061740784584c807be44f52e632b6fcafa7893cab07ca93723103ca41e759cd2`  
		Last Modified: Wed, 11 Nov 2020 21:03:23 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a051df7f978fd750beb5e55b7a7da2d50550a52c97baf897cd3452347196147`  
		Last Modified: Wed, 11 Nov 2020 21:03:23 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94db8d6fb716d4c43b34e09a05176f94701accb480ce613c231d70ef23c649b`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eeb5cfdcdca36082954b3510135aea31966da19679b9cc7d8d4e43a3892f2f5`  
		Last Modified: Wed, 11 Nov 2020 21:03:19 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50cc11877f41dad7cb21c9e61379268e564a03b044ec4cfb124cccd267ef551c`  
		Last Modified: Wed, 11 Nov 2020 21:03:21 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9914893b848ce6d71a6f99575e794219e1603afe1dcee2bcbf69f3a41451ab05`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab52b473d299810d7e49b3d9d98db42e6aa57e5426b79f4cd7f68fd766a8a9b`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3333f590132f229c9979af102fd15c4a5958d9e3d94d50632eeb045c14028ac1`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12c4e6df6d5faa8f29b56e44eb52dc65c9d6795322a0e6d743a9d373f97adf9`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a015ed900b4c4b4d23631449b68473b1e31eda520fa22c7c19a845ac6f133f31`  
		Last Modified: Wed, 11 Nov 2020 21:03:16 GMT  
		Size: 1.1 KB (1069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f354d2a4fb61ae55364b2ae298552e22165583c076c39e05707e906633b8a2`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc11e1af39f958f492359f3242aa5205230791b166e14ab2f94067e9999464e`  
		Last Modified: Wed, 11 Nov 2020 21:03:16 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a4e622ed285e795cc2fd731f38022c2e6ca478f2223fb9fcafe0a61b5e969`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f936683e767d2733a4a898519ce7c8bc6a608fede4e7cc04c41b5fed180287`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b4fbe6665c83c229d90ec42acce959b356dbf1a97ca281604625a29d8437133`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6966c1a2733b248361e0fbafefb3b58805b223ef954ced160cb1ca7f239c25`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 251.9 KB (251913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3d08972458dc80b8c379340207e2cfeee9ea33d9e9e405ebbf52421ef16dd5`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-alpine`

```console
$ docker pull caddy@sha256:ea06de9c9cb10eacb9f77e50817d2ad8dd63c977549f26c19d57df1a194fefdc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.2.1-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:4ebad49f78a3f98164d89431978046ee6e94f1e8a70454abc7f49ce1a5ee7826
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14635232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bb0137bab0e21a92b0bc9ec1cc22c259b097d5bf239b161ae1eac0de1833e67`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:33:22 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 04:33:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 04:33:55 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 04:33:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 04:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 04:34:01 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 04:34:01 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 04:34:01 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 04:34:02 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 04:34:02 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 04:34:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 04:34:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 04:34:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 04:34:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 04:34:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 04:34:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 04:34:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 04:34:05 GMT
EXPOSE 80
# Thu, 22 Oct 2020 04:34:05 GMT
EXPOSE 443
# Thu, 22 Oct 2020 04:34:06 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 04:34:06 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 04:34:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2e2d825895b6421ca5dbd63db0d99f790ef84a84c7bcaff51e60b654397858`  
		Last Modified: Thu, 22 Oct 2020 04:34:47 GMT  
		Size: 300.0 KB (299956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaf2e3dee2e74b401fce928bf9502e48df68da4e8c1933bfd6b00b1137529fc`  
		Last Modified: Thu, 22 Oct 2020 04:35:02 GMT  
		Size: 5.8 KB (5754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2215cf93250599c5db984cee0fddd5d0cd59ef035ab5a317387b67211bde86d`  
		Last Modified: Thu, 22 Oct 2020 04:35:06 GMT  
		Size: 11.5 MB (11532508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060365e49ba5ee96a2859e269b366f5a5c9f386e5bdbf07d2ef31b1fc6934baa`  
		Last Modified: Thu, 22 Oct 2020 04:35:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:abba73dc860b2f35703cb7d27f08baf5bfc084e18e627b94661d01a8e2befdaf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13784259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f0aad5a281913821dd39ffed5e144daae22ac81ac4314731395ab65eedde72a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:58:10 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 02:58:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 02:58:46 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 02:58:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 02:58:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:59:00 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 02:59:01 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 02:59:01 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 02:59:03 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 02:59:08 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 02:59:09 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 02:59:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 02:59:11 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 02:59:11 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 02:59:12 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 02:59:13 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 02:59:14 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 02:59:15 GMT
EXPOSE 80
# Thu, 22 Oct 2020 02:59:19 GMT
EXPOSE 443
# Thu, 22 Oct 2020 02:59:20 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 02:59:21 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 02:59:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7369c3ac4b39c55c74e96dd3eb61ac2fa65e5671b1c2acca9697a7c9d20c3cf`  
		Last Modified: Thu, 22 Oct 2020 02:59:49 GMT  
		Size: 300.1 KB (300086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8f4045920069dff3382a5993783c5d846d9e28d0f5a63c475ed298fce0abb7`  
		Last Modified: Thu, 22 Oct 2020 03:00:03 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db6bde4735da15e5db23ad62f3d64d78aed8713a40d12547f5538c15c90f9da`  
		Last Modified: Thu, 22 Oct 2020 03:00:06 GMT  
		Size: 10.9 MB (10876280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a95efd7a14ed98a53a238da45faa7e3b0fdd2a93529b83bfe9d0823dafac67c`  
		Last Modified: Thu, 22 Oct 2020 03:00:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:8cf66cbe3c03273ca54bdab908092a6a9b9f02d39595ed15b1111f1465430426
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13565251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b20723dea614fc40d9f3cb59eddd33bf0e89dfda3f8ed4a7b404ef334632a4b9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:04:57 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 03:05:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 03:05:45 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 03:05:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 03:05:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:05:53 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 03:05:53 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 03:05:54 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 03:05:55 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 03:05:56 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 03:05:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 03:05:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 03:05:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 03:05:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 03:05:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 03:06:00 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 03:06:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 03:06:01 GMT
EXPOSE 80
# Thu, 22 Oct 2020 03:06:02 GMT
EXPOSE 443
# Thu, 22 Oct 2020 03:06:02 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 03:06:03 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 03:06:04 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a8e7fe5034ac502626b0a921d79be80c092890176e33b236c489d6f00710a2`  
		Last Modified: Thu, 22 Oct 2020 03:06:32 GMT  
		Size: 299.2 KB (299211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14db75acdaca15b1e81890f29b3b757fcc73e7a69a55f5ed659bf800f6340108`  
		Last Modified: Thu, 22 Oct 2020 03:06:43 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2197c38adf245bca8f229a4cd718c4d0f619a87bae5786572ccdac1a286882c`  
		Last Modified: Thu, 22 Oct 2020 03:06:46 GMT  
		Size: 10.9 MB (10854384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0104bc6a595940856019d00d9ff8e04365338a7964d948b64cc44bf73cc59e`  
		Last Modified: Thu, 22 Oct 2020 03:06:42 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:da121cf42d1759ed03af3130533d365c365af1d738d550744ad863e05e64cf46
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13540356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89b4aa38988ab2442575062d99c3cb44976de6c227256c118f35340e7c21c303`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:40:04 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 02:40:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 02:40:57 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 02:41:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 02:41:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:41:07 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 02:41:08 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 02:41:09 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 02:41:10 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 02:41:10 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 02:41:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 02:41:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 02:41:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 02:41:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 02:41:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 02:41:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 02:41:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 02:41:19 GMT
EXPOSE 80
# Thu, 22 Oct 2020 02:41:20 GMT
EXPOSE 443
# Thu, 22 Oct 2020 02:41:20 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 02:41:21 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 02:41:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dbde357077a97c0f831033bf03c9828203cb7e3e6cb33217ce4d7cfd71c931`  
		Last Modified: Thu, 22 Oct 2020 02:41:47 GMT  
		Size: 300.3 KB (300348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a5ab0aa923ce1fe233b904008bbf932c4787f48bcd59f07a85616147b7cbc3`  
		Last Modified: Thu, 22 Oct 2020 02:41:56 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc398339860cf826624c9c22b5de9b45a193260e2ff24826d210b493483398f`  
		Last Modified: Thu, 22 Oct 2020 02:41:59 GMT  
		Size: 10.5 MB (10527465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6e7d61d1d4a00550447ea1f67edc0463cc527e49356e98959edfafba0df879`  
		Last Modified: Thu, 22 Oct 2020 02:41:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:09208042b4d19d7ed87b51b99dc20b390dab20d9ae7e235a62a3af3aaf472bd5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13291756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe5c77284adc35481d13003d31a866f637b6eaf9f5764f667e536db79ce23129`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 13:39:52 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 13:44:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 13:44:04 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 13:44:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 13:44:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 13:44:33 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 13:44:37 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 13:44:40 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 13:44:44 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 13:44:48 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 13:44:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 13:44:56 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 13:45:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 13:45:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 13:45:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 13:45:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 13:45:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 13:45:23 GMT
EXPOSE 80
# Thu, 22 Oct 2020 13:45:26 GMT
EXPOSE 443
# Thu, 22 Oct 2020 13:45:30 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 13:45:35 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 13:45:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649a4964211b7ce86541a0c1dad8ef3800ec38a3ca90aff94b76759b4cb8e279`  
		Last Modified: Thu, 22 Oct 2020 13:47:22 GMT  
		Size: 302.3 KB (302327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58dd938ef3e3eae8509deda8fab9ab5f9344169d912e35a802633e799feed1bb`  
		Last Modified: Thu, 22 Oct 2020 13:47:52 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe23c296ee12ee12ef84dbabbb4f7bf0362a9a12b684782ebd3f44a97c8fcf8e`  
		Last Modified: Thu, 22 Oct 2020 13:47:55 GMT  
		Size: 10.2 MB (10180223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d2f3c084745fecafaa9ff33626a81124f2d70267ceee705da555714238bfa1`  
		Last Modified: Thu, 22 Oct 2020 13:47:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:3e18b421d651721239cb3422bc890d1211535681219b7696816f487b4cebc4ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14074857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4d5562f1d148d3d67ff7f5995be8f860553ad0f3d07091335643306b83385e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:41:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 02:41:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 02:41:31 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 02:41:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 02:41:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:41:36 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 02:41:36 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 02:41:37 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 02:41:37 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 02:41:37 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 02:41:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 02:41:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 02:41:38 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 02:41:38 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 02:41:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 02:41:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 02:41:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 02:41:40 GMT
EXPOSE 80
# Thu, 22 Oct 2020 02:41:40 GMT
EXPOSE 443
# Thu, 22 Oct 2020 02:41:40 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 02:41:41 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 02:41:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f988ff23f3cbb35bfed69e33f3b7ee69403bfae4f46363a08eea4830053e9c`  
		Last Modified: Thu, 22 Oct 2020 02:42:01 GMT  
		Size: 300.5 KB (300481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd6a4e0db99510879c5dfceabd1e629a0692c4544bb0da34971f8722b881e92`  
		Last Modified: Thu, 22 Oct 2020 02:42:09 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e13b938aa802e74610585cabba77d625db4baf219f577a81195c272408c7d3`  
		Last Modified: Thu, 22 Oct 2020 02:42:16 GMT  
		Size: 11.2 MB (11202559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a221fff082950a8a98db12eb99f532a39008f0d6e21684bc1aed06fa1ed2a764`  
		Last Modified: Thu, 22 Oct 2020 02:42:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-builder`

```console
$ docker pull caddy@sha256:11b6dc688f10fd45996d660117a4567192599b9dc33e0ed69376f3e771473085
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1577; amd64
	-	windows version 10.0.14393.4046; amd64

### `caddy:2.2.1-builder` - linux; amd64

```console
$ docker pull caddy@sha256:d7b066e0ae6a58162afa38de124bde6cafbcf0a7f4d056489ce88cc394471bed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119881414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d52e2ef96ee9bf6c12304aac59194314ca7a1e076d5904b34eac04d61337d964`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:34:56 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:34:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:34:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:21:55 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:24:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:24:09 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:24:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:24:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:24:10 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:49:11 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:49:12 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:49:12 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:49:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:49:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:49:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:49:15 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef7d3d256c8367c41c431143c63d083a25dd62ec9ee9d9773dd9e6c7b70ec9e`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 280.8 KB (280812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9db76c5a1d06710ed4f3073476b2d883ff8e911f8e47c558bc4a8d1d8663fa`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b5e3429cf30be490cdf3c5018e8693e0e1d319ea295c9b0c37dedaa7a1cafb`  
		Last Modified: Fri, 04 Dec 2020 00:31:08 GMT  
		Size: 107.1 MB (107085919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07aa6a0961518234df34a1cf391ec7269a68b99fc112f60e8a7270db07eb3974`  
		Last Modified: Fri, 04 Dec 2020 00:30:49 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fe1a6296183cbfcabe79353a47f9336d847b7ea66b4fb61ae86fc689de5d77`  
		Last Modified: Fri, 04 Dec 2020 00:49:47 GMT  
		Size: 8.3 MB (8309940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1da5ba704ae92109544c4683fde8e8be5eea27b6110540c808341c3b43145c6`  
		Last Modified: Fri, 04 Dec 2020 00:49:45 GMT  
		Size: 1.4 MB (1407200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572698d0ecf1dba5c0b8c6a996637e0de1f7e30e2901dae6927647fc8e0d63e7`  
		Last Modified: Fri, 04 Dec 2020 00:49:44 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:d6805920da89344546ce60bd4b91be62fa46da72cef37f871a07d829a0e6b39d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.1 MB (115088466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ad4d3264c7202d2a8117e3dd2a7c46d4164b1e58f8da8ab94016ec14fc9737b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:07:24 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:07:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:07:27 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:54:37 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:57:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:57:18 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:57:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:57:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:57:23 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:23:51 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:23:52 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:23:52 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 01:23:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:23:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:23:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:23:56 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20cc27a60e8ac1bf56dec787d3d52ba856e657179cfd56050036db79abb4267`  
		Last Modified: Thu, 22 Oct 2020 05:34:55 GMT  
		Size: 281.0 KB (280971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ecce92c3d2de40638d73e682dec26c2b79a055e85c8d70b88f4ccb9485bb9c9`  
		Last Modified: Thu, 22 Oct 2020 05:34:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcce644b45ccf744ed14c7b9273179dc1ad732ffa1bd944e61407793f983b983`  
		Last Modified: Fri, 04 Dec 2020 01:05:18 GMT  
		Size: 102.9 MB (102948648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909e21afe9abe4c8685162bb1ca820c4c1d140304436933b524bf4b048cdbc25`  
		Last Modified: Fri, 04 Dec 2020 01:04:48 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba23987bf60560a98e2e39c226cdf37070ca4f72a514be647528077fe286b3e`  
		Last Modified: Fri, 04 Dec 2020 01:24:26 GMT  
		Size: 7.9 MB (7928869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebe92d17d7243c87fc37008c3e65cbbe4b1b675ccaca7fd4760bc44d7bd7ea3`  
		Last Modified: Fri, 04 Dec 2020 01:24:23 GMT  
		Size: 1.3 MB (1327351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41a9e416157b507873d5b48a6159cf7d013314b857201f0d66921bab89875a1`  
		Last Modified: Fri, 04 Dec 2020 01:24:23 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:bd9531e4414b412e4a1bdb2fbe16e0c83e38c8d058aaa93a6a40245cfd5c8f05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.9 MB (113880893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3158c399bfa2628c5054f9d4e14c2dd225c2b4a45b8130026e462667ba683ce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:21:35 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:23:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:23:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:03:17 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:05:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:05:41 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:05:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:05:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:05:44 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:33:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:33:33 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:33:34 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:33:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:33:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:33:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:33:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b753cfc04fdce9640aac1e7a4b3e7ce15fa60b8e357376e42f294f463a6e890`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 280.1 KB (280084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e90c422e5e4668cb4140aadb622d734faa93c81cc1e283da9b08bbbc65c45c5`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c37b023a65a717d26fdb8c72bba66adc8625ca96fab4d08e70954da6b10139`  
		Last Modified: Fri, 04 Dec 2020 00:14:22 GMT  
		Size: 102.7 MB (102723691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f091034d1629ecd6c35f9bbcb2754721bbfa4e5183794ff2b6ecc75b7b2e0e`  
		Last Modified: Fri, 04 Dec 2020 00:13:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6809b32049841fc890dd29c935db10e86e95c4005906b5eddc3fa42f131cdb5`  
		Last Modified: Fri, 04 Dec 2020 00:34:08 GMT  
		Size: 7.1 MB (7144891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818ba8d461e1618211000580b6f229d2fd9775115c3c4049fb7be235094e0625`  
		Last Modified: Fri, 04 Dec 2020 00:34:07 GMT  
		Size: 1.3 MB (1325838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af262af67e01cb4ef945fd8c992860308e9509dc4810d2cab9ed6955b52a700`  
		Last Modified: Fri, 04 Dec 2020 00:34:07 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:3bd8e226aa9f4fef563f2a76b0c165434ab3145a2b629512dcab6495c677202c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115210346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d5e537fc1b6fe653ff07e33f1a30ba036846e07eb585a5a75815eeabb89e21f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:08:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 04:09:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 04:09:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:59:20 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 01:01:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:01:23 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:01:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:01:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:01:29 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:28:26 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:28:27 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:28:28 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 01:28:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:28:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:28:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:28:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4357932f1b6fb010e1461cc5c673712fb832ac44ee627c691db0b64adf95d13`  
		Last Modified: Thu, 22 Oct 2020 04:28:32 GMT  
		Size: 281.2 KB (281230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c013af1878066e59b688e31fd962e7267430963de27c5257241e3c223aa1d6`  
		Last Modified: Thu, 22 Oct 2020 04:28:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37128a32d7b17416d88331ec94958c63f643120f6e40870110ef00f387be80e5`  
		Last Modified: Fri, 04 Dec 2020 01:09:15 GMT  
		Size: 102.4 MB (102411796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0279cf9b51b6c7d1d4937560cb5536f262e9f4e9c5a1685489387c9753062e04`  
		Last Modified: Fri, 04 Dec 2020 01:08:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed38fb55682cdaae259822fc0a1e349a7992f9f99404e4bdc58b4bee6e75d059`  
		Last Modified: Fri, 04 Dec 2020 01:29:03 GMT  
		Size: 8.5 MB (8499869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9fdec9db4728520c427e5ae86d67521591251e09a667e19f8e6d0419c50d24`  
		Last Modified: Fri, 04 Dec 2020 01:29:01 GMT  
		Size: 1.3 MB (1310181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96eec8ba730f3d05a0aac92b2d5d603ab21395ee6bd7cd3a0dcb0d80a1e4c96`  
		Last Modified: Fri, 04 Dec 2020 01:29:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:8ad160201c4f5ecf7844ef8865006660c67a29f3ded38b197e4d1ceac08966ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114386918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c06890463e50025481be858d0e654711df6c38fe2c7236f9c20dabbd7038590`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 13:27:26 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 13:27:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 13:27:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:56:29 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 01:58:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:58:26 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:58:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:58:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:58:38 GMT
WORKDIR /go
# Fri, 04 Dec 2020 03:13:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 03:13:32 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 03:13:36 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 03:13:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 03:13:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 03:13:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 03:14:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9900411dc7c8c88618743573bf89478d726007403bd002d8b00d21b7fecd40a`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 283.2 KB (283205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbd106374e3baf7eb8e3d8f7ffd4c364a35e57dcb3a89f8a153327a4c3fa3f9`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018c21191f366f1d0001ca2ec647fe3454179351700e264f9025f3efe636d5a2`  
		Last Modified: Fri, 04 Dec 2020 02:07:13 GMT  
		Size: 101.1 MB (101092006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b3c970f8c564da928ce32db5cc7981e5bc4819b99016458cf9f2ceda95aa31`  
		Last Modified: Fri, 04 Dec 2020 02:06:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6379430057b0313b2aa26fed01de99735afdc60ab9085d4a8660e5bbaa2b5595`  
		Last Modified: Fri, 04 Dec 2020 03:14:44 GMT  
		Size: 8.9 MB (8919986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71eeeb13c478d19d8ddd430419adba93210219538a556c2f13d6888de61b01d`  
		Last Modified: Fri, 04 Dec 2020 03:14:43 GMT  
		Size: 1.3 MB (1287788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b553b21761e1bd135a537841af7ef976560d1e74642f117e38ae3254ddf4eb9`  
		Last Modified: Fri, 04 Dec 2020 03:14:42 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - linux; s390x

```console
$ docker pull caddy@sha256:f52177d55e579fb060a4948c8ab350ec391cb66981aa3c19f6679b89bc11d21c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118805074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46e9b596fe9e786ef15184f4d52c8e67a630830ea348c7be3d5ffdbbe4519dba`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:53:28 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 02:53:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:53:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:43:59 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:45:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:45:26 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:45:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:45:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:45:28 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:07:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:07:54 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:07:54 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 01:07:54 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:07:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:07:56 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:07:56 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5139d7663b8674a989574c2161166fb137f26ef16b2f701159c126628be75101`  
		Last Modified: Thu, 22 Oct 2020 02:58:32 GMT  
		Size: 281.4 KB (281363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d31a06258ad66efe2dedbf67809ebc107a55757b8a4543af77982f55ff6c067`  
		Last Modified: Thu, 22 Oct 2020 02:58:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaad7db4ec01c554a618ebac1f61b959bccd70e3f8fc0785a59184f339aa86d3`  
		Last Modified: Fri, 04 Dec 2020 00:50:40 GMT  
		Size: 106.2 MB (106216195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b39947ffb8ce26e266d93d67e3f57f7809db37f576d55d81e2615141795de7`  
		Last Modified: Fri, 04 Dec 2020 00:50:26 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5794dec4cffbe160fd928ee6d98a33715cafe7ae3207a7fe00d667f02b3ddb9`  
		Last Modified: Fri, 04 Dec 2020 01:08:24 GMT  
		Size: 8.4 MB (8352221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9902eaeb6b923e986d4208b2672bd9b954eddcd687fbd6599bdd15a0f991fa93`  
		Last Modified: Fri, 04 Dec 2020 01:08:22 GMT  
		Size: 1.4 MB (1388750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c240f721a1a8d8fc37cfad83efafb1aa384fb0043d664639cfe0af964230f8`  
		Last Modified: Fri, 04 Dec 2020 01:08:22 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - windows version 10.0.17763.1577; amd64

```console
$ docker pull caddy@sha256:1b4c71d3f63a5d9c7028f75729bd4e074594246b727128334e435b2a41c5b29f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2562830037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d09fa3868f18fb9bd00dcaaae39f70c15647ee55b70d3010a4cfcbfad3c064eb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 13:43:36 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Nov 2020 13:43:37 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Nov 2020 13:43:38 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Nov 2020 13:43:38 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Nov 2020 13:44:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 13:44:33 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Nov 2020 13:44:55 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Dec 2020 00:15:09 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:17:48 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Dec 2020 00:17:50 GMT
WORKDIR C:\gopath
# Fri, 04 Dec 2020 00:57:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Dec 2020 00:57:33 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:57:33 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:57:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:57:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Dec 2020 00:57:57 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19e00ae033e023d5973e57402eb3f05fe0908fa3f40cd0a36ae20bc72df3927`  
		Last Modified: Wed, 11 Nov 2020 14:08:35 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7f2350f21c33479862fe11c4c46ef7fc8054cb8e0acb2581b663d9e71d37f4`  
		Last Modified: Wed, 11 Nov 2020 14:08:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b816110035a14bde6916267f7e5f008617773d19d8f23f77597d10b021b787c`  
		Last Modified: Wed, 11 Nov 2020 14:08:30 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7a389242a4449d1ca90994817f199ce0b9ec502e46035e6ea9c78c29282ce8`  
		Last Modified: Wed, 11 Nov 2020 14:08:29 GMT  
		Size: 1.1 KB (1098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c993585709f02af194d96f01fb74b3158a083cac1cbf2036662bd0abab75e3bf`  
		Last Modified: Wed, 11 Nov 2020 14:08:38 GMT  
		Size: 34.3 MB (34333277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822a63153155fc14ab856f02664a39a3dbf45ef8601277d161d64e9475748111`  
		Last Modified: Wed, 11 Nov 2020 14:08:26 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758771af484f25fbbe9ef11107e3680d525f6bfc5a1666db73f0eb9d84be3ef1`  
		Last Modified: Wed, 11 Nov 2020 14:08:26 GMT  
		Size: 311.3 KB (311320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05164df22cc1044ebebf255e3f078aca1c5d0b01cfed997c4c52ac57268041e`  
		Last Modified: Fri, 04 Dec 2020 00:33:08 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d208cb88aaef7d49293e8b5fe6cb80e9520f49d127c6991f47c4a360628ef2`  
		Last Modified: Fri, 04 Dec 2020 00:33:47 GMT  
		Size: 138.4 MB (138372930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219a39d338a89418edc5b2a3e6949d4b7c9055ce4dac36812ee963d3454525ec`  
		Last Modified: Fri, 04 Dec 2020 00:33:08 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1991b3df8a0a87849ff8adb054c48ad26020037337edecf17239b67df9f893`  
		Last Modified: Fri, 04 Dec 2020 01:00:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0b12c4d6b7ca2ef8c70722895e566350e366cfef8befa849c5c8411d906ee3`  
		Last Modified: Fri, 04 Dec 2020 01:00:35 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21e20193de473a33dd040821d1d0c9b3b1ebbfc6613419a329bc10a69d70446`  
		Last Modified: Fri, 04 Dec 2020 01:00:34 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70e2aaadeededbaa5d5a0210375f6e763495d701d736cd1f1d43828b73f4b51`  
		Last Modified: Fri, 04 Dec 2020 01:00:35 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a92e145c6f6fc1ec4a2d2848f07d18ec1f37325a509d874a358a03df6527bad`  
		Last Modified: Fri, 04 Dec 2020 01:00:36 GMT  
		Size: 1.8 MB (1768395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b0df0a8c483f3ae7deb4e4b40fa21008023092e18794654eff3ed0187c7eaa`  
		Last Modified: Fri, 04 Dec 2020 01:00:35 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - windows version 10.0.14393.4046; amd64

```console
$ docker pull caddy@sha256:be0e7ff69ac06bf8741750f6e7c5660ca4e2db3a6f66b8108cd168840c9e20bb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5966466109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:988068fcd7e874d95af542fe45cb6d609b55c7186dca28b21a4336f0bc87e73e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 13:23:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 13:47:33 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Nov 2020 13:47:34 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Nov 2020 13:47:34 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Nov 2020 13:47:35 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Nov 2020 13:49:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 13:49:05 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Nov 2020 13:51:21 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Dec 2020 00:18:05 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:21:33 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Dec 2020 00:21:34 GMT
WORKDIR C:\gopath
# Fri, 04 Dec 2020 00:58:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Dec 2020 00:58:03 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:58:04 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:58:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:59:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Dec 2020 00:59:19 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:126d9a92c0cb7b68c56dec2dd5ba118de9dde3ec6368db734c5135fdf1528a33`  
		Last Modified: Wed, 11 Nov 2020 13:34:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48cdfe7c39f0358056c4c821593e466beab0dd18e49c8fae5aead3044dc4fcc`  
		Last Modified: Wed, 11 Nov 2020 14:09:26 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725a072d8cce622c524652fc146ce1398a73435bfe34b503ce6df7c2ba1954c5`  
		Last Modified: Wed, 11 Nov 2020 14:09:26 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff5342fb3e45a27028014ad657c3d05414fac6d9ea2e1213ac67ebd51c174f5`  
		Last Modified: Wed, 11 Nov 2020 14:09:23 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada6bdd6092185cd48a4b7a37d2fccf12a0598e2793361256a3658393e27de45`  
		Last Modified: Wed, 11 Nov 2020 14:09:22 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcaf43c793d08d3feb1cb8666a774e8709fd62cf468af1fcf7c3470bb777e5bc`  
		Last Modified: Wed, 11 Nov 2020 14:10:05 GMT  
		Size: 35.2 MB (35173627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e19e3e1a800738fb7127bdfaabdc86eb626a4b1ea386389bcc158ee6afcf2e8`  
		Last Modified: Wed, 11 Nov 2020 14:09:19 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8d4839ac80d0d8b637b35572732039f3c4bc755fbfa2ca871d32cf344c0032`  
		Last Modified: Wed, 11 Nov 2020 14:09:25 GMT  
		Size: 5.5 MB (5520399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d4de7953b3278a0185f6a1290763d910034fdd6a6ff612ba88e8cbe9d65316`  
		Last Modified: Fri, 04 Dec 2020 00:34:04 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98d400ad57d745f041190f63e7592642bd84fe503e52beb192ae33fe1a616dc`  
		Last Modified: Fri, 04 Dec 2020 00:34:34 GMT  
		Size: 143.7 MB (143715722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bc180fe611f0157f85450283f2e49a5ce41cea0896671a39bd2f636ae4e2a3`  
		Last Modified: Fri, 04 Dec 2020 00:34:05 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b42e7fb13992aa07e801901bcd8bd61a9dcda76fa6791d68c3bfb3eea1131ae`  
		Last Modified: Fri, 04 Dec 2020 01:00:58 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e814c85456355f9ccc653cc66261b55c1e5a54da713223c960ac9ec7b9e0b207`  
		Last Modified: Fri, 04 Dec 2020 01:00:54 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1b56b590c16755e3db6717e32d5dd0517ab2f6dc7f57419f0e1af7ac2a605e`  
		Last Modified: Fri, 04 Dec 2020 01:00:54 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8844c556721bdbecb70fe920a7c98338fe934a8570a1977bd7feb5554c5e821`  
		Last Modified: Fri, 04 Dec 2020 01:00:54 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247766b9da1eed45f517bad1aaeeccc1644d9672610f79700f35c47784cd7384`  
		Last Modified: Fri, 04 Dec 2020 01:00:58 GMT  
		Size: 11.5 MB (11482569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e585ac8b3a4bcaf593aba5ddb48833a65ee3df816033f13393c575baafd417e`  
		Last Modified: Fri, 04 Dec 2020 01:00:55 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-builder-alpine`

```console
$ docker pull caddy@sha256:6296d8b40dadaa9bdfeba6b6bd67d6d499da9d30c38bea1dbc27ff01999d23ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.2.1-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:d7b066e0ae6a58162afa38de124bde6cafbcf0a7f4d056489ce88cc394471bed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119881414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d52e2ef96ee9bf6c12304aac59194314ca7a1e076d5904b34eac04d61337d964`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:34:56 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:34:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:34:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:21:55 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:24:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:24:09 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:24:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:24:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:24:10 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:49:11 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:49:12 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:49:12 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:49:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:49:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:49:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:49:15 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef7d3d256c8367c41c431143c63d083a25dd62ec9ee9d9773dd9e6c7b70ec9e`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 280.8 KB (280812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9db76c5a1d06710ed4f3073476b2d883ff8e911f8e47c558bc4a8d1d8663fa`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b5e3429cf30be490cdf3c5018e8693e0e1d319ea295c9b0c37dedaa7a1cafb`  
		Last Modified: Fri, 04 Dec 2020 00:31:08 GMT  
		Size: 107.1 MB (107085919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07aa6a0961518234df34a1cf391ec7269a68b99fc112f60e8a7270db07eb3974`  
		Last Modified: Fri, 04 Dec 2020 00:30:49 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fe1a6296183cbfcabe79353a47f9336d847b7ea66b4fb61ae86fc689de5d77`  
		Last Modified: Fri, 04 Dec 2020 00:49:47 GMT  
		Size: 8.3 MB (8309940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1da5ba704ae92109544c4683fde8e8be5eea27b6110540c808341c3b43145c6`  
		Last Modified: Fri, 04 Dec 2020 00:49:45 GMT  
		Size: 1.4 MB (1407200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572698d0ecf1dba5c0b8c6a996637e0de1f7e30e2901dae6927647fc8e0d63e7`  
		Last Modified: Fri, 04 Dec 2020 00:49:44 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:d6805920da89344546ce60bd4b91be62fa46da72cef37f871a07d829a0e6b39d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.1 MB (115088466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ad4d3264c7202d2a8117e3dd2a7c46d4164b1e58f8da8ab94016ec14fc9737b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:07:24 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:07:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:07:27 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:54:37 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:57:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:57:18 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:57:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:57:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:57:23 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:23:51 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:23:52 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:23:52 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 01:23:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:23:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:23:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:23:56 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20cc27a60e8ac1bf56dec787d3d52ba856e657179cfd56050036db79abb4267`  
		Last Modified: Thu, 22 Oct 2020 05:34:55 GMT  
		Size: 281.0 KB (280971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ecce92c3d2de40638d73e682dec26c2b79a055e85c8d70b88f4ccb9485bb9c9`  
		Last Modified: Thu, 22 Oct 2020 05:34:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcce644b45ccf744ed14c7b9273179dc1ad732ffa1bd944e61407793f983b983`  
		Last Modified: Fri, 04 Dec 2020 01:05:18 GMT  
		Size: 102.9 MB (102948648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909e21afe9abe4c8685162bb1ca820c4c1d140304436933b524bf4b048cdbc25`  
		Last Modified: Fri, 04 Dec 2020 01:04:48 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba23987bf60560a98e2e39c226cdf37070ca4f72a514be647528077fe286b3e`  
		Last Modified: Fri, 04 Dec 2020 01:24:26 GMT  
		Size: 7.9 MB (7928869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebe92d17d7243c87fc37008c3e65cbbe4b1b675ccaca7fd4760bc44d7bd7ea3`  
		Last Modified: Fri, 04 Dec 2020 01:24:23 GMT  
		Size: 1.3 MB (1327351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41a9e416157b507873d5b48a6159cf7d013314b857201f0d66921bab89875a1`  
		Last Modified: Fri, 04 Dec 2020 01:24:23 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:bd9531e4414b412e4a1bdb2fbe16e0c83e38c8d058aaa93a6a40245cfd5c8f05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.9 MB (113880893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3158c399bfa2628c5054f9d4e14c2dd225c2b4a45b8130026e462667ba683ce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:21:35 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:23:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:23:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:03:17 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:05:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:05:41 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:05:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:05:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:05:44 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:33:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:33:33 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:33:34 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:33:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:33:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:33:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:33:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b753cfc04fdce9640aac1e7a4b3e7ce15fa60b8e357376e42f294f463a6e890`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 280.1 KB (280084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e90c422e5e4668cb4140aadb622d734faa93c81cc1e283da9b08bbbc65c45c5`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c37b023a65a717d26fdb8c72bba66adc8625ca96fab4d08e70954da6b10139`  
		Last Modified: Fri, 04 Dec 2020 00:14:22 GMT  
		Size: 102.7 MB (102723691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f091034d1629ecd6c35f9bbcb2754721bbfa4e5183794ff2b6ecc75b7b2e0e`  
		Last Modified: Fri, 04 Dec 2020 00:13:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6809b32049841fc890dd29c935db10e86e95c4005906b5eddc3fa42f131cdb5`  
		Last Modified: Fri, 04 Dec 2020 00:34:08 GMT  
		Size: 7.1 MB (7144891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818ba8d461e1618211000580b6f229d2fd9775115c3c4049fb7be235094e0625`  
		Last Modified: Fri, 04 Dec 2020 00:34:07 GMT  
		Size: 1.3 MB (1325838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af262af67e01cb4ef945fd8c992860308e9509dc4810d2cab9ed6955b52a700`  
		Last Modified: Fri, 04 Dec 2020 00:34:07 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:3bd8e226aa9f4fef563f2a76b0c165434ab3145a2b629512dcab6495c677202c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115210346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d5e537fc1b6fe653ff07e33f1a30ba036846e07eb585a5a75815eeabb89e21f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:08:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 04:09:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 04:09:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:59:20 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 01:01:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:01:23 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:01:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:01:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:01:29 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:28:26 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:28:27 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:28:28 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 01:28:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:28:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:28:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:28:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4357932f1b6fb010e1461cc5c673712fb832ac44ee627c691db0b64adf95d13`  
		Last Modified: Thu, 22 Oct 2020 04:28:32 GMT  
		Size: 281.2 KB (281230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c013af1878066e59b688e31fd962e7267430963de27c5257241e3c223aa1d6`  
		Last Modified: Thu, 22 Oct 2020 04:28:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37128a32d7b17416d88331ec94958c63f643120f6e40870110ef00f387be80e5`  
		Last Modified: Fri, 04 Dec 2020 01:09:15 GMT  
		Size: 102.4 MB (102411796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0279cf9b51b6c7d1d4937560cb5536f262e9f4e9c5a1685489387c9753062e04`  
		Last Modified: Fri, 04 Dec 2020 01:08:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed38fb55682cdaae259822fc0a1e349a7992f9f99404e4bdc58b4bee6e75d059`  
		Last Modified: Fri, 04 Dec 2020 01:29:03 GMT  
		Size: 8.5 MB (8499869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9fdec9db4728520c427e5ae86d67521591251e09a667e19f8e6d0419c50d24`  
		Last Modified: Fri, 04 Dec 2020 01:29:01 GMT  
		Size: 1.3 MB (1310181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96eec8ba730f3d05a0aac92b2d5d603ab21395ee6bd7cd3a0dcb0d80a1e4c96`  
		Last Modified: Fri, 04 Dec 2020 01:29:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:8ad160201c4f5ecf7844ef8865006660c67a29f3ded38b197e4d1ceac08966ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114386918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c06890463e50025481be858d0e654711df6c38fe2c7236f9c20dabbd7038590`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 13:27:26 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 13:27:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 13:27:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:56:29 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 01:58:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:58:26 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:58:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:58:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:58:38 GMT
WORKDIR /go
# Fri, 04 Dec 2020 03:13:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 03:13:32 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 03:13:36 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 03:13:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 03:13:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 03:13:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 03:14:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9900411dc7c8c88618743573bf89478d726007403bd002d8b00d21b7fecd40a`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 283.2 KB (283205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbd106374e3baf7eb8e3d8f7ffd4c364a35e57dcb3a89f8a153327a4c3fa3f9`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018c21191f366f1d0001ca2ec647fe3454179351700e264f9025f3efe636d5a2`  
		Last Modified: Fri, 04 Dec 2020 02:07:13 GMT  
		Size: 101.1 MB (101092006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b3c970f8c564da928ce32db5cc7981e5bc4819b99016458cf9f2ceda95aa31`  
		Last Modified: Fri, 04 Dec 2020 02:06:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6379430057b0313b2aa26fed01de99735afdc60ab9085d4a8660e5bbaa2b5595`  
		Last Modified: Fri, 04 Dec 2020 03:14:44 GMT  
		Size: 8.9 MB (8919986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71eeeb13c478d19d8ddd430419adba93210219538a556c2f13d6888de61b01d`  
		Last Modified: Fri, 04 Dec 2020 03:14:43 GMT  
		Size: 1.3 MB (1287788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b553b21761e1bd135a537841af7ef976560d1e74642f117e38ae3254ddf4eb9`  
		Last Modified: Fri, 04 Dec 2020 03:14:42 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:f52177d55e579fb060a4948c8ab350ec391cb66981aa3c19f6679b89bc11d21c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118805074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46e9b596fe9e786ef15184f4d52c8e67a630830ea348c7be3d5ffdbbe4519dba`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:53:28 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 02:53:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:53:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:43:59 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:45:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:45:26 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:45:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:45:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:45:28 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:07:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:07:54 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:07:54 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 01:07:54 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:07:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:07:56 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:07:56 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5139d7663b8674a989574c2161166fb137f26ef16b2f701159c126628be75101`  
		Last Modified: Thu, 22 Oct 2020 02:58:32 GMT  
		Size: 281.4 KB (281363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d31a06258ad66efe2dedbf67809ebc107a55757b8a4543af77982f55ff6c067`  
		Last Modified: Thu, 22 Oct 2020 02:58:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaad7db4ec01c554a618ebac1f61b959bccd70e3f8fc0785a59184f339aa86d3`  
		Last Modified: Fri, 04 Dec 2020 00:50:40 GMT  
		Size: 106.2 MB (106216195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b39947ffb8ce26e266d93d67e3f57f7809db37f576d55d81e2615141795de7`  
		Last Modified: Fri, 04 Dec 2020 00:50:26 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5794dec4cffbe160fd928ee6d98a33715cafe7ae3207a7fe00d667f02b3ddb9`  
		Last Modified: Fri, 04 Dec 2020 01:08:24 GMT  
		Size: 8.4 MB (8352221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9902eaeb6b923e986d4208b2672bd9b954eddcd687fbd6599bdd15a0f991fa93`  
		Last Modified: Fri, 04 Dec 2020 01:08:22 GMT  
		Size: 1.4 MB (1388750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c240f721a1a8d8fc37cfad83efafb1aa384fb0043d664639cfe0af964230f8`  
		Last Modified: Fri, 04 Dec 2020 01:08:22 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:c1be9c3404f3bbfc27d368ff0dce5e7a279260fec6705f96e6cdfea4854b4dde
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `caddy:2.2.1-builder-windowsservercore-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull caddy@sha256:1b4c71d3f63a5d9c7028f75729bd4e074594246b727128334e435b2a41c5b29f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2562830037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d09fa3868f18fb9bd00dcaaae39f70c15647ee55b70d3010a4cfcbfad3c064eb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 13:43:36 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Nov 2020 13:43:37 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Nov 2020 13:43:38 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Nov 2020 13:43:38 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Nov 2020 13:44:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 13:44:33 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Nov 2020 13:44:55 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Dec 2020 00:15:09 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:17:48 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Dec 2020 00:17:50 GMT
WORKDIR C:\gopath
# Fri, 04 Dec 2020 00:57:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Dec 2020 00:57:33 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:57:33 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:57:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:57:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Dec 2020 00:57:57 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19e00ae033e023d5973e57402eb3f05fe0908fa3f40cd0a36ae20bc72df3927`  
		Last Modified: Wed, 11 Nov 2020 14:08:35 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7f2350f21c33479862fe11c4c46ef7fc8054cb8e0acb2581b663d9e71d37f4`  
		Last Modified: Wed, 11 Nov 2020 14:08:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b816110035a14bde6916267f7e5f008617773d19d8f23f77597d10b021b787c`  
		Last Modified: Wed, 11 Nov 2020 14:08:30 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7a389242a4449d1ca90994817f199ce0b9ec502e46035e6ea9c78c29282ce8`  
		Last Modified: Wed, 11 Nov 2020 14:08:29 GMT  
		Size: 1.1 KB (1098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c993585709f02af194d96f01fb74b3158a083cac1cbf2036662bd0abab75e3bf`  
		Last Modified: Wed, 11 Nov 2020 14:08:38 GMT  
		Size: 34.3 MB (34333277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822a63153155fc14ab856f02664a39a3dbf45ef8601277d161d64e9475748111`  
		Last Modified: Wed, 11 Nov 2020 14:08:26 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758771af484f25fbbe9ef11107e3680d525f6bfc5a1666db73f0eb9d84be3ef1`  
		Last Modified: Wed, 11 Nov 2020 14:08:26 GMT  
		Size: 311.3 KB (311320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05164df22cc1044ebebf255e3f078aca1c5d0b01cfed997c4c52ac57268041e`  
		Last Modified: Fri, 04 Dec 2020 00:33:08 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d208cb88aaef7d49293e8b5fe6cb80e9520f49d127c6991f47c4a360628ef2`  
		Last Modified: Fri, 04 Dec 2020 00:33:47 GMT  
		Size: 138.4 MB (138372930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219a39d338a89418edc5b2a3e6949d4b7c9055ce4dac36812ee963d3454525ec`  
		Last Modified: Fri, 04 Dec 2020 00:33:08 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1991b3df8a0a87849ff8adb054c48ad26020037337edecf17239b67df9f893`  
		Last Modified: Fri, 04 Dec 2020 01:00:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0b12c4d6b7ca2ef8c70722895e566350e366cfef8befa849c5c8411d906ee3`  
		Last Modified: Fri, 04 Dec 2020 01:00:35 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21e20193de473a33dd040821d1d0c9b3b1ebbfc6613419a329bc10a69d70446`  
		Last Modified: Fri, 04 Dec 2020 01:00:34 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70e2aaadeededbaa5d5a0210375f6e763495d701d736cd1f1d43828b73f4b51`  
		Last Modified: Fri, 04 Dec 2020 01:00:35 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a92e145c6f6fc1ec4a2d2848f07d18ec1f37325a509d874a358a03df6527bad`  
		Last Modified: Fri, 04 Dec 2020 01:00:36 GMT  
		Size: 1.8 MB (1768395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b0df0a8c483f3ae7deb4e4b40fa21008023092e18794654eff3ed0187c7eaa`  
		Last Modified: Fri, 04 Dec 2020 01:00:35 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:6db0a189d7bf711b05b117f6ebc582b950dd1786574b3fa36cec30140ed6fdc1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64

### `caddy:2.2.1-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4046; amd64

```console
$ docker pull caddy@sha256:be0e7ff69ac06bf8741750f6e7c5660ca4e2db3a6f66b8108cd168840c9e20bb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5966466109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:988068fcd7e874d95af542fe45cb6d609b55c7186dca28b21a4336f0bc87e73e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 13:23:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 13:47:33 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Nov 2020 13:47:34 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Nov 2020 13:47:34 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Nov 2020 13:47:35 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Nov 2020 13:49:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 13:49:05 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Nov 2020 13:51:21 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Dec 2020 00:18:05 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:21:33 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Dec 2020 00:21:34 GMT
WORKDIR C:\gopath
# Fri, 04 Dec 2020 00:58:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Dec 2020 00:58:03 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:58:04 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:58:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:59:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Dec 2020 00:59:19 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:126d9a92c0cb7b68c56dec2dd5ba118de9dde3ec6368db734c5135fdf1528a33`  
		Last Modified: Wed, 11 Nov 2020 13:34:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48cdfe7c39f0358056c4c821593e466beab0dd18e49c8fae5aead3044dc4fcc`  
		Last Modified: Wed, 11 Nov 2020 14:09:26 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725a072d8cce622c524652fc146ce1398a73435bfe34b503ce6df7c2ba1954c5`  
		Last Modified: Wed, 11 Nov 2020 14:09:26 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff5342fb3e45a27028014ad657c3d05414fac6d9ea2e1213ac67ebd51c174f5`  
		Last Modified: Wed, 11 Nov 2020 14:09:23 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada6bdd6092185cd48a4b7a37d2fccf12a0598e2793361256a3658393e27de45`  
		Last Modified: Wed, 11 Nov 2020 14:09:22 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcaf43c793d08d3feb1cb8666a774e8709fd62cf468af1fcf7c3470bb777e5bc`  
		Last Modified: Wed, 11 Nov 2020 14:10:05 GMT  
		Size: 35.2 MB (35173627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e19e3e1a800738fb7127bdfaabdc86eb626a4b1ea386389bcc158ee6afcf2e8`  
		Last Modified: Wed, 11 Nov 2020 14:09:19 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8d4839ac80d0d8b637b35572732039f3c4bc755fbfa2ca871d32cf344c0032`  
		Last Modified: Wed, 11 Nov 2020 14:09:25 GMT  
		Size: 5.5 MB (5520399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d4de7953b3278a0185f6a1290763d910034fdd6a6ff612ba88e8cbe9d65316`  
		Last Modified: Fri, 04 Dec 2020 00:34:04 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98d400ad57d745f041190f63e7592642bd84fe503e52beb192ae33fe1a616dc`  
		Last Modified: Fri, 04 Dec 2020 00:34:34 GMT  
		Size: 143.7 MB (143715722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bc180fe611f0157f85450283f2e49a5ce41cea0896671a39bd2f636ae4e2a3`  
		Last Modified: Fri, 04 Dec 2020 00:34:05 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b42e7fb13992aa07e801901bcd8bd61a9dcda76fa6791d68c3bfb3eea1131ae`  
		Last Modified: Fri, 04 Dec 2020 01:00:58 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e814c85456355f9ccc653cc66261b55c1e5a54da713223c960ac9ec7b9e0b207`  
		Last Modified: Fri, 04 Dec 2020 01:00:54 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1b56b590c16755e3db6717e32d5dd0517ab2f6dc7f57419f0e1af7ac2a605e`  
		Last Modified: Fri, 04 Dec 2020 01:00:54 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8844c556721bdbecb70fe920a7c98338fe934a8570a1977bd7feb5554c5e821`  
		Last Modified: Fri, 04 Dec 2020 01:00:54 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247766b9da1eed45f517bad1aaeeccc1644d9672610f79700f35c47784cd7384`  
		Last Modified: Fri, 04 Dec 2020 01:00:58 GMT  
		Size: 11.5 MB (11482569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e585ac8b3a4bcaf593aba5ddb48833a65ee3df816033f13393c575baafd417e`  
		Last Modified: Fri, 04 Dec 2020 01:00:55 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-windowsservercore`

```console
$ docker pull caddy@sha256:f89d8c6aed62c51f8b74d1f7d4512f6a16ffde44052f047d9df284b02996413a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64
	-	windows version 10.0.14393.4046; amd64

### `caddy:2.2.1-windowsservercore` - windows version 10.0.17763.1577; amd64

```console
$ docker pull caddy@sha256:dad45b6df45cf6f4c45f010c391544a830a6372847bb2504a23a870eb9e96638
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2413941176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61f3df5163746a4530d03a8bc80f3b1318d935f9f1b3e26f00a31af891a9ba86`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 20:53:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Nov 2020 20:53:31 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 11 Nov 2020 20:54:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Nov 2020 20:54:04 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Nov 2020 20:54:04 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Nov 2020 20:54:05 GMT
VOLUME [c:/config]
# Wed, 11 Nov 2020 20:54:06 GMT
VOLUME [c:/data]
# Wed, 11 Nov 2020 20:54:07 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 11 Nov 2020 20:54:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Nov 2020 20:54:09 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Nov 2020 20:54:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Nov 2020 20:54:11 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Nov 2020 20:54:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Nov 2020 20:54:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Nov 2020 20:54:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Nov 2020 20:54:13 GMT
EXPOSE 80
# Wed, 11 Nov 2020 20:54:14 GMT
EXPOSE 443
# Wed, 11 Nov 2020 20:54:14 GMT
EXPOSE 2019
# Wed, 11 Nov 2020 20:54:30 GMT
RUN caddy version
# Wed, 11 Nov 2020 20:54:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01dcdd0030882c54a82d0a279a4099081c604810ccccb17d3d7c04a2057bf657`  
		Last Modified: Wed, 11 Nov 2020 21:02:39 GMT  
		Size: 9.2 MB (9248045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3be730f5a5cc9d1dd7080908242b9ed33ba6541e7120addf14e416b944b577`  
		Last Modified: Wed, 11 Nov 2020 21:02:36 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d70ac9fb0285fe6670a558e9c1da67b5594dd483872376ac91425a3058f95b9`  
		Last Modified: Wed, 11 Nov 2020 21:02:54 GMT  
		Size: 16.3 MB (16343997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72340d1f03d76debdf2a014ab06bbd3bc5cb1e8358520912f0c9f71f2b4a6ea`  
		Last Modified: Wed, 11 Nov 2020 21:02:34 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ae7bc4f9eb3af2fa576dd096f9992ad2cfc8a2e9aad0af79e1ebf11c95065d`  
		Last Modified: Wed, 11 Nov 2020 21:02:33 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46832c7bcb0b053968836644798024f37cfede18aaac00abed0c1571fbeeca4c`  
		Last Modified: Wed, 11 Nov 2020 21:02:33 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdafb0d35a00870fdb93efde60b2d5c002b5ec117bb07526ec1d744787529f58`  
		Last Modified: Wed, 11 Nov 2020 21:02:31 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af235cb3a2a159b44c6b773e30cbd6f7931055fb7cfed2aee403c9197e0defc`  
		Last Modified: Wed, 11 Nov 2020 21:02:32 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493ee2907458eb7d47b217b59e2f23b4dd4a6974a36a70462fa54e5b9201f26b`  
		Last Modified: Wed, 11 Nov 2020 21:02:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2f8b9a7de64bd747e2afbc20e6ca964b00d3b48ccdb9245e162300a5ef9b44`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc59b5cb8ee3554d8e4971222e0208e7b6dd831b33894abeba76400bbcb7d56`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c88104f4e1fc6125880b248f3e1edcc5cbf3daf73aaf26bf3782972f11203c3`  
		Last Modified: Wed, 11 Nov 2020 21:02:30 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7cb21eb1cd8ca039940f462fdfe3348c877262adbbc5891cdbc3601ffa2649`  
		Last Modified: Wed, 11 Nov 2020 21:02:27 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef21802812d7f9ad5dcebb2efbf8d4831fcdf5b024bac00c22d04e7406a420b`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed806482965bf605e395b83f00ba44639cc1c88b1b8ec7c75bb708d9c031610`  
		Last Modified: Wed, 11 Nov 2020 21:02:24 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee097b51db8b06f6e93d48da3e914d6a598b32681fdf27785279f3f5dbb5796`  
		Last Modified: Wed, 11 Nov 2020 21:02:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf5349d69a690d25aa14a10fab1fc6e7a82ec345bae9e1a01a4dfd95f09cd1b`  
		Last Modified: Wed, 11 Nov 2020 21:02:22 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0b5aa8db0e75c1ef349905a29ef299882814b7937d14753d2e6a972f7b13b1`  
		Last Modified: Wed, 11 Nov 2020 21:02:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cac55d84f022bb91b78bfb339492198e3fa96a7d1e25c1f8e09ad648376d45d`  
		Last Modified: Wed, 11 Nov 2020 21:02:21 GMT  
		Size: 299.3 KB (299301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7476d855c257a4a27ce525860567dd9bd67e74abb01c0fd1b334444ffaa8504c`  
		Last Modified: Wed, 11 Nov 2020 21:02:24 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-windowsservercore` - windows version 10.0.14393.4046; amd64

```console
$ docker pull caddy@sha256:405a17b713c3f1517124a2506ac9b4ed33285819013417e6b90fb2aa07cb0bd6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5802615067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:371225d0afbf64a113a3745e99535e2e17239829f4e36d99aa36e7aee3be9efc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 13:23:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 20:56:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Nov 2020 20:56:05 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 11 Nov 2020 20:57:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Nov 2020 20:57:25 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Nov 2020 20:57:26 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Nov 2020 20:57:28 GMT
VOLUME [c:/config]
# Wed, 11 Nov 2020 20:57:29 GMT
VOLUME [c:/data]
# Wed, 11 Nov 2020 20:57:30 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 11 Nov 2020 20:57:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Nov 2020 20:57:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Nov 2020 20:57:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Nov 2020 20:57:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Nov 2020 20:57:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Nov 2020 20:57:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Nov 2020 20:57:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Nov 2020 20:57:35 GMT
EXPOSE 80
# Wed, 11 Nov 2020 20:57:36 GMT
EXPOSE 443
# Wed, 11 Nov 2020 20:57:37 GMT
EXPOSE 2019
# Wed, 11 Nov 2020 20:58:18 GMT
RUN caddy version
# Wed, 11 Nov 2020 20:58:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:126d9a92c0cb7b68c56dec2dd5ba118de9dde3ec6368db734c5135fdf1528a33`  
		Last Modified: Wed, 11 Nov 2020 13:34:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5595cf12db880fdffb7bc7e0ceef81a68e0766ff34fdc357635566a05b60085`  
		Last Modified: Wed, 11 Nov 2020 21:03:35 GMT  
		Size: 10.1 MB (10089893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47fc9d917c611e97ffa642af414764e4712d012a3b2c10700a357a771d58bf3`  
		Last Modified: Wed, 11 Nov 2020 21:03:24 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2b332d20177fb217e2744454885bba6eb94e9c7512c35bef53cf1222f10b3a`  
		Last Modified: Wed, 11 Nov 2020 21:03:50 GMT  
		Size: 21.7 MB (21694741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061740784584c807be44f52e632b6fcafa7893cab07ca93723103ca41e759cd2`  
		Last Modified: Wed, 11 Nov 2020 21:03:23 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a051df7f978fd750beb5e55b7a7da2d50550a52c97baf897cd3452347196147`  
		Last Modified: Wed, 11 Nov 2020 21:03:23 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94db8d6fb716d4c43b34e09a05176f94701accb480ce613c231d70ef23c649b`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eeb5cfdcdca36082954b3510135aea31966da19679b9cc7d8d4e43a3892f2f5`  
		Last Modified: Wed, 11 Nov 2020 21:03:19 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50cc11877f41dad7cb21c9e61379268e564a03b044ec4cfb124cccd267ef551c`  
		Last Modified: Wed, 11 Nov 2020 21:03:21 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9914893b848ce6d71a6f99575e794219e1603afe1dcee2bcbf69f3a41451ab05`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab52b473d299810d7e49b3d9d98db42e6aa57e5426b79f4cd7f68fd766a8a9b`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3333f590132f229c9979af102fd15c4a5958d9e3d94d50632eeb045c14028ac1`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12c4e6df6d5faa8f29b56e44eb52dc65c9d6795322a0e6d743a9d373f97adf9`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a015ed900b4c4b4d23631449b68473b1e31eda520fa22c7c19a845ac6f133f31`  
		Last Modified: Wed, 11 Nov 2020 21:03:16 GMT  
		Size: 1.1 KB (1069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f354d2a4fb61ae55364b2ae298552e22165583c076c39e05707e906633b8a2`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc11e1af39f958f492359f3242aa5205230791b166e14ab2f94067e9999464e`  
		Last Modified: Wed, 11 Nov 2020 21:03:16 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a4e622ed285e795cc2fd731f38022c2e6ca478f2223fb9fcafe0a61b5e969`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f936683e767d2733a4a898519ce7c8bc6a608fede4e7cc04c41b5fed180287`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b4fbe6665c83c229d90ec42acce959b356dbf1a97ca281604625a29d8437133`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6966c1a2733b248361e0fbafefb3b58805b223ef954ced160cb1ca7f239c25`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 251.9 KB (251913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3d08972458dc80b8c379340207e2cfeee9ea33d9e9e405ebbf52421ef16dd5`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-windowsservercore-1809`

```console
$ docker pull caddy@sha256:89299b443724d4b0e89af13958b82e2d8fc4185f2a5a8dbfb83a284bab6f5b1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `caddy:2.2.1-windowsservercore-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull caddy@sha256:dad45b6df45cf6f4c45f010c391544a830a6372847bb2504a23a870eb9e96638
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2413941176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61f3df5163746a4530d03a8bc80f3b1318d935f9f1b3e26f00a31af891a9ba86`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 20:53:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Nov 2020 20:53:31 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 11 Nov 2020 20:54:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Nov 2020 20:54:04 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Nov 2020 20:54:04 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Nov 2020 20:54:05 GMT
VOLUME [c:/config]
# Wed, 11 Nov 2020 20:54:06 GMT
VOLUME [c:/data]
# Wed, 11 Nov 2020 20:54:07 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 11 Nov 2020 20:54:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Nov 2020 20:54:09 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Nov 2020 20:54:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Nov 2020 20:54:11 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Nov 2020 20:54:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Nov 2020 20:54:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Nov 2020 20:54:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Nov 2020 20:54:13 GMT
EXPOSE 80
# Wed, 11 Nov 2020 20:54:14 GMT
EXPOSE 443
# Wed, 11 Nov 2020 20:54:14 GMT
EXPOSE 2019
# Wed, 11 Nov 2020 20:54:30 GMT
RUN caddy version
# Wed, 11 Nov 2020 20:54:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01dcdd0030882c54a82d0a279a4099081c604810ccccb17d3d7c04a2057bf657`  
		Last Modified: Wed, 11 Nov 2020 21:02:39 GMT  
		Size: 9.2 MB (9248045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3be730f5a5cc9d1dd7080908242b9ed33ba6541e7120addf14e416b944b577`  
		Last Modified: Wed, 11 Nov 2020 21:02:36 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d70ac9fb0285fe6670a558e9c1da67b5594dd483872376ac91425a3058f95b9`  
		Last Modified: Wed, 11 Nov 2020 21:02:54 GMT  
		Size: 16.3 MB (16343997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72340d1f03d76debdf2a014ab06bbd3bc5cb1e8358520912f0c9f71f2b4a6ea`  
		Last Modified: Wed, 11 Nov 2020 21:02:34 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ae7bc4f9eb3af2fa576dd096f9992ad2cfc8a2e9aad0af79e1ebf11c95065d`  
		Last Modified: Wed, 11 Nov 2020 21:02:33 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46832c7bcb0b053968836644798024f37cfede18aaac00abed0c1571fbeeca4c`  
		Last Modified: Wed, 11 Nov 2020 21:02:33 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdafb0d35a00870fdb93efde60b2d5c002b5ec117bb07526ec1d744787529f58`  
		Last Modified: Wed, 11 Nov 2020 21:02:31 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af235cb3a2a159b44c6b773e30cbd6f7931055fb7cfed2aee403c9197e0defc`  
		Last Modified: Wed, 11 Nov 2020 21:02:32 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493ee2907458eb7d47b217b59e2f23b4dd4a6974a36a70462fa54e5b9201f26b`  
		Last Modified: Wed, 11 Nov 2020 21:02:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2f8b9a7de64bd747e2afbc20e6ca964b00d3b48ccdb9245e162300a5ef9b44`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc59b5cb8ee3554d8e4971222e0208e7b6dd831b33894abeba76400bbcb7d56`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c88104f4e1fc6125880b248f3e1edcc5cbf3daf73aaf26bf3782972f11203c3`  
		Last Modified: Wed, 11 Nov 2020 21:02:30 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7cb21eb1cd8ca039940f462fdfe3348c877262adbbc5891cdbc3601ffa2649`  
		Last Modified: Wed, 11 Nov 2020 21:02:27 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef21802812d7f9ad5dcebb2efbf8d4831fcdf5b024bac00c22d04e7406a420b`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed806482965bf605e395b83f00ba44639cc1c88b1b8ec7c75bb708d9c031610`  
		Last Modified: Wed, 11 Nov 2020 21:02:24 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee097b51db8b06f6e93d48da3e914d6a598b32681fdf27785279f3f5dbb5796`  
		Last Modified: Wed, 11 Nov 2020 21:02:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf5349d69a690d25aa14a10fab1fc6e7a82ec345bae9e1a01a4dfd95f09cd1b`  
		Last Modified: Wed, 11 Nov 2020 21:02:22 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0b5aa8db0e75c1ef349905a29ef299882814b7937d14753d2e6a972f7b13b1`  
		Last Modified: Wed, 11 Nov 2020 21:02:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cac55d84f022bb91b78bfb339492198e3fa96a7d1e25c1f8e09ad648376d45d`  
		Last Modified: Wed, 11 Nov 2020 21:02:21 GMT  
		Size: 299.3 KB (299301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7476d855c257a4a27ce525860567dd9bd67e74abb01c0fd1b334444ffaa8504c`  
		Last Modified: Wed, 11 Nov 2020 21:02:24 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:de5b23a8826e65de497ac7335464d39371cbda3c5c4a3c0b3a3c2a816ad67149
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64

### `caddy:2.2.1-windowsservercore-ltsc2016` - windows version 10.0.14393.4046; amd64

```console
$ docker pull caddy@sha256:405a17b713c3f1517124a2506ac9b4ed33285819013417e6b90fb2aa07cb0bd6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5802615067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:371225d0afbf64a113a3745e99535e2e17239829f4e36d99aa36e7aee3be9efc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 13:23:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 20:56:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Nov 2020 20:56:05 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 11 Nov 2020 20:57:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Nov 2020 20:57:25 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Nov 2020 20:57:26 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Nov 2020 20:57:28 GMT
VOLUME [c:/config]
# Wed, 11 Nov 2020 20:57:29 GMT
VOLUME [c:/data]
# Wed, 11 Nov 2020 20:57:30 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 11 Nov 2020 20:57:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Nov 2020 20:57:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Nov 2020 20:57:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Nov 2020 20:57:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Nov 2020 20:57:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Nov 2020 20:57:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Nov 2020 20:57:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Nov 2020 20:57:35 GMT
EXPOSE 80
# Wed, 11 Nov 2020 20:57:36 GMT
EXPOSE 443
# Wed, 11 Nov 2020 20:57:37 GMT
EXPOSE 2019
# Wed, 11 Nov 2020 20:58:18 GMT
RUN caddy version
# Wed, 11 Nov 2020 20:58:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:126d9a92c0cb7b68c56dec2dd5ba118de9dde3ec6368db734c5135fdf1528a33`  
		Last Modified: Wed, 11 Nov 2020 13:34:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5595cf12db880fdffb7bc7e0ceef81a68e0766ff34fdc357635566a05b60085`  
		Last Modified: Wed, 11 Nov 2020 21:03:35 GMT  
		Size: 10.1 MB (10089893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47fc9d917c611e97ffa642af414764e4712d012a3b2c10700a357a771d58bf3`  
		Last Modified: Wed, 11 Nov 2020 21:03:24 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2b332d20177fb217e2744454885bba6eb94e9c7512c35bef53cf1222f10b3a`  
		Last Modified: Wed, 11 Nov 2020 21:03:50 GMT  
		Size: 21.7 MB (21694741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061740784584c807be44f52e632b6fcafa7893cab07ca93723103ca41e759cd2`  
		Last Modified: Wed, 11 Nov 2020 21:03:23 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a051df7f978fd750beb5e55b7a7da2d50550a52c97baf897cd3452347196147`  
		Last Modified: Wed, 11 Nov 2020 21:03:23 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94db8d6fb716d4c43b34e09a05176f94701accb480ce613c231d70ef23c649b`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eeb5cfdcdca36082954b3510135aea31966da19679b9cc7d8d4e43a3892f2f5`  
		Last Modified: Wed, 11 Nov 2020 21:03:19 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50cc11877f41dad7cb21c9e61379268e564a03b044ec4cfb124cccd267ef551c`  
		Last Modified: Wed, 11 Nov 2020 21:03:21 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9914893b848ce6d71a6f99575e794219e1603afe1dcee2bcbf69f3a41451ab05`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab52b473d299810d7e49b3d9d98db42e6aa57e5426b79f4cd7f68fd766a8a9b`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3333f590132f229c9979af102fd15c4a5958d9e3d94d50632eeb045c14028ac1`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12c4e6df6d5faa8f29b56e44eb52dc65c9d6795322a0e6d743a9d373f97adf9`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a015ed900b4c4b4d23631449b68473b1e31eda520fa22c7c19a845ac6f133f31`  
		Last Modified: Wed, 11 Nov 2020 21:03:16 GMT  
		Size: 1.1 KB (1069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f354d2a4fb61ae55364b2ae298552e22165583c076c39e05707e906633b8a2`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc11e1af39f958f492359f3242aa5205230791b166e14ab2f94067e9999464e`  
		Last Modified: Wed, 11 Nov 2020 21:03:16 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a4e622ed285e795cc2fd731f38022c2e6ca478f2223fb9fcafe0a61b5e969`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f936683e767d2733a4a898519ce7c8bc6a608fede4e7cc04c41b5fed180287`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b4fbe6665c83c229d90ec42acce959b356dbf1a97ca281604625a29d8437133`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6966c1a2733b248361e0fbafefb3b58805b223ef954ced160cb1ca7f239c25`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 251.9 KB (251913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3d08972458dc80b8c379340207e2cfeee9ea33d9e9e405ebbf52421ef16dd5`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:ea06de9c9cb10eacb9f77e50817d2ad8dd63c977549f26c19d57df1a194fefdc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:4ebad49f78a3f98164d89431978046ee6e94f1e8a70454abc7f49ce1a5ee7826
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14635232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bb0137bab0e21a92b0bc9ec1cc22c259b097d5bf239b161ae1eac0de1833e67`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:33:22 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 04:33:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 04:33:55 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 04:33:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 04:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 04:34:01 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 04:34:01 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 04:34:01 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 04:34:02 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 04:34:02 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 04:34:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 04:34:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 04:34:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 04:34:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 04:34:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 04:34:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 04:34:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 04:34:05 GMT
EXPOSE 80
# Thu, 22 Oct 2020 04:34:05 GMT
EXPOSE 443
# Thu, 22 Oct 2020 04:34:06 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 04:34:06 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 04:34:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2e2d825895b6421ca5dbd63db0d99f790ef84a84c7bcaff51e60b654397858`  
		Last Modified: Thu, 22 Oct 2020 04:34:47 GMT  
		Size: 300.0 KB (299956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaf2e3dee2e74b401fce928bf9502e48df68da4e8c1933bfd6b00b1137529fc`  
		Last Modified: Thu, 22 Oct 2020 04:35:02 GMT  
		Size: 5.8 KB (5754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2215cf93250599c5db984cee0fddd5d0cd59ef035ab5a317387b67211bde86d`  
		Last Modified: Thu, 22 Oct 2020 04:35:06 GMT  
		Size: 11.5 MB (11532508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060365e49ba5ee96a2859e269b366f5a5c9f386e5bdbf07d2ef31b1fc6934baa`  
		Last Modified: Thu, 22 Oct 2020 04:35:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:abba73dc860b2f35703cb7d27f08baf5bfc084e18e627b94661d01a8e2befdaf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13784259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f0aad5a281913821dd39ffed5e144daae22ac81ac4314731395ab65eedde72a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:58:10 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 02:58:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 02:58:46 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 02:58:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 02:58:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:59:00 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 02:59:01 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 02:59:01 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 02:59:03 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 02:59:08 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 02:59:09 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 02:59:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 02:59:11 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 02:59:11 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 02:59:12 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 02:59:13 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 02:59:14 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 02:59:15 GMT
EXPOSE 80
# Thu, 22 Oct 2020 02:59:19 GMT
EXPOSE 443
# Thu, 22 Oct 2020 02:59:20 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 02:59:21 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 02:59:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7369c3ac4b39c55c74e96dd3eb61ac2fa65e5671b1c2acca9697a7c9d20c3cf`  
		Last Modified: Thu, 22 Oct 2020 02:59:49 GMT  
		Size: 300.1 KB (300086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8f4045920069dff3382a5993783c5d846d9e28d0f5a63c475ed298fce0abb7`  
		Last Modified: Thu, 22 Oct 2020 03:00:03 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db6bde4735da15e5db23ad62f3d64d78aed8713a40d12547f5538c15c90f9da`  
		Last Modified: Thu, 22 Oct 2020 03:00:06 GMT  
		Size: 10.9 MB (10876280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a95efd7a14ed98a53a238da45faa7e3b0fdd2a93529b83bfe9d0823dafac67c`  
		Last Modified: Thu, 22 Oct 2020 03:00:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:8cf66cbe3c03273ca54bdab908092a6a9b9f02d39595ed15b1111f1465430426
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13565251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b20723dea614fc40d9f3cb59eddd33bf0e89dfda3f8ed4a7b404ef334632a4b9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:04:57 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 03:05:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 03:05:45 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 03:05:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 03:05:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:05:53 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 03:05:53 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 03:05:54 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 03:05:55 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 03:05:56 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 03:05:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 03:05:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 03:05:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 03:05:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 03:05:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 03:06:00 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 03:06:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 03:06:01 GMT
EXPOSE 80
# Thu, 22 Oct 2020 03:06:02 GMT
EXPOSE 443
# Thu, 22 Oct 2020 03:06:02 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 03:06:03 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 03:06:04 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a8e7fe5034ac502626b0a921d79be80c092890176e33b236c489d6f00710a2`  
		Last Modified: Thu, 22 Oct 2020 03:06:32 GMT  
		Size: 299.2 KB (299211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14db75acdaca15b1e81890f29b3b757fcc73e7a69a55f5ed659bf800f6340108`  
		Last Modified: Thu, 22 Oct 2020 03:06:43 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2197c38adf245bca8f229a4cd718c4d0f619a87bae5786572ccdac1a286882c`  
		Last Modified: Thu, 22 Oct 2020 03:06:46 GMT  
		Size: 10.9 MB (10854384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0104bc6a595940856019d00d9ff8e04365338a7964d948b64cc44bf73cc59e`  
		Last Modified: Thu, 22 Oct 2020 03:06:42 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:da121cf42d1759ed03af3130533d365c365af1d738d550744ad863e05e64cf46
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13540356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89b4aa38988ab2442575062d99c3cb44976de6c227256c118f35340e7c21c303`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:40:04 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 02:40:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 02:40:57 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 02:41:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 02:41:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:41:07 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 02:41:08 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 02:41:09 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 02:41:10 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 02:41:10 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 02:41:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 02:41:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 02:41:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 02:41:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 02:41:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 02:41:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 02:41:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 02:41:19 GMT
EXPOSE 80
# Thu, 22 Oct 2020 02:41:20 GMT
EXPOSE 443
# Thu, 22 Oct 2020 02:41:20 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 02:41:21 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 02:41:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dbde357077a97c0f831033bf03c9828203cb7e3e6cb33217ce4d7cfd71c931`  
		Last Modified: Thu, 22 Oct 2020 02:41:47 GMT  
		Size: 300.3 KB (300348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a5ab0aa923ce1fe233b904008bbf932c4787f48bcd59f07a85616147b7cbc3`  
		Last Modified: Thu, 22 Oct 2020 02:41:56 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc398339860cf826624c9c22b5de9b45a193260e2ff24826d210b493483398f`  
		Last Modified: Thu, 22 Oct 2020 02:41:59 GMT  
		Size: 10.5 MB (10527465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6e7d61d1d4a00550447ea1f67edc0463cc527e49356e98959edfafba0df879`  
		Last Modified: Thu, 22 Oct 2020 02:41:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:09208042b4d19d7ed87b51b99dc20b390dab20d9ae7e235a62a3af3aaf472bd5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13291756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe5c77284adc35481d13003d31a866f637b6eaf9f5764f667e536db79ce23129`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 13:39:52 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 13:44:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 13:44:04 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 13:44:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 13:44:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 13:44:33 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 13:44:37 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 13:44:40 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 13:44:44 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 13:44:48 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 13:44:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 13:44:56 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 13:45:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 13:45:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 13:45:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 13:45:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 13:45:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 13:45:23 GMT
EXPOSE 80
# Thu, 22 Oct 2020 13:45:26 GMT
EXPOSE 443
# Thu, 22 Oct 2020 13:45:30 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 13:45:35 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 13:45:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649a4964211b7ce86541a0c1dad8ef3800ec38a3ca90aff94b76759b4cb8e279`  
		Last Modified: Thu, 22 Oct 2020 13:47:22 GMT  
		Size: 302.3 KB (302327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58dd938ef3e3eae8509deda8fab9ab5f9344169d912e35a802633e799feed1bb`  
		Last Modified: Thu, 22 Oct 2020 13:47:52 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe23c296ee12ee12ef84dbabbb4f7bf0362a9a12b684782ebd3f44a97c8fcf8e`  
		Last Modified: Thu, 22 Oct 2020 13:47:55 GMT  
		Size: 10.2 MB (10180223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d2f3c084745fecafaa9ff33626a81124f2d70267ceee705da555714238bfa1`  
		Last Modified: Thu, 22 Oct 2020 13:47:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:3e18b421d651721239cb3422bc890d1211535681219b7696816f487b4cebc4ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14074857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4d5562f1d148d3d67ff7f5995be8f860553ad0f3d07091335643306b83385e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:41:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 02:41:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 02:41:31 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 02:41:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 02:41:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:41:36 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 02:41:36 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 02:41:37 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 02:41:37 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 02:41:37 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 02:41:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 02:41:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 02:41:38 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 02:41:38 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 02:41:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 02:41:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 02:41:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 02:41:40 GMT
EXPOSE 80
# Thu, 22 Oct 2020 02:41:40 GMT
EXPOSE 443
# Thu, 22 Oct 2020 02:41:40 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 02:41:41 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 02:41:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f988ff23f3cbb35bfed69e33f3b7ee69403bfae4f46363a08eea4830053e9c`  
		Last Modified: Thu, 22 Oct 2020 02:42:01 GMT  
		Size: 300.5 KB (300481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd6a4e0db99510879c5dfceabd1e629a0692c4544bb0da34971f8722b881e92`  
		Last Modified: Thu, 22 Oct 2020 02:42:09 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e13b938aa802e74610585cabba77d625db4baf219f577a81195c272408c7d3`  
		Last Modified: Thu, 22 Oct 2020 02:42:16 GMT  
		Size: 11.2 MB (11202559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a221fff082950a8a98db12eb99f532a39008f0d6e21684bc1aed06fa1ed2a764`  
		Last Modified: Thu, 22 Oct 2020 02:42:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:11b6dc688f10fd45996d660117a4567192599b9dc33e0ed69376f3e771473085
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1577; amd64
	-	windows version 10.0.14393.4046; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:d7b066e0ae6a58162afa38de124bde6cafbcf0a7f4d056489ce88cc394471bed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119881414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d52e2ef96ee9bf6c12304aac59194314ca7a1e076d5904b34eac04d61337d964`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:34:56 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:34:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:34:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:21:55 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:24:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:24:09 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:24:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:24:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:24:10 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:49:11 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:49:12 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:49:12 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:49:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:49:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:49:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:49:15 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef7d3d256c8367c41c431143c63d083a25dd62ec9ee9d9773dd9e6c7b70ec9e`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 280.8 KB (280812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9db76c5a1d06710ed4f3073476b2d883ff8e911f8e47c558bc4a8d1d8663fa`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b5e3429cf30be490cdf3c5018e8693e0e1d319ea295c9b0c37dedaa7a1cafb`  
		Last Modified: Fri, 04 Dec 2020 00:31:08 GMT  
		Size: 107.1 MB (107085919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07aa6a0961518234df34a1cf391ec7269a68b99fc112f60e8a7270db07eb3974`  
		Last Modified: Fri, 04 Dec 2020 00:30:49 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fe1a6296183cbfcabe79353a47f9336d847b7ea66b4fb61ae86fc689de5d77`  
		Last Modified: Fri, 04 Dec 2020 00:49:47 GMT  
		Size: 8.3 MB (8309940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1da5ba704ae92109544c4683fde8e8be5eea27b6110540c808341c3b43145c6`  
		Last Modified: Fri, 04 Dec 2020 00:49:45 GMT  
		Size: 1.4 MB (1407200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572698d0ecf1dba5c0b8c6a996637e0de1f7e30e2901dae6927647fc8e0d63e7`  
		Last Modified: Fri, 04 Dec 2020 00:49:44 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:d6805920da89344546ce60bd4b91be62fa46da72cef37f871a07d829a0e6b39d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.1 MB (115088466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ad4d3264c7202d2a8117e3dd2a7c46d4164b1e58f8da8ab94016ec14fc9737b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:07:24 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:07:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:07:27 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:54:37 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:57:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:57:18 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:57:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:57:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:57:23 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:23:51 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:23:52 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:23:52 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 01:23:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:23:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:23:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:23:56 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20cc27a60e8ac1bf56dec787d3d52ba856e657179cfd56050036db79abb4267`  
		Last Modified: Thu, 22 Oct 2020 05:34:55 GMT  
		Size: 281.0 KB (280971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ecce92c3d2de40638d73e682dec26c2b79a055e85c8d70b88f4ccb9485bb9c9`  
		Last Modified: Thu, 22 Oct 2020 05:34:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcce644b45ccf744ed14c7b9273179dc1ad732ffa1bd944e61407793f983b983`  
		Last Modified: Fri, 04 Dec 2020 01:05:18 GMT  
		Size: 102.9 MB (102948648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909e21afe9abe4c8685162bb1ca820c4c1d140304436933b524bf4b048cdbc25`  
		Last Modified: Fri, 04 Dec 2020 01:04:48 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba23987bf60560a98e2e39c226cdf37070ca4f72a514be647528077fe286b3e`  
		Last Modified: Fri, 04 Dec 2020 01:24:26 GMT  
		Size: 7.9 MB (7928869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebe92d17d7243c87fc37008c3e65cbbe4b1b675ccaca7fd4760bc44d7bd7ea3`  
		Last Modified: Fri, 04 Dec 2020 01:24:23 GMT  
		Size: 1.3 MB (1327351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41a9e416157b507873d5b48a6159cf7d013314b857201f0d66921bab89875a1`  
		Last Modified: Fri, 04 Dec 2020 01:24:23 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:bd9531e4414b412e4a1bdb2fbe16e0c83e38c8d058aaa93a6a40245cfd5c8f05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.9 MB (113880893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3158c399bfa2628c5054f9d4e14c2dd225c2b4a45b8130026e462667ba683ce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:21:35 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:23:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:23:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:03:17 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:05:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:05:41 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:05:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:05:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:05:44 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:33:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:33:33 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:33:34 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:33:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:33:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:33:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:33:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b753cfc04fdce9640aac1e7a4b3e7ce15fa60b8e357376e42f294f463a6e890`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 280.1 KB (280084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e90c422e5e4668cb4140aadb622d734faa93c81cc1e283da9b08bbbc65c45c5`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c37b023a65a717d26fdb8c72bba66adc8625ca96fab4d08e70954da6b10139`  
		Last Modified: Fri, 04 Dec 2020 00:14:22 GMT  
		Size: 102.7 MB (102723691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f091034d1629ecd6c35f9bbcb2754721bbfa4e5183794ff2b6ecc75b7b2e0e`  
		Last Modified: Fri, 04 Dec 2020 00:13:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6809b32049841fc890dd29c935db10e86e95c4005906b5eddc3fa42f131cdb5`  
		Last Modified: Fri, 04 Dec 2020 00:34:08 GMT  
		Size: 7.1 MB (7144891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818ba8d461e1618211000580b6f229d2fd9775115c3c4049fb7be235094e0625`  
		Last Modified: Fri, 04 Dec 2020 00:34:07 GMT  
		Size: 1.3 MB (1325838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af262af67e01cb4ef945fd8c992860308e9509dc4810d2cab9ed6955b52a700`  
		Last Modified: Fri, 04 Dec 2020 00:34:07 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:3bd8e226aa9f4fef563f2a76b0c165434ab3145a2b629512dcab6495c677202c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115210346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d5e537fc1b6fe653ff07e33f1a30ba036846e07eb585a5a75815eeabb89e21f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:08:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 04:09:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 04:09:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:59:20 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 01:01:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:01:23 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:01:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:01:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:01:29 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:28:26 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:28:27 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:28:28 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 01:28:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:28:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:28:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:28:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4357932f1b6fb010e1461cc5c673712fb832ac44ee627c691db0b64adf95d13`  
		Last Modified: Thu, 22 Oct 2020 04:28:32 GMT  
		Size: 281.2 KB (281230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c013af1878066e59b688e31fd962e7267430963de27c5257241e3c223aa1d6`  
		Last Modified: Thu, 22 Oct 2020 04:28:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37128a32d7b17416d88331ec94958c63f643120f6e40870110ef00f387be80e5`  
		Last Modified: Fri, 04 Dec 2020 01:09:15 GMT  
		Size: 102.4 MB (102411796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0279cf9b51b6c7d1d4937560cb5536f262e9f4e9c5a1685489387c9753062e04`  
		Last Modified: Fri, 04 Dec 2020 01:08:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed38fb55682cdaae259822fc0a1e349a7992f9f99404e4bdc58b4bee6e75d059`  
		Last Modified: Fri, 04 Dec 2020 01:29:03 GMT  
		Size: 8.5 MB (8499869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9fdec9db4728520c427e5ae86d67521591251e09a667e19f8e6d0419c50d24`  
		Last Modified: Fri, 04 Dec 2020 01:29:01 GMT  
		Size: 1.3 MB (1310181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96eec8ba730f3d05a0aac92b2d5d603ab21395ee6bd7cd3a0dcb0d80a1e4c96`  
		Last Modified: Fri, 04 Dec 2020 01:29:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:8ad160201c4f5ecf7844ef8865006660c67a29f3ded38b197e4d1ceac08966ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114386918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c06890463e50025481be858d0e654711df6c38fe2c7236f9c20dabbd7038590`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 13:27:26 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 13:27:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 13:27:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:56:29 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 01:58:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:58:26 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:58:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:58:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:58:38 GMT
WORKDIR /go
# Fri, 04 Dec 2020 03:13:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 03:13:32 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 03:13:36 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 03:13:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 03:13:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 03:13:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 03:14:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9900411dc7c8c88618743573bf89478d726007403bd002d8b00d21b7fecd40a`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 283.2 KB (283205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbd106374e3baf7eb8e3d8f7ffd4c364a35e57dcb3a89f8a153327a4c3fa3f9`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018c21191f366f1d0001ca2ec647fe3454179351700e264f9025f3efe636d5a2`  
		Last Modified: Fri, 04 Dec 2020 02:07:13 GMT  
		Size: 101.1 MB (101092006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b3c970f8c564da928ce32db5cc7981e5bc4819b99016458cf9f2ceda95aa31`  
		Last Modified: Fri, 04 Dec 2020 02:06:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6379430057b0313b2aa26fed01de99735afdc60ab9085d4a8660e5bbaa2b5595`  
		Last Modified: Fri, 04 Dec 2020 03:14:44 GMT  
		Size: 8.9 MB (8919986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71eeeb13c478d19d8ddd430419adba93210219538a556c2f13d6888de61b01d`  
		Last Modified: Fri, 04 Dec 2020 03:14:43 GMT  
		Size: 1.3 MB (1287788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b553b21761e1bd135a537841af7ef976560d1e74642f117e38ae3254ddf4eb9`  
		Last Modified: Fri, 04 Dec 2020 03:14:42 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:f52177d55e579fb060a4948c8ab350ec391cb66981aa3c19f6679b89bc11d21c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118805074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46e9b596fe9e786ef15184f4d52c8e67a630830ea348c7be3d5ffdbbe4519dba`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:53:28 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 02:53:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:53:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:43:59 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:45:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:45:26 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:45:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:45:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:45:28 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:07:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:07:54 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:07:54 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 01:07:54 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:07:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:07:56 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:07:56 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5139d7663b8674a989574c2161166fb137f26ef16b2f701159c126628be75101`  
		Last Modified: Thu, 22 Oct 2020 02:58:32 GMT  
		Size: 281.4 KB (281363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d31a06258ad66efe2dedbf67809ebc107a55757b8a4543af77982f55ff6c067`  
		Last Modified: Thu, 22 Oct 2020 02:58:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaad7db4ec01c554a618ebac1f61b959bccd70e3f8fc0785a59184f339aa86d3`  
		Last Modified: Fri, 04 Dec 2020 00:50:40 GMT  
		Size: 106.2 MB (106216195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b39947ffb8ce26e266d93d67e3f57f7809db37f576d55d81e2615141795de7`  
		Last Modified: Fri, 04 Dec 2020 00:50:26 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5794dec4cffbe160fd928ee6d98a33715cafe7ae3207a7fe00d667f02b3ddb9`  
		Last Modified: Fri, 04 Dec 2020 01:08:24 GMT  
		Size: 8.4 MB (8352221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9902eaeb6b923e986d4208b2672bd9b954eddcd687fbd6599bdd15a0f991fa93`  
		Last Modified: Fri, 04 Dec 2020 01:08:22 GMT  
		Size: 1.4 MB (1388750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c240f721a1a8d8fc37cfad83efafb1aa384fb0043d664639cfe0af964230f8`  
		Last Modified: Fri, 04 Dec 2020 01:08:22 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.1577; amd64

```console
$ docker pull caddy@sha256:1b4c71d3f63a5d9c7028f75729bd4e074594246b727128334e435b2a41c5b29f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2562830037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d09fa3868f18fb9bd00dcaaae39f70c15647ee55b70d3010a4cfcbfad3c064eb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 13:43:36 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Nov 2020 13:43:37 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Nov 2020 13:43:38 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Nov 2020 13:43:38 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Nov 2020 13:44:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 13:44:33 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Nov 2020 13:44:55 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Dec 2020 00:15:09 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:17:48 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Dec 2020 00:17:50 GMT
WORKDIR C:\gopath
# Fri, 04 Dec 2020 00:57:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Dec 2020 00:57:33 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:57:33 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:57:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:57:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Dec 2020 00:57:57 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19e00ae033e023d5973e57402eb3f05fe0908fa3f40cd0a36ae20bc72df3927`  
		Last Modified: Wed, 11 Nov 2020 14:08:35 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7f2350f21c33479862fe11c4c46ef7fc8054cb8e0acb2581b663d9e71d37f4`  
		Last Modified: Wed, 11 Nov 2020 14:08:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b816110035a14bde6916267f7e5f008617773d19d8f23f77597d10b021b787c`  
		Last Modified: Wed, 11 Nov 2020 14:08:30 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7a389242a4449d1ca90994817f199ce0b9ec502e46035e6ea9c78c29282ce8`  
		Last Modified: Wed, 11 Nov 2020 14:08:29 GMT  
		Size: 1.1 KB (1098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c993585709f02af194d96f01fb74b3158a083cac1cbf2036662bd0abab75e3bf`  
		Last Modified: Wed, 11 Nov 2020 14:08:38 GMT  
		Size: 34.3 MB (34333277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822a63153155fc14ab856f02664a39a3dbf45ef8601277d161d64e9475748111`  
		Last Modified: Wed, 11 Nov 2020 14:08:26 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758771af484f25fbbe9ef11107e3680d525f6bfc5a1666db73f0eb9d84be3ef1`  
		Last Modified: Wed, 11 Nov 2020 14:08:26 GMT  
		Size: 311.3 KB (311320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05164df22cc1044ebebf255e3f078aca1c5d0b01cfed997c4c52ac57268041e`  
		Last Modified: Fri, 04 Dec 2020 00:33:08 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d208cb88aaef7d49293e8b5fe6cb80e9520f49d127c6991f47c4a360628ef2`  
		Last Modified: Fri, 04 Dec 2020 00:33:47 GMT  
		Size: 138.4 MB (138372930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219a39d338a89418edc5b2a3e6949d4b7c9055ce4dac36812ee963d3454525ec`  
		Last Modified: Fri, 04 Dec 2020 00:33:08 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1991b3df8a0a87849ff8adb054c48ad26020037337edecf17239b67df9f893`  
		Last Modified: Fri, 04 Dec 2020 01:00:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0b12c4d6b7ca2ef8c70722895e566350e366cfef8befa849c5c8411d906ee3`  
		Last Modified: Fri, 04 Dec 2020 01:00:35 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21e20193de473a33dd040821d1d0c9b3b1ebbfc6613419a329bc10a69d70446`  
		Last Modified: Fri, 04 Dec 2020 01:00:34 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70e2aaadeededbaa5d5a0210375f6e763495d701d736cd1f1d43828b73f4b51`  
		Last Modified: Fri, 04 Dec 2020 01:00:35 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a92e145c6f6fc1ec4a2d2848f07d18ec1f37325a509d874a358a03df6527bad`  
		Last Modified: Fri, 04 Dec 2020 01:00:36 GMT  
		Size: 1.8 MB (1768395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b0df0a8c483f3ae7deb4e4b40fa21008023092e18794654eff3ed0187c7eaa`  
		Last Modified: Fri, 04 Dec 2020 01:00:35 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.14393.4046; amd64

```console
$ docker pull caddy@sha256:be0e7ff69ac06bf8741750f6e7c5660ca4e2db3a6f66b8108cd168840c9e20bb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5966466109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:988068fcd7e874d95af542fe45cb6d609b55c7186dca28b21a4336f0bc87e73e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 13:23:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 13:47:33 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Nov 2020 13:47:34 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Nov 2020 13:47:34 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Nov 2020 13:47:35 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Nov 2020 13:49:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 13:49:05 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Nov 2020 13:51:21 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Dec 2020 00:18:05 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:21:33 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Dec 2020 00:21:34 GMT
WORKDIR C:\gopath
# Fri, 04 Dec 2020 00:58:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Dec 2020 00:58:03 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:58:04 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:58:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:59:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Dec 2020 00:59:19 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:126d9a92c0cb7b68c56dec2dd5ba118de9dde3ec6368db734c5135fdf1528a33`  
		Last Modified: Wed, 11 Nov 2020 13:34:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48cdfe7c39f0358056c4c821593e466beab0dd18e49c8fae5aead3044dc4fcc`  
		Last Modified: Wed, 11 Nov 2020 14:09:26 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725a072d8cce622c524652fc146ce1398a73435bfe34b503ce6df7c2ba1954c5`  
		Last Modified: Wed, 11 Nov 2020 14:09:26 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff5342fb3e45a27028014ad657c3d05414fac6d9ea2e1213ac67ebd51c174f5`  
		Last Modified: Wed, 11 Nov 2020 14:09:23 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada6bdd6092185cd48a4b7a37d2fccf12a0598e2793361256a3658393e27de45`  
		Last Modified: Wed, 11 Nov 2020 14:09:22 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcaf43c793d08d3feb1cb8666a774e8709fd62cf468af1fcf7c3470bb777e5bc`  
		Last Modified: Wed, 11 Nov 2020 14:10:05 GMT  
		Size: 35.2 MB (35173627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e19e3e1a800738fb7127bdfaabdc86eb626a4b1ea386389bcc158ee6afcf2e8`  
		Last Modified: Wed, 11 Nov 2020 14:09:19 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8d4839ac80d0d8b637b35572732039f3c4bc755fbfa2ca871d32cf344c0032`  
		Last Modified: Wed, 11 Nov 2020 14:09:25 GMT  
		Size: 5.5 MB (5520399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d4de7953b3278a0185f6a1290763d910034fdd6a6ff612ba88e8cbe9d65316`  
		Last Modified: Fri, 04 Dec 2020 00:34:04 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98d400ad57d745f041190f63e7592642bd84fe503e52beb192ae33fe1a616dc`  
		Last Modified: Fri, 04 Dec 2020 00:34:34 GMT  
		Size: 143.7 MB (143715722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bc180fe611f0157f85450283f2e49a5ce41cea0896671a39bd2f636ae4e2a3`  
		Last Modified: Fri, 04 Dec 2020 00:34:05 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b42e7fb13992aa07e801901bcd8bd61a9dcda76fa6791d68c3bfb3eea1131ae`  
		Last Modified: Fri, 04 Dec 2020 01:00:58 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e814c85456355f9ccc653cc66261b55c1e5a54da713223c960ac9ec7b9e0b207`  
		Last Modified: Fri, 04 Dec 2020 01:00:54 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1b56b590c16755e3db6717e32d5dd0517ab2f6dc7f57419f0e1af7ac2a605e`  
		Last Modified: Fri, 04 Dec 2020 01:00:54 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8844c556721bdbecb70fe920a7c98338fe934a8570a1977bd7feb5554c5e821`  
		Last Modified: Fri, 04 Dec 2020 01:00:54 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247766b9da1eed45f517bad1aaeeccc1644d9672610f79700f35c47784cd7384`  
		Last Modified: Fri, 04 Dec 2020 01:00:58 GMT  
		Size: 11.5 MB (11482569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e585ac8b3a4bcaf593aba5ddb48833a65ee3df816033f13393c575baafd417e`  
		Last Modified: Fri, 04 Dec 2020 01:00:55 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:6296d8b40dadaa9bdfeba6b6bd67d6d499da9d30c38bea1dbc27ff01999d23ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:d7b066e0ae6a58162afa38de124bde6cafbcf0a7f4d056489ce88cc394471bed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119881414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d52e2ef96ee9bf6c12304aac59194314ca7a1e076d5904b34eac04d61337d964`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:34:56 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:34:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:34:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:21:55 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:24:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:24:09 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:24:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:24:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:24:10 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:49:11 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:49:12 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:49:12 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:49:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:49:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:49:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:49:15 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef7d3d256c8367c41c431143c63d083a25dd62ec9ee9d9773dd9e6c7b70ec9e`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 280.8 KB (280812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9db76c5a1d06710ed4f3073476b2d883ff8e911f8e47c558bc4a8d1d8663fa`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b5e3429cf30be490cdf3c5018e8693e0e1d319ea295c9b0c37dedaa7a1cafb`  
		Last Modified: Fri, 04 Dec 2020 00:31:08 GMT  
		Size: 107.1 MB (107085919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07aa6a0961518234df34a1cf391ec7269a68b99fc112f60e8a7270db07eb3974`  
		Last Modified: Fri, 04 Dec 2020 00:30:49 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fe1a6296183cbfcabe79353a47f9336d847b7ea66b4fb61ae86fc689de5d77`  
		Last Modified: Fri, 04 Dec 2020 00:49:47 GMT  
		Size: 8.3 MB (8309940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1da5ba704ae92109544c4683fde8e8be5eea27b6110540c808341c3b43145c6`  
		Last Modified: Fri, 04 Dec 2020 00:49:45 GMT  
		Size: 1.4 MB (1407200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572698d0ecf1dba5c0b8c6a996637e0de1f7e30e2901dae6927647fc8e0d63e7`  
		Last Modified: Fri, 04 Dec 2020 00:49:44 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:d6805920da89344546ce60bd4b91be62fa46da72cef37f871a07d829a0e6b39d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.1 MB (115088466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ad4d3264c7202d2a8117e3dd2a7c46d4164b1e58f8da8ab94016ec14fc9737b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:07:24 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:07:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:07:27 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:54:37 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:57:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:57:18 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:57:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:57:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:57:23 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:23:51 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:23:52 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:23:52 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 01:23:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:23:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:23:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:23:56 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20cc27a60e8ac1bf56dec787d3d52ba856e657179cfd56050036db79abb4267`  
		Last Modified: Thu, 22 Oct 2020 05:34:55 GMT  
		Size: 281.0 KB (280971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ecce92c3d2de40638d73e682dec26c2b79a055e85c8d70b88f4ccb9485bb9c9`  
		Last Modified: Thu, 22 Oct 2020 05:34:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcce644b45ccf744ed14c7b9273179dc1ad732ffa1bd944e61407793f983b983`  
		Last Modified: Fri, 04 Dec 2020 01:05:18 GMT  
		Size: 102.9 MB (102948648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909e21afe9abe4c8685162bb1ca820c4c1d140304436933b524bf4b048cdbc25`  
		Last Modified: Fri, 04 Dec 2020 01:04:48 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba23987bf60560a98e2e39c226cdf37070ca4f72a514be647528077fe286b3e`  
		Last Modified: Fri, 04 Dec 2020 01:24:26 GMT  
		Size: 7.9 MB (7928869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebe92d17d7243c87fc37008c3e65cbbe4b1b675ccaca7fd4760bc44d7bd7ea3`  
		Last Modified: Fri, 04 Dec 2020 01:24:23 GMT  
		Size: 1.3 MB (1327351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41a9e416157b507873d5b48a6159cf7d013314b857201f0d66921bab89875a1`  
		Last Modified: Fri, 04 Dec 2020 01:24:23 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:bd9531e4414b412e4a1bdb2fbe16e0c83e38c8d058aaa93a6a40245cfd5c8f05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.9 MB (113880893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3158c399bfa2628c5054f9d4e14c2dd225c2b4a45b8130026e462667ba683ce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:21:35 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:23:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:23:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:03:17 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:05:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:05:41 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:05:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:05:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:05:44 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:33:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:33:33 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:33:34 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:33:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:33:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:33:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:33:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b753cfc04fdce9640aac1e7a4b3e7ce15fa60b8e357376e42f294f463a6e890`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 280.1 KB (280084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e90c422e5e4668cb4140aadb622d734faa93c81cc1e283da9b08bbbc65c45c5`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c37b023a65a717d26fdb8c72bba66adc8625ca96fab4d08e70954da6b10139`  
		Last Modified: Fri, 04 Dec 2020 00:14:22 GMT  
		Size: 102.7 MB (102723691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f091034d1629ecd6c35f9bbcb2754721bbfa4e5183794ff2b6ecc75b7b2e0e`  
		Last Modified: Fri, 04 Dec 2020 00:13:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6809b32049841fc890dd29c935db10e86e95c4005906b5eddc3fa42f131cdb5`  
		Last Modified: Fri, 04 Dec 2020 00:34:08 GMT  
		Size: 7.1 MB (7144891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818ba8d461e1618211000580b6f229d2fd9775115c3c4049fb7be235094e0625`  
		Last Modified: Fri, 04 Dec 2020 00:34:07 GMT  
		Size: 1.3 MB (1325838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af262af67e01cb4ef945fd8c992860308e9509dc4810d2cab9ed6955b52a700`  
		Last Modified: Fri, 04 Dec 2020 00:34:07 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:3bd8e226aa9f4fef563f2a76b0c165434ab3145a2b629512dcab6495c677202c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115210346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d5e537fc1b6fe653ff07e33f1a30ba036846e07eb585a5a75815eeabb89e21f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:08:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 04:09:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 04:09:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:59:20 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 01:01:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:01:23 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:01:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:01:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:01:29 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:28:26 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:28:27 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:28:28 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 01:28:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:28:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:28:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:28:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4357932f1b6fb010e1461cc5c673712fb832ac44ee627c691db0b64adf95d13`  
		Last Modified: Thu, 22 Oct 2020 04:28:32 GMT  
		Size: 281.2 KB (281230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c013af1878066e59b688e31fd962e7267430963de27c5257241e3c223aa1d6`  
		Last Modified: Thu, 22 Oct 2020 04:28:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37128a32d7b17416d88331ec94958c63f643120f6e40870110ef00f387be80e5`  
		Last Modified: Fri, 04 Dec 2020 01:09:15 GMT  
		Size: 102.4 MB (102411796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0279cf9b51b6c7d1d4937560cb5536f262e9f4e9c5a1685489387c9753062e04`  
		Last Modified: Fri, 04 Dec 2020 01:08:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed38fb55682cdaae259822fc0a1e349a7992f9f99404e4bdc58b4bee6e75d059`  
		Last Modified: Fri, 04 Dec 2020 01:29:03 GMT  
		Size: 8.5 MB (8499869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9fdec9db4728520c427e5ae86d67521591251e09a667e19f8e6d0419c50d24`  
		Last Modified: Fri, 04 Dec 2020 01:29:01 GMT  
		Size: 1.3 MB (1310181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96eec8ba730f3d05a0aac92b2d5d603ab21395ee6bd7cd3a0dcb0d80a1e4c96`  
		Last Modified: Fri, 04 Dec 2020 01:29:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:8ad160201c4f5ecf7844ef8865006660c67a29f3ded38b197e4d1ceac08966ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114386918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c06890463e50025481be858d0e654711df6c38fe2c7236f9c20dabbd7038590`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 13:27:26 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 13:27:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 13:27:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:56:29 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 01:58:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:58:26 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:58:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:58:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:58:38 GMT
WORKDIR /go
# Fri, 04 Dec 2020 03:13:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 03:13:32 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 03:13:36 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 03:13:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 03:13:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 03:13:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 03:14:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9900411dc7c8c88618743573bf89478d726007403bd002d8b00d21b7fecd40a`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 283.2 KB (283205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbd106374e3baf7eb8e3d8f7ffd4c364a35e57dcb3a89f8a153327a4c3fa3f9`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018c21191f366f1d0001ca2ec647fe3454179351700e264f9025f3efe636d5a2`  
		Last Modified: Fri, 04 Dec 2020 02:07:13 GMT  
		Size: 101.1 MB (101092006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b3c970f8c564da928ce32db5cc7981e5bc4819b99016458cf9f2ceda95aa31`  
		Last Modified: Fri, 04 Dec 2020 02:06:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6379430057b0313b2aa26fed01de99735afdc60ab9085d4a8660e5bbaa2b5595`  
		Last Modified: Fri, 04 Dec 2020 03:14:44 GMT  
		Size: 8.9 MB (8919986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71eeeb13c478d19d8ddd430419adba93210219538a556c2f13d6888de61b01d`  
		Last Modified: Fri, 04 Dec 2020 03:14:43 GMT  
		Size: 1.3 MB (1287788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b553b21761e1bd135a537841af7ef976560d1e74642f117e38ae3254ddf4eb9`  
		Last Modified: Fri, 04 Dec 2020 03:14:42 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:f52177d55e579fb060a4948c8ab350ec391cb66981aa3c19f6679b89bc11d21c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118805074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46e9b596fe9e786ef15184f4d52c8e67a630830ea348c7be3d5ffdbbe4519dba`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:53:28 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 02:53:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:53:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:43:59 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:45:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:45:26 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:45:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:45:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:45:28 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:07:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:07:54 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:07:54 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 01:07:54 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:07:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:07:56 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:07:56 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5139d7663b8674a989574c2161166fb137f26ef16b2f701159c126628be75101`  
		Last Modified: Thu, 22 Oct 2020 02:58:32 GMT  
		Size: 281.4 KB (281363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d31a06258ad66efe2dedbf67809ebc107a55757b8a4543af77982f55ff6c067`  
		Last Modified: Thu, 22 Oct 2020 02:58:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaad7db4ec01c554a618ebac1f61b959bccd70e3f8fc0785a59184f339aa86d3`  
		Last Modified: Fri, 04 Dec 2020 00:50:40 GMT  
		Size: 106.2 MB (106216195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b39947ffb8ce26e266d93d67e3f57f7809db37f576d55d81e2615141795de7`  
		Last Modified: Fri, 04 Dec 2020 00:50:26 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5794dec4cffbe160fd928ee6d98a33715cafe7ae3207a7fe00d667f02b3ddb9`  
		Last Modified: Fri, 04 Dec 2020 01:08:24 GMT  
		Size: 8.4 MB (8352221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9902eaeb6b923e986d4208b2672bd9b954eddcd687fbd6599bdd15a0f991fa93`  
		Last Modified: Fri, 04 Dec 2020 01:08:22 GMT  
		Size: 1.4 MB (1388750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c240f721a1a8d8fc37cfad83efafb1aa384fb0043d664639cfe0af964230f8`  
		Last Modified: Fri, 04 Dec 2020 01:08:22 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:c1be9c3404f3bbfc27d368ff0dce5e7a279260fec6705f96e6cdfea4854b4dde
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull caddy@sha256:1b4c71d3f63a5d9c7028f75729bd4e074594246b727128334e435b2a41c5b29f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2562830037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d09fa3868f18fb9bd00dcaaae39f70c15647ee55b70d3010a4cfcbfad3c064eb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 13:43:36 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Nov 2020 13:43:37 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Nov 2020 13:43:38 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Nov 2020 13:43:38 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Nov 2020 13:44:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 13:44:33 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Nov 2020 13:44:55 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Dec 2020 00:15:09 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:17:48 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Dec 2020 00:17:50 GMT
WORKDIR C:\gopath
# Fri, 04 Dec 2020 00:57:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Dec 2020 00:57:33 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:57:33 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:57:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:57:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Dec 2020 00:57:57 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19e00ae033e023d5973e57402eb3f05fe0908fa3f40cd0a36ae20bc72df3927`  
		Last Modified: Wed, 11 Nov 2020 14:08:35 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7f2350f21c33479862fe11c4c46ef7fc8054cb8e0acb2581b663d9e71d37f4`  
		Last Modified: Wed, 11 Nov 2020 14:08:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b816110035a14bde6916267f7e5f008617773d19d8f23f77597d10b021b787c`  
		Last Modified: Wed, 11 Nov 2020 14:08:30 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7a389242a4449d1ca90994817f199ce0b9ec502e46035e6ea9c78c29282ce8`  
		Last Modified: Wed, 11 Nov 2020 14:08:29 GMT  
		Size: 1.1 KB (1098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c993585709f02af194d96f01fb74b3158a083cac1cbf2036662bd0abab75e3bf`  
		Last Modified: Wed, 11 Nov 2020 14:08:38 GMT  
		Size: 34.3 MB (34333277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822a63153155fc14ab856f02664a39a3dbf45ef8601277d161d64e9475748111`  
		Last Modified: Wed, 11 Nov 2020 14:08:26 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758771af484f25fbbe9ef11107e3680d525f6bfc5a1666db73f0eb9d84be3ef1`  
		Last Modified: Wed, 11 Nov 2020 14:08:26 GMT  
		Size: 311.3 KB (311320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05164df22cc1044ebebf255e3f078aca1c5d0b01cfed997c4c52ac57268041e`  
		Last Modified: Fri, 04 Dec 2020 00:33:08 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d208cb88aaef7d49293e8b5fe6cb80e9520f49d127c6991f47c4a360628ef2`  
		Last Modified: Fri, 04 Dec 2020 00:33:47 GMT  
		Size: 138.4 MB (138372930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219a39d338a89418edc5b2a3e6949d4b7c9055ce4dac36812ee963d3454525ec`  
		Last Modified: Fri, 04 Dec 2020 00:33:08 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1991b3df8a0a87849ff8adb054c48ad26020037337edecf17239b67df9f893`  
		Last Modified: Fri, 04 Dec 2020 01:00:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0b12c4d6b7ca2ef8c70722895e566350e366cfef8befa849c5c8411d906ee3`  
		Last Modified: Fri, 04 Dec 2020 01:00:35 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21e20193de473a33dd040821d1d0c9b3b1ebbfc6613419a329bc10a69d70446`  
		Last Modified: Fri, 04 Dec 2020 01:00:34 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70e2aaadeededbaa5d5a0210375f6e763495d701d736cd1f1d43828b73f4b51`  
		Last Modified: Fri, 04 Dec 2020 01:00:35 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a92e145c6f6fc1ec4a2d2848f07d18ec1f37325a509d874a358a03df6527bad`  
		Last Modified: Fri, 04 Dec 2020 01:00:36 GMT  
		Size: 1.8 MB (1768395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b0df0a8c483f3ae7deb4e4b40fa21008023092e18794654eff3ed0187c7eaa`  
		Last Modified: Fri, 04 Dec 2020 01:00:35 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:6db0a189d7bf711b05b117f6ebc582b950dd1786574b3fa36cec30140ed6fdc1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64

### `caddy:2-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4046; amd64

```console
$ docker pull caddy@sha256:be0e7ff69ac06bf8741750f6e7c5660ca4e2db3a6f66b8108cd168840c9e20bb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5966466109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:988068fcd7e874d95af542fe45cb6d609b55c7186dca28b21a4336f0bc87e73e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 13:23:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 13:47:33 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Nov 2020 13:47:34 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Nov 2020 13:47:34 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Nov 2020 13:47:35 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Nov 2020 13:49:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 13:49:05 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Nov 2020 13:51:21 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Dec 2020 00:18:05 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:21:33 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Dec 2020 00:21:34 GMT
WORKDIR C:\gopath
# Fri, 04 Dec 2020 00:58:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Dec 2020 00:58:03 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:58:04 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:58:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:59:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Dec 2020 00:59:19 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:126d9a92c0cb7b68c56dec2dd5ba118de9dde3ec6368db734c5135fdf1528a33`  
		Last Modified: Wed, 11 Nov 2020 13:34:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48cdfe7c39f0358056c4c821593e466beab0dd18e49c8fae5aead3044dc4fcc`  
		Last Modified: Wed, 11 Nov 2020 14:09:26 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725a072d8cce622c524652fc146ce1398a73435bfe34b503ce6df7c2ba1954c5`  
		Last Modified: Wed, 11 Nov 2020 14:09:26 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff5342fb3e45a27028014ad657c3d05414fac6d9ea2e1213ac67ebd51c174f5`  
		Last Modified: Wed, 11 Nov 2020 14:09:23 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada6bdd6092185cd48a4b7a37d2fccf12a0598e2793361256a3658393e27de45`  
		Last Modified: Wed, 11 Nov 2020 14:09:22 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcaf43c793d08d3feb1cb8666a774e8709fd62cf468af1fcf7c3470bb777e5bc`  
		Last Modified: Wed, 11 Nov 2020 14:10:05 GMT  
		Size: 35.2 MB (35173627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e19e3e1a800738fb7127bdfaabdc86eb626a4b1ea386389bcc158ee6afcf2e8`  
		Last Modified: Wed, 11 Nov 2020 14:09:19 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8d4839ac80d0d8b637b35572732039f3c4bc755fbfa2ca871d32cf344c0032`  
		Last Modified: Wed, 11 Nov 2020 14:09:25 GMT  
		Size: 5.5 MB (5520399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d4de7953b3278a0185f6a1290763d910034fdd6a6ff612ba88e8cbe9d65316`  
		Last Modified: Fri, 04 Dec 2020 00:34:04 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98d400ad57d745f041190f63e7592642bd84fe503e52beb192ae33fe1a616dc`  
		Last Modified: Fri, 04 Dec 2020 00:34:34 GMT  
		Size: 143.7 MB (143715722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bc180fe611f0157f85450283f2e49a5ce41cea0896671a39bd2f636ae4e2a3`  
		Last Modified: Fri, 04 Dec 2020 00:34:05 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b42e7fb13992aa07e801901bcd8bd61a9dcda76fa6791d68c3bfb3eea1131ae`  
		Last Modified: Fri, 04 Dec 2020 01:00:58 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e814c85456355f9ccc653cc66261b55c1e5a54da713223c960ac9ec7b9e0b207`  
		Last Modified: Fri, 04 Dec 2020 01:00:54 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1b56b590c16755e3db6717e32d5dd0517ab2f6dc7f57419f0e1af7ac2a605e`  
		Last Modified: Fri, 04 Dec 2020 01:00:54 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8844c556721bdbecb70fe920a7c98338fe934a8570a1977bd7feb5554c5e821`  
		Last Modified: Fri, 04 Dec 2020 01:00:54 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247766b9da1eed45f517bad1aaeeccc1644d9672610f79700f35c47784cd7384`  
		Last Modified: Fri, 04 Dec 2020 01:00:58 GMT  
		Size: 11.5 MB (11482569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e585ac8b3a4bcaf593aba5ddb48833a65ee3df816033f13393c575baafd417e`  
		Last Modified: Fri, 04 Dec 2020 01:00:55 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:f89d8c6aed62c51f8b74d1f7d4512f6a16ffde44052f047d9df284b02996413a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64
	-	windows version 10.0.14393.4046; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.1577; amd64

```console
$ docker pull caddy@sha256:dad45b6df45cf6f4c45f010c391544a830a6372847bb2504a23a870eb9e96638
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2413941176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61f3df5163746a4530d03a8bc80f3b1318d935f9f1b3e26f00a31af891a9ba86`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 20:53:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Nov 2020 20:53:31 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 11 Nov 2020 20:54:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Nov 2020 20:54:04 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Nov 2020 20:54:04 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Nov 2020 20:54:05 GMT
VOLUME [c:/config]
# Wed, 11 Nov 2020 20:54:06 GMT
VOLUME [c:/data]
# Wed, 11 Nov 2020 20:54:07 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 11 Nov 2020 20:54:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Nov 2020 20:54:09 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Nov 2020 20:54:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Nov 2020 20:54:11 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Nov 2020 20:54:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Nov 2020 20:54:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Nov 2020 20:54:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Nov 2020 20:54:13 GMT
EXPOSE 80
# Wed, 11 Nov 2020 20:54:14 GMT
EXPOSE 443
# Wed, 11 Nov 2020 20:54:14 GMT
EXPOSE 2019
# Wed, 11 Nov 2020 20:54:30 GMT
RUN caddy version
# Wed, 11 Nov 2020 20:54:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01dcdd0030882c54a82d0a279a4099081c604810ccccb17d3d7c04a2057bf657`  
		Last Modified: Wed, 11 Nov 2020 21:02:39 GMT  
		Size: 9.2 MB (9248045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3be730f5a5cc9d1dd7080908242b9ed33ba6541e7120addf14e416b944b577`  
		Last Modified: Wed, 11 Nov 2020 21:02:36 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d70ac9fb0285fe6670a558e9c1da67b5594dd483872376ac91425a3058f95b9`  
		Last Modified: Wed, 11 Nov 2020 21:02:54 GMT  
		Size: 16.3 MB (16343997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72340d1f03d76debdf2a014ab06bbd3bc5cb1e8358520912f0c9f71f2b4a6ea`  
		Last Modified: Wed, 11 Nov 2020 21:02:34 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ae7bc4f9eb3af2fa576dd096f9992ad2cfc8a2e9aad0af79e1ebf11c95065d`  
		Last Modified: Wed, 11 Nov 2020 21:02:33 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46832c7bcb0b053968836644798024f37cfede18aaac00abed0c1571fbeeca4c`  
		Last Modified: Wed, 11 Nov 2020 21:02:33 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdafb0d35a00870fdb93efde60b2d5c002b5ec117bb07526ec1d744787529f58`  
		Last Modified: Wed, 11 Nov 2020 21:02:31 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af235cb3a2a159b44c6b773e30cbd6f7931055fb7cfed2aee403c9197e0defc`  
		Last Modified: Wed, 11 Nov 2020 21:02:32 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493ee2907458eb7d47b217b59e2f23b4dd4a6974a36a70462fa54e5b9201f26b`  
		Last Modified: Wed, 11 Nov 2020 21:02:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2f8b9a7de64bd747e2afbc20e6ca964b00d3b48ccdb9245e162300a5ef9b44`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc59b5cb8ee3554d8e4971222e0208e7b6dd831b33894abeba76400bbcb7d56`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c88104f4e1fc6125880b248f3e1edcc5cbf3daf73aaf26bf3782972f11203c3`  
		Last Modified: Wed, 11 Nov 2020 21:02:30 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7cb21eb1cd8ca039940f462fdfe3348c877262adbbc5891cdbc3601ffa2649`  
		Last Modified: Wed, 11 Nov 2020 21:02:27 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef21802812d7f9ad5dcebb2efbf8d4831fcdf5b024bac00c22d04e7406a420b`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed806482965bf605e395b83f00ba44639cc1c88b1b8ec7c75bb708d9c031610`  
		Last Modified: Wed, 11 Nov 2020 21:02:24 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee097b51db8b06f6e93d48da3e914d6a598b32681fdf27785279f3f5dbb5796`  
		Last Modified: Wed, 11 Nov 2020 21:02:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf5349d69a690d25aa14a10fab1fc6e7a82ec345bae9e1a01a4dfd95f09cd1b`  
		Last Modified: Wed, 11 Nov 2020 21:02:22 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0b5aa8db0e75c1ef349905a29ef299882814b7937d14753d2e6a972f7b13b1`  
		Last Modified: Wed, 11 Nov 2020 21:02:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cac55d84f022bb91b78bfb339492198e3fa96a7d1e25c1f8e09ad648376d45d`  
		Last Modified: Wed, 11 Nov 2020 21:02:21 GMT  
		Size: 299.3 KB (299301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7476d855c257a4a27ce525860567dd9bd67e74abb01c0fd1b334444ffaa8504c`  
		Last Modified: Wed, 11 Nov 2020 21:02:24 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.14393.4046; amd64

```console
$ docker pull caddy@sha256:405a17b713c3f1517124a2506ac9b4ed33285819013417e6b90fb2aa07cb0bd6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5802615067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:371225d0afbf64a113a3745e99535e2e17239829f4e36d99aa36e7aee3be9efc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 13:23:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 20:56:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Nov 2020 20:56:05 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 11 Nov 2020 20:57:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Nov 2020 20:57:25 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Nov 2020 20:57:26 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Nov 2020 20:57:28 GMT
VOLUME [c:/config]
# Wed, 11 Nov 2020 20:57:29 GMT
VOLUME [c:/data]
# Wed, 11 Nov 2020 20:57:30 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 11 Nov 2020 20:57:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Nov 2020 20:57:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Nov 2020 20:57:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Nov 2020 20:57:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Nov 2020 20:57:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Nov 2020 20:57:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Nov 2020 20:57:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Nov 2020 20:57:35 GMT
EXPOSE 80
# Wed, 11 Nov 2020 20:57:36 GMT
EXPOSE 443
# Wed, 11 Nov 2020 20:57:37 GMT
EXPOSE 2019
# Wed, 11 Nov 2020 20:58:18 GMT
RUN caddy version
# Wed, 11 Nov 2020 20:58:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:126d9a92c0cb7b68c56dec2dd5ba118de9dde3ec6368db734c5135fdf1528a33`  
		Last Modified: Wed, 11 Nov 2020 13:34:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5595cf12db880fdffb7bc7e0ceef81a68e0766ff34fdc357635566a05b60085`  
		Last Modified: Wed, 11 Nov 2020 21:03:35 GMT  
		Size: 10.1 MB (10089893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47fc9d917c611e97ffa642af414764e4712d012a3b2c10700a357a771d58bf3`  
		Last Modified: Wed, 11 Nov 2020 21:03:24 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2b332d20177fb217e2744454885bba6eb94e9c7512c35bef53cf1222f10b3a`  
		Last Modified: Wed, 11 Nov 2020 21:03:50 GMT  
		Size: 21.7 MB (21694741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061740784584c807be44f52e632b6fcafa7893cab07ca93723103ca41e759cd2`  
		Last Modified: Wed, 11 Nov 2020 21:03:23 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a051df7f978fd750beb5e55b7a7da2d50550a52c97baf897cd3452347196147`  
		Last Modified: Wed, 11 Nov 2020 21:03:23 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94db8d6fb716d4c43b34e09a05176f94701accb480ce613c231d70ef23c649b`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eeb5cfdcdca36082954b3510135aea31966da19679b9cc7d8d4e43a3892f2f5`  
		Last Modified: Wed, 11 Nov 2020 21:03:19 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50cc11877f41dad7cb21c9e61379268e564a03b044ec4cfb124cccd267ef551c`  
		Last Modified: Wed, 11 Nov 2020 21:03:21 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9914893b848ce6d71a6f99575e794219e1603afe1dcee2bcbf69f3a41451ab05`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab52b473d299810d7e49b3d9d98db42e6aa57e5426b79f4cd7f68fd766a8a9b`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3333f590132f229c9979af102fd15c4a5958d9e3d94d50632eeb045c14028ac1`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12c4e6df6d5faa8f29b56e44eb52dc65c9d6795322a0e6d743a9d373f97adf9`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a015ed900b4c4b4d23631449b68473b1e31eda520fa22c7c19a845ac6f133f31`  
		Last Modified: Wed, 11 Nov 2020 21:03:16 GMT  
		Size: 1.1 KB (1069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f354d2a4fb61ae55364b2ae298552e22165583c076c39e05707e906633b8a2`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc11e1af39f958f492359f3242aa5205230791b166e14ab2f94067e9999464e`  
		Last Modified: Wed, 11 Nov 2020 21:03:16 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a4e622ed285e795cc2fd731f38022c2e6ca478f2223fb9fcafe0a61b5e969`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f936683e767d2733a4a898519ce7c8bc6a608fede4e7cc04c41b5fed180287`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b4fbe6665c83c229d90ec42acce959b356dbf1a97ca281604625a29d8437133`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6966c1a2733b248361e0fbafefb3b58805b223ef954ced160cb1ca7f239c25`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 251.9 KB (251913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3d08972458dc80b8c379340207e2cfeee9ea33d9e9e405ebbf52421ef16dd5`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:89299b443724d4b0e89af13958b82e2d8fc4185f2a5a8dbfb83a284bab6f5b1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull caddy@sha256:dad45b6df45cf6f4c45f010c391544a830a6372847bb2504a23a870eb9e96638
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2413941176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61f3df5163746a4530d03a8bc80f3b1318d935f9f1b3e26f00a31af891a9ba86`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 20:53:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Nov 2020 20:53:31 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 11 Nov 2020 20:54:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Nov 2020 20:54:04 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Nov 2020 20:54:04 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Nov 2020 20:54:05 GMT
VOLUME [c:/config]
# Wed, 11 Nov 2020 20:54:06 GMT
VOLUME [c:/data]
# Wed, 11 Nov 2020 20:54:07 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 11 Nov 2020 20:54:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Nov 2020 20:54:09 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Nov 2020 20:54:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Nov 2020 20:54:11 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Nov 2020 20:54:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Nov 2020 20:54:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Nov 2020 20:54:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Nov 2020 20:54:13 GMT
EXPOSE 80
# Wed, 11 Nov 2020 20:54:14 GMT
EXPOSE 443
# Wed, 11 Nov 2020 20:54:14 GMT
EXPOSE 2019
# Wed, 11 Nov 2020 20:54:30 GMT
RUN caddy version
# Wed, 11 Nov 2020 20:54:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01dcdd0030882c54a82d0a279a4099081c604810ccccb17d3d7c04a2057bf657`  
		Last Modified: Wed, 11 Nov 2020 21:02:39 GMT  
		Size: 9.2 MB (9248045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3be730f5a5cc9d1dd7080908242b9ed33ba6541e7120addf14e416b944b577`  
		Last Modified: Wed, 11 Nov 2020 21:02:36 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d70ac9fb0285fe6670a558e9c1da67b5594dd483872376ac91425a3058f95b9`  
		Last Modified: Wed, 11 Nov 2020 21:02:54 GMT  
		Size: 16.3 MB (16343997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72340d1f03d76debdf2a014ab06bbd3bc5cb1e8358520912f0c9f71f2b4a6ea`  
		Last Modified: Wed, 11 Nov 2020 21:02:34 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ae7bc4f9eb3af2fa576dd096f9992ad2cfc8a2e9aad0af79e1ebf11c95065d`  
		Last Modified: Wed, 11 Nov 2020 21:02:33 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46832c7bcb0b053968836644798024f37cfede18aaac00abed0c1571fbeeca4c`  
		Last Modified: Wed, 11 Nov 2020 21:02:33 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdafb0d35a00870fdb93efde60b2d5c002b5ec117bb07526ec1d744787529f58`  
		Last Modified: Wed, 11 Nov 2020 21:02:31 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af235cb3a2a159b44c6b773e30cbd6f7931055fb7cfed2aee403c9197e0defc`  
		Last Modified: Wed, 11 Nov 2020 21:02:32 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493ee2907458eb7d47b217b59e2f23b4dd4a6974a36a70462fa54e5b9201f26b`  
		Last Modified: Wed, 11 Nov 2020 21:02:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2f8b9a7de64bd747e2afbc20e6ca964b00d3b48ccdb9245e162300a5ef9b44`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc59b5cb8ee3554d8e4971222e0208e7b6dd831b33894abeba76400bbcb7d56`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c88104f4e1fc6125880b248f3e1edcc5cbf3daf73aaf26bf3782972f11203c3`  
		Last Modified: Wed, 11 Nov 2020 21:02:30 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7cb21eb1cd8ca039940f462fdfe3348c877262adbbc5891cdbc3601ffa2649`  
		Last Modified: Wed, 11 Nov 2020 21:02:27 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef21802812d7f9ad5dcebb2efbf8d4831fcdf5b024bac00c22d04e7406a420b`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed806482965bf605e395b83f00ba44639cc1c88b1b8ec7c75bb708d9c031610`  
		Last Modified: Wed, 11 Nov 2020 21:02:24 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee097b51db8b06f6e93d48da3e914d6a598b32681fdf27785279f3f5dbb5796`  
		Last Modified: Wed, 11 Nov 2020 21:02:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf5349d69a690d25aa14a10fab1fc6e7a82ec345bae9e1a01a4dfd95f09cd1b`  
		Last Modified: Wed, 11 Nov 2020 21:02:22 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0b5aa8db0e75c1ef349905a29ef299882814b7937d14753d2e6a972f7b13b1`  
		Last Modified: Wed, 11 Nov 2020 21:02:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cac55d84f022bb91b78bfb339492198e3fa96a7d1e25c1f8e09ad648376d45d`  
		Last Modified: Wed, 11 Nov 2020 21:02:21 GMT  
		Size: 299.3 KB (299301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7476d855c257a4a27ce525860567dd9bd67e74abb01c0fd1b334444ffaa8504c`  
		Last Modified: Wed, 11 Nov 2020 21:02:24 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:de5b23a8826e65de497ac7335464d39371cbda3c5c4a3c0b3a3c2a816ad67149
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64

### `caddy:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4046; amd64

```console
$ docker pull caddy@sha256:405a17b713c3f1517124a2506ac9b4ed33285819013417e6b90fb2aa07cb0bd6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5802615067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:371225d0afbf64a113a3745e99535e2e17239829f4e36d99aa36e7aee3be9efc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 13:23:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 20:56:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Nov 2020 20:56:05 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 11 Nov 2020 20:57:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Nov 2020 20:57:25 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Nov 2020 20:57:26 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Nov 2020 20:57:28 GMT
VOLUME [c:/config]
# Wed, 11 Nov 2020 20:57:29 GMT
VOLUME [c:/data]
# Wed, 11 Nov 2020 20:57:30 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 11 Nov 2020 20:57:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Nov 2020 20:57:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Nov 2020 20:57:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Nov 2020 20:57:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Nov 2020 20:57:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Nov 2020 20:57:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Nov 2020 20:57:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Nov 2020 20:57:35 GMT
EXPOSE 80
# Wed, 11 Nov 2020 20:57:36 GMT
EXPOSE 443
# Wed, 11 Nov 2020 20:57:37 GMT
EXPOSE 2019
# Wed, 11 Nov 2020 20:58:18 GMT
RUN caddy version
# Wed, 11 Nov 2020 20:58:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:126d9a92c0cb7b68c56dec2dd5ba118de9dde3ec6368db734c5135fdf1528a33`  
		Last Modified: Wed, 11 Nov 2020 13:34:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5595cf12db880fdffb7bc7e0ceef81a68e0766ff34fdc357635566a05b60085`  
		Last Modified: Wed, 11 Nov 2020 21:03:35 GMT  
		Size: 10.1 MB (10089893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47fc9d917c611e97ffa642af414764e4712d012a3b2c10700a357a771d58bf3`  
		Last Modified: Wed, 11 Nov 2020 21:03:24 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2b332d20177fb217e2744454885bba6eb94e9c7512c35bef53cf1222f10b3a`  
		Last Modified: Wed, 11 Nov 2020 21:03:50 GMT  
		Size: 21.7 MB (21694741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061740784584c807be44f52e632b6fcafa7893cab07ca93723103ca41e759cd2`  
		Last Modified: Wed, 11 Nov 2020 21:03:23 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a051df7f978fd750beb5e55b7a7da2d50550a52c97baf897cd3452347196147`  
		Last Modified: Wed, 11 Nov 2020 21:03:23 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94db8d6fb716d4c43b34e09a05176f94701accb480ce613c231d70ef23c649b`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eeb5cfdcdca36082954b3510135aea31966da19679b9cc7d8d4e43a3892f2f5`  
		Last Modified: Wed, 11 Nov 2020 21:03:19 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50cc11877f41dad7cb21c9e61379268e564a03b044ec4cfb124cccd267ef551c`  
		Last Modified: Wed, 11 Nov 2020 21:03:21 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9914893b848ce6d71a6f99575e794219e1603afe1dcee2bcbf69f3a41451ab05`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab52b473d299810d7e49b3d9d98db42e6aa57e5426b79f4cd7f68fd766a8a9b`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3333f590132f229c9979af102fd15c4a5958d9e3d94d50632eeb045c14028ac1`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12c4e6df6d5faa8f29b56e44eb52dc65c9d6795322a0e6d743a9d373f97adf9`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a015ed900b4c4b4d23631449b68473b1e31eda520fa22c7c19a845ac6f133f31`  
		Last Modified: Wed, 11 Nov 2020 21:03:16 GMT  
		Size: 1.1 KB (1069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f354d2a4fb61ae55364b2ae298552e22165583c076c39e05707e906633b8a2`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc11e1af39f958f492359f3242aa5205230791b166e14ab2f94067e9999464e`  
		Last Modified: Wed, 11 Nov 2020 21:03:16 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a4e622ed285e795cc2fd731f38022c2e6ca478f2223fb9fcafe0a61b5e969`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f936683e767d2733a4a898519ce7c8bc6a608fede4e7cc04c41b5fed180287`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b4fbe6665c83c229d90ec42acce959b356dbf1a97ca281604625a29d8437133`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6966c1a2733b248361e0fbafefb3b58805b223ef954ced160cb1ca7f239c25`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 251.9 KB (251913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3d08972458dc80b8c379340207e2cfeee9ea33d9e9e405ebbf52421ef16dd5`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:ea06de9c9cb10eacb9f77e50817d2ad8dd63c977549f26c19d57df1a194fefdc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:alpine` - linux; amd64

```console
$ docker pull caddy@sha256:4ebad49f78a3f98164d89431978046ee6e94f1e8a70454abc7f49ce1a5ee7826
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14635232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bb0137bab0e21a92b0bc9ec1cc22c259b097d5bf239b161ae1eac0de1833e67`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:33:22 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 04:33:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 04:33:55 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 04:33:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 04:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 04:34:01 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 04:34:01 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 04:34:01 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 04:34:02 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 04:34:02 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 04:34:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 04:34:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 04:34:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 04:34:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 04:34:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 04:34:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 04:34:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 04:34:05 GMT
EXPOSE 80
# Thu, 22 Oct 2020 04:34:05 GMT
EXPOSE 443
# Thu, 22 Oct 2020 04:34:06 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 04:34:06 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 04:34:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2e2d825895b6421ca5dbd63db0d99f790ef84a84c7bcaff51e60b654397858`  
		Last Modified: Thu, 22 Oct 2020 04:34:47 GMT  
		Size: 300.0 KB (299956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaf2e3dee2e74b401fce928bf9502e48df68da4e8c1933bfd6b00b1137529fc`  
		Last Modified: Thu, 22 Oct 2020 04:35:02 GMT  
		Size: 5.8 KB (5754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2215cf93250599c5db984cee0fddd5d0cd59ef035ab5a317387b67211bde86d`  
		Last Modified: Thu, 22 Oct 2020 04:35:06 GMT  
		Size: 11.5 MB (11532508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060365e49ba5ee96a2859e269b366f5a5c9f386e5bdbf07d2ef31b1fc6934baa`  
		Last Modified: Thu, 22 Oct 2020 04:35:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:abba73dc860b2f35703cb7d27f08baf5bfc084e18e627b94661d01a8e2befdaf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13784259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f0aad5a281913821dd39ffed5e144daae22ac81ac4314731395ab65eedde72a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:58:10 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 02:58:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 02:58:46 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 02:58:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 02:58:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:59:00 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 02:59:01 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 02:59:01 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 02:59:03 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 02:59:08 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 02:59:09 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 02:59:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 02:59:11 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 02:59:11 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 02:59:12 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 02:59:13 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 02:59:14 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 02:59:15 GMT
EXPOSE 80
# Thu, 22 Oct 2020 02:59:19 GMT
EXPOSE 443
# Thu, 22 Oct 2020 02:59:20 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 02:59:21 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 02:59:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7369c3ac4b39c55c74e96dd3eb61ac2fa65e5671b1c2acca9697a7c9d20c3cf`  
		Last Modified: Thu, 22 Oct 2020 02:59:49 GMT  
		Size: 300.1 KB (300086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8f4045920069dff3382a5993783c5d846d9e28d0f5a63c475ed298fce0abb7`  
		Last Modified: Thu, 22 Oct 2020 03:00:03 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db6bde4735da15e5db23ad62f3d64d78aed8713a40d12547f5538c15c90f9da`  
		Last Modified: Thu, 22 Oct 2020 03:00:06 GMT  
		Size: 10.9 MB (10876280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a95efd7a14ed98a53a238da45faa7e3b0fdd2a93529b83bfe9d0823dafac67c`  
		Last Modified: Thu, 22 Oct 2020 03:00:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:8cf66cbe3c03273ca54bdab908092a6a9b9f02d39595ed15b1111f1465430426
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13565251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b20723dea614fc40d9f3cb59eddd33bf0e89dfda3f8ed4a7b404ef334632a4b9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:04:57 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 03:05:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 03:05:45 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 03:05:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 03:05:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:05:53 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 03:05:53 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 03:05:54 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 03:05:55 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 03:05:56 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 03:05:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 03:05:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 03:05:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 03:05:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 03:05:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 03:06:00 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 03:06:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 03:06:01 GMT
EXPOSE 80
# Thu, 22 Oct 2020 03:06:02 GMT
EXPOSE 443
# Thu, 22 Oct 2020 03:06:02 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 03:06:03 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 03:06:04 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a8e7fe5034ac502626b0a921d79be80c092890176e33b236c489d6f00710a2`  
		Last Modified: Thu, 22 Oct 2020 03:06:32 GMT  
		Size: 299.2 KB (299211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14db75acdaca15b1e81890f29b3b757fcc73e7a69a55f5ed659bf800f6340108`  
		Last Modified: Thu, 22 Oct 2020 03:06:43 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2197c38adf245bca8f229a4cd718c4d0f619a87bae5786572ccdac1a286882c`  
		Last Modified: Thu, 22 Oct 2020 03:06:46 GMT  
		Size: 10.9 MB (10854384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0104bc6a595940856019d00d9ff8e04365338a7964d948b64cc44bf73cc59e`  
		Last Modified: Thu, 22 Oct 2020 03:06:42 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:da121cf42d1759ed03af3130533d365c365af1d738d550744ad863e05e64cf46
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13540356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89b4aa38988ab2442575062d99c3cb44976de6c227256c118f35340e7c21c303`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:40:04 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 02:40:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 02:40:57 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 02:41:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 02:41:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:41:07 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 02:41:08 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 02:41:09 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 02:41:10 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 02:41:10 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 02:41:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 02:41:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 02:41:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 02:41:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 02:41:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 02:41:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 02:41:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 02:41:19 GMT
EXPOSE 80
# Thu, 22 Oct 2020 02:41:20 GMT
EXPOSE 443
# Thu, 22 Oct 2020 02:41:20 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 02:41:21 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 02:41:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dbde357077a97c0f831033bf03c9828203cb7e3e6cb33217ce4d7cfd71c931`  
		Last Modified: Thu, 22 Oct 2020 02:41:47 GMT  
		Size: 300.3 KB (300348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a5ab0aa923ce1fe233b904008bbf932c4787f48bcd59f07a85616147b7cbc3`  
		Last Modified: Thu, 22 Oct 2020 02:41:56 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc398339860cf826624c9c22b5de9b45a193260e2ff24826d210b493483398f`  
		Last Modified: Thu, 22 Oct 2020 02:41:59 GMT  
		Size: 10.5 MB (10527465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6e7d61d1d4a00550447ea1f67edc0463cc527e49356e98959edfafba0df879`  
		Last Modified: Thu, 22 Oct 2020 02:41:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:09208042b4d19d7ed87b51b99dc20b390dab20d9ae7e235a62a3af3aaf472bd5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13291756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe5c77284adc35481d13003d31a866f637b6eaf9f5764f667e536db79ce23129`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 13:39:52 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 13:44:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 13:44:04 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 13:44:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 13:44:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 13:44:33 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 13:44:37 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 13:44:40 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 13:44:44 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 13:44:48 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 13:44:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 13:44:56 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 13:45:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 13:45:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 13:45:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 13:45:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 13:45:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 13:45:23 GMT
EXPOSE 80
# Thu, 22 Oct 2020 13:45:26 GMT
EXPOSE 443
# Thu, 22 Oct 2020 13:45:30 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 13:45:35 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 13:45:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649a4964211b7ce86541a0c1dad8ef3800ec38a3ca90aff94b76759b4cb8e279`  
		Last Modified: Thu, 22 Oct 2020 13:47:22 GMT  
		Size: 302.3 KB (302327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58dd938ef3e3eae8509deda8fab9ab5f9344169d912e35a802633e799feed1bb`  
		Last Modified: Thu, 22 Oct 2020 13:47:52 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe23c296ee12ee12ef84dbabbb4f7bf0362a9a12b684782ebd3f44a97c8fcf8e`  
		Last Modified: Thu, 22 Oct 2020 13:47:55 GMT  
		Size: 10.2 MB (10180223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d2f3c084745fecafaa9ff33626a81124f2d70267ceee705da555714238bfa1`  
		Last Modified: Thu, 22 Oct 2020 13:47:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:3e18b421d651721239cb3422bc890d1211535681219b7696816f487b4cebc4ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14074857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4d5562f1d148d3d67ff7f5995be8f860553ad0f3d07091335643306b83385e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:41:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 02:41:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 02:41:31 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 02:41:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 02:41:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:41:36 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 02:41:36 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 02:41:37 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 02:41:37 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 02:41:37 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 02:41:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 02:41:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 02:41:38 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 02:41:38 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 02:41:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 02:41:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 02:41:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 02:41:40 GMT
EXPOSE 80
# Thu, 22 Oct 2020 02:41:40 GMT
EXPOSE 443
# Thu, 22 Oct 2020 02:41:40 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 02:41:41 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 02:41:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f988ff23f3cbb35bfed69e33f3b7ee69403bfae4f46363a08eea4830053e9c`  
		Last Modified: Thu, 22 Oct 2020 02:42:01 GMT  
		Size: 300.5 KB (300481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd6a4e0db99510879c5dfceabd1e629a0692c4544bb0da34971f8722b881e92`  
		Last Modified: Thu, 22 Oct 2020 02:42:09 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e13b938aa802e74610585cabba77d625db4baf219f577a81195c272408c7d3`  
		Last Modified: Thu, 22 Oct 2020 02:42:16 GMT  
		Size: 11.2 MB (11202559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a221fff082950a8a98db12eb99f532a39008f0d6e21684bc1aed06fa1ed2a764`  
		Last Modified: Thu, 22 Oct 2020 02:42:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:11b6dc688f10fd45996d660117a4567192599b9dc33e0ed69376f3e771473085
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1577; amd64
	-	windows version 10.0.14393.4046; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:d7b066e0ae6a58162afa38de124bde6cafbcf0a7f4d056489ce88cc394471bed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119881414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d52e2ef96ee9bf6c12304aac59194314ca7a1e076d5904b34eac04d61337d964`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:34:56 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:34:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:34:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:21:55 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:24:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:24:09 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:24:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:24:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:24:10 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:49:11 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:49:12 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:49:12 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:49:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:49:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:49:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:49:15 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef7d3d256c8367c41c431143c63d083a25dd62ec9ee9d9773dd9e6c7b70ec9e`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 280.8 KB (280812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9db76c5a1d06710ed4f3073476b2d883ff8e911f8e47c558bc4a8d1d8663fa`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b5e3429cf30be490cdf3c5018e8693e0e1d319ea295c9b0c37dedaa7a1cafb`  
		Last Modified: Fri, 04 Dec 2020 00:31:08 GMT  
		Size: 107.1 MB (107085919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07aa6a0961518234df34a1cf391ec7269a68b99fc112f60e8a7270db07eb3974`  
		Last Modified: Fri, 04 Dec 2020 00:30:49 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fe1a6296183cbfcabe79353a47f9336d847b7ea66b4fb61ae86fc689de5d77`  
		Last Modified: Fri, 04 Dec 2020 00:49:47 GMT  
		Size: 8.3 MB (8309940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1da5ba704ae92109544c4683fde8e8be5eea27b6110540c808341c3b43145c6`  
		Last Modified: Fri, 04 Dec 2020 00:49:45 GMT  
		Size: 1.4 MB (1407200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572698d0ecf1dba5c0b8c6a996637e0de1f7e30e2901dae6927647fc8e0d63e7`  
		Last Modified: Fri, 04 Dec 2020 00:49:44 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:d6805920da89344546ce60bd4b91be62fa46da72cef37f871a07d829a0e6b39d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.1 MB (115088466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ad4d3264c7202d2a8117e3dd2a7c46d4164b1e58f8da8ab94016ec14fc9737b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:07:24 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:07:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:07:27 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:54:37 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:57:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:57:18 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:57:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:57:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:57:23 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:23:51 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:23:52 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:23:52 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 01:23:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:23:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:23:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:23:56 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20cc27a60e8ac1bf56dec787d3d52ba856e657179cfd56050036db79abb4267`  
		Last Modified: Thu, 22 Oct 2020 05:34:55 GMT  
		Size: 281.0 KB (280971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ecce92c3d2de40638d73e682dec26c2b79a055e85c8d70b88f4ccb9485bb9c9`  
		Last Modified: Thu, 22 Oct 2020 05:34:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcce644b45ccf744ed14c7b9273179dc1ad732ffa1bd944e61407793f983b983`  
		Last Modified: Fri, 04 Dec 2020 01:05:18 GMT  
		Size: 102.9 MB (102948648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909e21afe9abe4c8685162bb1ca820c4c1d140304436933b524bf4b048cdbc25`  
		Last Modified: Fri, 04 Dec 2020 01:04:48 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba23987bf60560a98e2e39c226cdf37070ca4f72a514be647528077fe286b3e`  
		Last Modified: Fri, 04 Dec 2020 01:24:26 GMT  
		Size: 7.9 MB (7928869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebe92d17d7243c87fc37008c3e65cbbe4b1b675ccaca7fd4760bc44d7bd7ea3`  
		Last Modified: Fri, 04 Dec 2020 01:24:23 GMT  
		Size: 1.3 MB (1327351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41a9e416157b507873d5b48a6159cf7d013314b857201f0d66921bab89875a1`  
		Last Modified: Fri, 04 Dec 2020 01:24:23 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:bd9531e4414b412e4a1bdb2fbe16e0c83e38c8d058aaa93a6a40245cfd5c8f05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.9 MB (113880893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3158c399bfa2628c5054f9d4e14c2dd225c2b4a45b8130026e462667ba683ce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:21:35 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:23:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:23:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:03:17 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:05:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:05:41 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:05:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:05:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:05:44 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:33:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:33:33 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:33:34 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:33:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:33:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:33:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:33:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b753cfc04fdce9640aac1e7a4b3e7ce15fa60b8e357376e42f294f463a6e890`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 280.1 KB (280084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e90c422e5e4668cb4140aadb622d734faa93c81cc1e283da9b08bbbc65c45c5`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c37b023a65a717d26fdb8c72bba66adc8625ca96fab4d08e70954da6b10139`  
		Last Modified: Fri, 04 Dec 2020 00:14:22 GMT  
		Size: 102.7 MB (102723691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f091034d1629ecd6c35f9bbcb2754721bbfa4e5183794ff2b6ecc75b7b2e0e`  
		Last Modified: Fri, 04 Dec 2020 00:13:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6809b32049841fc890dd29c935db10e86e95c4005906b5eddc3fa42f131cdb5`  
		Last Modified: Fri, 04 Dec 2020 00:34:08 GMT  
		Size: 7.1 MB (7144891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818ba8d461e1618211000580b6f229d2fd9775115c3c4049fb7be235094e0625`  
		Last Modified: Fri, 04 Dec 2020 00:34:07 GMT  
		Size: 1.3 MB (1325838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af262af67e01cb4ef945fd8c992860308e9509dc4810d2cab9ed6955b52a700`  
		Last Modified: Fri, 04 Dec 2020 00:34:07 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:3bd8e226aa9f4fef563f2a76b0c165434ab3145a2b629512dcab6495c677202c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115210346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d5e537fc1b6fe653ff07e33f1a30ba036846e07eb585a5a75815eeabb89e21f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:08:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 04:09:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 04:09:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:59:20 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 01:01:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:01:23 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:01:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:01:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:01:29 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:28:26 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:28:27 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:28:28 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 01:28:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:28:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:28:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:28:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4357932f1b6fb010e1461cc5c673712fb832ac44ee627c691db0b64adf95d13`  
		Last Modified: Thu, 22 Oct 2020 04:28:32 GMT  
		Size: 281.2 KB (281230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c013af1878066e59b688e31fd962e7267430963de27c5257241e3c223aa1d6`  
		Last Modified: Thu, 22 Oct 2020 04:28:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37128a32d7b17416d88331ec94958c63f643120f6e40870110ef00f387be80e5`  
		Last Modified: Fri, 04 Dec 2020 01:09:15 GMT  
		Size: 102.4 MB (102411796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0279cf9b51b6c7d1d4937560cb5536f262e9f4e9c5a1685489387c9753062e04`  
		Last Modified: Fri, 04 Dec 2020 01:08:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed38fb55682cdaae259822fc0a1e349a7992f9f99404e4bdc58b4bee6e75d059`  
		Last Modified: Fri, 04 Dec 2020 01:29:03 GMT  
		Size: 8.5 MB (8499869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9fdec9db4728520c427e5ae86d67521591251e09a667e19f8e6d0419c50d24`  
		Last Modified: Fri, 04 Dec 2020 01:29:01 GMT  
		Size: 1.3 MB (1310181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96eec8ba730f3d05a0aac92b2d5d603ab21395ee6bd7cd3a0dcb0d80a1e4c96`  
		Last Modified: Fri, 04 Dec 2020 01:29:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:8ad160201c4f5ecf7844ef8865006660c67a29f3ded38b197e4d1ceac08966ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114386918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c06890463e50025481be858d0e654711df6c38fe2c7236f9c20dabbd7038590`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 13:27:26 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 13:27:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 13:27:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:56:29 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 01:58:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:58:26 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:58:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:58:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:58:38 GMT
WORKDIR /go
# Fri, 04 Dec 2020 03:13:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 03:13:32 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 03:13:36 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 03:13:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 03:13:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 03:13:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 03:14:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9900411dc7c8c88618743573bf89478d726007403bd002d8b00d21b7fecd40a`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 283.2 KB (283205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbd106374e3baf7eb8e3d8f7ffd4c364a35e57dcb3a89f8a153327a4c3fa3f9`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018c21191f366f1d0001ca2ec647fe3454179351700e264f9025f3efe636d5a2`  
		Last Modified: Fri, 04 Dec 2020 02:07:13 GMT  
		Size: 101.1 MB (101092006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b3c970f8c564da928ce32db5cc7981e5bc4819b99016458cf9f2ceda95aa31`  
		Last Modified: Fri, 04 Dec 2020 02:06:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6379430057b0313b2aa26fed01de99735afdc60ab9085d4a8660e5bbaa2b5595`  
		Last Modified: Fri, 04 Dec 2020 03:14:44 GMT  
		Size: 8.9 MB (8919986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71eeeb13c478d19d8ddd430419adba93210219538a556c2f13d6888de61b01d`  
		Last Modified: Fri, 04 Dec 2020 03:14:43 GMT  
		Size: 1.3 MB (1287788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b553b21761e1bd135a537841af7ef976560d1e74642f117e38ae3254ddf4eb9`  
		Last Modified: Fri, 04 Dec 2020 03:14:42 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:f52177d55e579fb060a4948c8ab350ec391cb66981aa3c19f6679b89bc11d21c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118805074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46e9b596fe9e786ef15184f4d52c8e67a630830ea348c7be3d5ffdbbe4519dba`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:53:28 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 02:53:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:53:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:43:59 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:45:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:45:26 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:45:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:45:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:45:28 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:07:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:07:54 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:07:54 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 01:07:54 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:07:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:07:56 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:07:56 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5139d7663b8674a989574c2161166fb137f26ef16b2f701159c126628be75101`  
		Last Modified: Thu, 22 Oct 2020 02:58:32 GMT  
		Size: 281.4 KB (281363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d31a06258ad66efe2dedbf67809ebc107a55757b8a4543af77982f55ff6c067`  
		Last Modified: Thu, 22 Oct 2020 02:58:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaad7db4ec01c554a618ebac1f61b959bccd70e3f8fc0785a59184f339aa86d3`  
		Last Modified: Fri, 04 Dec 2020 00:50:40 GMT  
		Size: 106.2 MB (106216195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b39947ffb8ce26e266d93d67e3f57f7809db37f576d55d81e2615141795de7`  
		Last Modified: Fri, 04 Dec 2020 00:50:26 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5794dec4cffbe160fd928ee6d98a33715cafe7ae3207a7fe00d667f02b3ddb9`  
		Last Modified: Fri, 04 Dec 2020 01:08:24 GMT  
		Size: 8.4 MB (8352221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9902eaeb6b923e986d4208b2672bd9b954eddcd687fbd6599bdd15a0f991fa93`  
		Last Modified: Fri, 04 Dec 2020 01:08:22 GMT  
		Size: 1.4 MB (1388750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c240f721a1a8d8fc37cfad83efafb1aa384fb0043d664639cfe0af964230f8`  
		Last Modified: Fri, 04 Dec 2020 01:08:22 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.1577; amd64

```console
$ docker pull caddy@sha256:1b4c71d3f63a5d9c7028f75729bd4e074594246b727128334e435b2a41c5b29f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2562830037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d09fa3868f18fb9bd00dcaaae39f70c15647ee55b70d3010a4cfcbfad3c064eb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 13:43:36 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Nov 2020 13:43:37 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Nov 2020 13:43:38 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Nov 2020 13:43:38 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Nov 2020 13:44:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 13:44:33 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Nov 2020 13:44:55 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Dec 2020 00:15:09 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:17:48 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Dec 2020 00:17:50 GMT
WORKDIR C:\gopath
# Fri, 04 Dec 2020 00:57:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Dec 2020 00:57:33 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:57:33 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:57:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:57:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Dec 2020 00:57:57 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19e00ae033e023d5973e57402eb3f05fe0908fa3f40cd0a36ae20bc72df3927`  
		Last Modified: Wed, 11 Nov 2020 14:08:35 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7f2350f21c33479862fe11c4c46ef7fc8054cb8e0acb2581b663d9e71d37f4`  
		Last Modified: Wed, 11 Nov 2020 14:08:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b816110035a14bde6916267f7e5f008617773d19d8f23f77597d10b021b787c`  
		Last Modified: Wed, 11 Nov 2020 14:08:30 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7a389242a4449d1ca90994817f199ce0b9ec502e46035e6ea9c78c29282ce8`  
		Last Modified: Wed, 11 Nov 2020 14:08:29 GMT  
		Size: 1.1 KB (1098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c993585709f02af194d96f01fb74b3158a083cac1cbf2036662bd0abab75e3bf`  
		Last Modified: Wed, 11 Nov 2020 14:08:38 GMT  
		Size: 34.3 MB (34333277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822a63153155fc14ab856f02664a39a3dbf45ef8601277d161d64e9475748111`  
		Last Modified: Wed, 11 Nov 2020 14:08:26 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758771af484f25fbbe9ef11107e3680d525f6bfc5a1666db73f0eb9d84be3ef1`  
		Last Modified: Wed, 11 Nov 2020 14:08:26 GMT  
		Size: 311.3 KB (311320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05164df22cc1044ebebf255e3f078aca1c5d0b01cfed997c4c52ac57268041e`  
		Last Modified: Fri, 04 Dec 2020 00:33:08 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d208cb88aaef7d49293e8b5fe6cb80e9520f49d127c6991f47c4a360628ef2`  
		Last Modified: Fri, 04 Dec 2020 00:33:47 GMT  
		Size: 138.4 MB (138372930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219a39d338a89418edc5b2a3e6949d4b7c9055ce4dac36812ee963d3454525ec`  
		Last Modified: Fri, 04 Dec 2020 00:33:08 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1991b3df8a0a87849ff8adb054c48ad26020037337edecf17239b67df9f893`  
		Last Modified: Fri, 04 Dec 2020 01:00:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0b12c4d6b7ca2ef8c70722895e566350e366cfef8befa849c5c8411d906ee3`  
		Last Modified: Fri, 04 Dec 2020 01:00:35 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21e20193de473a33dd040821d1d0c9b3b1ebbfc6613419a329bc10a69d70446`  
		Last Modified: Fri, 04 Dec 2020 01:00:34 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70e2aaadeededbaa5d5a0210375f6e763495d701d736cd1f1d43828b73f4b51`  
		Last Modified: Fri, 04 Dec 2020 01:00:35 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a92e145c6f6fc1ec4a2d2848f07d18ec1f37325a509d874a358a03df6527bad`  
		Last Modified: Fri, 04 Dec 2020 01:00:36 GMT  
		Size: 1.8 MB (1768395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b0df0a8c483f3ae7deb4e4b40fa21008023092e18794654eff3ed0187c7eaa`  
		Last Modified: Fri, 04 Dec 2020 01:00:35 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.14393.4046; amd64

```console
$ docker pull caddy@sha256:be0e7ff69ac06bf8741750f6e7c5660ca4e2db3a6f66b8108cd168840c9e20bb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5966466109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:988068fcd7e874d95af542fe45cb6d609b55c7186dca28b21a4336f0bc87e73e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 13:23:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 13:47:33 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Nov 2020 13:47:34 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Nov 2020 13:47:34 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Nov 2020 13:47:35 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Nov 2020 13:49:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 13:49:05 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Nov 2020 13:51:21 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Dec 2020 00:18:05 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:21:33 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Dec 2020 00:21:34 GMT
WORKDIR C:\gopath
# Fri, 04 Dec 2020 00:58:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Dec 2020 00:58:03 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:58:04 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:58:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:59:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Dec 2020 00:59:19 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:126d9a92c0cb7b68c56dec2dd5ba118de9dde3ec6368db734c5135fdf1528a33`  
		Last Modified: Wed, 11 Nov 2020 13:34:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48cdfe7c39f0358056c4c821593e466beab0dd18e49c8fae5aead3044dc4fcc`  
		Last Modified: Wed, 11 Nov 2020 14:09:26 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725a072d8cce622c524652fc146ce1398a73435bfe34b503ce6df7c2ba1954c5`  
		Last Modified: Wed, 11 Nov 2020 14:09:26 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff5342fb3e45a27028014ad657c3d05414fac6d9ea2e1213ac67ebd51c174f5`  
		Last Modified: Wed, 11 Nov 2020 14:09:23 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada6bdd6092185cd48a4b7a37d2fccf12a0598e2793361256a3658393e27de45`  
		Last Modified: Wed, 11 Nov 2020 14:09:22 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcaf43c793d08d3feb1cb8666a774e8709fd62cf468af1fcf7c3470bb777e5bc`  
		Last Modified: Wed, 11 Nov 2020 14:10:05 GMT  
		Size: 35.2 MB (35173627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e19e3e1a800738fb7127bdfaabdc86eb626a4b1ea386389bcc158ee6afcf2e8`  
		Last Modified: Wed, 11 Nov 2020 14:09:19 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8d4839ac80d0d8b637b35572732039f3c4bc755fbfa2ca871d32cf344c0032`  
		Last Modified: Wed, 11 Nov 2020 14:09:25 GMT  
		Size: 5.5 MB (5520399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d4de7953b3278a0185f6a1290763d910034fdd6a6ff612ba88e8cbe9d65316`  
		Last Modified: Fri, 04 Dec 2020 00:34:04 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98d400ad57d745f041190f63e7592642bd84fe503e52beb192ae33fe1a616dc`  
		Last Modified: Fri, 04 Dec 2020 00:34:34 GMT  
		Size: 143.7 MB (143715722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bc180fe611f0157f85450283f2e49a5ce41cea0896671a39bd2f636ae4e2a3`  
		Last Modified: Fri, 04 Dec 2020 00:34:05 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b42e7fb13992aa07e801901bcd8bd61a9dcda76fa6791d68c3bfb3eea1131ae`  
		Last Modified: Fri, 04 Dec 2020 01:00:58 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e814c85456355f9ccc653cc66261b55c1e5a54da713223c960ac9ec7b9e0b207`  
		Last Modified: Fri, 04 Dec 2020 01:00:54 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1b56b590c16755e3db6717e32d5dd0517ab2f6dc7f57419f0e1af7ac2a605e`  
		Last Modified: Fri, 04 Dec 2020 01:00:54 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8844c556721bdbecb70fe920a7c98338fe934a8570a1977bd7feb5554c5e821`  
		Last Modified: Fri, 04 Dec 2020 01:00:54 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247766b9da1eed45f517bad1aaeeccc1644d9672610f79700f35c47784cd7384`  
		Last Modified: Fri, 04 Dec 2020 01:00:58 GMT  
		Size: 11.5 MB (11482569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e585ac8b3a4bcaf593aba5ddb48833a65ee3df816033f13393c575baafd417e`  
		Last Modified: Fri, 04 Dec 2020 01:00:55 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:6296d8b40dadaa9bdfeba6b6bd67d6d499da9d30c38bea1dbc27ff01999d23ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:d7b066e0ae6a58162afa38de124bde6cafbcf0a7f4d056489ce88cc394471bed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119881414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d52e2ef96ee9bf6c12304aac59194314ca7a1e076d5904b34eac04d61337d964`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:34:56 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:34:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:34:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:21:55 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:24:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:24:09 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:24:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:24:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:24:10 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:49:11 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:49:12 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:49:12 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:49:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:49:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:49:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:49:15 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef7d3d256c8367c41c431143c63d083a25dd62ec9ee9d9773dd9e6c7b70ec9e`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 280.8 KB (280812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9db76c5a1d06710ed4f3073476b2d883ff8e911f8e47c558bc4a8d1d8663fa`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b5e3429cf30be490cdf3c5018e8693e0e1d319ea295c9b0c37dedaa7a1cafb`  
		Last Modified: Fri, 04 Dec 2020 00:31:08 GMT  
		Size: 107.1 MB (107085919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07aa6a0961518234df34a1cf391ec7269a68b99fc112f60e8a7270db07eb3974`  
		Last Modified: Fri, 04 Dec 2020 00:30:49 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fe1a6296183cbfcabe79353a47f9336d847b7ea66b4fb61ae86fc689de5d77`  
		Last Modified: Fri, 04 Dec 2020 00:49:47 GMT  
		Size: 8.3 MB (8309940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1da5ba704ae92109544c4683fde8e8be5eea27b6110540c808341c3b43145c6`  
		Last Modified: Fri, 04 Dec 2020 00:49:45 GMT  
		Size: 1.4 MB (1407200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572698d0ecf1dba5c0b8c6a996637e0de1f7e30e2901dae6927647fc8e0d63e7`  
		Last Modified: Fri, 04 Dec 2020 00:49:44 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:d6805920da89344546ce60bd4b91be62fa46da72cef37f871a07d829a0e6b39d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.1 MB (115088466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ad4d3264c7202d2a8117e3dd2a7c46d4164b1e58f8da8ab94016ec14fc9737b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:07:24 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:07:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:07:27 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:54:37 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:57:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:57:18 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:57:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:57:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:57:23 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:23:51 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:23:52 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:23:52 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 01:23:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:23:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:23:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:23:56 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20cc27a60e8ac1bf56dec787d3d52ba856e657179cfd56050036db79abb4267`  
		Last Modified: Thu, 22 Oct 2020 05:34:55 GMT  
		Size: 281.0 KB (280971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ecce92c3d2de40638d73e682dec26c2b79a055e85c8d70b88f4ccb9485bb9c9`  
		Last Modified: Thu, 22 Oct 2020 05:34:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcce644b45ccf744ed14c7b9273179dc1ad732ffa1bd944e61407793f983b983`  
		Last Modified: Fri, 04 Dec 2020 01:05:18 GMT  
		Size: 102.9 MB (102948648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909e21afe9abe4c8685162bb1ca820c4c1d140304436933b524bf4b048cdbc25`  
		Last Modified: Fri, 04 Dec 2020 01:04:48 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba23987bf60560a98e2e39c226cdf37070ca4f72a514be647528077fe286b3e`  
		Last Modified: Fri, 04 Dec 2020 01:24:26 GMT  
		Size: 7.9 MB (7928869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebe92d17d7243c87fc37008c3e65cbbe4b1b675ccaca7fd4760bc44d7bd7ea3`  
		Last Modified: Fri, 04 Dec 2020 01:24:23 GMT  
		Size: 1.3 MB (1327351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41a9e416157b507873d5b48a6159cf7d013314b857201f0d66921bab89875a1`  
		Last Modified: Fri, 04 Dec 2020 01:24:23 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:bd9531e4414b412e4a1bdb2fbe16e0c83e38c8d058aaa93a6a40245cfd5c8f05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.9 MB (113880893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3158c399bfa2628c5054f9d4e14c2dd225c2b4a45b8130026e462667ba683ce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:21:35 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:23:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:23:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:03:17 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:05:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:05:41 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:05:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:05:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:05:44 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:33:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:33:33 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:33:34 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:33:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:33:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:33:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:33:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b753cfc04fdce9640aac1e7a4b3e7ce15fa60b8e357376e42f294f463a6e890`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 280.1 KB (280084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e90c422e5e4668cb4140aadb622d734faa93c81cc1e283da9b08bbbc65c45c5`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c37b023a65a717d26fdb8c72bba66adc8625ca96fab4d08e70954da6b10139`  
		Last Modified: Fri, 04 Dec 2020 00:14:22 GMT  
		Size: 102.7 MB (102723691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f091034d1629ecd6c35f9bbcb2754721bbfa4e5183794ff2b6ecc75b7b2e0e`  
		Last Modified: Fri, 04 Dec 2020 00:13:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6809b32049841fc890dd29c935db10e86e95c4005906b5eddc3fa42f131cdb5`  
		Last Modified: Fri, 04 Dec 2020 00:34:08 GMT  
		Size: 7.1 MB (7144891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818ba8d461e1618211000580b6f229d2fd9775115c3c4049fb7be235094e0625`  
		Last Modified: Fri, 04 Dec 2020 00:34:07 GMT  
		Size: 1.3 MB (1325838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af262af67e01cb4ef945fd8c992860308e9509dc4810d2cab9ed6955b52a700`  
		Last Modified: Fri, 04 Dec 2020 00:34:07 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:3bd8e226aa9f4fef563f2a76b0c165434ab3145a2b629512dcab6495c677202c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115210346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d5e537fc1b6fe653ff07e33f1a30ba036846e07eb585a5a75815eeabb89e21f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:08:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 04:09:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 04:09:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:59:20 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 01:01:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:01:23 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:01:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:01:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:01:29 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:28:26 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:28:27 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:28:28 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 01:28:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:28:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:28:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:28:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4357932f1b6fb010e1461cc5c673712fb832ac44ee627c691db0b64adf95d13`  
		Last Modified: Thu, 22 Oct 2020 04:28:32 GMT  
		Size: 281.2 KB (281230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c013af1878066e59b688e31fd962e7267430963de27c5257241e3c223aa1d6`  
		Last Modified: Thu, 22 Oct 2020 04:28:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37128a32d7b17416d88331ec94958c63f643120f6e40870110ef00f387be80e5`  
		Last Modified: Fri, 04 Dec 2020 01:09:15 GMT  
		Size: 102.4 MB (102411796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0279cf9b51b6c7d1d4937560cb5536f262e9f4e9c5a1685489387c9753062e04`  
		Last Modified: Fri, 04 Dec 2020 01:08:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed38fb55682cdaae259822fc0a1e349a7992f9f99404e4bdc58b4bee6e75d059`  
		Last Modified: Fri, 04 Dec 2020 01:29:03 GMT  
		Size: 8.5 MB (8499869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9fdec9db4728520c427e5ae86d67521591251e09a667e19f8e6d0419c50d24`  
		Last Modified: Fri, 04 Dec 2020 01:29:01 GMT  
		Size: 1.3 MB (1310181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96eec8ba730f3d05a0aac92b2d5d603ab21395ee6bd7cd3a0dcb0d80a1e4c96`  
		Last Modified: Fri, 04 Dec 2020 01:29:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:8ad160201c4f5ecf7844ef8865006660c67a29f3ded38b197e4d1ceac08966ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114386918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c06890463e50025481be858d0e654711df6c38fe2c7236f9c20dabbd7038590`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 13:27:26 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 13:27:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 13:27:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:56:29 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 01:58:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:58:26 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:58:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:58:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:58:38 GMT
WORKDIR /go
# Fri, 04 Dec 2020 03:13:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 03:13:32 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 03:13:36 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 03:13:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 03:13:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 03:13:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 03:14:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9900411dc7c8c88618743573bf89478d726007403bd002d8b00d21b7fecd40a`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 283.2 KB (283205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbd106374e3baf7eb8e3d8f7ffd4c364a35e57dcb3a89f8a153327a4c3fa3f9`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018c21191f366f1d0001ca2ec647fe3454179351700e264f9025f3efe636d5a2`  
		Last Modified: Fri, 04 Dec 2020 02:07:13 GMT  
		Size: 101.1 MB (101092006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b3c970f8c564da928ce32db5cc7981e5bc4819b99016458cf9f2ceda95aa31`  
		Last Modified: Fri, 04 Dec 2020 02:06:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6379430057b0313b2aa26fed01de99735afdc60ab9085d4a8660e5bbaa2b5595`  
		Last Modified: Fri, 04 Dec 2020 03:14:44 GMT  
		Size: 8.9 MB (8919986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71eeeb13c478d19d8ddd430419adba93210219538a556c2f13d6888de61b01d`  
		Last Modified: Fri, 04 Dec 2020 03:14:43 GMT  
		Size: 1.3 MB (1287788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b553b21761e1bd135a537841af7ef976560d1e74642f117e38ae3254ddf4eb9`  
		Last Modified: Fri, 04 Dec 2020 03:14:42 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:f52177d55e579fb060a4948c8ab350ec391cb66981aa3c19f6679b89bc11d21c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118805074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46e9b596fe9e786ef15184f4d52c8e67a630830ea348c7be3d5ffdbbe4519dba`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:53:28 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 02:53:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:53:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:43:59 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:45:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:45:26 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:45:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:45:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:45:28 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:07:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:07:54 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:07:54 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 01:07:54 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:07:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:07:56 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:07:56 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5139d7663b8674a989574c2161166fb137f26ef16b2f701159c126628be75101`  
		Last Modified: Thu, 22 Oct 2020 02:58:32 GMT  
		Size: 281.4 KB (281363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d31a06258ad66efe2dedbf67809ebc107a55757b8a4543af77982f55ff6c067`  
		Last Modified: Thu, 22 Oct 2020 02:58:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaad7db4ec01c554a618ebac1f61b959bccd70e3f8fc0785a59184f339aa86d3`  
		Last Modified: Fri, 04 Dec 2020 00:50:40 GMT  
		Size: 106.2 MB (106216195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b39947ffb8ce26e266d93d67e3f57f7809db37f576d55d81e2615141795de7`  
		Last Modified: Fri, 04 Dec 2020 00:50:26 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5794dec4cffbe160fd928ee6d98a33715cafe7ae3207a7fe00d667f02b3ddb9`  
		Last Modified: Fri, 04 Dec 2020 01:08:24 GMT  
		Size: 8.4 MB (8352221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9902eaeb6b923e986d4208b2672bd9b954eddcd687fbd6599bdd15a0f991fa93`  
		Last Modified: Fri, 04 Dec 2020 01:08:22 GMT  
		Size: 1.4 MB (1388750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c240f721a1a8d8fc37cfad83efafb1aa384fb0043d664639cfe0af964230f8`  
		Last Modified: Fri, 04 Dec 2020 01:08:22 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:c1be9c3404f3bbfc27d368ff0dce5e7a279260fec6705f96e6cdfea4854b4dde
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull caddy@sha256:1b4c71d3f63a5d9c7028f75729bd4e074594246b727128334e435b2a41c5b29f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2562830037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d09fa3868f18fb9bd00dcaaae39f70c15647ee55b70d3010a4cfcbfad3c064eb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 13:43:36 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Nov 2020 13:43:37 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Nov 2020 13:43:38 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Nov 2020 13:43:38 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Nov 2020 13:44:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 13:44:33 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Nov 2020 13:44:55 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Dec 2020 00:15:09 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:17:48 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Dec 2020 00:17:50 GMT
WORKDIR C:\gopath
# Fri, 04 Dec 2020 00:57:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Dec 2020 00:57:33 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:57:33 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:57:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:57:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Dec 2020 00:57:57 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19e00ae033e023d5973e57402eb3f05fe0908fa3f40cd0a36ae20bc72df3927`  
		Last Modified: Wed, 11 Nov 2020 14:08:35 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7f2350f21c33479862fe11c4c46ef7fc8054cb8e0acb2581b663d9e71d37f4`  
		Last Modified: Wed, 11 Nov 2020 14:08:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b816110035a14bde6916267f7e5f008617773d19d8f23f77597d10b021b787c`  
		Last Modified: Wed, 11 Nov 2020 14:08:30 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7a389242a4449d1ca90994817f199ce0b9ec502e46035e6ea9c78c29282ce8`  
		Last Modified: Wed, 11 Nov 2020 14:08:29 GMT  
		Size: 1.1 KB (1098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c993585709f02af194d96f01fb74b3158a083cac1cbf2036662bd0abab75e3bf`  
		Last Modified: Wed, 11 Nov 2020 14:08:38 GMT  
		Size: 34.3 MB (34333277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822a63153155fc14ab856f02664a39a3dbf45ef8601277d161d64e9475748111`  
		Last Modified: Wed, 11 Nov 2020 14:08:26 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758771af484f25fbbe9ef11107e3680d525f6bfc5a1666db73f0eb9d84be3ef1`  
		Last Modified: Wed, 11 Nov 2020 14:08:26 GMT  
		Size: 311.3 KB (311320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05164df22cc1044ebebf255e3f078aca1c5d0b01cfed997c4c52ac57268041e`  
		Last Modified: Fri, 04 Dec 2020 00:33:08 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d208cb88aaef7d49293e8b5fe6cb80e9520f49d127c6991f47c4a360628ef2`  
		Last Modified: Fri, 04 Dec 2020 00:33:47 GMT  
		Size: 138.4 MB (138372930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219a39d338a89418edc5b2a3e6949d4b7c9055ce4dac36812ee963d3454525ec`  
		Last Modified: Fri, 04 Dec 2020 00:33:08 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1991b3df8a0a87849ff8adb054c48ad26020037337edecf17239b67df9f893`  
		Last Modified: Fri, 04 Dec 2020 01:00:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0b12c4d6b7ca2ef8c70722895e566350e366cfef8befa849c5c8411d906ee3`  
		Last Modified: Fri, 04 Dec 2020 01:00:35 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21e20193de473a33dd040821d1d0c9b3b1ebbfc6613419a329bc10a69d70446`  
		Last Modified: Fri, 04 Dec 2020 01:00:34 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70e2aaadeededbaa5d5a0210375f6e763495d701d736cd1f1d43828b73f4b51`  
		Last Modified: Fri, 04 Dec 2020 01:00:35 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a92e145c6f6fc1ec4a2d2848f07d18ec1f37325a509d874a358a03df6527bad`  
		Last Modified: Fri, 04 Dec 2020 01:00:36 GMT  
		Size: 1.8 MB (1768395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b0df0a8c483f3ae7deb4e4b40fa21008023092e18794654eff3ed0187c7eaa`  
		Last Modified: Fri, 04 Dec 2020 01:00:35 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:6db0a189d7bf711b05b117f6ebc582b950dd1786574b3fa36cec30140ed6fdc1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64

### `caddy:builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4046; amd64

```console
$ docker pull caddy@sha256:be0e7ff69ac06bf8741750f6e7c5660ca4e2db3a6f66b8108cd168840c9e20bb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5966466109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:988068fcd7e874d95af542fe45cb6d609b55c7186dca28b21a4336f0bc87e73e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 13:23:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 13:47:33 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Nov 2020 13:47:34 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Nov 2020 13:47:34 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Nov 2020 13:47:35 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Nov 2020 13:49:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 13:49:05 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Nov 2020 13:51:21 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Dec 2020 00:18:05 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:21:33 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Dec 2020 00:21:34 GMT
WORKDIR C:\gopath
# Fri, 04 Dec 2020 00:58:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Dec 2020 00:58:03 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:58:04 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:58:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:59:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Dec 2020 00:59:19 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:126d9a92c0cb7b68c56dec2dd5ba118de9dde3ec6368db734c5135fdf1528a33`  
		Last Modified: Wed, 11 Nov 2020 13:34:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48cdfe7c39f0358056c4c821593e466beab0dd18e49c8fae5aead3044dc4fcc`  
		Last Modified: Wed, 11 Nov 2020 14:09:26 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725a072d8cce622c524652fc146ce1398a73435bfe34b503ce6df7c2ba1954c5`  
		Last Modified: Wed, 11 Nov 2020 14:09:26 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff5342fb3e45a27028014ad657c3d05414fac6d9ea2e1213ac67ebd51c174f5`  
		Last Modified: Wed, 11 Nov 2020 14:09:23 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada6bdd6092185cd48a4b7a37d2fccf12a0598e2793361256a3658393e27de45`  
		Last Modified: Wed, 11 Nov 2020 14:09:22 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcaf43c793d08d3feb1cb8666a774e8709fd62cf468af1fcf7c3470bb777e5bc`  
		Last Modified: Wed, 11 Nov 2020 14:10:05 GMT  
		Size: 35.2 MB (35173627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e19e3e1a800738fb7127bdfaabdc86eb626a4b1ea386389bcc158ee6afcf2e8`  
		Last Modified: Wed, 11 Nov 2020 14:09:19 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8d4839ac80d0d8b637b35572732039f3c4bc755fbfa2ca871d32cf344c0032`  
		Last Modified: Wed, 11 Nov 2020 14:09:25 GMT  
		Size: 5.5 MB (5520399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d4de7953b3278a0185f6a1290763d910034fdd6a6ff612ba88e8cbe9d65316`  
		Last Modified: Fri, 04 Dec 2020 00:34:04 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98d400ad57d745f041190f63e7592642bd84fe503e52beb192ae33fe1a616dc`  
		Last Modified: Fri, 04 Dec 2020 00:34:34 GMT  
		Size: 143.7 MB (143715722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bc180fe611f0157f85450283f2e49a5ce41cea0896671a39bd2f636ae4e2a3`  
		Last Modified: Fri, 04 Dec 2020 00:34:05 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b42e7fb13992aa07e801901bcd8bd61a9dcda76fa6791d68c3bfb3eea1131ae`  
		Last Modified: Fri, 04 Dec 2020 01:00:58 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e814c85456355f9ccc653cc66261b55c1e5a54da713223c960ac9ec7b9e0b207`  
		Last Modified: Fri, 04 Dec 2020 01:00:54 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1b56b590c16755e3db6717e32d5dd0517ab2f6dc7f57419f0e1af7ac2a605e`  
		Last Modified: Fri, 04 Dec 2020 01:00:54 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8844c556721bdbecb70fe920a7c98338fe934a8570a1977bd7feb5554c5e821`  
		Last Modified: Fri, 04 Dec 2020 01:00:54 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247766b9da1eed45f517bad1aaeeccc1644d9672610f79700f35c47784cd7384`  
		Last Modified: Fri, 04 Dec 2020 01:00:58 GMT  
		Size: 11.5 MB (11482569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e585ac8b3a4bcaf593aba5ddb48833a65ee3df816033f13393c575baafd417e`  
		Last Modified: Fri, 04 Dec 2020 01:00:55 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:e46050590a9ac1a411b5da0349f735b5977e9dcbe6ab91e9a95c9a731533aba8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1577; amd64
	-	windows version 10.0.14393.4046; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:4ebad49f78a3f98164d89431978046ee6e94f1e8a70454abc7f49ce1a5ee7826
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14635232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bb0137bab0e21a92b0bc9ec1cc22c259b097d5bf239b161ae1eac0de1833e67`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:33:22 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 04:33:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 04:33:55 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 04:33:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 04:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 04:34:01 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 04:34:01 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 04:34:01 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 04:34:02 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 04:34:02 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 04:34:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 04:34:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 04:34:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 04:34:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 04:34:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 04:34:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 04:34:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 04:34:05 GMT
EXPOSE 80
# Thu, 22 Oct 2020 04:34:05 GMT
EXPOSE 443
# Thu, 22 Oct 2020 04:34:06 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 04:34:06 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 04:34:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2e2d825895b6421ca5dbd63db0d99f790ef84a84c7bcaff51e60b654397858`  
		Last Modified: Thu, 22 Oct 2020 04:34:47 GMT  
		Size: 300.0 KB (299956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaf2e3dee2e74b401fce928bf9502e48df68da4e8c1933bfd6b00b1137529fc`  
		Last Modified: Thu, 22 Oct 2020 04:35:02 GMT  
		Size: 5.8 KB (5754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2215cf93250599c5db984cee0fddd5d0cd59ef035ab5a317387b67211bde86d`  
		Last Modified: Thu, 22 Oct 2020 04:35:06 GMT  
		Size: 11.5 MB (11532508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060365e49ba5ee96a2859e269b366f5a5c9f386e5bdbf07d2ef31b1fc6934baa`  
		Last Modified: Thu, 22 Oct 2020 04:35:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:abba73dc860b2f35703cb7d27f08baf5bfc084e18e627b94661d01a8e2befdaf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13784259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f0aad5a281913821dd39ffed5e144daae22ac81ac4314731395ab65eedde72a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:58:10 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 02:58:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 02:58:46 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 02:58:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 02:58:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:59:00 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 02:59:01 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 02:59:01 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 02:59:03 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 02:59:08 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 02:59:09 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 02:59:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 02:59:11 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 02:59:11 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 02:59:12 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 02:59:13 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 02:59:14 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 02:59:15 GMT
EXPOSE 80
# Thu, 22 Oct 2020 02:59:19 GMT
EXPOSE 443
# Thu, 22 Oct 2020 02:59:20 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 02:59:21 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 02:59:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7369c3ac4b39c55c74e96dd3eb61ac2fa65e5671b1c2acca9697a7c9d20c3cf`  
		Last Modified: Thu, 22 Oct 2020 02:59:49 GMT  
		Size: 300.1 KB (300086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8f4045920069dff3382a5993783c5d846d9e28d0f5a63c475ed298fce0abb7`  
		Last Modified: Thu, 22 Oct 2020 03:00:03 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db6bde4735da15e5db23ad62f3d64d78aed8713a40d12547f5538c15c90f9da`  
		Last Modified: Thu, 22 Oct 2020 03:00:06 GMT  
		Size: 10.9 MB (10876280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a95efd7a14ed98a53a238da45faa7e3b0fdd2a93529b83bfe9d0823dafac67c`  
		Last Modified: Thu, 22 Oct 2020 03:00:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:8cf66cbe3c03273ca54bdab908092a6a9b9f02d39595ed15b1111f1465430426
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13565251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b20723dea614fc40d9f3cb59eddd33bf0e89dfda3f8ed4a7b404ef334632a4b9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:04:57 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 03:05:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 03:05:45 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 03:05:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 03:05:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:05:53 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 03:05:53 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 03:05:54 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 03:05:55 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 03:05:56 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 03:05:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 03:05:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 03:05:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 03:05:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 03:05:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 03:06:00 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 03:06:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 03:06:01 GMT
EXPOSE 80
# Thu, 22 Oct 2020 03:06:02 GMT
EXPOSE 443
# Thu, 22 Oct 2020 03:06:02 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 03:06:03 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 03:06:04 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a8e7fe5034ac502626b0a921d79be80c092890176e33b236c489d6f00710a2`  
		Last Modified: Thu, 22 Oct 2020 03:06:32 GMT  
		Size: 299.2 KB (299211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14db75acdaca15b1e81890f29b3b757fcc73e7a69a55f5ed659bf800f6340108`  
		Last Modified: Thu, 22 Oct 2020 03:06:43 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2197c38adf245bca8f229a4cd718c4d0f619a87bae5786572ccdac1a286882c`  
		Last Modified: Thu, 22 Oct 2020 03:06:46 GMT  
		Size: 10.9 MB (10854384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0104bc6a595940856019d00d9ff8e04365338a7964d948b64cc44bf73cc59e`  
		Last Modified: Thu, 22 Oct 2020 03:06:42 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:da121cf42d1759ed03af3130533d365c365af1d738d550744ad863e05e64cf46
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13540356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89b4aa38988ab2442575062d99c3cb44976de6c227256c118f35340e7c21c303`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:40:04 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 02:40:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 02:40:57 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 02:41:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 02:41:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:41:07 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 02:41:08 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 02:41:09 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 02:41:10 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 02:41:10 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 02:41:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 02:41:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 02:41:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 02:41:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 02:41:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 02:41:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 02:41:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 02:41:19 GMT
EXPOSE 80
# Thu, 22 Oct 2020 02:41:20 GMT
EXPOSE 443
# Thu, 22 Oct 2020 02:41:20 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 02:41:21 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 02:41:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dbde357077a97c0f831033bf03c9828203cb7e3e6cb33217ce4d7cfd71c931`  
		Last Modified: Thu, 22 Oct 2020 02:41:47 GMT  
		Size: 300.3 KB (300348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a5ab0aa923ce1fe233b904008bbf932c4787f48bcd59f07a85616147b7cbc3`  
		Last Modified: Thu, 22 Oct 2020 02:41:56 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc398339860cf826624c9c22b5de9b45a193260e2ff24826d210b493483398f`  
		Last Modified: Thu, 22 Oct 2020 02:41:59 GMT  
		Size: 10.5 MB (10527465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6e7d61d1d4a00550447ea1f67edc0463cc527e49356e98959edfafba0df879`  
		Last Modified: Thu, 22 Oct 2020 02:41:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:09208042b4d19d7ed87b51b99dc20b390dab20d9ae7e235a62a3af3aaf472bd5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13291756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe5c77284adc35481d13003d31a866f637b6eaf9f5764f667e536db79ce23129`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 13:39:52 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 13:44:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 13:44:04 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 13:44:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 13:44:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 13:44:33 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 13:44:37 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 13:44:40 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 13:44:44 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 13:44:48 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 13:44:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 13:44:56 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 13:45:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 13:45:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 13:45:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 13:45:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 13:45:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 13:45:23 GMT
EXPOSE 80
# Thu, 22 Oct 2020 13:45:26 GMT
EXPOSE 443
# Thu, 22 Oct 2020 13:45:30 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 13:45:35 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 13:45:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649a4964211b7ce86541a0c1dad8ef3800ec38a3ca90aff94b76759b4cb8e279`  
		Last Modified: Thu, 22 Oct 2020 13:47:22 GMT  
		Size: 302.3 KB (302327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58dd938ef3e3eae8509deda8fab9ab5f9344169d912e35a802633e799feed1bb`  
		Last Modified: Thu, 22 Oct 2020 13:47:52 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe23c296ee12ee12ef84dbabbb4f7bf0362a9a12b684782ebd3f44a97c8fcf8e`  
		Last Modified: Thu, 22 Oct 2020 13:47:55 GMT  
		Size: 10.2 MB (10180223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d2f3c084745fecafaa9ff33626a81124f2d70267ceee705da555714238bfa1`  
		Last Modified: Thu, 22 Oct 2020 13:47:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:3e18b421d651721239cb3422bc890d1211535681219b7696816f487b4cebc4ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14074857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4d5562f1d148d3d67ff7f5995be8f860553ad0f3d07091335643306b83385e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:41:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 02:41:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 02:41:31 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 02:41:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 02:41:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:41:36 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 02:41:36 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 02:41:37 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 02:41:37 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 02:41:37 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 02:41:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 02:41:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 02:41:38 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 02:41:38 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 02:41:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 02:41:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 02:41:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 02:41:40 GMT
EXPOSE 80
# Thu, 22 Oct 2020 02:41:40 GMT
EXPOSE 443
# Thu, 22 Oct 2020 02:41:40 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 02:41:41 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 02:41:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f988ff23f3cbb35bfed69e33f3b7ee69403bfae4f46363a08eea4830053e9c`  
		Last Modified: Thu, 22 Oct 2020 02:42:01 GMT  
		Size: 300.5 KB (300481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd6a4e0db99510879c5dfceabd1e629a0692c4544bb0da34971f8722b881e92`  
		Last Modified: Thu, 22 Oct 2020 02:42:09 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e13b938aa802e74610585cabba77d625db4baf219f577a81195c272408c7d3`  
		Last Modified: Thu, 22 Oct 2020 02:42:16 GMT  
		Size: 11.2 MB (11202559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a221fff082950a8a98db12eb99f532a39008f0d6e21684bc1aed06fa1ed2a764`  
		Last Modified: Thu, 22 Oct 2020 02:42:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.1577; amd64

```console
$ docker pull caddy@sha256:dad45b6df45cf6f4c45f010c391544a830a6372847bb2504a23a870eb9e96638
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2413941176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61f3df5163746a4530d03a8bc80f3b1318d935f9f1b3e26f00a31af891a9ba86`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 20:53:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Nov 2020 20:53:31 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 11 Nov 2020 20:54:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Nov 2020 20:54:04 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Nov 2020 20:54:04 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Nov 2020 20:54:05 GMT
VOLUME [c:/config]
# Wed, 11 Nov 2020 20:54:06 GMT
VOLUME [c:/data]
# Wed, 11 Nov 2020 20:54:07 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 11 Nov 2020 20:54:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Nov 2020 20:54:09 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Nov 2020 20:54:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Nov 2020 20:54:11 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Nov 2020 20:54:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Nov 2020 20:54:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Nov 2020 20:54:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Nov 2020 20:54:13 GMT
EXPOSE 80
# Wed, 11 Nov 2020 20:54:14 GMT
EXPOSE 443
# Wed, 11 Nov 2020 20:54:14 GMT
EXPOSE 2019
# Wed, 11 Nov 2020 20:54:30 GMT
RUN caddy version
# Wed, 11 Nov 2020 20:54:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01dcdd0030882c54a82d0a279a4099081c604810ccccb17d3d7c04a2057bf657`  
		Last Modified: Wed, 11 Nov 2020 21:02:39 GMT  
		Size: 9.2 MB (9248045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3be730f5a5cc9d1dd7080908242b9ed33ba6541e7120addf14e416b944b577`  
		Last Modified: Wed, 11 Nov 2020 21:02:36 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d70ac9fb0285fe6670a558e9c1da67b5594dd483872376ac91425a3058f95b9`  
		Last Modified: Wed, 11 Nov 2020 21:02:54 GMT  
		Size: 16.3 MB (16343997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72340d1f03d76debdf2a014ab06bbd3bc5cb1e8358520912f0c9f71f2b4a6ea`  
		Last Modified: Wed, 11 Nov 2020 21:02:34 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ae7bc4f9eb3af2fa576dd096f9992ad2cfc8a2e9aad0af79e1ebf11c95065d`  
		Last Modified: Wed, 11 Nov 2020 21:02:33 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46832c7bcb0b053968836644798024f37cfede18aaac00abed0c1571fbeeca4c`  
		Last Modified: Wed, 11 Nov 2020 21:02:33 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdafb0d35a00870fdb93efde60b2d5c002b5ec117bb07526ec1d744787529f58`  
		Last Modified: Wed, 11 Nov 2020 21:02:31 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af235cb3a2a159b44c6b773e30cbd6f7931055fb7cfed2aee403c9197e0defc`  
		Last Modified: Wed, 11 Nov 2020 21:02:32 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493ee2907458eb7d47b217b59e2f23b4dd4a6974a36a70462fa54e5b9201f26b`  
		Last Modified: Wed, 11 Nov 2020 21:02:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2f8b9a7de64bd747e2afbc20e6ca964b00d3b48ccdb9245e162300a5ef9b44`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc59b5cb8ee3554d8e4971222e0208e7b6dd831b33894abeba76400bbcb7d56`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c88104f4e1fc6125880b248f3e1edcc5cbf3daf73aaf26bf3782972f11203c3`  
		Last Modified: Wed, 11 Nov 2020 21:02:30 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7cb21eb1cd8ca039940f462fdfe3348c877262adbbc5891cdbc3601ffa2649`  
		Last Modified: Wed, 11 Nov 2020 21:02:27 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef21802812d7f9ad5dcebb2efbf8d4831fcdf5b024bac00c22d04e7406a420b`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed806482965bf605e395b83f00ba44639cc1c88b1b8ec7c75bb708d9c031610`  
		Last Modified: Wed, 11 Nov 2020 21:02:24 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee097b51db8b06f6e93d48da3e914d6a598b32681fdf27785279f3f5dbb5796`  
		Last Modified: Wed, 11 Nov 2020 21:02:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf5349d69a690d25aa14a10fab1fc6e7a82ec345bae9e1a01a4dfd95f09cd1b`  
		Last Modified: Wed, 11 Nov 2020 21:02:22 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0b5aa8db0e75c1ef349905a29ef299882814b7937d14753d2e6a972f7b13b1`  
		Last Modified: Wed, 11 Nov 2020 21:02:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cac55d84f022bb91b78bfb339492198e3fa96a7d1e25c1f8e09ad648376d45d`  
		Last Modified: Wed, 11 Nov 2020 21:02:21 GMT  
		Size: 299.3 KB (299301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7476d855c257a4a27ce525860567dd9bd67e74abb01c0fd1b334444ffaa8504c`  
		Last Modified: Wed, 11 Nov 2020 21:02:24 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.14393.4046; amd64

```console
$ docker pull caddy@sha256:405a17b713c3f1517124a2506ac9b4ed33285819013417e6b90fb2aa07cb0bd6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5802615067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:371225d0afbf64a113a3745e99535e2e17239829f4e36d99aa36e7aee3be9efc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 13:23:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 20:56:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Nov 2020 20:56:05 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 11 Nov 2020 20:57:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Nov 2020 20:57:25 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Nov 2020 20:57:26 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Nov 2020 20:57:28 GMT
VOLUME [c:/config]
# Wed, 11 Nov 2020 20:57:29 GMT
VOLUME [c:/data]
# Wed, 11 Nov 2020 20:57:30 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 11 Nov 2020 20:57:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Nov 2020 20:57:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Nov 2020 20:57:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Nov 2020 20:57:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Nov 2020 20:57:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Nov 2020 20:57:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Nov 2020 20:57:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Nov 2020 20:57:35 GMT
EXPOSE 80
# Wed, 11 Nov 2020 20:57:36 GMT
EXPOSE 443
# Wed, 11 Nov 2020 20:57:37 GMT
EXPOSE 2019
# Wed, 11 Nov 2020 20:58:18 GMT
RUN caddy version
# Wed, 11 Nov 2020 20:58:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:126d9a92c0cb7b68c56dec2dd5ba118de9dde3ec6368db734c5135fdf1528a33`  
		Last Modified: Wed, 11 Nov 2020 13:34:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5595cf12db880fdffb7bc7e0ceef81a68e0766ff34fdc357635566a05b60085`  
		Last Modified: Wed, 11 Nov 2020 21:03:35 GMT  
		Size: 10.1 MB (10089893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47fc9d917c611e97ffa642af414764e4712d012a3b2c10700a357a771d58bf3`  
		Last Modified: Wed, 11 Nov 2020 21:03:24 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2b332d20177fb217e2744454885bba6eb94e9c7512c35bef53cf1222f10b3a`  
		Last Modified: Wed, 11 Nov 2020 21:03:50 GMT  
		Size: 21.7 MB (21694741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061740784584c807be44f52e632b6fcafa7893cab07ca93723103ca41e759cd2`  
		Last Modified: Wed, 11 Nov 2020 21:03:23 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a051df7f978fd750beb5e55b7a7da2d50550a52c97baf897cd3452347196147`  
		Last Modified: Wed, 11 Nov 2020 21:03:23 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94db8d6fb716d4c43b34e09a05176f94701accb480ce613c231d70ef23c649b`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eeb5cfdcdca36082954b3510135aea31966da19679b9cc7d8d4e43a3892f2f5`  
		Last Modified: Wed, 11 Nov 2020 21:03:19 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50cc11877f41dad7cb21c9e61379268e564a03b044ec4cfb124cccd267ef551c`  
		Last Modified: Wed, 11 Nov 2020 21:03:21 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9914893b848ce6d71a6f99575e794219e1603afe1dcee2bcbf69f3a41451ab05`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab52b473d299810d7e49b3d9d98db42e6aa57e5426b79f4cd7f68fd766a8a9b`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3333f590132f229c9979af102fd15c4a5958d9e3d94d50632eeb045c14028ac1`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12c4e6df6d5faa8f29b56e44eb52dc65c9d6795322a0e6d743a9d373f97adf9`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a015ed900b4c4b4d23631449b68473b1e31eda520fa22c7c19a845ac6f133f31`  
		Last Modified: Wed, 11 Nov 2020 21:03:16 GMT  
		Size: 1.1 KB (1069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f354d2a4fb61ae55364b2ae298552e22165583c076c39e05707e906633b8a2`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc11e1af39f958f492359f3242aa5205230791b166e14ab2f94067e9999464e`  
		Last Modified: Wed, 11 Nov 2020 21:03:16 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a4e622ed285e795cc2fd731f38022c2e6ca478f2223fb9fcafe0a61b5e969`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f936683e767d2733a4a898519ce7c8bc6a608fede4e7cc04c41b5fed180287`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b4fbe6665c83c229d90ec42acce959b356dbf1a97ca281604625a29d8437133`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6966c1a2733b248361e0fbafefb3b58805b223ef954ced160cb1ca7f239c25`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 251.9 KB (251913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3d08972458dc80b8c379340207e2cfeee9ea33d9e9e405ebbf52421ef16dd5`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:f89d8c6aed62c51f8b74d1f7d4512f6a16ffde44052f047d9df284b02996413a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64
	-	windows version 10.0.14393.4046; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.1577; amd64

```console
$ docker pull caddy@sha256:dad45b6df45cf6f4c45f010c391544a830a6372847bb2504a23a870eb9e96638
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2413941176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61f3df5163746a4530d03a8bc80f3b1318d935f9f1b3e26f00a31af891a9ba86`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 20:53:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Nov 2020 20:53:31 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 11 Nov 2020 20:54:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Nov 2020 20:54:04 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Nov 2020 20:54:04 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Nov 2020 20:54:05 GMT
VOLUME [c:/config]
# Wed, 11 Nov 2020 20:54:06 GMT
VOLUME [c:/data]
# Wed, 11 Nov 2020 20:54:07 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 11 Nov 2020 20:54:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Nov 2020 20:54:09 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Nov 2020 20:54:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Nov 2020 20:54:11 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Nov 2020 20:54:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Nov 2020 20:54:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Nov 2020 20:54:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Nov 2020 20:54:13 GMT
EXPOSE 80
# Wed, 11 Nov 2020 20:54:14 GMT
EXPOSE 443
# Wed, 11 Nov 2020 20:54:14 GMT
EXPOSE 2019
# Wed, 11 Nov 2020 20:54:30 GMT
RUN caddy version
# Wed, 11 Nov 2020 20:54:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01dcdd0030882c54a82d0a279a4099081c604810ccccb17d3d7c04a2057bf657`  
		Last Modified: Wed, 11 Nov 2020 21:02:39 GMT  
		Size: 9.2 MB (9248045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3be730f5a5cc9d1dd7080908242b9ed33ba6541e7120addf14e416b944b577`  
		Last Modified: Wed, 11 Nov 2020 21:02:36 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d70ac9fb0285fe6670a558e9c1da67b5594dd483872376ac91425a3058f95b9`  
		Last Modified: Wed, 11 Nov 2020 21:02:54 GMT  
		Size: 16.3 MB (16343997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72340d1f03d76debdf2a014ab06bbd3bc5cb1e8358520912f0c9f71f2b4a6ea`  
		Last Modified: Wed, 11 Nov 2020 21:02:34 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ae7bc4f9eb3af2fa576dd096f9992ad2cfc8a2e9aad0af79e1ebf11c95065d`  
		Last Modified: Wed, 11 Nov 2020 21:02:33 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46832c7bcb0b053968836644798024f37cfede18aaac00abed0c1571fbeeca4c`  
		Last Modified: Wed, 11 Nov 2020 21:02:33 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdafb0d35a00870fdb93efde60b2d5c002b5ec117bb07526ec1d744787529f58`  
		Last Modified: Wed, 11 Nov 2020 21:02:31 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af235cb3a2a159b44c6b773e30cbd6f7931055fb7cfed2aee403c9197e0defc`  
		Last Modified: Wed, 11 Nov 2020 21:02:32 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493ee2907458eb7d47b217b59e2f23b4dd4a6974a36a70462fa54e5b9201f26b`  
		Last Modified: Wed, 11 Nov 2020 21:02:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2f8b9a7de64bd747e2afbc20e6ca964b00d3b48ccdb9245e162300a5ef9b44`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc59b5cb8ee3554d8e4971222e0208e7b6dd831b33894abeba76400bbcb7d56`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c88104f4e1fc6125880b248f3e1edcc5cbf3daf73aaf26bf3782972f11203c3`  
		Last Modified: Wed, 11 Nov 2020 21:02:30 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7cb21eb1cd8ca039940f462fdfe3348c877262adbbc5891cdbc3601ffa2649`  
		Last Modified: Wed, 11 Nov 2020 21:02:27 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef21802812d7f9ad5dcebb2efbf8d4831fcdf5b024bac00c22d04e7406a420b`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed806482965bf605e395b83f00ba44639cc1c88b1b8ec7c75bb708d9c031610`  
		Last Modified: Wed, 11 Nov 2020 21:02:24 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee097b51db8b06f6e93d48da3e914d6a598b32681fdf27785279f3f5dbb5796`  
		Last Modified: Wed, 11 Nov 2020 21:02:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf5349d69a690d25aa14a10fab1fc6e7a82ec345bae9e1a01a4dfd95f09cd1b`  
		Last Modified: Wed, 11 Nov 2020 21:02:22 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0b5aa8db0e75c1ef349905a29ef299882814b7937d14753d2e6a972f7b13b1`  
		Last Modified: Wed, 11 Nov 2020 21:02:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cac55d84f022bb91b78bfb339492198e3fa96a7d1e25c1f8e09ad648376d45d`  
		Last Modified: Wed, 11 Nov 2020 21:02:21 GMT  
		Size: 299.3 KB (299301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7476d855c257a4a27ce525860567dd9bd67e74abb01c0fd1b334444ffaa8504c`  
		Last Modified: Wed, 11 Nov 2020 21:02:24 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.14393.4046; amd64

```console
$ docker pull caddy@sha256:405a17b713c3f1517124a2506ac9b4ed33285819013417e6b90fb2aa07cb0bd6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5802615067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:371225d0afbf64a113a3745e99535e2e17239829f4e36d99aa36e7aee3be9efc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 13:23:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 20:56:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Nov 2020 20:56:05 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 11 Nov 2020 20:57:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Nov 2020 20:57:25 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Nov 2020 20:57:26 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Nov 2020 20:57:28 GMT
VOLUME [c:/config]
# Wed, 11 Nov 2020 20:57:29 GMT
VOLUME [c:/data]
# Wed, 11 Nov 2020 20:57:30 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 11 Nov 2020 20:57:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Nov 2020 20:57:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Nov 2020 20:57:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Nov 2020 20:57:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Nov 2020 20:57:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Nov 2020 20:57:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Nov 2020 20:57:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Nov 2020 20:57:35 GMT
EXPOSE 80
# Wed, 11 Nov 2020 20:57:36 GMT
EXPOSE 443
# Wed, 11 Nov 2020 20:57:37 GMT
EXPOSE 2019
# Wed, 11 Nov 2020 20:58:18 GMT
RUN caddy version
# Wed, 11 Nov 2020 20:58:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:126d9a92c0cb7b68c56dec2dd5ba118de9dde3ec6368db734c5135fdf1528a33`  
		Last Modified: Wed, 11 Nov 2020 13:34:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5595cf12db880fdffb7bc7e0ceef81a68e0766ff34fdc357635566a05b60085`  
		Last Modified: Wed, 11 Nov 2020 21:03:35 GMT  
		Size: 10.1 MB (10089893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47fc9d917c611e97ffa642af414764e4712d012a3b2c10700a357a771d58bf3`  
		Last Modified: Wed, 11 Nov 2020 21:03:24 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2b332d20177fb217e2744454885bba6eb94e9c7512c35bef53cf1222f10b3a`  
		Last Modified: Wed, 11 Nov 2020 21:03:50 GMT  
		Size: 21.7 MB (21694741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061740784584c807be44f52e632b6fcafa7893cab07ca93723103ca41e759cd2`  
		Last Modified: Wed, 11 Nov 2020 21:03:23 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a051df7f978fd750beb5e55b7a7da2d50550a52c97baf897cd3452347196147`  
		Last Modified: Wed, 11 Nov 2020 21:03:23 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94db8d6fb716d4c43b34e09a05176f94701accb480ce613c231d70ef23c649b`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eeb5cfdcdca36082954b3510135aea31966da19679b9cc7d8d4e43a3892f2f5`  
		Last Modified: Wed, 11 Nov 2020 21:03:19 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50cc11877f41dad7cb21c9e61379268e564a03b044ec4cfb124cccd267ef551c`  
		Last Modified: Wed, 11 Nov 2020 21:03:21 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9914893b848ce6d71a6f99575e794219e1603afe1dcee2bcbf69f3a41451ab05`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab52b473d299810d7e49b3d9d98db42e6aa57e5426b79f4cd7f68fd766a8a9b`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3333f590132f229c9979af102fd15c4a5958d9e3d94d50632eeb045c14028ac1`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12c4e6df6d5faa8f29b56e44eb52dc65c9d6795322a0e6d743a9d373f97adf9`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a015ed900b4c4b4d23631449b68473b1e31eda520fa22c7c19a845ac6f133f31`  
		Last Modified: Wed, 11 Nov 2020 21:03:16 GMT  
		Size: 1.1 KB (1069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f354d2a4fb61ae55364b2ae298552e22165583c076c39e05707e906633b8a2`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc11e1af39f958f492359f3242aa5205230791b166e14ab2f94067e9999464e`  
		Last Modified: Wed, 11 Nov 2020 21:03:16 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a4e622ed285e795cc2fd731f38022c2e6ca478f2223fb9fcafe0a61b5e969`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f936683e767d2733a4a898519ce7c8bc6a608fede4e7cc04c41b5fed180287`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b4fbe6665c83c229d90ec42acce959b356dbf1a97ca281604625a29d8437133`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6966c1a2733b248361e0fbafefb3b58805b223ef954ced160cb1ca7f239c25`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 251.9 KB (251913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3d08972458dc80b8c379340207e2cfeee9ea33d9e9e405ebbf52421ef16dd5`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:89299b443724d4b0e89af13958b82e2d8fc4185f2a5a8dbfb83a284bab6f5b1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull caddy@sha256:dad45b6df45cf6f4c45f010c391544a830a6372847bb2504a23a870eb9e96638
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2413941176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61f3df5163746a4530d03a8bc80f3b1318d935f9f1b3e26f00a31af891a9ba86`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 20:53:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Nov 2020 20:53:31 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 11 Nov 2020 20:54:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Nov 2020 20:54:04 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Nov 2020 20:54:04 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Nov 2020 20:54:05 GMT
VOLUME [c:/config]
# Wed, 11 Nov 2020 20:54:06 GMT
VOLUME [c:/data]
# Wed, 11 Nov 2020 20:54:07 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 11 Nov 2020 20:54:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Nov 2020 20:54:09 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Nov 2020 20:54:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Nov 2020 20:54:11 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Nov 2020 20:54:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Nov 2020 20:54:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Nov 2020 20:54:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Nov 2020 20:54:13 GMT
EXPOSE 80
# Wed, 11 Nov 2020 20:54:14 GMT
EXPOSE 443
# Wed, 11 Nov 2020 20:54:14 GMT
EXPOSE 2019
# Wed, 11 Nov 2020 20:54:30 GMT
RUN caddy version
# Wed, 11 Nov 2020 20:54:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01dcdd0030882c54a82d0a279a4099081c604810ccccb17d3d7c04a2057bf657`  
		Last Modified: Wed, 11 Nov 2020 21:02:39 GMT  
		Size: 9.2 MB (9248045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3be730f5a5cc9d1dd7080908242b9ed33ba6541e7120addf14e416b944b577`  
		Last Modified: Wed, 11 Nov 2020 21:02:36 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d70ac9fb0285fe6670a558e9c1da67b5594dd483872376ac91425a3058f95b9`  
		Last Modified: Wed, 11 Nov 2020 21:02:54 GMT  
		Size: 16.3 MB (16343997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72340d1f03d76debdf2a014ab06bbd3bc5cb1e8358520912f0c9f71f2b4a6ea`  
		Last Modified: Wed, 11 Nov 2020 21:02:34 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ae7bc4f9eb3af2fa576dd096f9992ad2cfc8a2e9aad0af79e1ebf11c95065d`  
		Last Modified: Wed, 11 Nov 2020 21:02:33 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46832c7bcb0b053968836644798024f37cfede18aaac00abed0c1571fbeeca4c`  
		Last Modified: Wed, 11 Nov 2020 21:02:33 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdafb0d35a00870fdb93efde60b2d5c002b5ec117bb07526ec1d744787529f58`  
		Last Modified: Wed, 11 Nov 2020 21:02:31 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af235cb3a2a159b44c6b773e30cbd6f7931055fb7cfed2aee403c9197e0defc`  
		Last Modified: Wed, 11 Nov 2020 21:02:32 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493ee2907458eb7d47b217b59e2f23b4dd4a6974a36a70462fa54e5b9201f26b`  
		Last Modified: Wed, 11 Nov 2020 21:02:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2f8b9a7de64bd747e2afbc20e6ca964b00d3b48ccdb9245e162300a5ef9b44`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc59b5cb8ee3554d8e4971222e0208e7b6dd831b33894abeba76400bbcb7d56`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c88104f4e1fc6125880b248f3e1edcc5cbf3daf73aaf26bf3782972f11203c3`  
		Last Modified: Wed, 11 Nov 2020 21:02:30 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7cb21eb1cd8ca039940f462fdfe3348c877262adbbc5891cdbc3601ffa2649`  
		Last Modified: Wed, 11 Nov 2020 21:02:27 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef21802812d7f9ad5dcebb2efbf8d4831fcdf5b024bac00c22d04e7406a420b`  
		Last Modified: Wed, 11 Nov 2020 21:02:28 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed806482965bf605e395b83f00ba44639cc1c88b1b8ec7c75bb708d9c031610`  
		Last Modified: Wed, 11 Nov 2020 21:02:24 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee097b51db8b06f6e93d48da3e914d6a598b32681fdf27785279f3f5dbb5796`  
		Last Modified: Wed, 11 Nov 2020 21:02:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf5349d69a690d25aa14a10fab1fc6e7a82ec345bae9e1a01a4dfd95f09cd1b`  
		Last Modified: Wed, 11 Nov 2020 21:02:22 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0b5aa8db0e75c1ef349905a29ef299882814b7937d14753d2e6a972f7b13b1`  
		Last Modified: Wed, 11 Nov 2020 21:02:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cac55d84f022bb91b78bfb339492198e3fa96a7d1e25c1f8e09ad648376d45d`  
		Last Modified: Wed, 11 Nov 2020 21:02:21 GMT  
		Size: 299.3 KB (299301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7476d855c257a4a27ce525860567dd9bd67e74abb01c0fd1b334444ffaa8504c`  
		Last Modified: Wed, 11 Nov 2020 21:02:24 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:de5b23a8826e65de497ac7335464d39371cbda3c5c4a3c0b3a3c2a816ad67149
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64

### `caddy:windowsservercore-ltsc2016` - windows version 10.0.14393.4046; amd64

```console
$ docker pull caddy@sha256:405a17b713c3f1517124a2506ac9b4ed33285819013417e6b90fb2aa07cb0bd6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5802615067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:371225d0afbf64a113a3745e99535e2e17239829f4e36d99aa36e7aee3be9efc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 13:23:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 20:56:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Nov 2020 20:56:05 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 11 Nov 2020 20:57:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Nov 2020 20:57:25 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Nov 2020 20:57:26 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Nov 2020 20:57:28 GMT
VOLUME [c:/config]
# Wed, 11 Nov 2020 20:57:29 GMT
VOLUME [c:/data]
# Wed, 11 Nov 2020 20:57:30 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 11 Nov 2020 20:57:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Nov 2020 20:57:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Nov 2020 20:57:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Nov 2020 20:57:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Nov 2020 20:57:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Nov 2020 20:57:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Nov 2020 20:57:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Nov 2020 20:57:35 GMT
EXPOSE 80
# Wed, 11 Nov 2020 20:57:36 GMT
EXPOSE 443
# Wed, 11 Nov 2020 20:57:37 GMT
EXPOSE 2019
# Wed, 11 Nov 2020 20:58:18 GMT
RUN caddy version
# Wed, 11 Nov 2020 20:58:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:126d9a92c0cb7b68c56dec2dd5ba118de9dde3ec6368db734c5135fdf1528a33`  
		Last Modified: Wed, 11 Nov 2020 13:34:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5595cf12db880fdffb7bc7e0ceef81a68e0766ff34fdc357635566a05b60085`  
		Last Modified: Wed, 11 Nov 2020 21:03:35 GMT  
		Size: 10.1 MB (10089893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47fc9d917c611e97ffa642af414764e4712d012a3b2c10700a357a771d58bf3`  
		Last Modified: Wed, 11 Nov 2020 21:03:24 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2b332d20177fb217e2744454885bba6eb94e9c7512c35bef53cf1222f10b3a`  
		Last Modified: Wed, 11 Nov 2020 21:03:50 GMT  
		Size: 21.7 MB (21694741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061740784584c807be44f52e632b6fcafa7893cab07ca93723103ca41e759cd2`  
		Last Modified: Wed, 11 Nov 2020 21:03:23 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a051df7f978fd750beb5e55b7a7da2d50550a52c97baf897cd3452347196147`  
		Last Modified: Wed, 11 Nov 2020 21:03:23 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94db8d6fb716d4c43b34e09a05176f94701accb480ce613c231d70ef23c649b`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eeb5cfdcdca36082954b3510135aea31966da19679b9cc7d8d4e43a3892f2f5`  
		Last Modified: Wed, 11 Nov 2020 21:03:19 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50cc11877f41dad7cb21c9e61379268e564a03b044ec4cfb124cccd267ef551c`  
		Last Modified: Wed, 11 Nov 2020 21:03:21 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9914893b848ce6d71a6f99575e794219e1603afe1dcee2bcbf69f3a41451ab05`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab52b473d299810d7e49b3d9d98db42e6aa57e5426b79f4cd7f68fd766a8a9b`  
		Last Modified: Wed, 11 Nov 2020 21:03:20 GMT  
		Size: 1.1 KB (1068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3333f590132f229c9979af102fd15c4a5958d9e3d94d50632eeb045c14028ac1`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12c4e6df6d5faa8f29b56e44eb52dc65c9d6795322a0e6d743a9d373f97adf9`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a015ed900b4c4b4d23631449b68473b1e31eda520fa22c7c19a845ac6f133f31`  
		Last Modified: Wed, 11 Nov 2020 21:03:16 GMT  
		Size: 1.1 KB (1069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f354d2a4fb61ae55364b2ae298552e22165583c076c39e05707e906633b8a2`  
		Last Modified: Wed, 11 Nov 2020 21:03:17 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc11e1af39f958f492359f3242aa5205230791b166e14ab2f94067e9999464e`  
		Last Modified: Wed, 11 Nov 2020 21:03:16 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a4e622ed285e795cc2fd731f38022c2e6ca478f2223fb9fcafe0a61b5e969`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f936683e767d2733a4a898519ce7c8bc6a608fede4e7cc04c41b5fed180287`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b4fbe6665c83c229d90ec42acce959b356dbf1a97ca281604625a29d8437133`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6966c1a2733b248361e0fbafefb3b58805b223ef954ced160cb1ca7f239c25`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 251.9 KB (251913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3d08972458dc80b8c379340207e2cfeee9ea33d9e9e405ebbf52421ef16dd5`  
		Last Modified: Wed, 11 Nov 2020 21:03:13 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
