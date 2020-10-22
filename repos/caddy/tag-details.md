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
$ docker pull caddy@sha256:b44006ca7a107edd0fca2ff7a70cf75b81b20b61b722dff8a720364a3764ffd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

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

### `caddy:2` - windows version 10.0.17763.1518; amd64

```console
$ docker pull caddy@sha256:5b0edc0113282eff2b0b97cb2768aef9406975982b52b5801fe66a3b7e0f1f6b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2399991421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4a3be7f6340286c7cad100a7baf86ff095c7d81ce5c10b5c314e8d7e73a9ade`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 21:03:47 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Oct 2020 21:03:48 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 14 Oct 2020 21:04:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Oct 2020 21:04:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Oct 2020 21:04:21 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Oct 2020 21:04:22 GMT
VOLUME [c:/config]
# Wed, 14 Oct 2020 21:04:23 GMT
VOLUME [c:/data]
# Wed, 14 Oct 2020 21:04:24 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 14 Oct 2020 21:04:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Oct 2020 21:04:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Oct 2020 21:04:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Oct 2020 21:04:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Oct 2020 21:04:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Oct 2020 21:04:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Oct 2020 21:04:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Oct 2020 21:04:29 GMT
EXPOSE 80
# Wed, 14 Oct 2020 21:04:30 GMT
EXPOSE 443
# Wed, 14 Oct 2020 21:04:30 GMT
EXPOSE 2019
# Wed, 14 Oct 2020 21:04:46 GMT
RUN caddy version
# Wed, 14 Oct 2020 21:04:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590b685e6f8e8fa4cbca8ce94e257baf1c179f183afabfc59bdff4420027e080`  
		Last Modified: Wed, 14 Oct 2020 21:13:24 GMT  
		Size: 9.2 MB (9237870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8a16e6bfc40544aeeaa55e8406570aec66018352db80098da3663138201f74`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468f02630a43054839d6262fe9f0d41cdd551ab83bbbb35c26cd9ead72ce6985`  
		Last Modified: Wed, 14 Oct 2020 21:13:25 GMT  
		Size: 16.3 MB (16343904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcdb09f7b5a57cb7fce28be7e54975dfc770735e4570b259b9104ddc8421bbd`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4b2b1c53bbf344fa90b58a9d5ee4b990881289dde49074cecd1f0da649c20a`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01bade2ee2333f9cd004bd1812f0c1fc7f55b2297cf57b8343e17b48c9d3535`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b312fdc7f27df222f05918031d72e4457582b08c8fdeff7cde88a6a402b6f0c`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053d376e7f1eb8e50a394d7247f16006d36ae65144e75d37fe8bb0740d91695f`  
		Last Modified: Wed, 14 Oct 2020 21:13:18 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d88dd9c5821fcba44cce1002ed12b8702e0cbec6ee8d137cbec8e5bd145acd5`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca72f02c89a70e463873f7095a54263f02a7dc1fc35b8b3d92d0d6ed1114e1c3`  
		Last Modified: Wed, 14 Oct 2020 21:13:16 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744bfb9438a82d19472dbb92037ab018420b16a677b9451e9b92d13d9d4cc309`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab7908db3cd309e1cf3200fc5b51374d626702ea4ff411559cfa15da77b097d`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691b1b3fc24e5b473537703fcabf8cdc0acd56705ab671452b135de184ffbe0c`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba327018ef360de6c48ecbdb06f66a73defdb3996be6c2f17f0731514dbece5`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c122dffbcf7af8877cc67b8f468cd74a76d63a739b85f3ac429fb27794f724`  
		Last Modified: Wed, 14 Oct 2020 21:13:13 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbf77f12be69367c8fcf09b53209ec5b25083762192120e9ed3f8e429569a4f`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c631d9175a05b1f8c784df5ccc0daeda8990f4cfa0faebc76e525dc737e034`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b5835866e9c4e5a927e7b41da88a4c61a54547cc83fc91db1c1a43494bbac2`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13669d36e52f3d6963333d5102e23ad22fd5892d4fd1a9468f12194c39c2753`  
		Last Modified: Wed, 14 Oct 2020 21:13:11 GMT  
		Size: 299.0 KB (299047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f0e09c2bd5ebc6729c8f1d852f4adefae35e2335cd7dbbcc09c95205e95ab0`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.14393.3986; amd64

```console
$ docker pull caddy@sha256:4c7f9ebc39d2e00064b805df702d5364f55de8cb8cf5ae58d8e4f438988069e8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5773083905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0ce891f0605eaed2c51c683e9fe3d70f29bf6588b85b1f2be21dfcba2c4fb3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 21:06:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Oct 2020 21:06:25 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 14 Oct 2020 21:07:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Oct 2020 21:07:57 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Oct 2020 21:07:58 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Oct 2020 21:07:59 GMT
VOLUME [c:/config]
# Wed, 14 Oct 2020 21:08:00 GMT
VOLUME [c:/data]
# Wed, 14 Oct 2020 21:08:01 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 14 Oct 2020 21:08:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Oct 2020 21:08:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Oct 2020 21:08:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Oct 2020 21:08:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Oct 2020 21:08:05 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Oct 2020 21:08:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Oct 2020 21:08:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Oct 2020 21:08:08 GMT
EXPOSE 80
# Wed, 14 Oct 2020 21:08:08 GMT
EXPOSE 443
# Wed, 14 Oct 2020 21:08:09 GMT
EXPOSE 2019
# Wed, 14 Oct 2020 21:08:53 GMT
RUN caddy version
# Wed, 14 Oct 2020 21:08:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2b4a4f0660702b9f47920e1e7ea79666ac43584dadc8412d8a7b7eb0490a2c`  
		Last Modified: Wed, 14 Oct 2020 21:13:59 GMT  
		Size: 9.9 MB (9925104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3c401ae3441b3e5b7543d5482214980c1c14958e2713fee5966c2622a53963`  
		Last Modified: Wed, 14 Oct 2020 21:13:55 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffab013bf500710ef95125418f98138723e756c560a1de0145379662b77335db`  
		Last Modified: Wed, 14 Oct 2020 21:14:00 GMT  
		Size: 21.5 MB (21518510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcf1f0773bd9f450a654eb5dcecd55e2e3fe3ba01eb0dae7dbf27e84402a6be`  
		Last Modified: Wed, 14 Oct 2020 21:13:53 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7077da12d3b43ef9b9dad1d8c770898c3a0224a8a0a3b99dc4656cc594d09b62`  
		Last Modified: Wed, 14 Oct 2020 21:13:53 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3976aabb2b169dd3bb85d39e2473fe70f7f15de0124b56095dd3c25fbbc27c`  
		Last Modified: Wed, 14 Oct 2020 21:13:52 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e5576c4d0eac332d8332455193ed1057c55aa90bd5e9a6bca884a25623c3c8`  
		Last Modified: Wed, 14 Oct 2020 21:13:52 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7210dc7c5fabd3bf6636614bc150a0965808e559f2b293340b4d8e049a185684`  
		Last Modified: Wed, 14 Oct 2020 21:13:50 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7af1dab2b20db7484c30ac3175b1dc3b89884f843ece3209fdab4882f5e018`  
		Last Modified: Wed, 14 Oct 2020 21:13:49 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe18c02535b810df5a6916e6ffe0a4532c5a70dae17b5ce28956695be585480`  
		Last Modified: Wed, 14 Oct 2020 21:13:50 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb1797af36c3af3ecc1e7db5ddfdba44c6bfff97b0515b3463d0948fed92ac4`  
		Last Modified: Wed, 14 Oct 2020 21:13:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98a2d0f6d0934d8a3b866e68ca5e7775b2af52b170aa71f2113de2d32d532a3`  
		Last Modified: Wed, 14 Oct 2020 21:13:48 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f14b6955af73ac11170ddb2c596a1dd963ceafda86300b2de8466357d56aa4`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ce0d3817eff364f0101431f28cb70cde3766120bbe5fb10b53ebf59363136f`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dd973289c284ff507f57773413c00c41a54ad2015bafb509c68a044b609cda`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6c2b7b482e55dcb167623e29563231f659e1a523cb8f6e83423bb1d69a2014`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7811e07229200779f1a17a1899bf48c49f0250685f18fdffb38ee7c30ab779`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d7cb4258c8b7eab1c92df575a363d8685d8d783672e5256208f715c662b27b`  
		Last Modified: Wed, 14 Oct 2020 21:13:44 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ab63ba04ec1b983074014465794ebf2e437ec4c03997ac40e1be3a4abcce61`  
		Last Modified: Wed, 14 Oct 2020 21:13:44 GMT  
		Size: 268.2 KB (268209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac54f9c3e58e5d406091c73dec798c29e2ee3134663b63d3ddb4959f10f4f32`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1`

```console
$ docker pull caddy@sha256:2ba92290b2abd80fc97283c3b3a1636f7614c0a5cd38d1ad318c034055540545
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

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

### `caddy:2.1.1` - windows version 10.0.17763.1518; amd64

```console
$ docker pull caddy@sha256:66f70d738fddf55c60091b6aef8e41b63c76802b802ab717413fe9c818037124
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2401370099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1397040752ad41e2b18db058da0b7e519033692fcea840d807a898de17943dde`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 20:55:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Oct 2020 20:55:53 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 14 Oct 2020 20:56:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Oct 2020 20:56:28 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Oct 2020 20:56:29 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Oct 2020 20:56:30 GMT
VOLUME [c:/config]
# Wed, 14 Oct 2020 20:56:30 GMT
VOLUME [c:/data]
# Wed, 14 Oct 2020 20:56:31 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 14 Oct 2020 20:56:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Oct 2020 20:56:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Oct 2020 20:56:34 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Oct 2020 20:56:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Oct 2020 20:56:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Oct 2020 20:56:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Oct 2020 20:56:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Oct 2020 20:56:37 GMT
EXPOSE 80
# Wed, 14 Oct 2020 20:56:38 GMT
EXPOSE 443
# Wed, 14 Oct 2020 20:56:39 GMT
EXPOSE 2019
# Wed, 14 Oct 2020 20:56:55 GMT
RUN caddy version
# Wed, 14 Oct 2020 20:56:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b188d60ff330af293d4e64c0e8d02efc672b84164a7f28c2b88c6fa69e773b`  
		Last Modified: Wed, 14 Oct 2020 21:11:59 GMT  
		Size: 9.2 MB (9238100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7cca4341580aaef49dda3a35fbe74dea069dea552f29d609095c28ae31c7c9`  
		Last Modified: Wed, 14 Oct 2020 21:11:55 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bc6acc9f3a56b460718597090a53b19d8ae56936b8c1f305a0fc5b6c8ae834`  
		Last Modified: Wed, 14 Oct 2020 21:12:01 GMT  
		Size: 17.7 MB (17721908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59da2dbe8389d72a6c47be48a14049de1017ecd0bfe42e9b39137feb681a86e2`  
		Last Modified: Wed, 14 Oct 2020 21:11:55 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08f4acb6066947f91cc9e9472c80e0f37f13d618d651351b8b3d6efd0d972d9`  
		Last Modified: Wed, 14 Oct 2020 21:11:54 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc07733f0dbd5754df935d2dd9eb9b99ec6a8833f5801ce1d28dfbd5dc06537d`  
		Last Modified: Wed, 14 Oct 2020 21:11:52 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f794342b0d24d7695630534ed119afcfd13154a5661e49b0fb63a9d09239389`  
		Last Modified: Wed, 14 Oct 2020 21:11:52 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f8231f3a84092e779185d6075769d2024c8ca7743081f3c9da45468d7f3550`  
		Last Modified: Wed, 14 Oct 2020 21:11:52 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e35f7ff6908cb027518acbf4190fa1665763a290334d11445f85785ee2b6eb6`  
		Last Modified: Wed, 14 Oct 2020 21:11:52 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a6ac3896b488a27e5a2289f4a62b934db8638756d02666690ff6e80621f0b3`  
		Last Modified: Wed, 14 Oct 2020 21:11:52 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42fa5374e20ab60dd6a7d2bdd71a4996a10f825e28542c0a038a25b5bc64fc10`  
		Last Modified: Wed, 14 Oct 2020 21:11:49 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f8e08e4c4e4262e9a897ff6a2366db843c277188a19522c2b3a238a70d2e92`  
		Last Modified: Wed, 14 Oct 2020 21:11:49 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2309bc178193a0f7b99147d5aabc6bfb9a799756c1893656a74c945570438c75`  
		Last Modified: Wed, 14 Oct 2020 21:11:48 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c0747bfbf50db12f814e3dea2b3a71b1bb951fc8f401365199cf535793880b`  
		Last Modified: Wed, 14 Oct 2020 21:11:49 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492e7f435eff381b7d6b25eb81362a6c0fd4b461ddc05978afdfaf175ff99756`  
		Last Modified: Wed, 14 Oct 2020 21:11:48 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d5be9e7e60f33a1a982e2fd5a12de9103b8c6c763d561b14577abf49c36209`  
		Last Modified: Wed, 14 Oct 2020 21:11:45 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e705ffea3945c47a37e15327ec3683dbc90a9e05a214b10f7384f782dd4d066c`  
		Last Modified: Wed, 14 Oct 2020 21:11:46 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a59c3c8fe6d1b33da8d76616405e7bf142019d8d8e2a5d372496773d29a50f5`  
		Last Modified: Wed, 14 Oct 2020 21:11:46 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e00a541946fdd8a1f98a5d34d51dca7bd037860ba1aa2a85c978213e80d25f`  
		Last Modified: Wed, 14 Oct 2020 21:11:46 GMT  
		Size: 299.5 KB (299487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17888b1c5a918fe0001ed5ea3f284e619eaa9c54b6de64d7f8def19bc9a4f7f7`  
		Last Modified: Wed, 14 Oct 2020 21:11:46 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - windows version 10.0.14393.3986; amd64

```console
$ docker pull caddy@sha256:3df3617581091c8a721884e7886ef930f68708e6be320bd2252ef6f490f2512e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5774462347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cc16ee492900dee7e9f4e124e5439d5a2a26376ffe0e4c4b85461f0907b2abf`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 20:58:29 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Oct 2020 20:58:30 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 14 Oct 2020 20:59:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Oct 2020 21:00:00 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Oct 2020 21:00:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Oct 2020 21:00:03 GMT
VOLUME [c:/config]
# Wed, 14 Oct 2020 21:00:04 GMT
VOLUME [c:/data]
# Wed, 14 Oct 2020 21:00:05 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 14 Oct 2020 21:00:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Oct 2020 21:00:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Oct 2020 21:00:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Oct 2020 21:00:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Oct 2020 21:00:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Oct 2020 21:00:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Oct 2020 21:00:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Oct 2020 21:00:11 GMT
EXPOSE 80
# Wed, 14 Oct 2020 21:00:11 GMT
EXPOSE 443
# Wed, 14 Oct 2020 21:00:12 GMT
EXPOSE 2019
# Wed, 14 Oct 2020 21:00:53 GMT
RUN caddy version
# Wed, 14 Oct 2020 21:00:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0621c6e14481e8b7931a54a60b5f552ab50344f6a75362eb856e08a00a6e121d`  
		Last Modified: Wed, 14 Oct 2020 21:12:28 GMT  
		Size: 9.9 MB (9924480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4a1346a3116e78ed00103d93f985d7f4bf3df06cb8088bca9b316cc656a1b8`  
		Last Modified: Wed, 14 Oct 2020 21:12:24 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828c93647c40ffc8bcbe621b61aef3677861ae673ef3b66ac1792c99c95234d9`  
		Last Modified: Wed, 14 Oct 2020 21:12:30 GMT  
		Size: 22.9 MB (22896440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4726960f8ff938227c56d540f881d9bc18e607f3301cd3cead8b652ec7ef517`  
		Last Modified: Wed, 14 Oct 2020 21:12:21 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b5e13596b93a65158bebc3e1cfb8345e098bd9a27f4171069026fc575224d8`  
		Last Modified: Wed, 14 Oct 2020 21:12:21 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06356772b928f71cb618db080d52bdca9588cf499ea10913136623ea3c89ac9d`  
		Last Modified: Wed, 14 Oct 2020 21:12:19 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35687f4e534a86ba4f3538c39b22db8a401bc0335da0a91c471f9eff0e934abd`  
		Last Modified: Wed, 14 Oct 2020 21:12:21 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0234c902cd868cb06435cb99ba8470182d7955305dd550a6f9e85dfdbf0589`  
		Last Modified: Wed, 14 Oct 2020 21:12:18 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdc33faacf12c704737e72c800eaa28e3da94d8ed7df679e786358a09d471bf`  
		Last Modified: Wed, 14 Oct 2020 21:12:18 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550f0814377cdb217e3609cccb0c763feeab8b5f8a35b447a95dfd89ed1cad48`  
		Last Modified: Wed, 14 Oct 2020 21:12:17 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c94837bff217cff65168fc6eebe67956699dbee13427803f6970aa8f224dc10`  
		Last Modified: Wed, 14 Oct 2020 21:12:16 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37d2486511a0c9601a2bdd89e2ebd54297bb2c78735b569e84014aa00cfb6d3`  
		Last Modified: Wed, 14 Oct 2020 21:12:21 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1435a16a8f89084f597da43cb9ce1413ac817712fad3e6683dd165dc7cc36296`  
		Last Modified: Wed, 14 Oct 2020 21:12:14 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9479319b79d0a97d0b6d91034585fb6f52136095829c563c4b36d57bdfe54c23`  
		Last Modified: Wed, 14 Oct 2020 21:12:15 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f84c09f0f902199fdd83bb5ec0da426140430cf1ae9b37d63635d70b45ddad`  
		Last Modified: Wed, 14 Oct 2020 21:12:13 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c89752e1d722e1a2bdb8c5936cbf20f3ca2c699136b1279ac27f93b75110cf`  
		Last Modified: Wed, 14 Oct 2020 21:12:11 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b75e4a8389cdb23c1d9ebf7fc2e685469542f5e1ac0f7a32e1818e04001d88`  
		Last Modified: Wed, 14 Oct 2020 21:12:11 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58bcc9da6dff9ee1073dd37c941b628f26ee80400f5a9e8c2bbbd8749815c42`  
		Last Modified: Wed, 14 Oct 2020 21:12:11 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46327701e2d8e59d0173f0db37999a9d1e633a41f36e739bfe94a37c34406aee`  
		Last Modified: Wed, 14 Oct 2020 21:12:11 GMT  
		Size: 269.3 KB (269317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd16f3084947685df6d6043025f0d44efccb637918ffc69bbebafea7e3c94970`  
		Last Modified: Wed, 14 Oct 2020 21:12:11 GMT  
		Size: 1.1 KB (1133 bytes)  
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
$ docker pull caddy@sha256:013473816bb2bcd0389abd4a802e986f6e1f71fd29552f21d7b87c0b0389ba8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

### `caddy:2.1.1-builder` - linux; amd64

```console
$ docker pull caddy@sha256:a1ca5aef4bc523c4b55da91aa02b570741b0f2163b936ae4be9abcaad6f82f21
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119784441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9b5c41c3e4866d231ac7f23ef96a0cd9600c18c6936c0d2618d5627357c7472`
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
# Thu, 22 Oct 2020 03:38:24 GMT
ENV GOLANG_VERSION=1.14.10
# Thu, 22 Oct 2020 03:43:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.10.src.tar.gz'; 	sha256='b37699a7e3eab0f90412b3969a90fd072023ecf61e0b86369da532810a95d665'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 03:43:02 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 03:43:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 03:43:04 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 03:43:04 GMT
WORKDIR /go
# Thu, 22 Oct 2020 04:33:44 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 04:33:44 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 04:33:44 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 22 Oct 2020 04:33:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 04:33:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 04:33:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 04:33:48 GMT
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
	-	`sha256:cdb4a6b39b2d21d1277c9ba67ab2e5fd437239a30a05bf1d73728d9e6d2f683e`  
		Last Modified: Thu, 22 Oct 2020 03:44:45 GMT  
		Size: 107.0 MB (106989015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a9bb10921410f36b1a48483845a6c4292529431dc9a2b1fe3c3ced5a938a60`  
		Last Modified: Thu, 22 Oct 2020 03:44:26 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05389e76306689f77fef500da53a5c3a6b345255917c2a4de18cc582a06ca628`  
		Last Modified: Thu, 22 Oct 2020 04:34:57 GMT  
		Size: 8.3 MB (8309869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb52e6c84acef0c6a548e8e88a3cb1c537c93fb0d83da426aa539606071f8ff`  
		Last Modified: Thu, 22 Oct 2020 04:34:56 GMT  
		Size: 1.4 MB (1407201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ab68384cc5d7bb9b6f62b949575de8d14c9010c395f3b5dbb23c74a23f11fc1`  
		Last Modified: Thu, 22 Oct 2020 04:34:55 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:4b32f6562092fcc63f1da4c5cb0d4105d8bc9e0d8cc12d6b5842b109c2576e37
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115461004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dc1aac72921d1945c9e56e8166472d45bd4e256667ff22b9a8dd3029a5d9392`
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
# Thu, 22 Oct 2020 04:10:35 GMT
ENV GOLANG_VERSION=1.14.10
# Thu, 22 Oct 2020 05:31:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.10.src.tar.gz'; 	sha256='b37699a7e3eab0f90412b3969a90fd072023ecf61e0b86369da532810a95d665'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 05:31:48 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 05:32:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 05:33:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 05:34:14 GMT
WORKDIR /go
# Thu, 22 Oct 2020 10:04:43 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 10:04:44 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 10:04:44 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 22 Oct 2020 10:04:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 10:04:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 10:04:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 10:04:50 GMT
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
	-	`sha256:95473b5332349ad0921731f08428a0b7b882a70e6a4da8b3d18e0fa9dd50b249`  
		Last Modified: Thu, 22 Oct 2020 05:36:30 GMT  
		Size: 103.3 MB (103321216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3197891b8a485d86436fba9677655cff8a932bafe497cfd41c5e26d92ba6c3a7`  
		Last Modified: Thu, 22 Oct 2020 05:35:56 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d347eaa2e0048fe2b866b62957f2b17c14b4fd5aac43160406d6d2ae3a952e`  
		Last Modified: Thu, 22 Oct 2020 10:05:31 GMT  
		Size: 7.9 MB (7928842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366afd8971e89c8f3ec8cf9c95acd065a1b76f5c588e0d3e4d3a2ad6b53f3dc9`  
		Last Modified: Thu, 22 Oct 2020 10:05:29 GMT  
		Size: 1.3 MB (1327348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a959303f2a76a68f0f47fb34c8e412bf251126b9c3f0e3ba4de41f5e7a49a776`  
		Last Modified: Thu, 22 Oct 2020 10:05:29 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:aeff153ca2ac180e8c4819f310b73e5e85e19e237b6bbab51524dda200623ca5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114254728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79909097bc7b22bf53d999887ba85f136762da0aedfe12ea83d16219fbc73c65`
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
# Thu, 22 Oct 2020 04:42:40 GMT
ENV GOLANG_VERSION=1.14.10
# Thu, 22 Oct 2020 05:58:07 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.10.src.tar.gz'; 	sha256='b37699a7e3eab0f90412b3969a90fd072023ecf61e0b86369da532810a95d665'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 05:58:14 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 05:58:21 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 05:58:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 05:58:54 GMT
WORKDIR /go
# Thu, 22 Oct 2020 09:24:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 09:24:31 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 09:24:31 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 22 Oct 2020 09:24:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 09:24:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 09:24:35 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 09:24:36 GMT
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
	-	`sha256:1981ecd0c1e29cfd4c996e12394b7429dfb7c7ead2a7311ab429881bd0479be6`  
		Last Modified: Thu, 22 Oct 2020 06:01:12 GMT  
		Size: 103.1 MB (103097599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1d000205aa12c72541870f9b48bf4217d2d79ff76cee1d70172df25ab469f3`  
		Last Modified: Thu, 22 Oct 2020 06:00:40 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522d024ff4526d7c9120773c2cc3ec50aa7d9bf350da80c48fcc9ef09a33d6d6`  
		Last Modified: Thu, 22 Oct 2020 09:25:16 GMT  
		Size: 7.1 MB (7144813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132085c9482c3da52b0166a84785d02605b36947340f17367e40f038919fde1c`  
		Last Modified: Thu, 22 Oct 2020 09:25:15 GMT  
		Size: 1.3 MB (1325845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f897f01efbc7f64e491843e470a9cc0ee591de8dd91992f5cbc2807374ab62`  
		Last Modified: Thu, 22 Oct 2020 09:25:14 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:0dfffb389aae084b62ccbab0813d7f5c6bd9167f070567fdcb9470aa9d3d165d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115199338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b327cac5ef2ddadeefacb2cf90286219b28596430323fbfb46302b435d5d046`
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
# Thu, 22 Oct 2020 04:18:31 GMT
ENV GOLANG_VERSION=1.14.10
# Thu, 22 Oct 2020 04:24:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.10.src.tar.gz'; 	sha256='b37699a7e3eab0f90412b3969a90fd072023ecf61e0b86369da532810a95d665'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 04:24:23 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 04:24:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 04:25:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 04:25:37 GMT
WORKDIR /go
# Thu, 22 Oct 2020 09:30:09 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 09:30:10 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 09:30:12 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 22 Oct 2020 09:30:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 09:30:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 09:30:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 09:30:18 GMT
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
	-	`sha256:69ce710a6099356e25b3da6af64fc6e46acdf514538e57f38b14d3e2cca7edac`  
		Last Modified: Thu, 22 Oct 2020 04:30:40 GMT  
		Size: 102.4 MB (102400780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f55348d42dbd0758b0cd20fbb8e58aa698aed0de212227840e02843837f80cb`  
		Last Modified: Thu, 22 Oct 2020 04:30:16 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:487eb4300fbf77d26826625c2e642d7bacf9141b7257a8c6f890050c4e7035aa`  
		Last Modified: Thu, 22 Oct 2020 09:31:24 GMT  
		Size: 8.5 MB (8499881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969cec8006955007232a74b84bd5efabf3300d8972f128e9fbd7e291a4a78292`  
		Last Modified: Thu, 22 Oct 2020 09:31:23 GMT  
		Size: 1.3 MB (1310178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba28ebfbc71bc0a12c3ce1eeb9291279230bf93c28eb5e1d30b33288a0dbfcf`  
		Last Modified: Thu, 22 Oct 2020 09:31:23 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:d74c56f6b268621ad01faad4c452154c140f770302210b003aa7a487236c97d3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114564613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea9400357f25cfc8461289104fca981eaf6e4829cd2ccb89cef2fd335cb21633`
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
# Thu, 22 Oct 2020 13:31:09 GMT
ENV GOLANG_VERSION=1.14.10
# Thu, 22 Oct 2020 13:34:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.10.src.tar.gz'; 	sha256='b37699a7e3eab0f90412b3969a90fd072023ecf61e0b86369da532810a95d665'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 13:34:25 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 13:34:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 13:34:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 13:34:53 GMT
WORKDIR /go
# Thu, 22 Oct 2020 13:43:09 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 13:43:14 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 13:43:16 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 22 Oct 2020 13:43:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 13:43:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 13:43:36 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 13:43:42 GMT
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
	-	`sha256:0afc34056aad42cb622c4a16f8802a847cdf4118db488848ea4cf93ca0576e65`  
		Last Modified: Thu, 22 Oct 2020 13:37:58 GMT  
		Size: 101.3 MB (101269675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355f171af44a0fb04dc83f9a42ad7fd9eed395ba77bc4f3a0bb78a7f4634036d`  
		Last Modified: Thu, 22 Oct 2020 13:37:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df79d7110ae8c85cd4d447839a27b6050b401d433cf1b28491edd9cf1a4124dd`  
		Last Modified: Thu, 22 Oct 2020 13:47:40 GMT  
		Size: 8.9 MB (8920007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20992d167e8c191e39343bc8c1ac146f821607d4e6dd3ac66fad4637541e1b98`  
		Last Modified: Thu, 22 Oct 2020 13:47:38 GMT  
		Size: 1.3 MB (1287792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dbcc70525d5a55ca421844e5a0b30ba74fc2bceadaf13a59965a218d5887e28`  
		Last Modified: Thu, 22 Oct 2020 13:47:38 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; s390x

```console
$ docker pull caddy@sha256:b1ee4e6e020c9752a2befaa0eac4bd2409c04305c7ab75220a1617a22f160ba2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119459725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdba81b7a03b9c038d6f2de3deb10615ace283b9e84c154fe9f6d8d43d71fdd2`
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
# Thu, 22 Oct 2020 02:55:51 GMT
ENV GOLANG_VERSION=1.14.10
# Thu, 22 Oct 2020 02:57:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.10.src.tar.gz'; 	sha256='b37699a7e3eab0f90412b3969a90fd072023ecf61e0b86369da532810a95d665'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 02:57:56 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 02:57:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 02:57:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 02:57:59 GMT
WORKDIR /go
# Thu, 22 Oct 2020 10:13:33 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 10:13:35 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 10:13:35 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 22 Oct 2020 10:13:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 10:13:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 10:13:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 10:13:39 GMT
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
	-	`sha256:2104274731c354d3642b61bc93cddbc5ff4755ae4320bda0b953a2d6920e78c0`  
		Last Modified: Thu, 22 Oct 2020 02:59:15 GMT  
		Size: 106.9 MB (106870845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70046ac743c9766ece51cb4f6120c8346b8493490eae60a820882b58981a03e9`  
		Last Modified: Thu, 22 Oct 2020 02:59:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282f0fb8ce31428108eb5d76fd098bf54cab1ae308801d8ee8ed4efcd2dfa1b3`  
		Last Modified: Thu, 22 Oct 2020 10:14:18 GMT  
		Size: 8.4 MB (8352221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3d9f1ab63e224c4e7530eb3eb16a95edccdfe245d2aa155d4550b8199689b5`  
		Last Modified: Thu, 22 Oct 2020 10:14:16 GMT  
		Size: 1.4 MB (1388752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1599908db3425dfb83e371b8694daa19643201d95ead1f190d42d2b08c834436`  
		Last Modified: Thu, 22 Oct 2020 10:14:17 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - windows version 10.0.17763.1518; amd64

```console
$ docker pull caddy@sha256:6fa20a788931550e2c74b9f59ad995ed0c96c4205a698030d58c13ca7959808d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2548362879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42877c0988528594a4ddf0bb37b85627c3ef9ddb2010b4336ebf5767225a161b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 12:27:03 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Oct 2020 12:27:04 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Oct 2020 12:27:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Oct 2020 12:27:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Oct 2020 12:28:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Oct 2020 12:28:38 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Oct 2020 12:29:02 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 15 Oct 2020 01:24:32 GMT
ENV GOLANG_VERSION=1.14.10
# Thu, 15 Oct 2020 01:57:19 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.14.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ca216afc0906f113d1c5b3498bb0015204e7ce2fd14091f5a99aae82bfb16af3'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 15 Oct 2020 01:57:20 GMT
WORKDIR C:\gopath
# Thu, 15 Oct 2020 02:30:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 15 Oct 2020 02:30:11 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 15 Oct 2020 02:30:11 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 15 Oct 2020 02:30:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 15 Oct 2020 02:30:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 15 Oct 2020 02:30:36 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23a75d88f9f5980bb112e2c28248975f107144d8d2e40dc4755e2a09f5e56df`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bea6d8b9d9b014ffa471b7bb8882ddb7e9d378ddcacc099f0710073bd6361b9`  
		Last Modified: Wed, 14 Oct 2020 12:50:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75c1905c0573cc5706bc066d23624f0e92a8871832c744fbe7eabdcbc6f8a85`  
		Last Modified: Wed, 14 Oct 2020 12:50:24 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938695376d9deeba8819539ff3245935c28f93229d1c332bb8b6a16e67013fbc`  
		Last Modified: Wed, 14 Oct 2020 12:50:23 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41106c6a476cf9666c6d8c3c853c982a841c29db05b3ef8a072baba537b6d74c`  
		Last Modified: Wed, 14 Oct 2020 12:50:48 GMT  
		Size: 34.3 MB (34312667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d6d6258831f87f3b455e6316e2bed430465a760272614de7cdd28c7c6e9f3e`  
		Last Modified: Wed, 14 Oct 2020 12:50:19 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e3f66638c4d5ce9adba16e49844f57efbab1d628d9d6c73133511b7c1c3892`  
		Last Modified: Wed, 14 Oct 2020 12:50:20 GMT  
		Size: 310.5 KB (310525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97742f1f2a85065ea66be4166c6d8678ee23b85158953dbda96c7de272cb1924`  
		Last Modified: Thu, 15 Oct 2020 02:07:41 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46d96ac99bdb6c35f3d4a07cd1a7c6abcc2f64b81410bef53ef6dfcafd3de53`  
		Last Modified: Thu, 15 Oct 2020 02:08:08 GMT  
		Size: 137.9 MB (137853657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c372b08e62adf0c7e3ce57cc1e3a441877c5273c7c14ff314452a131d9340d`  
		Last Modified: Thu, 15 Oct 2020 02:07:41 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c78b13364ced61d2c2113930f0a21dc88d9e8953d7e1b93788f21dbecc94776`  
		Last Modified: Thu, 15 Oct 2020 02:34:44 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2731139c25f0e17b644c20b8e37060e36a1a2ce37338793e20103435e517e5`  
		Last Modified: Thu, 15 Oct 2020 02:34:42 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b8c1dd3aa525167f83506f0cac7e61eec19ae88ac3a5faeef184e2e292de1d`  
		Last Modified: Thu, 15 Oct 2020 02:34:42 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4ae6b995c9c57ece90c43e4a4963d43825845148fbf37d274abcb8d0201fc7`  
		Last Modified: Thu, 15 Oct 2020 02:34:42 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17419d26c66b24af23d820bcc73ad06f55d56b9dcb863425862914ec2d860871`  
		Last Modified: Thu, 15 Oct 2020 02:34:43 GMT  
		Size: 1.8 MB (1781023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fbe0ae3f821ad6f5fd1c24531f79755b774264487647b08966957cda9c98ae`  
		Last Modified: Thu, 15 Oct 2020 02:34:42 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - windows version 10.0.14393.3986; amd64

```console
$ docker pull caddy@sha256:f5212ee2bb29dbfe55d07be46937a8e42f2ba6c5563a1d0455fb96100043164e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5940574785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99c329b2d41299d6faf53a7d6c9c029b4657d1431945e4d33c0b9f1d9a5fdf5c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 12:31:45 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Oct 2020 12:31:46 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Oct 2020 12:31:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Oct 2020 12:31:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Oct 2020 12:33:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Oct 2020 12:33:58 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Oct 2020 12:35:13 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 15 Oct 2020 01:57:35 GMT
ENV GOLANG_VERSION=1.14.10
# Thu, 15 Oct 2020 02:01:12 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.14.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ca216afc0906f113d1c5b3498bb0015204e7ce2fd14091f5a99aae82bfb16af3'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 15 Oct 2020 02:01:13 GMT
WORKDIR C:\gopath
# Thu, 15 Oct 2020 02:30:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 15 Oct 2020 02:30:41 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 15 Oct 2020 02:30:42 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 15 Oct 2020 02:30:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 15 Oct 2020 02:31:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 15 Oct 2020 02:32:01 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528ba1d9759adcc464112008fe49672e1f545981d69bab31186587ab32f92138`  
		Last Modified: Wed, 14 Oct 2020 12:51:33 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53bf4e6180661653575845d30a4d882dea92f395cb540b1cdf91170e9ee58731`  
		Last Modified: Wed, 14 Oct 2020 12:51:30 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e973f094614bb2cebe16df6f6004c05895ed077151aecdbbd0c476513054fc`  
		Last Modified: Wed, 14 Oct 2020 12:51:25 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1089b875ac355097876e23760dd2166f096a8645e312660ffd3c0e617a2df9a0`  
		Last Modified: Wed, 14 Oct 2020 12:51:29 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8934a016b666d0691307c6414d84c36eb82de4b2fc4d74dd04c75f632dc3a78c`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 35.0 MB (35016991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4d95d13c0a45aa19a623e51cb112530a589a3a4d15d5c119610f8196912fab`  
		Last Modified: Wed, 14 Oct 2020 12:51:20 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf8226941bb8f5af9f2be8fdb54da3e3caef344b0061a73e3debde23a55e98f`  
		Last Modified: Wed, 14 Oct 2020 12:51:24 GMT  
		Size: 9.9 MB (9870100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4d79d377a9bc1f2fd9d43573b64dfec63d917ef75dd8bbeb80b19596792a82`  
		Last Modified: Thu, 15 Oct 2020 02:08:20 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a16286b4ccfa55ad1e0d4a052874bc274b3dec7de10503afcf0aad170fe817d`  
		Last Modified: Thu, 15 Oct 2020 02:11:08 GMT  
		Size: 143.0 MB (143016244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4faff7295ca17da6be5593ac9ab9ca220e801280840e352fd9841e0cb3ee06f`  
		Last Modified: Thu, 15 Oct 2020 02:08:22 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20546103bd5d6aaef628bd25aafa9a015245d2728ec2f573c838dcdb05b79ae`  
		Last Modified: Thu, 15 Oct 2020 02:34:58 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3661013834b30ff74cea50d6ac30ec6574ada38cd04141a7436f5b8bc62055aa`  
		Last Modified: Thu, 15 Oct 2020 02:34:55 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6133eaf1bfe70c46e36bf0c3f18dfda1a0e4246cc05c22022c15fe1b2cd3c07`  
		Last Modified: Thu, 15 Oct 2020 02:34:54 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1850083a8636b528f74401e328a01a0f448cc8fc23d5c8e80608ca02ed09bc31`  
		Last Modified: Thu, 15 Oct 2020 02:34:54 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0372cbbeb7a181347e9c41a1ca102a33fba36773ef4f48abe590413d1528fd`  
		Last Modified: Thu, 15 Oct 2020 02:34:56 GMT  
		Size: 11.3 MB (11304746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d46efd1702d5e561af800fc23233b8945b12994eb1c7686a6083ec0e6ab3a48`  
		Last Modified: Thu, 15 Oct 2020 02:34:58 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-builder-alpine`

```console
$ docker pull caddy@sha256:5b0365b74a89491e0d7e9756466ea91ac6f6733deca385897381a25ae13526ce
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
$ docker pull caddy@sha256:a1ca5aef4bc523c4b55da91aa02b570741b0f2163b936ae4be9abcaad6f82f21
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119784441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9b5c41c3e4866d231ac7f23ef96a0cd9600c18c6936c0d2618d5627357c7472`
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
# Thu, 22 Oct 2020 03:38:24 GMT
ENV GOLANG_VERSION=1.14.10
# Thu, 22 Oct 2020 03:43:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.10.src.tar.gz'; 	sha256='b37699a7e3eab0f90412b3969a90fd072023ecf61e0b86369da532810a95d665'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 03:43:02 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 03:43:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 03:43:04 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 03:43:04 GMT
WORKDIR /go
# Thu, 22 Oct 2020 04:33:44 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 04:33:44 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 04:33:44 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 22 Oct 2020 04:33:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 04:33:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 04:33:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 04:33:48 GMT
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
	-	`sha256:cdb4a6b39b2d21d1277c9ba67ab2e5fd437239a30a05bf1d73728d9e6d2f683e`  
		Last Modified: Thu, 22 Oct 2020 03:44:45 GMT  
		Size: 107.0 MB (106989015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a9bb10921410f36b1a48483845a6c4292529431dc9a2b1fe3c3ced5a938a60`  
		Last Modified: Thu, 22 Oct 2020 03:44:26 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05389e76306689f77fef500da53a5c3a6b345255917c2a4de18cc582a06ca628`  
		Last Modified: Thu, 22 Oct 2020 04:34:57 GMT  
		Size: 8.3 MB (8309869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb52e6c84acef0c6a548e8e88a3cb1c537c93fb0d83da426aa539606071f8ff`  
		Last Modified: Thu, 22 Oct 2020 04:34:56 GMT  
		Size: 1.4 MB (1407201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ab68384cc5d7bb9b6f62b949575de8d14c9010c395f3b5dbb23c74a23f11fc1`  
		Last Modified: Thu, 22 Oct 2020 04:34:55 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:4b32f6562092fcc63f1da4c5cb0d4105d8bc9e0d8cc12d6b5842b109c2576e37
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115461004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dc1aac72921d1945c9e56e8166472d45bd4e256667ff22b9a8dd3029a5d9392`
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
# Thu, 22 Oct 2020 04:10:35 GMT
ENV GOLANG_VERSION=1.14.10
# Thu, 22 Oct 2020 05:31:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.10.src.tar.gz'; 	sha256='b37699a7e3eab0f90412b3969a90fd072023ecf61e0b86369da532810a95d665'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 05:31:48 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 05:32:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 05:33:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 05:34:14 GMT
WORKDIR /go
# Thu, 22 Oct 2020 10:04:43 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 10:04:44 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 10:04:44 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 22 Oct 2020 10:04:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 10:04:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 10:04:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 10:04:50 GMT
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
	-	`sha256:95473b5332349ad0921731f08428a0b7b882a70e6a4da8b3d18e0fa9dd50b249`  
		Last Modified: Thu, 22 Oct 2020 05:36:30 GMT  
		Size: 103.3 MB (103321216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3197891b8a485d86436fba9677655cff8a932bafe497cfd41c5e26d92ba6c3a7`  
		Last Modified: Thu, 22 Oct 2020 05:35:56 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d347eaa2e0048fe2b866b62957f2b17c14b4fd5aac43160406d6d2ae3a952e`  
		Last Modified: Thu, 22 Oct 2020 10:05:31 GMT  
		Size: 7.9 MB (7928842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366afd8971e89c8f3ec8cf9c95acd065a1b76f5c588e0d3e4d3a2ad6b53f3dc9`  
		Last Modified: Thu, 22 Oct 2020 10:05:29 GMT  
		Size: 1.3 MB (1327348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a959303f2a76a68f0f47fb34c8e412bf251126b9c3f0e3ba4de41f5e7a49a776`  
		Last Modified: Thu, 22 Oct 2020 10:05:29 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:aeff153ca2ac180e8c4819f310b73e5e85e19e237b6bbab51524dda200623ca5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114254728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79909097bc7b22bf53d999887ba85f136762da0aedfe12ea83d16219fbc73c65`
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
# Thu, 22 Oct 2020 04:42:40 GMT
ENV GOLANG_VERSION=1.14.10
# Thu, 22 Oct 2020 05:58:07 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.10.src.tar.gz'; 	sha256='b37699a7e3eab0f90412b3969a90fd072023ecf61e0b86369da532810a95d665'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 05:58:14 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 05:58:21 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 05:58:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 05:58:54 GMT
WORKDIR /go
# Thu, 22 Oct 2020 09:24:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 09:24:31 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 09:24:31 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 22 Oct 2020 09:24:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 09:24:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 09:24:35 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 09:24:36 GMT
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
	-	`sha256:1981ecd0c1e29cfd4c996e12394b7429dfb7c7ead2a7311ab429881bd0479be6`  
		Last Modified: Thu, 22 Oct 2020 06:01:12 GMT  
		Size: 103.1 MB (103097599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1d000205aa12c72541870f9b48bf4217d2d79ff76cee1d70172df25ab469f3`  
		Last Modified: Thu, 22 Oct 2020 06:00:40 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522d024ff4526d7c9120773c2cc3ec50aa7d9bf350da80c48fcc9ef09a33d6d6`  
		Last Modified: Thu, 22 Oct 2020 09:25:16 GMT  
		Size: 7.1 MB (7144813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132085c9482c3da52b0166a84785d02605b36947340f17367e40f038919fde1c`  
		Last Modified: Thu, 22 Oct 2020 09:25:15 GMT  
		Size: 1.3 MB (1325845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f897f01efbc7f64e491843e470a9cc0ee591de8dd91992f5cbc2807374ab62`  
		Last Modified: Thu, 22 Oct 2020 09:25:14 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:0dfffb389aae084b62ccbab0813d7f5c6bd9167f070567fdcb9470aa9d3d165d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115199338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b327cac5ef2ddadeefacb2cf90286219b28596430323fbfb46302b435d5d046`
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
# Thu, 22 Oct 2020 04:18:31 GMT
ENV GOLANG_VERSION=1.14.10
# Thu, 22 Oct 2020 04:24:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.10.src.tar.gz'; 	sha256='b37699a7e3eab0f90412b3969a90fd072023ecf61e0b86369da532810a95d665'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 04:24:23 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 04:24:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 04:25:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 04:25:37 GMT
WORKDIR /go
# Thu, 22 Oct 2020 09:30:09 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 09:30:10 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 09:30:12 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 22 Oct 2020 09:30:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 09:30:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 09:30:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 09:30:18 GMT
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
	-	`sha256:69ce710a6099356e25b3da6af64fc6e46acdf514538e57f38b14d3e2cca7edac`  
		Last Modified: Thu, 22 Oct 2020 04:30:40 GMT  
		Size: 102.4 MB (102400780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f55348d42dbd0758b0cd20fbb8e58aa698aed0de212227840e02843837f80cb`  
		Last Modified: Thu, 22 Oct 2020 04:30:16 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:487eb4300fbf77d26826625c2e642d7bacf9141b7257a8c6f890050c4e7035aa`  
		Last Modified: Thu, 22 Oct 2020 09:31:24 GMT  
		Size: 8.5 MB (8499881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969cec8006955007232a74b84bd5efabf3300d8972f128e9fbd7e291a4a78292`  
		Last Modified: Thu, 22 Oct 2020 09:31:23 GMT  
		Size: 1.3 MB (1310178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba28ebfbc71bc0a12c3ce1eeb9291279230bf93c28eb5e1d30b33288a0dbfcf`  
		Last Modified: Thu, 22 Oct 2020 09:31:23 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:d74c56f6b268621ad01faad4c452154c140f770302210b003aa7a487236c97d3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114564613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea9400357f25cfc8461289104fca981eaf6e4829cd2ccb89cef2fd335cb21633`
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
# Thu, 22 Oct 2020 13:31:09 GMT
ENV GOLANG_VERSION=1.14.10
# Thu, 22 Oct 2020 13:34:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.10.src.tar.gz'; 	sha256='b37699a7e3eab0f90412b3969a90fd072023ecf61e0b86369da532810a95d665'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 13:34:25 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 13:34:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 13:34:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 13:34:53 GMT
WORKDIR /go
# Thu, 22 Oct 2020 13:43:09 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 13:43:14 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 13:43:16 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 22 Oct 2020 13:43:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 13:43:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 13:43:36 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 13:43:42 GMT
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
	-	`sha256:0afc34056aad42cb622c4a16f8802a847cdf4118db488848ea4cf93ca0576e65`  
		Last Modified: Thu, 22 Oct 2020 13:37:58 GMT  
		Size: 101.3 MB (101269675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355f171af44a0fb04dc83f9a42ad7fd9eed395ba77bc4f3a0bb78a7f4634036d`  
		Last Modified: Thu, 22 Oct 2020 13:37:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df79d7110ae8c85cd4d447839a27b6050b401d433cf1b28491edd9cf1a4124dd`  
		Last Modified: Thu, 22 Oct 2020 13:47:40 GMT  
		Size: 8.9 MB (8920007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20992d167e8c191e39343bc8c1ac146f821607d4e6dd3ac66fad4637541e1b98`  
		Last Modified: Thu, 22 Oct 2020 13:47:38 GMT  
		Size: 1.3 MB (1287792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dbcc70525d5a55ca421844e5a0b30ba74fc2bceadaf13a59965a218d5887e28`  
		Last Modified: Thu, 22 Oct 2020 13:47:38 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:b1ee4e6e020c9752a2befaa0eac4bd2409c04305c7ab75220a1617a22f160ba2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119459725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdba81b7a03b9c038d6f2de3deb10615ace283b9e84c154fe9f6d8d43d71fdd2`
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
# Thu, 22 Oct 2020 02:55:51 GMT
ENV GOLANG_VERSION=1.14.10
# Thu, 22 Oct 2020 02:57:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.10.src.tar.gz'; 	sha256='b37699a7e3eab0f90412b3969a90fd072023ecf61e0b86369da532810a95d665'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 02:57:56 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 02:57:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 02:57:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 02:57:59 GMT
WORKDIR /go
# Thu, 22 Oct 2020 10:13:33 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 10:13:35 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 10:13:35 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 22 Oct 2020 10:13:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 10:13:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 10:13:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 10:13:39 GMT
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
	-	`sha256:2104274731c354d3642b61bc93cddbc5ff4755ae4320bda0b953a2d6920e78c0`  
		Last Modified: Thu, 22 Oct 2020 02:59:15 GMT  
		Size: 106.9 MB (106870845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70046ac743c9766ece51cb4f6120c8346b8493490eae60a820882b58981a03e9`  
		Last Modified: Thu, 22 Oct 2020 02:59:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282f0fb8ce31428108eb5d76fd098bf54cab1ae308801d8ee8ed4efcd2dfa1b3`  
		Last Modified: Thu, 22 Oct 2020 10:14:18 GMT  
		Size: 8.4 MB (8352221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3d9f1ab63e224c4e7530eb3eb16a95edccdfe245d2aa155d4550b8199689b5`  
		Last Modified: Thu, 22 Oct 2020 10:14:16 GMT  
		Size: 1.4 MB (1388752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1599908db3425dfb83e371b8694daa19643201d95ead1f190d42d2b08c834436`  
		Last Modified: Thu, 22 Oct 2020 10:14:17 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:03b057e8ac2023ea0fdf3f81532acfa4cd6dd4b114224da6d3d09d6d0279b2a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `caddy:2.1.1-builder-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull caddy@sha256:6fa20a788931550e2c74b9f59ad995ed0c96c4205a698030d58c13ca7959808d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2548362879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42877c0988528594a4ddf0bb37b85627c3ef9ddb2010b4336ebf5767225a161b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 12:27:03 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Oct 2020 12:27:04 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Oct 2020 12:27:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Oct 2020 12:27:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Oct 2020 12:28:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Oct 2020 12:28:38 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Oct 2020 12:29:02 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 15 Oct 2020 01:24:32 GMT
ENV GOLANG_VERSION=1.14.10
# Thu, 15 Oct 2020 01:57:19 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.14.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ca216afc0906f113d1c5b3498bb0015204e7ce2fd14091f5a99aae82bfb16af3'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 15 Oct 2020 01:57:20 GMT
WORKDIR C:\gopath
# Thu, 15 Oct 2020 02:30:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 15 Oct 2020 02:30:11 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 15 Oct 2020 02:30:11 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 15 Oct 2020 02:30:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 15 Oct 2020 02:30:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 15 Oct 2020 02:30:36 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23a75d88f9f5980bb112e2c28248975f107144d8d2e40dc4755e2a09f5e56df`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bea6d8b9d9b014ffa471b7bb8882ddb7e9d378ddcacc099f0710073bd6361b9`  
		Last Modified: Wed, 14 Oct 2020 12:50:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75c1905c0573cc5706bc066d23624f0e92a8871832c744fbe7eabdcbc6f8a85`  
		Last Modified: Wed, 14 Oct 2020 12:50:24 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938695376d9deeba8819539ff3245935c28f93229d1c332bb8b6a16e67013fbc`  
		Last Modified: Wed, 14 Oct 2020 12:50:23 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41106c6a476cf9666c6d8c3c853c982a841c29db05b3ef8a072baba537b6d74c`  
		Last Modified: Wed, 14 Oct 2020 12:50:48 GMT  
		Size: 34.3 MB (34312667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d6d6258831f87f3b455e6316e2bed430465a760272614de7cdd28c7c6e9f3e`  
		Last Modified: Wed, 14 Oct 2020 12:50:19 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e3f66638c4d5ce9adba16e49844f57efbab1d628d9d6c73133511b7c1c3892`  
		Last Modified: Wed, 14 Oct 2020 12:50:20 GMT  
		Size: 310.5 KB (310525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97742f1f2a85065ea66be4166c6d8678ee23b85158953dbda96c7de272cb1924`  
		Last Modified: Thu, 15 Oct 2020 02:07:41 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46d96ac99bdb6c35f3d4a07cd1a7c6abcc2f64b81410bef53ef6dfcafd3de53`  
		Last Modified: Thu, 15 Oct 2020 02:08:08 GMT  
		Size: 137.9 MB (137853657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c372b08e62adf0c7e3ce57cc1e3a441877c5273c7c14ff314452a131d9340d`  
		Last Modified: Thu, 15 Oct 2020 02:07:41 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c78b13364ced61d2c2113930f0a21dc88d9e8953d7e1b93788f21dbecc94776`  
		Last Modified: Thu, 15 Oct 2020 02:34:44 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2731139c25f0e17b644c20b8e37060e36a1a2ce37338793e20103435e517e5`  
		Last Modified: Thu, 15 Oct 2020 02:34:42 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b8c1dd3aa525167f83506f0cac7e61eec19ae88ac3a5faeef184e2e292de1d`  
		Last Modified: Thu, 15 Oct 2020 02:34:42 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4ae6b995c9c57ece90c43e4a4963d43825845148fbf37d274abcb8d0201fc7`  
		Last Modified: Thu, 15 Oct 2020 02:34:42 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17419d26c66b24af23d820bcc73ad06f55d56b9dcb863425862914ec2d860871`  
		Last Modified: Thu, 15 Oct 2020 02:34:43 GMT  
		Size: 1.8 MB (1781023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fbe0ae3f821ad6f5fd1c24531f79755b774264487647b08966957cda9c98ae`  
		Last Modified: Thu, 15 Oct 2020 02:34:42 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:7f84179190fb41ed59276410e8b3561d41bcd67f4c73873c54c32fcb59601fde
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64

### `caddy:2.1.1-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.3986; amd64

```console
$ docker pull caddy@sha256:f5212ee2bb29dbfe55d07be46937a8e42f2ba6c5563a1d0455fb96100043164e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5940574785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99c329b2d41299d6faf53a7d6c9c029b4657d1431945e4d33c0b9f1d9a5fdf5c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 12:31:45 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Oct 2020 12:31:46 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Oct 2020 12:31:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Oct 2020 12:31:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Oct 2020 12:33:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Oct 2020 12:33:58 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Oct 2020 12:35:13 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 15 Oct 2020 01:57:35 GMT
ENV GOLANG_VERSION=1.14.10
# Thu, 15 Oct 2020 02:01:12 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.14.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ca216afc0906f113d1c5b3498bb0015204e7ce2fd14091f5a99aae82bfb16af3'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 15 Oct 2020 02:01:13 GMT
WORKDIR C:\gopath
# Thu, 15 Oct 2020 02:30:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 15 Oct 2020 02:30:41 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 15 Oct 2020 02:30:42 GMT
ENV CADDY_VERSION=v2.1.1
# Thu, 15 Oct 2020 02:30:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 15 Oct 2020 02:31:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 15 Oct 2020 02:32:01 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528ba1d9759adcc464112008fe49672e1f545981d69bab31186587ab32f92138`  
		Last Modified: Wed, 14 Oct 2020 12:51:33 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53bf4e6180661653575845d30a4d882dea92f395cb540b1cdf91170e9ee58731`  
		Last Modified: Wed, 14 Oct 2020 12:51:30 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e973f094614bb2cebe16df6f6004c05895ed077151aecdbbd0c476513054fc`  
		Last Modified: Wed, 14 Oct 2020 12:51:25 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1089b875ac355097876e23760dd2166f096a8645e312660ffd3c0e617a2df9a0`  
		Last Modified: Wed, 14 Oct 2020 12:51:29 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8934a016b666d0691307c6414d84c36eb82de4b2fc4d74dd04c75f632dc3a78c`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 35.0 MB (35016991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4d95d13c0a45aa19a623e51cb112530a589a3a4d15d5c119610f8196912fab`  
		Last Modified: Wed, 14 Oct 2020 12:51:20 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf8226941bb8f5af9f2be8fdb54da3e3caef344b0061a73e3debde23a55e98f`  
		Last Modified: Wed, 14 Oct 2020 12:51:24 GMT  
		Size: 9.9 MB (9870100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4d79d377a9bc1f2fd9d43573b64dfec63d917ef75dd8bbeb80b19596792a82`  
		Last Modified: Thu, 15 Oct 2020 02:08:20 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a16286b4ccfa55ad1e0d4a052874bc274b3dec7de10503afcf0aad170fe817d`  
		Last Modified: Thu, 15 Oct 2020 02:11:08 GMT  
		Size: 143.0 MB (143016244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4faff7295ca17da6be5593ac9ab9ca220e801280840e352fd9841e0cb3ee06f`  
		Last Modified: Thu, 15 Oct 2020 02:08:22 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20546103bd5d6aaef628bd25aafa9a015245d2728ec2f573c838dcdb05b79ae`  
		Last Modified: Thu, 15 Oct 2020 02:34:58 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3661013834b30ff74cea50d6ac30ec6574ada38cd04141a7436f5b8bc62055aa`  
		Last Modified: Thu, 15 Oct 2020 02:34:55 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6133eaf1bfe70c46e36bf0c3f18dfda1a0e4246cc05c22022c15fe1b2cd3c07`  
		Last Modified: Thu, 15 Oct 2020 02:34:54 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1850083a8636b528f74401e328a01a0f448cc8fc23d5c8e80608ca02ed09bc31`  
		Last Modified: Thu, 15 Oct 2020 02:34:54 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0372cbbeb7a181347e9c41a1ca102a33fba36773ef4f48abe590413d1528fd`  
		Last Modified: Thu, 15 Oct 2020 02:34:56 GMT  
		Size: 11.3 MB (11304746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d46efd1702d5e561af800fc23233b8945b12994eb1c7686a6083ec0e6ab3a48`  
		Last Modified: Thu, 15 Oct 2020 02:34:58 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-windowsservercore`

```console
$ docker pull caddy@sha256:f896aef1c898fbc3327acd681f132b4ad3ec5ac8ffffbad596a9b8ff1868968c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

### `caddy:2.1.1-windowsservercore` - windows version 10.0.17763.1518; amd64

```console
$ docker pull caddy@sha256:66f70d738fddf55c60091b6aef8e41b63c76802b802ab717413fe9c818037124
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2401370099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1397040752ad41e2b18db058da0b7e519033692fcea840d807a898de17943dde`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 20:55:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Oct 2020 20:55:53 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 14 Oct 2020 20:56:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Oct 2020 20:56:28 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Oct 2020 20:56:29 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Oct 2020 20:56:30 GMT
VOLUME [c:/config]
# Wed, 14 Oct 2020 20:56:30 GMT
VOLUME [c:/data]
# Wed, 14 Oct 2020 20:56:31 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 14 Oct 2020 20:56:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Oct 2020 20:56:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Oct 2020 20:56:34 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Oct 2020 20:56:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Oct 2020 20:56:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Oct 2020 20:56:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Oct 2020 20:56:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Oct 2020 20:56:37 GMT
EXPOSE 80
# Wed, 14 Oct 2020 20:56:38 GMT
EXPOSE 443
# Wed, 14 Oct 2020 20:56:39 GMT
EXPOSE 2019
# Wed, 14 Oct 2020 20:56:55 GMT
RUN caddy version
# Wed, 14 Oct 2020 20:56:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b188d60ff330af293d4e64c0e8d02efc672b84164a7f28c2b88c6fa69e773b`  
		Last Modified: Wed, 14 Oct 2020 21:11:59 GMT  
		Size: 9.2 MB (9238100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7cca4341580aaef49dda3a35fbe74dea069dea552f29d609095c28ae31c7c9`  
		Last Modified: Wed, 14 Oct 2020 21:11:55 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bc6acc9f3a56b460718597090a53b19d8ae56936b8c1f305a0fc5b6c8ae834`  
		Last Modified: Wed, 14 Oct 2020 21:12:01 GMT  
		Size: 17.7 MB (17721908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59da2dbe8389d72a6c47be48a14049de1017ecd0bfe42e9b39137feb681a86e2`  
		Last Modified: Wed, 14 Oct 2020 21:11:55 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08f4acb6066947f91cc9e9472c80e0f37f13d618d651351b8b3d6efd0d972d9`  
		Last Modified: Wed, 14 Oct 2020 21:11:54 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc07733f0dbd5754df935d2dd9eb9b99ec6a8833f5801ce1d28dfbd5dc06537d`  
		Last Modified: Wed, 14 Oct 2020 21:11:52 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f794342b0d24d7695630534ed119afcfd13154a5661e49b0fb63a9d09239389`  
		Last Modified: Wed, 14 Oct 2020 21:11:52 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f8231f3a84092e779185d6075769d2024c8ca7743081f3c9da45468d7f3550`  
		Last Modified: Wed, 14 Oct 2020 21:11:52 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e35f7ff6908cb027518acbf4190fa1665763a290334d11445f85785ee2b6eb6`  
		Last Modified: Wed, 14 Oct 2020 21:11:52 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a6ac3896b488a27e5a2289f4a62b934db8638756d02666690ff6e80621f0b3`  
		Last Modified: Wed, 14 Oct 2020 21:11:52 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42fa5374e20ab60dd6a7d2bdd71a4996a10f825e28542c0a038a25b5bc64fc10`  
		Last Modified: Wed, 14 Oct 2020 21:11:49 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f8e08e4c4e4262e9a897ff6a2366db843c277188a19522c2b3a238a70d2e92`  
		Last Modified: Wed, 14 Oct 2020 21:11:49 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2309bc178193a0f7b99147d5aabc6bfb9a799756c1893656a74c945570438c75`  
		Last Modified: Wed, 14 Oct 2020 21:11:48 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c0747bfbf50db12f814e3dea2b3a71b1bb951fc8f401365199cf535793880b`  
		Last Modified: Wed, 14 Oct 2020 21:11:49 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492e7f435eff381b7d6b25eb81362a6c0fd4b461ddc05978afdfaf175ff99756`  
		Last Modified: Wed, 14 Oct 2020 21:11:48 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d5be9e7e60f33a1a982e2fd5a12de9103b8c6c763d561b14577abf49c36209`  
		Last Modified: Wed, 14 Oct 2020 21:11:45 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e705ffea3945c47a37e15327ec3683dbc90a9e05a214b10f7384f782dd4d066c`  
		Last Modified: Wed, 14 Oct 2020 21:11:46 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a59c3c8fe6d1b33da8d76616405e7bf142019d8d8e2a5d372496773d29a50f5`  
		Last Modified: Wed, 14 Oct 2020 21:11:46 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e00a541946fdd8a1f98a5d34d51dca7bd037860ba1aa2a85c978213e80d25f`  
		Last Modified: Wed, 14 Oct 2020 21:11:46 GMT  
		Size: 299.5 KB (299487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17888b1c5a918fe0001ed5ea3f284e619eaa9c54b6de64d7f8def19bc9a4f7f7`  
		Last Modified: Wed, 14 Oct 2020 21:11:46 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-windowsservercore` - windows version 10.0.14393.3986; amd64

```console
$ docker pull caddy@sha256:3df3617581091c8a721884e7886ef930f68708e6be320bd2252ef6f490f2512e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5774462347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cc16ee492900dee7e9f4e124e5439d5a2a26376ffe0e4c4b85461f0907b2abf`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 20:58:29 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Oct 2020 20:58:30 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 14 Oct 2020 20:59:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Oct 2020 21:00:00 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Oct 2020 21:00:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Oct 2020 21:00:03 GMT
VOLUME [c:/config]
# Wed, 14 Oct 2020 21:00:04 GMT
VOLUME [c:/data]
# Wed, 14 Oct 2020 21:00:05 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 14 Oct 2020 21:00:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Oct 2020 21:00:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Oct 2020 21:00:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Oct 2020 21:00:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Oct 2020 21:00:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Oct 2020 21:00:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Oct 2020 21:00:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Oct 2020 21:00:11 GMT
EXPOSE 80
# Wed, 14 Oct 2020 21:00:11 GMT
EXPOSE 443
# Wed, 14 Oct 2020 21:00:12 GMT
EXPOSE 2019
# Wed, 14 Oct 2020 21:00:53 GMT
RUN caddy version
# Wed, 14 Oct 2020 21:00:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0621c6e14481e8b7931a54a60b5f552ab50344f6a75362eb856e08a00a6e121d`  
		Last Modified: Wed, 14 Oct 2020 21:12:28 GMT  
		Size: 9.9 MB (9924480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4a1346a3116e78ed00103d93f985d7f4bf3df06cb8088bca9b316cc656a1b8`  
		Last Modified: Wed, 14 Oct 2020 21:12:24 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828c93647c40ffc8bcbe621b61aef3677861ae673ef3b66ac1792c99c95234d9`  
		Last Modified: Wed, 14 Oct 2020 21:12:30 GMT  
		Size: 22.9 MB (22896440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4726960f8ff938227c56d540f881d9bc18e607f3301cd3cead8b652ec7ef517`  
		Last Modified: Wed, 14 Oct 2020 21:12:21 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b5e13596b93a65158bebc3e1cfb8345e098bd9a27f4171069026fc575224d8`  
		Last Modified: Wed, 14 Oct 2020 21:12:21 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06356772b928f71cb618db080d52bdca9588cf499ea10913136623ea3c89ac9d`  
		Last Modified: Wed, 14 Oct 2020 21:12:19 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35687f4e534a86ba4f3538c39b22db8a401bc0335da0a91c471f9eff0e934abd`  
		Last Modified: Wed, 14 Oct 2020 21:12:21 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0234c902cd868cb06435cb99ba8470182d7955305dd550a6f9e85dfdbf0589`  
		Last Modified: Wed, 14 Oct 2020 21:12:18 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdc33faacf12c704737e72c800eaa28e3da94d8ed7df679e786358a09d471bf`  
		Last Modified: Wed, 14 Oct 2020 21:12:18 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550f0814377cdb217e3609cccb0c763feeab8b5f8a35b447a95dfd89ed1cad48`  
		Last Modified: Wed, 14 Oct 2020 21:12:17 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c94837bff217cff65168fc6eebe67956699dbee13427803f6970aa8f224dc10`  
		Last Modified: Wed, 14 Oct 2020 21:12:16 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37d2486511a0c9601a2bdd89e2ebd54297bb2c78735b569e84014aa00cfb6d3`  
		Last Modified: Wed, 14 Oct 2020 21:12:21 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1435a16a8f89084f597da43cb9ce1413ac817712fad3e6683dd165dc7cc36296`  
		Last Modified: Wed, 14 Oct 2020 21:12:14 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9479319b79d0a97d0b6d91034585fb6f52136095829c563c4b36d57bdfe54c23`  
		Last Modified: Wed, 14 Oct 2020 21:12:15 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f84c09f0f902199fdd83bb5ec0da426140430cf1ae9b37d63635d70b45ddad`  
		Last Modified: Wed, 14 Oct 2020 21:12:13 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c89752e1d722e1a2bdb8c5936cbf20f3ca2c699136b1279ac27f93b75110cf`  
		Last Modified: Wed, 14 Oct 2020 21:12:11 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b75e4a8389cdb23c1d9ebf7fc2e685469542f5e1ac0f7a32e1818e04001d88`  
		Last Modified: Wed, 14 Oct 2020 21:12:11 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58bcc9da6dff9ee1073dd37c941b628f26ee80400f5a9e8c2bbbd8749815c42`  
		Last Modified: Wed, 14 Oct 2020 21:12:11 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46327701e2d8e59d0173f0db37999a9d1e633a41f36e739bfe94a37c34406aee`  
		Last Modified: Wed, 14 Oct 2020 21:12:11 GMT  
		Size: 269.3 KB (269317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd16f3084947685df6d6043025f0d44efccb637918ffc69bbebafea7e3c94970`  
		Last Modified: Wed, 14 Oct 2020 21:12:11 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-windowsservercore-1809`

```console
$ docker pull caddy@sha256:f2ae6026ebddfb02e729d888f5b5399c0bd6cbb64fe2412afc29ee983cdeaa30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `caddy:2.1.1-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull caddy@sha256:66f70d738fddf55c60091b6aef8e41b63c76802b802ab717413fe9c818037124
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2401370099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1397040752ad41e2b18db058da0b7e519033692fcea840d807a898de17943dde`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 20:55:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Oct 2020 20:55:53 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 14 Oct 2020 20:56:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Oct 2020 20:56:28 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Oct 2020 20:56:29 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Oct 2020 20:56:30 GMT
VOLUME [c:/config]
# Wed, 14 Oct 2020 20:56:30 GMT
VOLUME [c:/data]
# Wed, 14 Oct 2020 20:56:31 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 14 Oct 2020 20:56:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Oct 2020 20:56:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Oct 2020 20:56:34 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Oct 2020 20:56:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Oct 2020 20:56:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Oct 2020 20:56:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Oct 2020 20:56:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Oct 2020 20:56:37 GMT
EXPOSE 80
# Wed, 14 Oct 2020 20:56:38 GMT
EXPOSE 443
# Wed, 14 Oct 2020 20:56:39 GMT
EXPOSE 2019
# Wed, 14 Oct 2020 20:56:55 GMT
RUN caddy version
# Wed, 14 Oct 2020 20:56:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b188d60ff330af293d4e64c0e8d02efc672b84164a7f28c2b88c6fa69e773b`  
		Last Modified: Wed, 14 Oct 2020 21:11:59 GMT  
		Size: 9.2 MB (9238100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7cca4341580aaef49dda3a35fbe74dea069dea552f29d609095c28ae31c7c9`  
		Last Modified: Wed, 14 Oct 2020 21:11:55 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bc6acc9f3a56b460718597090a53b19d8ae56936b8c1f305a0fc5b6c8ae834`  
		Last Modified: Wed, 14 Oct 2020 21:12:01 GMT  
		Size: 17.7 MB (17721908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59da2dbe8389d72a6c47be48a14049de1017ecd0bfe42e9b39137feb681a86e2`  
		Last Modified: Wed, 14 Oct 2020 21:11:55 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08f4acb6066947f91cc9e9472c80e0f37f13d618d651351b8b3d6efd0d972d9`  
		Last Modified: Wed, 14 Oct 2020 21:11:54 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc07733f0dbd5754df935d2dd9eb9b99ec6a8833f5801ce1d28dfbd5dc06537d`  
		Last Modified: Wed, 14 Oct 2020 21:11:52 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f794342b0d24d7695630534ed119afcfd13154a5661e49b0fb63a9d09239389`  
		Last Modified: Wed, 14 Oct 2020 21:11:52 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f8231f3a84092e779185d6075769d2024c8ca7743081f3c9da45468d7f3550`  
		Last Modified: Wed, 14 Oct 2020 21:11:52 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e35f7ff6908cb027518acbf4190fa1665763a290334d11445f85785ee2b6eb6`  
		Last Modified: Wed, 14 Oct 2020 21:11:52 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a6ac3896b488a27e5a2289f4a62b934db8638756d02666690ff6e80621f0b3`  
		Last Modified: Wed, 14 Oct 2020 21:11:52 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42fa5374e20ab60dd6a7d2bdd71a4996a10f825e28542c0a038a25b5bc64fc10`  
		Last Modified: Wed, 14 Oct 2020 21:11:49 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f8e08e4c4e4262e9a897ff6a2366db843c277188a19522c2b3a238a70d2e92`  
		Last Modified: Wed, 14 Oct 2020 21:11:49 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2309bc178193a0f7b99147d5aabc6bfb9a799756c1893656a74c945570438c75`  
		Last Modified: Wed, 14 Oct 2020 21:11:48 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c0747bfbf50db12f814e3dea2b3a71b1bb951fc8f401365199cf535793880b`  
		Last Modified: Wed, 14 Oct 2020 21:11:49 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492e7f435eff381b7d6b25eb81362a6c0fd4b461ddc05978afdfaf175ff99756`  
		Last Modified: Wed, 14 Oct 2020 21:11:48 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d5be9e7e60f33a1a982e2fd5a12de9103b8c6c763d561b14577abf49c36209`  
		Last Modified: Wed, 14 Oct 2020 21:11:45 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e705ffea3945c47a37e15327ec3683dbc90a9e05a214b10f7384f782dd4d066c`  
		Last Modified: Wed, 14 Oct 2020 21:11:46 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a59c3c8fe6d1b33da8d76616405e7bf142019d8d8e2a5d372496773d29a50f5`  
		Last Modified: Wed, 14 Oct 2020 21:11:46 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e00a541946fdd8a1f98a5d34d51dca7bd037860ba1aa2a85c978213e80d25f`  
		Last Modified: Wed, 14 Oct 2020 21:11:46 GMT  
		Size: 299.5 KB (299487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17888b1c5a918fe0001ed5ea3f284e619eaa9c54b6de64d7f8def19bc9a4f7f7`  
		Last Modified: Wed, 14 Oct 2020 21:11:46 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:c300df341bc8b99cf983b6073f4bbf660ec3d1b4047cb274e3e00c5b19e26128
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64

### `caddy:2.1.1-windowsservercore-ltsc2016` - windows version 10.0.14393.3986; amd64

```console
$ docker pull caddy@sha256:3df3617581091c8a721884e7886ef930f68708e6be320bd2252ef6f490f2512e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5774462347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cc16ee492900dee7e9f4e124e5439d5a2a26376ffe0e4c4b85461f0907b2abf`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 20:58:29 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Oct 2020 20:58:30 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 14 Oct 2020 20:59:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Oct 2020 21:00:00 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Oct 2020 21:00:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Oct 2020 21:00:03 GMT
VOLUME [c:/config]
# Wed, 14 Oct 2020 21:00:04 GMT
VOLUME [c:/data]
# Wed, 14 Oct 2020 21:00:05 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 14 Oct 2020 21:00:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Oct 2020 21:00:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Oct 2020 21:00:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Oct 2020 21:00:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Oct 2020 21:00:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Oct 2020 21:00:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Oct 2020 21:00:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Oct 2020 21:00:11 GMT
EXPOSE 80
# Wed, 14 Oct 2020 21:00:11 GMT
EXPOSE 443
# Wed, 14 Oct 2020 21:00:12 GMT
EXPOSE 2019
# Wed, 14 Oct 2020 21:00:53 GMT
RUN caddy version
# Wed, 14 Oct 2020 21:00:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0621c6e14481e8b7931a54a60b5f552ab50344f6a75362eb856e08a00a6e121d`  
		Last Modified: Wed, 14 Oct 2020 21:12:28 GMT  
		Size: 9.9 MB (9924480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4a1346a3116e78ed00103d93f985d7f4bf3df06cb8088bca9b316cc656a1b8`  
		Last Modified: Wed, 14 Oct 2020 21:12:24 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828c93647c40ffc8bcbe621b61aef3677861ae673ef3b66ac1792c99c95234d9`  
		Last Modified: Wed, 14 Oct 2020 21:12:30 GMT  
		Size: 22.9 MB (22896440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4726960f8ff938227c56d540f881d9bc18e607f3301cd3cead8b652ec7ef517`  
		Last Modified: Wed, 14 Oct 2020 21:12:21 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b5e13596b93a65158bebc3e1cfb8345e098bd9a27f4171069026fc575224d8`  
		Last Modified: Wed, 14 Oct 2020 21:12:21 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06356772b928f71cb618db080d52bdca9588cf499ea10913136623ea3c89ac9d`  
		Last Modified: Wed, 14 Oct 2020 21:12:19 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35687f4e534a86ba4f3538c39b22db8a401bc0335da0a91c471f9eff0e934abd`  
		Last Modified: Wed, 14 Oct 2020 21:12:21 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0234c902cd868cb06435cb99ba8470182d7955305dd550a6f9e85dfdbf0589`  
		Last Modified: Wed, 14 Oct 2020 21:12:18 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdc33faacf12c704737e72c800eaa28e3da94d8ed7df679e786358a09d471bf`  
		Last Modified: Wed, 14 Oct 2020 21:12:18 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550f0814377cdb217e3609cccb0c763feeab8b5f8a35b447a95dfd89ed1cad48`  
		Last Modified: Wed, 14 Oct 2020 21:12:17 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c94837bff217cff65168fc6eebe67956699dbee13427803f6970aa8f224dc10`  
		Last Modified: Wed, 14 Oct 2020 21:12:16 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37d2486511a0c9601a2bdd89e2ebd54297bb2c78735b569e84014aa00cfb6d3`  
		Last Modified: Wed, 14 Oct 2020 21:12:21 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1435a16a8f89084f597da43cb9ce1413ac817712fad3e6683dd165dc7cc36296`  
		Last Modified: Wed, 14 Oct 2020 21:12:14 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9479319b79d0a97d0b6d91034585fb6f52136095829c563c4b36d57bdfe54c23`  
		Last Modified: Wed, 14 Oct 2020 21:12:15 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f84c09f0f902199fdd83bb5ec0da426140430cf1ae9b37d63635d70b45ddad`  
		Last Modified: Wed, 14 Oct 2020 21:12:13 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c89752e1d722e1a2bdb8c5936cbf20f3ca2c699136b1279ac27f93b75110cf`  
		Last Modified: Wed, 14 Oct 2020 21:12:11 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b75e4a8389cdb23c1d9ebf7fc2e685469542f5e1ac0f7a32e1818e04001d88`  
		Last Modified: Wed, 14 Oct 2020 21:12:11 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58bcc9da6dff9ee1073dd37c941b628f26ee80400f5a9e8c2bbbd8749815c42`  
		Last Modified: Wed, 14 Oct 2020 21:12:11 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46327701e2d8e59d0173f0db37999a9d1e633a41f36e739bfe94a37c34406aee`  
		Last Modified: Wed, 14 Oct 2020 21:12:11 GMT  
		Size: 269.3 KB (269317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd16f3084947685df6d6043025f0d44efccb637918ffc69bbebafea7e3c94970`  
		Last Modified: Wed, 14 Oct 2020 21:12:11 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1`

```console
$ docker pull caddy@sha256:b44006ca7a107edd0fca2ff7a70cf75b81b20b61b722dff8a720364a3764ffd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

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

### `caddy:2.2.1` - windows version 10.0.17763.1518; amd64

```console
$ docker pull caddy@sha256:5b0edc0113282eff2b0b97cb2768aef9406975982b52b5801fe66a3b7e0f1f6b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2399991421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4a3be7f6340286c7cad100a7baf86ff095c7d81ce5c10b5c314e8d7e73a9ade`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 21:03:47 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Oct 2020 21:03:48 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 14 Oct 2020 21:04:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Oct 2020 21:04:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Oct 2020 21:04:21 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Oct 2020 21:04:22 GMT
VOLUME [c:/config]
# Wed, 14 Oct 2020 21:04:23 GMT
VOLUME [c:/data]
# Wed, 14 Oct 2020 21:04:24 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 14 Oct 2020 21:04:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Oct 2020 21:04:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Oct 2020 21:04:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Oct 2020 21:04:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Oct 2020 21:04:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Oct 2020 21:04:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Oct 2020 21:04:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Oct 2020 21:04:29 GMT
EXPOSE 80
# Wed, 14 Oct 2020 21:04:30 GMT
EXPOSE 443
# Wed, 14 Oct 2020 21:04:30 GMT
EXPOSE 2019
# Wed, 14 Oct 2020 21:04:46 GMT
RUN caddy version
# Wed, 14 Oct 2020 21:04:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590b685e6f8e8fa4cbca8ce94e257baf1c179f183afabfc59bdff4420027e080`  
		Last Modified: Wed, 14 Oct 2020 21:13:24 GMT  
		Size: 9.2 MB (9237870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8a16e6bfc40544aeeaa55e8406570aec66018352db80098da3663138201f74`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468f02630a43054839d6262fe9f0d41cdd551ab83bbbb35c26cd9ead72ce6985`  
		Last Modified: Wed, 14 Oct 2020 21:13:25 GMT  
		Size: 16.3 MB (16343904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcdb09f7b5a57cb7fce28be7e54975dfc770735e4570b259b9104ddc8421bbd`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4b2b1c53bbf344fa90b58a9d5ee4b990881289dde49074cecd1f0da649c20a`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01bade2ee2333f9cd004bd1812f0c1fc7f55b2297cf57b8343e17b48c9d3535`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b312fdc7f27df222f05918031d72e4457582b08c8fdeff7cde88a6a402b6f0c`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053d376e7f1eb8e50a394d7247f16006d36ae65144e75d37fe8bb0740d91695f`  
		Last Modified: Wed, 14 Oct 2020 21:13:18 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d88dd9c5821fcba44cce1002ed12b8702e0cbec6ee8d137cbec8e5bd145acd5`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca72f02c89a70e463873f7095a54263f02a7dc1fc35b8b3d92d0d6ed1114e1c3`  
		Last Modified: Wed, 14 Oct 2020 21:13:16 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744bfb9438a82d19472dbb92037ab018420b16a677b9451e9b92d13d9d4cc309`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab7908db3cd309e1cf3200fc5b51374d626702ea4ff411559cfa15da77b097d`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691b1b3fc24e5b473537703fcabf8cdc0acd56705ab671452b135de184ffbe0c`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba327018ef360de6c48ecbdb06f66a73defdb3996be6c2f17f0731514dbece5`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c122dffbcf7af8877cc67b8f468cd74a76d63a739b85f3ac429fb27794f724`  
		Last Modified: Wed, 14 Oct 2020 21:13:13 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbf77f12be69367c8fcf09b53209ec5b25083762192120e9ed3f8e429569a4f`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c631d9175a05b1f8c784df5ccc0daeda8990f4cfa0faebc76e525dc737e034`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b5835866e9c4e5a927e7b41da88a4c61a54547cc83fc91db1c1a43494bbac2`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13669d36e52f3d6963333d5102e23ad22fd5892d4fd1a9468f12194c39c2753`  
		Last Modified: Wed, 14 Oct 2020 21:13:11 GMT  
		Size: 299.0 KB (299047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f0e09c2bd5ebc6729c8f1d852f4adefae35e2335cd7dbbcc09c95205e95ab0`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1` - windows version 10.0.14393.3986; amd64

```console
$ docker pull caddy@sha256:4c7f9ebc39d2e00064b805df702d5364f55de8cb8cf5ae58d8e4f438988069e8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5773083905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0ce891f0605eaed2c51c683e9fe3d70f29bf6588b85b1f2be21dfcba2c4fb3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 21:06:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Oct 2020 21:06:25 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 14 Oct 2020 21:07:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Oct 2020 21:07:57 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Oct 2020 21:07:58 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Oct 2020 21:07:59 GMT
VOLUME [c:/config]
# Wed, 14 Oct 2020 21:08:00 GMT
VOLUME [c:/data]
# Wed, 14 Oct 2020 21:08:01 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 14 Oct 2020 21:08:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Oct 2020 21:08:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Oct 2020 21:08:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Oct 2020 21:08:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Oct 2020 21:08:05 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Oct 2020 21:08:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Oct 2020 21:08:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Oct 2020 21:08:08 GMT
EXPOSE 80
# Wed, 14 Oct 2020 21:08:08 GMT
EXPOSE 443
# Wed, 14 Oct 2020 21:08:09 GMT
EXPOSE 2019
# Wed, 14 Oct 2020 21:08:53 GMT
RUN caddy version
# Wed, 14 Oct 2020 21:08:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2b4a4f0660702b9f47920e1e7ea79666ac43584dadc8412d8a7b7eb0490a2c`  
		Last Modified: Wed, 14 Oct 2020 21:13:59 GMT  
		Size: 9.9 MB (9925104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3c401ae3441b3e5b7543d5482214980c1c14958e2713fee5966c2622a53963`  
		Last Modified: Wed, 14 Oct 2020 21:13:55 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffab013bf500710ef95125418f98138723e756c560a1de0145379662b77335db`  
		Last Modified: Wed, 14 Oct 2020 21:14:00 GMT  
		Size: 21.5 MB (21518510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcf1f0773bd9f450a654eb5dcecd55e2e3fe3ba01eb0dae7dbf27e84402a6be`  
		Last Modified: Wed, 14 Oct 2020 21:13:53 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7077da12d3b43ef9b9dad1d8c770898c3a0224a8a0a3b99dc4656cc594d09b62`  
		Last Modified: Wed, 14 Oct 2020 21:13:53 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3976aabb2b169dd3bb85d39e2473fe70f7f15de0124b56095dd3c25fbbc27c`  
		Last Modified: Wed, 14 Oct 2020 21:13:52 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e5576c4d0eac332d8332455193ed1057c55aa90bd5e9a6bca884a25623c3c8`  
		Last Modified: Wed, 14 Oct 2020 21:13:52 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7210dc7c5fabd3bf6636614bc150a0965808e559f2b293340b4d8e049a185684`  
		Last Modified: Wed, 14 Oct 2020 21:13:50 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7af1dab2b20db7484c30ac3175b1dc3b89884f843ece3209fdab4882f5e018`  
		Last Modified: Wed, 14 Oct 2020 21:13:49 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe18c02535b810df5a6916e6ffe0a4532c5a70dae17b5ce28956695be585480`  
		Last Modified: Wed, 14 Oct 2020 21:13:50 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb1797af36c3af3ecc1e7db5ddfdba44c6bfff97b0515b3463d0948fed92ac4`  
		Last Modified: Wed, 14 Oct 2020 21:13:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98a2d0f6d0934d8a3b866e68ca5e7775b2af52b170aa71f2113de2d32d532a3`  
		Last Modified: Wed, 14 Oct 2020 21:13:48 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f14b6955af73ac11170ddb2c596a1dd963ceafda86300b2de8466357d56aa4`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ce0d3817eff364f0101431f28cb70cde3766120bbe5fb10b53ebf59363136f`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dd973289c284ff507f57773413c00c41a54ad2015bafb509c68a044b609cda`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6c2b7b482e55dcb167623e29563231f659e1a523cb8f6e83423bb1d69a2014`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7811e07229200779f1a17a1899bf48c49f0250685f18fdffb38ee7c30ab779`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d7cb4258c8b7eab1c92df575a363d8685d8d783672e5256208f715c662b27b`  
		Last Modified: Wed, 14 Oct 2020 21:13:44 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ab63ba04ec1b983074014465794ebf2e437ec4c03997ac40e1be3a4abcce61`  
		Last Modified: Wed, 14 Oct 2020 21:13:44 GMT  
		Size: 268.2 KB (268209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac54f9c3e58e5d406091c73dec798c29e2ee3134663b63d3ddb4959f10f4f32`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.2 KB (1152 bytes)  
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
$ docker pull caddy@sha256:d1feb42feaf8542d7efe2afee44c2a57540f14deb3961b86aa0b7ee6de1b7c77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

### `caddy:2.2.1-builder` - linux; amd64

```console
$ docker pull caddy@sha256:b506e57149af1435025a622cd356fc93257f02130f1e721a1a067362b1f88ddd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.7 MB (119671750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05d3a71d119dcebe678d25c39ff3d11b63d842f1cd4756e133e9c3a4faa0fe38`
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
# Thu, 22 Oct 2020 03:34:57 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 03:37:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 03:37:52 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 03:37:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 03:37:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 03:37:54 GMT
WORKDIR /go
# Thu, 22 Oct 2020 04:34:16 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 04:34:16 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 04:34:16 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 04:34:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 04:34:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 04:34:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 04:34:20 GMT
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
	-	`sha256:0eba1c9be4d292e332c2f27b821e199d8603b724238d9a4ce48c566533546298`  
		Last Modified: Thu, 22 Oct 2020 03:44:16 GMT  
		Size: 106.9 MB (106876307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d57e429df01b9589550363e9badf8beb2c0ef2cfb959fb7389948decaccc71f`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf71de68668ac772e9853d42397c63e34666b964b958c23d49616ecbd9df286`  
		Last Modified: Thu, 22 Oct 2020 04:35:15 GMT  
		Size: 8.3 MB (8309874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b116073137746923179401de3108b0ceda969a41fee25a4b097c75eaafee084`  
		Last Modified: Thu, 22 Oct 2020 04:35:14 GMT  
		Size: 1.4 MB (1407214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d809710fb5305cf38c3119a76bd45b286b83f7501326896adc101338a4766e`  
		Last Modified: Thu, 22 Oct 2020 04:35:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2f447ef196725a6fe1129ccca0b74d23ff3dfb38887d56e618348db89feae116
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114815426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b367cdbe3af19cc3dd00928134ec76ddeef267a733cb88a2e1c97b67a113b480`
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
# Thu, 22 Oct 2020 03:07:28 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 04:07:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 04:07:33 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 04:07:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 04:09:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 04:09:37 GMT
WORKDIR /go
# Thu, 22 Oct 2020 10:05:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 10:05:06 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 10:05:08 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 10:05:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 10:05:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 10:05:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 10:05:13 GMT
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
	-	`sha256:0861c41718d28217202ec1937beb9975a5bee4aec22544789a4941342423d823`  
		Last Modified: Thu, 22 Oct 2020 05:35:25 GMT  
		Size: 102.7 MB (102675647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189a4b66c7697ec4dec0236745f1b2130dd6699149d2259637327eef2d8fb5a3`  
		Last Modified: Thu, 22 Oct 2020 05:34:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43299b1fec8de48d0860d111e16df032ff921ceb1bfe97430ebe2d9c67900d99`  
		Last Modified: Thu, 22 Oct 2020 10:05:40 GMT  
		Size: 7.9 MB (7928833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4e67b21208cda0253a4fdeefdc15a2990ded4af282530e328cd7b48914ce8d`  
		Last Modified: Thu, 22 Oct 2020 10:05:38 GMT  
		Size: 1.3 MB (1327348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d25b580938f0aedbca674d485edf5de24f1e51289d0e2317ea8d1040f2fcaac`  
		Last Modified: Thu, 22 Oct 2020 10:05:38 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:53f07e930bd2ec03da216d3e8325f74985e425cfa28e027307b2165a68d918d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113627797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7140db1472303a8077c6b1e7cacc69b2d2594c3732b60b2a1c66257928694bd4`
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
# Thu, 22 Oct 2020 03:23:43 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 04:38:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 04:38:54 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 04:39:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 04:41:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 04:41:39 GMT
WORKDIR /go
# Thu, 22 Oct 2020 09:24:49 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 09:24:50 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 09:24:51 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 09:24:52 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 09:24:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 09:24:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 09:24:55 GMT
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
	-	`sha256:8cedb62f6546fc1b0d4fa80e293634cefa26d2336796ea8e8bc24eabc9bc501e`  
		Last Modified: Thu, 22 Oct 2020 06:00:08 GMT  
		Size: 102.5 MB (102470699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a88c985904d22a6adc07851b517bd17b6624e2b422ff3dfe8375de1283250d8`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc68f5c354cb3e9a5328b0f6341317092ad7a6081c8f1791c3857d479f79065`  
		Last Modified: Thu, 22 Oct 2020 09:25:24 GMT  
		Size: 7.1 MB (7144783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d905d9db6b8b7d05de2a2d569e2e8a9b617e197168db24c50a0fc2e6583f878`  
		Last Modified: Thu, 22 Oct 2020 09:25:24 GMT  
		Size: 1.3 MB (1325844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cb350ca3cb778c3ae223b0b0d844902b1ee234c91aa18341eaafc3a91cdc39`  
		Last Modified: Thu, 22 Oct 2020 09:25:22 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:33f8ff597086154bb625661b95eb1cf0ad74284a3fc00917506f2961ccc29a65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.0 MB (114950741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95c2f36f633ba51a79c3441793ba3bac5aa172347ccdbb8c8f371ce9e1e5fb41`
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
# Thu, 22 Oct 2020 04:10:13 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 04:15:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 04:15:31 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 04:15:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 04:17:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 04:17:40 GMT
WORKDIR /go
# Thu, 22 Oct 2020 09:30:37 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 09:30:38 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 09:30:45 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 09:30:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 09:30:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 09:30:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 09:30:59 GMT
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
	-	`sha256:5afe5f37f5b3016b6946fda75a1f4dce7778311971998bab26064ee548e69e57`  
		Last Modified: Thu, 22 Oct 2020 04:29:46 GMT  
		Size: 102.2 MB (102152165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d0fcabf3d036cdbe487c24ebdc36aa0cf4c2700b5b386791a3538d92071a62`  
		Last Modified: Thu, 22 Oct 2020 04:28:23 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466fde6265bf309aca5041a30a19ba0f889387ceb0872309caa82fd6531b221a`  
		Last Modified: Thu, 22 Oct 2020 09:31:34 GMT  
		Size: 8.5 MB (8499894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82672d1571ea79e8c88077d08e3c7022c89e0494a79368f22dd09e069761eeca`  
		Last Modified: Thu, 22 Oct 2020 09:31:32 GMT  
		Size: 1.3 MB (1310181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b29dbb8417e8cdce10eeeb84f0d7f37da96a00c256648362fd0a1130013462c`  
		Last Modified: Thu, 22 Oct 2020 09:31:32 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:1381ebb3e36c7f726363e75544a7cf23e07e34c50595cb35af607d6ead7655bf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.1 MB (114109814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8378d7f685f94342d985ca619645498434b64a6d62b7bf884dbb57030e7d923`
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
# Thu, 22 Oct 2020 13:27:55 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 13:30:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 13:30:31 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 13:30:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 13:30:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 13:30:50 GMT
WORKDIR /go
# Thu, 22 Oct 2020 13:45:58 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 13:46:02 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 13:46:10 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 13:46:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 13:46:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 13:46:34 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 13:46:37 GMT
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
	-	`sha256:a53757254f83d2b7412aa2718828ed0bd489d01d5bad2c6ee877672775244a8a`  
		Last Modified: Thu, 22 Oct 2020 13:36:50 GMT  
		Size: 100.8 MB (100814882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6876bebeafd85e7b46e88239c365eeec0a308353e7d1f7de434659ef597f889d`  
		Last Modified: Thu, 22 Oct 2020 13:36:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60beda9dadec93f6e90d3398b12787fc49427a3ba3a7e88e42e6105562016ec6`  
		Last Modified: Thu, 22 Oct 2020 13:48:15 GMT  
		Size: 8.9 MB (8920001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ca79d64160e09790e775af1b4204add8e6f21a3e837e1bd743c9b7b6b9c24a`  
		Last Modified: Thu, 22 Oct 2020 13:48:14 GMT  
		Size: 1.3 MB (1287791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7348aa6f5d47e3ce5091866c5cc3341d13a31faad6b1aa33e76e9432f45506a`  
		Last Modified: Thu, 22 Oct 2020 13:48:13 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - linux; s390x

```console
$ docker pull caddy@sha256:a8aa50ea100e687faa5739a6f62ec5843fc9846c874337726fed6ba09f3ac315
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118526471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7efeb3f913cdd9cdf7a017801f525a164c24a2efd93d1eb010477ca4094ac251`
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
# Thu, 22 Oct 2020 02:53:31 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 02:55:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 02:55:33 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 02:55:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 02:55:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 02:55:35 GMT
WORKDIR /go
# Thu, 22 Oct 2020 10:13:52 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 10:13:53 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 10:13:54 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 10:13:54 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 10:13:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 10:13:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 10:13:57 GMT
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
	-	`sha256:93a9f4b10b0ce05491e77b29b87fa3bbcbcd40e10a492d96185bf5ef0acc62f0`  
		Last Modified: Thu, 22 Oct 2020 02:58:45 GMT  
		Size: 105.9 MB (105937593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c973fb648f38c29beb5231f712f726631c6eb8fdaefbd4b7ac5408af2ea1a61`  
		Last Modified: Thu, 22 Oct 2020 02:58:32 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ff827958d5db211b007a45cc274d0658dcb49f4949f86888fa5f731d8df24a`  
		Last Modified: Thu, 22 Oct 2020 10:14:27 GMT  
		Size: 8.4 MB (8352218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36fa21e3b269069073c65c60c20545573892ddcd3d507593bc28a325da2b8c2`  
		Last Modified: Thu, 22 Oct 2020 10:14:26 GMT  
		Size: 1.4 MB (1388754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472fde2a1575da1d5a5924aab83ea94739ae66686513f4cfa7cd844707b59058`  
		Last Modified: Thu, 22 Oct 2020 10:14:26 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - windows version 10.0.17763.1518; amd64

```console
$ docker pull caddy@sha256:5f0ba224d2ff94370fd2e10a05b2e06f062b1e9ba4278b62e9ecb99056ff4802
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2549102284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a10b666950b6ddd3242011e2bf926b6d52b2bb6f910ac359ac1b4b08e6db235c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 12:27:03 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Oct 2020 12:27:04 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Oct 2020 12:27:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Oct 2020 12:27:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Oct 2020 12:28:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Oct 2020 12:28:38 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Oct 2020 12:29:02 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 15 Oct 2020 01:14:39 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 15 Oct 2020 01:17:39 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1d579d0e980763f60bf43afb7c3783caf63433a485731ef4d2e262878d634b3f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 15 Oct 2020 01:17:40 GMT
WORKDIR C:\gopath
# Thu, 15 Oct 2020 02:32:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 15 Oct 2020 02:32:16 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 15 Oct 2020 02:32:17 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 15 Oct 2020 02:32:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 15 Oct 2020 02:32:40 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 15 Oct 2020 02:32:41 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23a75d88f9f5980bb112e2c28248975f107144d8d2e40dc4755e2a09f5e56df`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bea6d8b9d9b014ffa471b7bb8882ddb7e9d378ddcacc099f0710073bd6361b9`  
		Last Modified: Wed, 14 Oct 2020 12:50:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75c1905c0573cc5706bc066d23624f0e92a8871832c744fbe7eabdcbc6f8a85`  
		Last Modified: Wed, 14 Oct 2020 12:50:24 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938695376d9deeba8819539ff3245935c28f93229d1c332bb8b6a16e67013fbc`  
		Last Modified: Wed, 14 Oct 2020 12:50:23 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41106c6a476cf9666c6d8c3c853c982a841c29db05b3ef8a072baba537b6d74c`  
		Last Modified: Wed, 14 Oct 2020 12:50:48 GMT  
		Size: 34.3 MB (34312667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d6d6258831f87f3b455e6316e2bed430465a760272614de7cdd28c7c6e9f3e`  
		Last Modified: Wed, 14 Oct 2020 12:50:19 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e3f66638c4d5ce9adba16e49844f57efbab1d628d9d6c73133511b7c1c3892`  
		Last Modified: Wed, 14 Oct 2020 12:50:20 GMT  
		Size: 310.5 KB (310525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe34732f84b95b980d0ae0624ebae44818ef7879e34a9ffbebe752f1dcd4badf`  
		Last Modified: Thu, 15 Oct 2020 02:05:08 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a6c4c70f4e593c0500bebe3fa23edab8bd791805ab4a5edf34cb053b21264f`  
		Last Modified: Thu, 15 Oct 2020 02:05:35 GMT  
		Size: 138.6 MB (138590451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123678d8baa038225b16066bfa2f971f7454f2d5b16b95db1663954869cf837a`  
		Last Modified: Thu, 15 Oct 2020 02:05:07 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99abf6100e15da95d12aff85cd77f0adf4d96b7b1b2815445a9fc6f576c3df79`  
		Last Modified: Thu, 15 Oct 2020 02:35:13 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908a905e414249fe5a6b10921f1505b4e5edb7bad45fd2f70a3095f99e8d3929`  
		Last Modified: Thu, 15 Oct 2020 02:35:10 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beea46a5312f34364874857e7fdd21b76239ae4028aeabd8ef4e7092e536fda0`  
		Last Modified: Thu, 15 Oct 2020 02:35:09 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb245ad725b068d3bb29ee875394207d019d445c185bf1ca1ddd2ce1c62ce38`  
		Last Modified: Thu, 15 Oct 2020 02:35:10 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9cd8369d2f668d2d300f35c9d9ee98488040b7b695efbaadb1d3b76f314eac`  
		Last Modified: Thu, 15 Oct 2020 02:35:10 GMT  
		Size: 1.8 MB (1783668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798dfde6e8213d06ef180571d9c1956e9b42899062509ff88cfbc453b3ff9c37`  
		Last Modified: Thu, 15 Oct 2020 02:35:09 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - windows version 10.0.14393.3986; amd64

```console
$ docker pull caddy@sha256:8fea2fa2956f6e7eb56eb8f745fe7b6f4a7ccf45bd259d7a8cccb3d2c71f3c1f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5941324722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4f39f7f404783da13552d7024d9a3262d0d6a1834385977fb514556a43e41f9`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 12:31:45 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Oct 2020 12:31:46 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Oct 2020 12:31:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Oct 2020 12:31:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Oct 2020 12:33:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Oct 2020 12:33:58 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Oct 2020 12:35:13 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 15 Oct 2020 01:17:52 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 15 Oct 2020 01:21:40 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1d579d0e980763f60bf43afb7c3783caf63433a485731ef4d2e262878d634b3f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 15 Oct 2020 01:21:41 GMT
WORKDIR C:\gopath
# Thu, 15 Oct 2020 02:32:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 15 Oct 2020 02:32:47 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 15 Oct 2020 02:32:48 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 15 Oct 2020 02:32:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 15 Oct 2020 02:34:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 15 Oct 2020 02:34:06 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528ba1d9759adcc464112008fe49672e1f545981d69bab31186587ab32f92138`  
		Last Modified: Wed, 14 Oct 2020 12:51:33 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53bf4e6180661653575845d30a4d882dea92f395cb540b1cdf91170e9ee58731`  
		Last Modified: Wed, 14 Oct 2020 12:51:30 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e973f094614bb2cebe16df6f6004c05895ed077151aecdbbd0c476513054fc`  
		Last Modified: Wed, 14 Oct 2020 12:51:25 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1089b875ac355097876e23760dd2166f096a8645e312660ffd3c0e617a2df9a0`  
		Last Modified: Wed, 14 Oct 2020 12:51:29 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8934a016b666d0691307c6414d84c36eb82de4b2fc4d74dd04c75f632dc3a78c`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 35.0 MB (35016991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4d95d13c0a45aa19a623e51cb112530a589a3a4d15d5c119610f8196912fab`  
		Last Modified: Wed, 14 Oct 2020 12:51:20 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf8226941bb8f5af9f2be8fdb54da3e3caef344b0061a73e3debde23a55e98f`  
		Last Modified: Wed, 14 Oct 2020 12:51:24 GMT  
		Size: 9.9 MB (9870100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b8d8683ed903732b7672eb374d957e4ad20a8936cd48bc9a69059c19163325`  
		Last Modified: Thu, 15 Oct 2020 02:05:58 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38f6e003c1013456c5993d4c122314dab53690c52405c373b2055e636353e47`  
		Last Modified: Thu, 15 Oct 2020 02:06:27 GMT  
		Size: 143.8 MB (143758677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbc6767c79760c5d4cd356ae2dd0742f8d13be9298959aa3009b1e4d2c18cbc`  
		Last Modified: Thu, 15 Oct 2020 02:05:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba9f5f016316461f4d80f3defd59bad0cd10886ae46ef3ad8802facb8a3330b`  
		Last Modified: Thu, 15 Oct 2020 02:35:33 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b074f2cce57588dbf6e04970c0be7db19be264eee3f4bb3a7b4bbcf4fd717b95`  
		Last Modified: Thu, 15 Oct 2020 02:35:30 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b1d6dbe2c318375f7055dc79b3b4b44a06e13238cb914eddfb5cfa258f86c6`  
		Last Modified: Thu, 15 Oct 2020 02:35:30 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c349a444d08c6b059ed2430ee7e28766f5ac7a411eeadb73dad01e26fc70916`  
		Last Modified: Thu, 15 Oct 2020 02:35:30 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1bc4e5aa1948e251b46da1e6c6c5632371f1bf5a60c64269247ec5d348fb22`  
		Last Modified: Thu, 15 Oct 2020 02:35:33 GMT  
		Size: 11.3 MB (11312385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed394fa51b2433c7ce756430011e4cc52ac6d67198f2bf0ae8144eafa44a2a89`  
		Last Modified: Thu, 15 Oct 2020 02:35:31 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-builder-alpine`

```console
$ docker pull caddy@sha256:a42199f0a07411337da8367217434680136db2e93e04b596aa8d9399325f25f6
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
$ docker pull caddy@sha256:b506e57149af1435025a622cd356fc93257f02130f1e721a1a067362b1f88ddd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.7 MB (119671750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05d3a71d119dcebe678d25c39ff3d11b63d842f1cd4756e133e9c3a4faa0fe38`
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
# Thu, 22 Oct 2020 03:34:57 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 03:37:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 03:37:52 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 03:37:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 03:37:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 03:37:54 GMT
WORKDIR /go
# Thu, 22 Oct 2020 04:34:16 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 04:34:16 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 04:34:16 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 04:34:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 04:34:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 04:34:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 04:34:20 GMT
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
	-	`sha256:0eba1c9be4d292e332c2f27b821e199d8603b724238d9a4ce48c566533546298`  
		Last Modified: Thu, 22 Oct 2020 03:44:16 GMT  
		Size: 106.9 MB (106876307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d57e429df01b9589550363e9badf8beb2c0ef2cfb959fb7389948decaccc71f`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf71de68668ac772e9853d42397c63e34666b964b958c23d49616ecbd9df286`  
		Last Modified: Thu, 22 Oct 2020 04:35:15 GMT  
		Size: 8.3 MB (8309874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b116073137746923179401de3108b0ceda969a41fee25a4b097c75eaafee084`  
		Last Modified: Thu, 22 Oct 2020 04:35:14 GMT  
		Size: 1.4 MB (1407214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d809710fb5305cf38c3119a76bd45b286b83f7501326896adc101338a4766e`  
		Last Modified: Thu, 22 Oct 2020 04:35:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2f447ef196725a6fe1129ccca0b74d23ff3dfb38887d56e618348db89feae116
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114815426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b367cdbe3af19cc3dd00928134ec76ddeef267a733cb88a2e1c97b67a113b480`
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
# Thu, 22 Oct 2020 03:07:28 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 04:07:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 04:07:33 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 04:07:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 04:09:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 04:09:37 GMT
WORKDIR /go
# Thu, 22 Oct 2020 10:05:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 10:05:06 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 10:05:08 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 10:05:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 10:05:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 10:05:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 10:05:13 GMT
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
	-	`sha256:0861c41718d28217202ec1937beb9975a5bee4aec22544789a4941342423d823`  
		Last Modified: Thu, 22 Oct 2020 05:35:25 GMT  
		Size: 102.7 MB (102675647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189a4b66c7697ec4dec0236745f1b2130dd6699149d2259637327eef2d8fb5a3`  
		Last Modified: Thu, 22 Oct 2020 05:34:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43299b1fec8de48d0860d111e16df032ff921ceb1bfe97430ebe2d9c67900d99`  
		Last Modified: Thu, 22 Oct 2020 10:05:40 GMT  
		Size: 7.9 MB (7928833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4e67b21208cda0253a4fdeefdc15a2990ded4af282530e328cd7b48914ce8d`  
		Last Modified: Thu, 22 Oct 2020 10:05:38 GMT  
		Size: 1.3 MB (1327348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d25b580938f0aedbca674d485edf5de24f1e51289d0e2317ea8d1040f2fcaac`  
		Last Modified: Thu, 22 Oct 2020 10:05:38 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:53f07e930bd2ec03da216d3e8325f74985e425cfa28e027307b2165a68d918d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113627797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7140db1472303a8077c6b1e7cacc69b2d2594c3732b60b2a1c66257928694bd4`
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
# Thu, 22 Oct 2020 03:23:43 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 04:38:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 04:38:54 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 04:39:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 04:41:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 04:41:39 GMT
WORKDIR /go
# Thu, 22 Oct 2020 09:24:49 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 09:24:50 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 09:24:51 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 09:24:52 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 09:24:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 09:24:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 09:24:55 GMT
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
	-	`sha256:8cedb62f6546fc1b0d4fa80e293634cefa26d2336796ea8e8bc24eabc9bc501e`  
		Last Modified: Thu, 22 Oct 2020 06:00:08 GMT  
		Size: 102.5 MB (102470699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a88c985904d22a6adc07851b517bd17b6624e2b422ff3dfe8375de1283250d8`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc68f5c354cb3e9a5328b0f6341317092ad7a6081c8f1791c3857d479f79065`  
		Last Modified: Thu, 22 Oct 2020 09:25:24 GMT  
		Size: 7.1 MB (7144783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d905d9db6b8b7d05de2a2d569e2e8a9b617e197168db24c50a0fc2e6583f878`  
		Last Modified: Thu, 22 Oct 2020 09:25:24 GMT  
		Size: 1.3 MB (1325844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cb350ca3cb778c3ae223b0b0d844902b1ee234c91aa18341eaafc3a91cdc39`  
		Last Modified: Thu, 22 Oct 2020 09:25:22 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:33f8ff597086154bb625661b95eb1cf0ad74284a3fc00917506f2961ccc29a65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.0 MB (114950741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95c2f36f633ba51a79c3441793ba3bac5aa172347ccdbb8c8f371ce9e1e5fb41`
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
# Thu, 22 Oct 2020 04:10:13 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 04:15:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 04:15:31 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 04:15:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 04:17:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 04:17:40 GMT
WORKDIR /go
# Thu, 22 Oct 2020 09:30:37 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 09:30:38 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 09:30:45 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 09:30:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 09:30:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 09:30:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 09:30:59 GMT
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
	-	`sha256:5afe5f37f5b3016b6946fda75a1f4dce7778311971998bab26064ee548e69e57`  
		Last Modified: Thu, 22 Oct 2020 04:29:46 GMT  
		Size: 102.2 MB (102152165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d0fcabf3d036cdbe487c24ebdc36aa0cf4c2700b5b386791a3538d92071a62`  
		Last Modified: Thu, 22 Oct 2020 04:28:23 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466fde6265bf309aca5041a30a19ba0f889387ceb0872309caa82fd6531b221a`  
		Last Modified: Thu, 22 Oct 2020 09:31:34 GMT  
		Size: 8.5 MB (8499894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82672d1571ea79e8c88077d08e3c7022c89e0494a79368f22dd09e069761eeca`  
		Last Modified: Thu, 22 Oct 2020 09:31:32 GMT  
		Size: 1.3 MB (1310181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b29dbb8417e8cdce10eeeb84f0d7f37da96a00c256648362fd0a1130013462c`  
		Last Modified: Thu, 22 Oct 2020 09:31:32 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:1381ebb3e36c7f726363e75544a7cf23e07e34c50595cb35af607d6ead7655bf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.1 MB (114109814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8378d7f685f94342d985ca619645498434b64a6d62b7bf884dbb57030e7d923`
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
# Thu, 22 Oct 2020 13:27:55 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 13:30:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 13:30:31 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 13:30:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 13:30:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 13:30:50 GMT
WORKDIR /go
# Thu, 22 Oct 2020 13:45:58 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 13:46:02 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 13:46:10 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 13:46:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 13:46:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 13:46:34 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 13:46:37 GMT
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
	-	`sha256:a53757254f83d2b7412aa2718828ed0bd489d01d5bad2c6ee877672775244a8a`  
		Last Modified: Thu, 22 Oct 2020 13:36:50 GMT  
		Size: 100.8 MB (100814882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6876bebeafd85e7b46e88239c365eeec0a308353e7d1f7de434659ef597f889d`  
		Last Modified: Thu, 22 Oct 2020 13:36:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60beda9dadec93f6e90d3398b12787fc49427a3ba3a7e88e42e6105562016ec6`  
		Last Modified: Thu, 22 Oct 2020 13:48:15 GMT  
		Size: 8.9 MB (8920001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ca79d64160e09790e775af1b4204add8e6f21a3e837e1bd743c9b7b6b9c24a`  
		Last Modified: Thu, 22 Oct 2020 13:48:14 GMT  
		Size: 1.3 MB (1287791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7348aa6f5d47e3ce5091866c5cc3341d13a31faad6b1aa33e76e9432f45506a`  
		Last Modified: Thu, 22 Oct 2020 13:48:13 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:a8aa50ea100e687faa5739a6f62ec5843fc9846c874337726fed6ba09f3ac315
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118526471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7efeb3f913cdd9cdf7a017801f525a164c24a2efd93d1eb010477ca4094ac251`
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
# Thu, 22 Oct 2020 02:53:31 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 02:55:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 02:55:33 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 02:55:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 02:55:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 02:55:35 GMT
WORKDIR /go
# Thu, 22 Oct 2020 10:13:52 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 10:13:53 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 10:13:54 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 10:13:54 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 10:13:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 10:13:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 10:13:57 GMT
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
	-	`sha256:93a9f4b10b0ce05491e77b29b87fa3bbcbcd40e10a492d96185bf5ef0acc62f0`  
		Last Modified: Thu, 22 Oct 2020 02:58:45 GMT  
		Size: 105.9 MB (105937593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c973fb648f38c29beb5231f712f726631c6eb8fdaefbd4b7ac5408af2ea1a61`  
		Last Modified: Thu, 22 Oct 2020 02:58:32 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ff827958d5db211b007a45cc274d0658dcb49f4949f86888fa5f731d8df24a`  
		Last Modified: Thu, 22 Oct 2020 10:14:27 GMT  
		Size: 8.4 MB (8352218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36fa21e3b269069073c65c60c20545573892ddcd3d507593bc28a325da2b8c2`  
		Last Modified: Thu, 22 Oct 2020 10:14:26 GMT  
		Size: 1.4 MB (1388754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472fde2a1575da1d5a5924aab83ea94739ae66686513f4cfa7cd844707b59058`  
		Last Modified: Thu, 22 Oct 2020 10:14:26 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:ab8f8e005e8197265d91e6dcb9b94990e7b89b8474a015df00bc498851522a81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `caddy:2.2.1-builder-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull caddy@sha256:5f0ba224d2ff94370fd2e10a05b2e06f062b1e9ba4278b62e9ecb99056ff4802
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2549102284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a10b666950b6ddd3242011e2bf926b6d52b2bb6f910ac359ac1b4b08e6db235c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 12:27:03 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Oct 2020 12:27:04 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Oct 2020 12:27:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Oct 2020 12:27:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Oct 2020 12:28:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Oct 2020 12:28:38 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Oct 2020 12:29:02 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 15 Oct 2020 01:14:39 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 15 Oct 2020 01:17:39 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1d579d0e980763f60bf43afb7c3783caf63433a485731ef4d2e262878d634b3f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 15 Oct 2020 01:17:40 GMT
WORKDIR C:\gopath
# Thu, 15 Oct 2020 02:32:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 15 Oct 2020 02:32:16 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 15 Oct 2020 02:32:17 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 15 Oct 2020 02:32:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 15 Oct 2020 02:32:40 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 15 Oct 2020 02:32:41 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23a75d88f9f5980bb112e2c28248975f107144d8d2e40dc4755e2a09f5e56df`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bea6d8b9d9b014ffa471b7bb8882ddb7e9d378ddcacc099f0710073bd6361b9`  
		Last Modified: Wed, 14 Oct 2020 12:50:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75c1905c0573cc5706bc066d23624f0e92a8871832c744fbe7eabdcbc6f8a85`  
		Last Modified: Wed, 14 Oct 2020 12:50:24 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938695376d9deeba8819539ff3245935c28f93229d1c332bb8b6a16e67013fbc`  
		Last Modified: Wed, 14 Oct 2020 12:50:23 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41106c6a476cf9666c6d8c3c853c982a841c29db05b3ef8a072baba537b6d74c`  
		Last Modified: Wed, 14 Oct 2020 12:50:48 GMT  
		Size: 34.3 MB (34312667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d6d6258831f87f3b455e6316e2bed430465a760272614de7cdd28c7c6e9f3e`  
		Last Modified: Wed, 14 Oct 2020 12:50:19 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e3f66638c4d5ce9adba16e49844f57efbab1d628d9d6c73133511b7c1c3892`  
		Last Modified: Wed, 14 Oct 2020 12:50:20 GMT  
		Size: 310.5 KB (310525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe34732f84b95b980d0ae0624ebae44818ef7879e34a9ffbebe752f1dcd4badf`  
		Last Modified: Thu, 15 Oct 2020 02:05:08 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a6c4c70f4e593c0500bebe3fa23edab8bd791805ab4a5edf34cb053b21264f`  
		Last Modified: Thu, 15 Oct 2020 02:05:35 GMT  
		Size: 138.6 MB (138590451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123678d8baa038225b16066bfa2f971f7454f2d5b16b95db1663954869cf837a`  
		Last Modified: Thu, 15 Oct 2020 02:05:07 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99abf6100e15da95d12aff85cd77f0adf4d96b7b1b2815445a9fc6f576c3df79`  
		Last Modified: Thu, 15 Oct 2020 02:35:13 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908a905e414249fe5a6b10921f1505b4e5edb7bad45fd2f70a3095f99e8d3929`  
		Last Modified: Thu, 15 Oct 2020 02:35:10 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beea46a5312f34364874857e7fdd21b76239ae4028aeabd8ef4e7092e536fda0`  
		Last Modified: Thu, 15 Oct 2020 02:35:09 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb245ad725b068d3bb29ee875394207d019d445c185bf1ca1ddd2ce1c62ce38`  
		Last Modified: Thu, 15 Oct 2020 02:35:10 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9cd8369d2f668d2d300f35c9d9ee98488040b7b695efbaadb1d3b76f314eac`  
		Last Modified: Thu, 15 Oct 2020 02:35:10 GMT  
		Size: 1.8 MB (1783668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798dfde6e8213d06ef180571d9c1956e9b42899062509ff88cfbc453b3ff9c37`  
		Last Modified: Thu, 15 Oct 2020 02:35:09 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:193e2b1f70d18f86f7e53052a5a343e8a9538646a3089c4eedf3e1441e7b1e4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64

### `caddy:2.2.1-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.3986; amd64

```console
$ docker pull caddy@sha256:8fea2fa2956f6e7eb56eb8f745fe7b6f4a7ccf45bd259d7a8cccb3d2c71f3c1f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5941324722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4f39f7f404783da13552d7024d9a3262d0d6a1834385977fb514556a43e41f9`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 12:31:45 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Oct 2020 12:31:46 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Oct 2020 12:31:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Oct 2020 12:31:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Oct 2020 12:33:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Oct 2020 12:33:58 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Oct 2020 12:35:13 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 15 Oct 2020 01:17:52 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 15 Oct 2020 01:21:40 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1d579d0e980763f60bf43afb7c3783caf63433a485731ef4d2e262878d634b3f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 15 Oct 2020 01:21:41 GMT
WORKDIR C:\gopath
# Thu, 15 Oct 2020 02:32:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 15 Oct 2020 02:32:47 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 15 Oct 2020 02:32:48 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 15 Oct 2020 02:32:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 15 Oct 2020 02:34:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 15 Oct 2020 02:34:06 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528ba1d9759adcc464112008fe49672e1f545981d69bab31186587ab32f92138`  
		Last Modified: Wed, 14 Oct 2020 12:51:33 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53bf4e6180661653575845d30a4d882dea92f395cb540b1cdf91170e9ee58731`  
		Last Modified: Wed, 14 Oct 2020 12:51:30 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e973f094614bb2cebe16df6f6004c05895ed077151aecdbbd0c476513054fc`  
		Last Modified: Wed, 14 Oct 2020 12:51:25 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1089b875ac355097876e23760dd2166f096a8645e312660ffd3c0e617a2df9a0`  
		Last Modified: Wed, 14 Oct 2020 12:51:29 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8934a016b666d0691307c6414d84c36eb82de4b2fc4d74dd04c75f632dc3a78c`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 35.0 MB (35016991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4d95d13c0a45aa19a623e51cb112530a589a3a4d15d5c119610f8196912fab`  
		Last Modified: Wed, 14 Oct 2020 12:51:20 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf8226941bb8f5af9f2be8fdb54da3e3caef344b0061a73e3debde23a55e98f`  
		Last Modified: Wed, 14 Oct 2020 12:51:24 GMT  
		Size: 9.9 MB (9870100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b8d8683ed903732b7672eb374d957e4ad20a8936cd48bc9a69059c19163325`  
		Last Modified: Thu, 15 Oct 2020 02:05:58 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38f6e003c1013456c5993d4c122314dab53690c52405c373b2055e636353e47`  
		Last Modified: Thu, 15 Oct 2020 02:06:27 GMT  
		Size: 143.8 MB (143758677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbc6767c79760c5d4cd356ae2dd0742f8d13be9298959aa3009b1e4d2c18cbc`  
		Last Modified: Thu, 15 Oct 2020 02:05:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba9f5f016316461f4d80f3defd59bad0cd10886ae46ef3ad8802facb8a3330b`  
		Last Modified: Thu, 15 Oct 2020 02:35:33 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b074f2cce57588dbf6e04970c0be7db19be264eee3f4bb3a7b4bbcf4fd717b95`  
		Last Modified: Thu, 15 Oct 2020 02:35:30 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b1d6dbe2c318375f7055dc79b3b4b44a06e13238cb914eddfb5cfa258f86c6`  
		Last Modified: Thu, 15 Oct 2020 02:35:30 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c349a444d08c6b059ed2430ee7e28766f5ac7a411eeadb73dad01e26fc70916`  
		Last Modified: Thu, 15 Oct 2020 02:35:30 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1bc4e5aa1948e251b46da1e6c6c5632371f1bf5a60c64269247ec5d348fb22`  
		Last Modified: Thu, 15 Oct 2020 02:35:33 GMT  
		Size: 11.3 MB (11312385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed394fa51b2433c7ce756430011e4cc52ac6d67198f2bf0ae8144eafa44a2a89`  
		Last Modified: Thu, 15 Oct 2020 02:35:31 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-windowsservercore`

```console
$ docker pull caddy@sha256:0cc9e18409440159fbf2ac241bce180b0214fc5d2358aa87fedf1189394d7469
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

### `caddy:2.2.1-windowsservercore` - windows version 10.0.17763.1518; amd64

```console
$ docker pull caddy@sha256:5b0edc0113282eff2b0b97cb2768aef9406975982b52b5801fe66a3b7e0f1f6b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2399991421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4a3be7f6340286c7cad100a7baf86ff095c7d81ce5c10b5c314e8d7e73a9ade`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 21:03:47 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Oct 2020 21:03:48 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 14 Oct 2020 21:04:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Oct 2020 21:04:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Oct 2020 21:04:21 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Oct 2020 21:04:22 GMT
VOLUME [c:/config]
# Wed, 14 Oct 2020 21:04:23 GMT
VOLUME [c:/data]
# Wed, 14 Oct 2020 21:04:24 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 14 Oct 2020 21:04:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Oct 2020 21:04:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Oct 2020 21:04:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Oct 2020 21:04:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Oct 2020 21:04:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Oct 2020 21:04:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Oct 2020 21:04:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Oct 2020 21:04:29 GMT
EXPOSE 80
# Wed, 14 Oct 2020 21:04:30 GMT
EXPOSE 443
# Wed, 14 Oct 2020 21:04:30 GMT
EXPOSE 2019
# Wed, 14 Oct 2020 21:04:46 GMT
RUN caddy version
# Wed, 14 Oct 2020 21:04:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590b685e6f8e8fa4cbca8ce94e257baf1c179f183afabfc59bdff4420027e080`  
		Last Modified: Wed, 14 Oct 2020 21:13:24 GMT  
		Size: 9.2 MB (9237870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8a16e6bfc40544aeeaa55e8406570aec66018352db80098da3663138201f74`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468f02630a43054839d6262fe9f0d41cdd551ab83bbbb35c26cd9ead72ce6985`  
		Last Modified: Wed, 14 Oct 2020 21:13:25 GMT  
		Size: 16.3 MB (16343904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcdb09f7b5a57cb7fce28be7e54975dfc770735e4570b259b9104ddc8421bbd`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4b2b1c53bbf344fa90b58a9d5ee4b990881289dde49074cecd1f0da649c20a`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01bade2ee2333f9cd004bd1812f0c1fc7f55b2297cf57b8343e17b48c9d3535`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b312fdc7f27df222f05918031d72e4457582b08c8fdeff7cde88a6a402b6f0c`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053d376e7f1eb8e50a394d7247f16006d36ae65144e75d37fe8bb0740d91695f`  
		Last Modified: Wed, 14 Oct 2020 21:13:18 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d88dd9c5821fcba44cce1002ed12b8702e0cbec6ee8d137cbec8e5bd145acd5`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca72f02c89a70e463873f7095a54263f02a7dc1fc35b8b3d92d0d6ed1114e1c3`  
		Last Modified: Wed, 14 Oct 2020 21:13:16 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744bfb9438a82d19472dbb92037ab018420b16a677b9451e9b92d13d9d4cc309`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab7908db3cd309e1cf3200fc5b51374d626702ea4ff411559cfa15da77b097d`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691b1b3fc24e5b473537703fcabf8cdc0acd56705ab671452b135de184ffbe0c`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba327018ef360de6c48ecbdb06f66a73defdb3996be6c2f17f0731514dbece5`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c122dffbcf7af8877cc67b8f468cd74a76d63a739b85f3ac429fb27794f724`  
		Last Modified: Wed, 14 Oct 2020 21:13:13 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbf77f12be69367c8fcf09b53209ec5b25083762192120e9ed3f8e429569a4f`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c631d9175a05b1f8c784df5ccc0daeda8990f4cfa0faebc76e525dc737e034`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b5835866e9c4e5a927e7b41da88a4c61a54547cc83fc91db1c1a43494bbac2`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13669d36e52f3d6963333d5102e23ad22fd5892d4fd1a9468f12194c39c2753`  
		Last Modified: Wed, 14 Oct 2020 21:13:11 GMT  
		Size: 299.0 KB (299047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f0e09c2bd5ebc6729c8f1d852f4adefae35e2335cd7dbbcc09c95205e95ab0`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-windowsservercore` - windows version 10.0.14393.3986; amd64

```console
$ docker pull caddy@sha256:4c7f9ebc39d2e00064b805df702d5364f55de8cb8cf5ae58d8e4f438988069e8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5773083905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0ce891f0605eaed2c51c683e9fe3d70f29bf6588b85b1f2be21dfcba2c4fb3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 21:06:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Oct 2020 21:06:25 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 14 Oct 2020 21:07:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Oct 2020 21:07:57 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Oct 2020 21:07:58 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Oct 2020 21:07:59 GMT
VOLUME [c:/config]
# Wed, 14 Oct 2020 21:08:00 GMT
VOLUME [c:/data]
# Wed, 14 Oct 2020 21:08:01 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 14 Oct 2020 21:08:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Oct 2020 21:08:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Oct 2020 21:08:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Oct 2020 21:08:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Oct 2020 21:08:05 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Oct 2020 21:08:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Oct 2020 21:08:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Oct 2020 21:08:08 GMT
EXPOSE 80
# Wed, 14 Oct 2020 21:08:08 GMT
EXPOSE 443
# Wed, 14 Oct 2020 21:08:09 GMT
EXPOSE 2019
# Wed, 14 Oct 2020 21:08:53 GMT
RUN caddy version
# Wed, 14 Oct 2020 21:08:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2b4a4f0660702b9f47920e1e7ea79666ac43584dadc8412d8a7b7eb0490a2c`  
		Last Modified: Wed, 14 Oct 2020 21:13:59 GMT  
		Size: 9.9 MB (9925104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3c401ae3441b3e5b7543d5482214980c1c14958e2713fee5966c2622a53963`  
		Last Modified: Wed, 14 Oct 2020 21:13:55 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffab013bf500710ef95125418f98138723e756c560a1de0145379662b77335db`  
		Last Modified: Wed, 14 Oct 2020 21:14:00 GMT  
		Size: 21.5 MB (21518510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcf1f0773bd9f450a654eb5dcecd55e2e3fe3ba01eb0dae7dbf27e84402a6be`  
		Last Modified: Wed, 14 Oct 2020 21:13:53 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7077da12d3b43ef9b9dad1d8c770898c3a0224a8a0a3b99dc4656cc594d09b62`  
		Last Modified: Wed, 14 Oct 2020 21:13:53 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3976aabb2b169dd3bb85d39e2473fe70f7f15de0124b56095dd3c25fbbc27c`  
		Last Modified: Wed, 14 Oct 2020 21:13:52 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e5576c4d0eac332d8332455193ed1057c55aa90bd5e9a6bca884a25623c3c8`  
		Last Modified: Wed, 14 Oct 2020 21:13:52 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7210dc7c5fabd3bf6636614bc150a0965808e559f2b293340b4d8e049a185684`  
		Last Modified: Wed, 14 Oct 2020 21:13:50 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7af1dab2b20db7484c30ac3175b1dc3b89884f843ece3209fdab4882f5e018`  
		Last Modified: Wed, 14 Oct 2020 21:13:49 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe18c02535b810df5a6916e6ffe0a4532c5a70dae17b5ce28956695be585480`  
		Last Modified: Wed, 14 Oct 2020 21:13:50 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb1797af36c3af3ecc1e7db5ddfdba44c6bfff97b0515b3463d0948fed92ac4`  
		Last Modified: Wed, 14 Oct 2020 21:13:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98a2d0f6d0934d8a3b866e68ca5e7775b2af52b170aa71f2113de2d32d532a3`  
		Last Modified: Wed, 14 Oct 2020 21:13:48 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f14b6955af73ac11170ddb2c596a1dd963ceafda86300b2de8466357d56aa4`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ce0d3817eff364f0101431f28cb70cde3766120bbe5fb10b53ebf59363136f`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dd973289c284ff507f57773413c00c41a54ad2015bafb509c68a044b609cda`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6c2b7b482e55dcb167623e29563231f659e1a523cb8f6e83423bb1d69a2014`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7811e07229200779f1a17a1899bf48c49f0250685f18fdffb38ee7c30ab779`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d7cb4258c8b7eab1c92df575a363d8685d8d783672e5256208f715c662b27b`  
		Last Modified: Wed, 14 Oct 2020 21:13:44 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ab63ba04ec1b983074014465794ebf2e437ec4c03997ac40e1be3a4abcce61`  
		Last Modified: Wed, 14 Oct 2020 21:13:44 GMT  
		Size: 268.2 KB (268209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac54f9c3e58e5d406091c73dec798c29e2ee3134663b63d3ddb4959f10f4f32`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-windowsservercore-1809`

```console
$ docker pull caddy@sha256:d720e5ab1579e03c0f86de11950434367743bdf8212a4501cd971c29d16942a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `caddy:2.2.1-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull caddy@sha256:5b0edc0113282eff2b0b97cb2768aef9406975982b52b5801fe66a3b7e0f1f6b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2399991421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4a3be7f6340286c7cad100a7baf86ff095c7d81ce5c10b5c314e8d7e73a9ade`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 21:03:47 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Oct 2020 21:03:48 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 14 Oct 2020 21:04:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Oct 2020 21:04:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Oct 2020 21:04:21 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Oct 2020 21:04:22 GMT
VOLUME [c:/config]
# Wed, 14 Oct 2020 21:04:23 GMT
VOLUME [c:/data]
# Wed, 14 Oct 2020 21:04:24 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 14 Oct 2020 21:04:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Oct 2020 21:04:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Oct 2020 21:04:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Oct 2020 21:04:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Oct 2020 21:04:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Oct 2020 21:04:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Oct 2020 21:04:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Oct 2020 21:04:29 GMT
EXPOSE 80
# Wed, 14 Oct 2020 21:04:30 GMT
EXPOSE 443
# Wed, 14 Oct 2020 21:04:30 GMT
EXPOSE 2019
# Wed, 14 Oct 2020 21:04:46 GMT
RUN caddy version
# Wed, 14 Oct 2020 21:04:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590b685e6f8e8fa4cbca8ce94e257baf1c179f183afabfc59bdff4420027e080`  
		Last Modified: Wed, 14 Oct 2020 21:13:24 GMT  
		Size: 9.2 MB (9237870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8a16e6bfc40544aeeaa55e8406570aec66018352db80098da3663138201f74`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468f02630a43054839d6262fe9f0d41cdd551ab83bbbb35c26cd9ead72ce6985`  
		Last Modified: Wed, 14 Oct 2020 21:13:25 GMT  
		Size: 16.3 MB (16343904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcdb09f7b5a57cb7fce28be7e54975dfc770735e4570b259b9104ddc8421bbd`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4b2b1c53bbf344fa90b58a9d5ee4b990881289dde49074cecd1f0da649c20a`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01bade2ee2333f9cd004bd1812f0c1fc7f55b2297cf57b8343e17b48c9d3535`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b312fdc7f27df222f05918031d72e4457582b08c8fdeff7cde88a6a402b6f0c`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053d376e7f1eb8e50a394d7247f16006d36ae65144e75d37fe8bb0740d91695f`  
		Last Modified: Wed, 14 Oct 2020 21:13:18 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d88dd9c5821fcba44cce1002ed12b8702e0cbec6ee8d137cbec8e5bd145acd5`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca72f02c89a70e463873f7095a54263f02a7dc1fc35b8b3d92d0d6ed1114e1c3`  
		Last Modified: Wed, 14 Oct 2020 21:13:16 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744bfb9438a82d19472dbb92037ab018420b16a677b9451e9b92d13d9d4cc309`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab7908db3cd309e1cf3200fc5b51374d626702ea4ff411559cfa15da77b097d`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691b1b3fc24e5b473537703fcabf8cdc0acd56705ab671452b135de184ffbe0c`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba327018ef360de6c48ecbdb06f66a73defdb3996be6c2f17f0731514dbece5`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c122dffbcf7af8877cc67b8f468cd74a76d63a739b85f3ac429fb27794f724`  
		Last Modified: Wed, 14 Oct 2020 21:13:13 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbf77f12be69367c8fcf09b53209ec5b25083762192120e9ed3f8e429569a4f`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c631d9175a05b1f8c784df5ccc0daeda8990f4cfa0faebc76e525dc737e034`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b5835866e9c4e5a927e7b41da88a4c61a54547cc83fc91db1c1a43494bbac2`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13669d36e52f3d6963333d5102e23ad22fd5892d4fd1a9468f12194c39c2753`  
		Last Modified: Wed, 14 Oct 2020 21:13:11 GMT  
		Size: 299.0 KB (299047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f0e09c2bd5ebc6729c8f1d852f4adefae35e2335cd7dbbcc09c95205e95ab0`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:155acd240efff18a38a7aff934be0f6976aeb1c76139025671c9833ed160c840
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64

### `caddy:2.2.1-windowsservercore-ltsc2016` - windows version 10.0.14393.3986; amd64

```console
$ docker pull caddy@sha256:4c7f9ebc39d2e00064b805df702d5364f55de8cb8cf5ae58d8e4f438988069e8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5773083905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0ce891f0605eaed2c51c683e9fe3d70f29bf6588b85b1f2be21dfcba2c4fb3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 21:06:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Oct 2020 21:06:25 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 14 Oct 2020 21:07:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Oct 2020 21:07:57 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Oct 2020 21:07:58 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Oct 2020 21:07:59 GMT
VOLUME [c:/config]
# Wed, 14 Oct 2020 21:08:00 GMT
VOLUME [c:/data]
# Wed, 14 Oct 2020 21:08:01 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 14 Oct 2020 21:08:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Oct 2020 21:08:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Oct 2020 21:08:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Oct 2020 21:08:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Oct 2020 21:08:05 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Oct 2020 21:08:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Oct 2020 21:08:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Oct 2020 21:08:08 GMT
EXPOSE 80
# Wed, 14 Oct 2020 21:08:08 GMT
EXPOSE 443
# Wed, 14 Oct 2020 21:08:09 GMT
EXPOSE 2019
# Wed, 14 Oct 2020 21:08:53 GMT
RUN caddy version
# Wed, 14 Oct 2020 21:08:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2b4a4f0660702b9f47920e1e7ea79666ac43584dadc8412d8a7b7eb0490a2c`  
		Last Modified: Wed, 14 Oct 2020 21:13:59 GMT  
		Size: 9.9 MB (9925104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3c401ae3441b3e5b7543d5482214980c1c14958e2713fee5966c2622a53963`  
		Last Modified: Wed, 14 Oct 2020 21:13:55 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffab013bf500710ef95125418f98138723e756c560a1de0145379662b77335db`  
		Last Modified: Wed, 14 Oct 2020 21:14:00 GMT  
		Size: 21.5 MB (21518510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcf1f0773bd9f450a654eb5dcecd55e2e3fe3ba01eb0dae7dbf27e84402a6be`  
		Last Modified: Wed, 14 Oct 2020 21:13:53 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7077da12d3b43ef9b9dad1d8c770898c3a0224a8a0a3b99dc4656cc594d09b62`  
		Last Modified: Wed, 14 Oct 2020 21:13:53 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3976aabb2b169dd3bb85d39e2473fe70f7f15de0124b56095dd3c25fbbc27c`  
		Last Modified: Wed, 14 Oct 2020 21:13:52 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e5576c4d0eac332d8332455193ed1057c55aa90bd5e9a6bca884a25623c3c8`  
		Last Modified: Wed, 14 Oct 2020 21:13:52 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7210dc7c5fabd3bf6636614bc150a0965808e559f2b293340b4d8e049a185684`  
		Last Modified: Wed, 14 Oct 2020 21:13:50 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7af1dab2b20db7484c30ac3175b1dc3b89884f843ece3209fdab4882f5e018`  
		Last Modified: Wed, 14 Oct 2020 21:13:49 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe18c02535b810df5a6916e6ffe0a4532c5a70dae17b5ce28956695be585480`  
		Last Modified: Wed, 14 Oct 2020 21:13:50 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb1797af36c3af3ecc1e7db5ddfdba44c6bfff97b0515b3463d0948fed92ac4`  
		Last Modified: Wed, 14 Oct 2020 21:13:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98a2d0f6d0934d8a3b866e68ca5e7775b2af52b170aa71f2113de2d32d532a3`  
		Last Modified: Wed, 14 Oct 2020 21:13:48 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f14b6955af73ac11170ddb2c596a1dd963ceafda86300b2de8466357d56aa4`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ce0d3817eff364f0101431f28cb70cde3766120bbe5fb10b53ebf59363136f`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dd973289c284ff507f57773413c00c41a54ad2015bafb509c68a044b609cda`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6c2b7b482e55dcb167623e29563231f659e1a523cb8f6e83423bb1d69a2014`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7811e07229200779f1a17a1899bf48c49f0250685f18fdffb38ee7c30ab779`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d7cb4258c8b7eab1c92df575a363d8685d8d783672e5256208f715c662b27b`  
		Last Modified: Wed, 14 Oct 2020 21:13:44 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ab63ba04ec1b983074014465794ebf2e437ec4c03997ac40e1be3a4abcce61`  
		Last Modified: Wed, 14 Oct 2020 21:13:44 GMT  
		Size: 268.2 KB (268209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac54f9c3e58e5d406091c73dec798c29e2ee3134663b63d3ddb4959f10f4f32`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.2 KB (1152 bytes)  
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
$ docker pull caddy@sha256:d1feb42feaf8542d7efe2afee44c2a57540f14deb3961b86aa0b7ee6de1b7c77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:b506e57149af1435025a622cd356fc93257f02130f1e721a1a067362b1f88ddd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.7 MB (119671750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05d3a71d119dcebe678d25c39ff3d11b63d842f1cd4756e133e9c3a4faa0fe38`
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
# Thu, 22 Oct 2020 03:34:57 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 03:37:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 03:37:52 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 03:37:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 03:37:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 03:37:54 GMT
WORKDIR /go
# Thu, 22 Oct 2020 04:34:16 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 04:34:16 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 04:34:16 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 04:34:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 04:34:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 04:34:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 04:34:20 GMT
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
	-	`sha256:0eba1c9be4d292e332c2f27b821e199d8603b724238d9a4ce48c566533546298`  
		Last Modified: Thu, 22 Oct 2020 03:44:16 GMT  
		Size: 106.9 MB (106876307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d57e429df01b9589550363e9badf8beb2c0ef2cfb959fb7389948decaccc71f`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf71de68668ac772e9853d42397c63e34666b964b958c23d49616ecbd9df286`  
		Last Modified: Thu, 22 Oct 2020 04:35:15 GMT  
		Size: 8.3 MB (8309874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b116073137746923179401de3108b0ceda969a41fee25a4b097c75eaafee084`  
		Last Modified: Thu, 22 Oct 2020 04:35:14 GMT  
		Size: 1.4 MB (1407214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d809710fb5305cf38c3119a76bd45b286b83f7501326896adc101338a4766e`  
		Last Modified: Thu, 22 Oct 2020 04:35:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2f447ef196725a6fe1129ccca0b74d23ff3dfb38887d56e618348db89feae116
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114815426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b367cdbe3af19cc3dd00928134ec76ddeef267a733cb88a2e1c97b67a113b480`
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
# Thu, 22 Oct 2020 03:07:28 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 04:07:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 04:07:33 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 04:07:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 04:09:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 04:09:37 GMT
WORKDIR /go
# Thu, 22 Oct 2020 10:05:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 10:05:06 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 10:05:08 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 10:05:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 10:05:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 10:05:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 10:05:13 GMT
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
	-	`sha256:0861c41718d28217202ec1937beb9975a5bee4aec22544789a4941342423d823`  
		Last Modified: Thu, 22 Oct 2020 05:35:25 GMT  
		Size: 102.7 MB (102675647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189a4b66c7697ec4dec0236745f1b2130dd6699149d2259637327eef2d8fb5a3`  
		Last Modified: Thu, 22 Oct 2020 05:34:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43299b1fec8de48d0860d111e16df032ff921ceb1bfe97430ebe2d9c67900d99`  
		Last Modified: Thu, 22 Oct 2020 10:05:40 GMT  
		Size: 7.9 MB (7928833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4e67b21208cda0253a4fdeefdc15a2990ded4af282530e328cd7b48914ce8d`  
		Last Modified: Thu, 22 Oct 2020 10:05:38 GMT  
		Size: 1.3 MB (1327348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d25b580938f0aedbca674d485edf5de24f1e51289d0e2317ea8d1040f2fcaac`  
		Last Modified: Thu, 22 Oct 2020 10:05:38 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:53f07e930bd2ec03da216d3e8325f74985e425cfa28e027307b2165a68d918d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113627797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7140db1472303a8077c6b1e7cacc69b2d2594c3732b60b2a1c66257928694bd4`
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
# Thu, 22 Oct 2020 03:23:43 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 04:38:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 04:38:54 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 04:39:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 04:41:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 04:41:39 GMT
WORKDIR /go
# Thu, 22 Oct 2020 09:24:49 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 09:24:50 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 09:24:51 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 09:24:52 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 09:24:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 09:24:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 09:24:55 GMT
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
	-	`sha256:8cedb62f6546fc1b0d4fa80e293634cefa26d2336796ea8e8bc24eabc9bc501e`  
		Last Modified: Thu, 22 Oct 2020 06:00:08 GMT  
		Size: 102.5 MB (102470699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a88c985904d22a6adc07851b517bd17b6624e2b422ff3dfe8375de1283250d8`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc68f5c354cb3e9a5328b0f6341317092ad7a6081c8f1791c3857d479f79065`  
		Last Modified: Thu, 22 Oct 2020 09:25:24 GMT  
		Size: 7.1 MB (7144783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d905d9db6b8b7d05de2a2d569e2e8a9b617e197168db24c50a0fc2e6583f878`  
		Last Modified: Thu, 22 Oct 2020 09:25:24 GMT  
		Size: 1.3 MB (1325844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cb350ca3cb778c3ae223b0b0d844902b1ee234c91aa18341eaafc3a91cdc39`  
		Last Modified: Thu, 22 Oct 2020 09:25:22 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:33f8ff597086154bb625661b95eb1cf0ad74284a3fc00917506f2961ccc29a65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.0 MB (114950741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95c2f36f633ba51a79c3441793ba3bac5aa172347ccdbb8c8f371ce9e1e5fb41`
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
# Thu, 22 Oct 2020 04:10:13 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 04:15:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 04:15:31 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 04:15:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 04:17:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 04:17:40 GMT
WORKDIR /go
# Thu, 22 Oct 2020 09:30:37 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 09:30:38 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 09:30:45 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 09:30:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 09:30:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 09:30:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 09:30:59 GMT
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
	-	`sha256:5afe5f37f5b3016b6946fda75a1f4dce7778311971998bab26064ee548e69e57`  
		Last Modified: Thu, 22 Oct 2020 04:29:46 GMT  
		Size: 102.2 MB (102152165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d0fcabf3d036cdbe487c24ebdc36aa0cf4c2700b5b386791a3538d92071a62`  
		Last Modified: Thu, 22 Oct 2020 04:28:23 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466fde6265bf309aca5041a30a19ba0f889387ceb0872309caa82fd6531b221a`  
		Last Modified: Thu, 22 Oct 2020 09:31:34 GMT  
		Size: 8.5 MB (8499894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82672d1571ea79e8c88077d08e3c7022c89e0494a79368f22dd09e069761eeca`  
		Last Modified: Thu, 22 Oct 2020 09:31:32 GMT  
		Size: 1.3 MB (1310181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b29dbb8417e8cdce10eeeb84f0d7f37da96a00c256648362fd0a1130013462c`  
		Last Modified: Thu, 22 Oct 2020 09:31:32 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:1381ebb3e36c7f726363e75544a7cf23e07e34c50595cb35af607d6ead7655bf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.1 MB (114109814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8378d7f685f94342d985ca619645498434b64a6d62b7bf884dbb57030e7d923`
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
# Thu, 22 Oct 2020 13:27:55 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 13:30:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 13:30:31 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 13:30:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 13:30:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 13:30:50 GMT
WORKDIR /go
# Thu, 22 Oct 2020 13:45:58 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 13:46:02 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 13:46:10 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 13:46:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 13:46:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 13:46:34 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 13:46:37 GMT
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
	-	`sha256:a53757254f83d2b7412aa2718828ed0bd489d01d5bad2c6ee877672775244a8a`  
		Last Modified: Thu, 22 Oct 2020 13:36:50 GMT  
		Size: 100.8 MB (100814882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6876bebeafd85e7b46e88239c365eeec0a308353e7d1f7de434659ef597f889d`  
		Last Modified: Thu, 22 Oct 2020 13:36:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60beda9dadec93f6e90d3398b12787fc49427a3ba3a7e88e42e6105562016ec6`  
		Last Modified: Thu, 22 Oct 2020 13:48:15 GMT  
		Size: 8.9 MB (8920001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ca79d64160e09790e775af1b4204add8e6f21a3e837e1bd743c9b7b6b9c24a`  
		Last Modified: Thu, 22 Oct 2020 13:48:14 GMT  
		Size: 1.3 MB (1287791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7348aa6f5d47e3ce5091866c5cc3341d13a31faad6b1aa33e76e9432f45506a`  
		Last Modified: Thu, 22 Oct 2020 13:48:13 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:a8aa50ea100e687faa5739a6f62ec5843fc9846c874337726fed6ba09f3ac315
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118526471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7efeb3f913cdd9cdf7a017801f525a164c24a2efd93d1eb010477ca4094ac251`
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
# Thu, 22 Oct 2020 02:53:31 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 02:55:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 02:55:33 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 02:55:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 02:55:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 02:55:35 GMT
WORKDIR /go
# Thu, 22 Oct 2020 10:13:52 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 10:13:53 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 10:13:54 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 10:13:54 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 10:13:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 10:13:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 10:13:57 GMT
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
	-	`sha256:93a9f4b10b0ce05491e77b29b87fa3bbcbcd40e10a492d96185bf5ef0acc62f0`  
		Last Modified: Thu, 22 Oct 2020 02:58:45 GMT  
		Size: 105.9 MB (105937593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c973fb648f38c29beb5231f712f726631c6eb8fdaefbd4b7ac5408af2ea1a61`  
		Last Modified: Thu, 22 Oct 2020 02:58:32 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ff827958d5db211b007a45cc274d0658dcb49f4949f86888fa5f731d8df24a`  
		Last Modified: Thu, 22 Oct 2020 10:14:27 GMT  
		Size: 8.4 MB (8352218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36fa21e3b269069073c65c60c20545573892ddcd3d507593bc28a325da2b8c2`  
		Last Modified: Thu, 22 Oct 2020 10:14:26 GMT  
		Size: 1.4 MB (1388754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472fde2a1575da1d5a5924aab83ea94739ae66686513f4cfa7cd844707b59058`  
		Last Modified: Thu, 22 Oct 2020 10:14:26 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.1518; amd64

```console
$ docker pull caddy@sha256:5f0ba224d2ff94370fd2e10a05b2e06f062b1e9ba4278b62e9ecb99056ff4802
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2549102284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a10b666950b6ddd3242011e2bf926b6d52b2bb6f910ac359ac1b4b08e6db235c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 12:27:03 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Oct 2020 12:27:04 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Oct 2020 12:27:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Oct 2020 12:27:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Oct 2020 12:28:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Oct 2020 12:28:38 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Oct 2020 12:29:02 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 15 Oct 2020 01:14:39 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 15 Oct 2020 01:17:39 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1d579d0e980763f60bf43afb7c3783caf63433a485731ef4d2e262878d634b3f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 15 Oct 2020 01:17:40 GMT
WORKDIR C:\gopath
# Thu, 15 Oct 2020 02:32:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 15 Oct 2020 02:32:16 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 15 Oct 2020 02:32:17 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 15 Oct 2020 02:32:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 15 Oct 2020 02:32:40 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 15 Oct 2020 02:32:41 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23a75d88f9f5980bb112e2c28248975f107144d8d2e40dc4755e2a09f5e56df`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bea6d8b9d9b014ffa471b7bb8882ddb7e9d378ddcacc099f0710073bd6361b9`  
		Last Modified: Wed, 14 Oct 2020 12:50:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75c1905c0573cc5706bc066d23624f0e92a8871832c744fbe7eabdcbc6f8a85`  
		Last Modified: Wed, 14 Oct 2020 12:50:24 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938695376d9deeba8819539ff3245935c28f93229d1c332bb8b6a16e67013fbc`  
		Last Modified: Wed, 14 Oct 2020 12:50:23 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41106c6a476cf9666c6d8c3c853c982a841c29db05b3ef8a072baba537b6d74c`  
		Last Modified: Wed, 14 Oct 2020 12:50:48 GMT  
		Size: 34.3 MB (34312667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d6d6258831f87f3b455e6316e2bed430465a760272614de7cdd28c7c6e9f3e`  
		Last Modified: Wed, 14 Oct 2020 12:50:19 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e3f66638c4d5ce9adba16e49844f57efbab1d628d9d6c73133511b7c1c3892`  
		Last Modified: Wed, 14 Oct 2020 12:50:20 GMT  
		Size: 310.5 KB (310525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe34732f84b95b980d0ae0624ebae44818ef7879e34a9ffbebe752f1dcd4badf`  
		Last Modified: Thu, 15 Oct 2020 02:05:08 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a6c4c70f4e593c0500bebe3fa23edab8bd791805ab4a5edf34cb053b21264f`  
		Last Modified: Thu, 15 Oct 2020 02:05:35 GMT  
		Size: 138.6 MB (138590451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123678d8baa038225b16066bfa2f971f7454f2d5b16b95db1663954869cf837a`  
		Last Modified: Thu, 15 Oct 2020 02:05:07 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99abf6100e15da95d12aff85cd77f0adf4d96b7b1b2815445a9fc6f576c3df79`  
		Last Modified: Thu, 15 Oct 2020 02:35:13 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908a905e414249fe5a6b10921f1505b4e5edb7bad45fd2f70a3095f99e8d3929`  
		Last Modified: Thu, 15 Oct 2020 02:35:10 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beea46a5312f34364874857e7fdd21b76239ae4028aeabd8ef4e7092e536fda0`  
		Last Modified: Thu, 15 Oct 2020 02:35:09 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb245ad725b068d3bb29ee875394207d019d445c185bf1ca1ddd2ce1c62ce38`  
		Last Modified: Thu, 15 Oct 2020 02:35:10 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9cd8369d2f668d2d300f35c9d9ee98488040b7b695efbaadb1d3b76f314eac`  
		Last Modified: Thu, 15 Oct 2020 02:35:10 GMT  
		Size: 1.8 MB (1783668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798dfde6e8213d06ef180571d9c1956e9b42899062509ff88cfbc453b3ff9c37`  
		Last Modified: Thu, 15 Oct 2020 02:35:09 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.14393.3986; amd64

```console
$ docker pull caddy@sha256:8fea2fa2956f6e7eb56eb8f745fe7b6f4a7ccf45bd259d7a8cccb3d2c71f3c1f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5941324722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4f39f7f404783da13552d7024d9a3262d0d6a1834385977fb514556a43e41f9`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 12:31:45 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Oct 2020 12:31:46 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Oct 2020 12:31:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Oct 2020 12:31:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Oct 2020 12:33:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Oct 2020 12:33:58 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Oct 2020 12:35:13 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 15 Oct 2020 01:17:52 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 15 Oct 2020 01:21:40 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1d579d0e980763f60bf43afb7c3783caf63433a485731ef4d2e262878d634b3f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 15 Oct 2020 01:21:41 GMT
WORKDIR C:\gopath
# Thu, 15 Oct 2020 02:32:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 15 Oct 2020 02:32:47 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 15 Oct 2020 02:32:48 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 15 Oct 2020 02:32:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 15 Oct 2020 02:34:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 15 Oct 2020 02:34:06 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528ba1d9759adcc464112008fe49672e1f545981d69bab31186587ab32f92138`  
		Last Modified: Wed, 14 Oct 2020 12:51:33 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53bf4e6180661653575845d30a4d882dea92f395cb540b1cdf91170e9ee58731`  
		Last Modified: Wed, 14 Oct 2020 12:51:30 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e973f094614bb2cebe16df6f6004c05895ed077151aecdbbd0c476513054fc`  
		Last Modified: Wed, 14 Oct 2020 12:51:25 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1089b875ac355097876e23760dd2166f096a8645e312660ffd3c0e617a2df9a0`  
		Last Modified: Wed, 14 Oct 2020 12:51:29 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8934a016b666d0691307c6414d84c36eb82de4b2fc4d74dd04c75f632dc3a78c`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 35.0 MB (35016991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4d95d13c0a45aa19a623e51cb112530a589a3a4d15d5c119610f8196912fab`  
		Last Modified: Wed, 14 Oct 2020 12:51:20 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf8226941bb8f5af9f2be8fdb54da3e3caef344b0061a73e3debde23a55e98f`  
		Last Modified: Wed, 14 Oct 2020 12:51:24 GMT  
		Size: 9.9 MB (9870100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b8d8683ed903732b7672eb374d957e4ad20a8936cd48bc9a69059c19163325`  
		Last Modified: Thu, 15 Oct 2020 02:05:58 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38f6e003c1013456c5993d4c122314dab53690c52405c373b2055e636353e47`  
		Last Modified: Thu, 15 Oct 2020 02:06:27 GMT  
		Size: 143.8 MB (143758677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbc6767c79760c5d4cd356ae2dd0742f8d13be9298959aa3009b1e4d2c18cbc`  
		Last Modified: Thu, 15 Oct 2020 02:05:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba9f5f016316461f4d80f3defd59bad0cd10886ae46ef3ad8802facb8a3330b`  
		Last Modified: Thu, 15 Oct 2020 02:35:33 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b074f2cce57588dbf6e04970c0be7db19be264eee3f4bb3a7b4bbcf4fd717b95`  
		Last Modified: Thu, 15 Oct 2020 02:35:30 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b1d6dbe2c318375f7055dc79b3b4b44a06e13238cb914eddfb5cfa258f86c6`  
		Last Modified: Thu, 15 Oct 2020 02:35:30 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c349a444d08c6b059ed2430ee7e28766f5ac7a411eeadb73dad01e26fc70916`  
		Last Modified: Thu, 15 Oct 2020 02:35:30 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1bc4e5aa1948e251b46da1e6c6c5632371f1bf5a60c64269247ec5d348fb22`  
		Last Modified: Thu, 15 Oct 2020 02:35:33 GMT  
		Size: 11.3 MB (11312385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed394fa51b2433c7ce756430011e4cc52ac6d67198f2bf0ae8144eafa44a2a89`  
		Last Modified: Thu, 15 Oct 2020 02:35:31 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:a42199f0a07411337da8367217434680136db2e93e04b596aa8d9399325f25f6
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
$ docker pull caddy@sha256:b506e57149af1435025a622cd356fc93257f02130f1e721a1a067362b1f88ddd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.7 MB (119671750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05d3a71d119dcebe678d25c39ff3d11b63d842f1cd4756e133e9c3a4faa0fe38`
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
# Thu, 22 Oct 2020 03:34:57 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 03:37:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 03:37:52 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 03:37:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 03:37:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 03:37:54 GMT
WORKDIR /go
# Thu, 22 Oct 2020 04:34:16 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 04:34:16 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 04:34:16 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 04:34:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 04:34:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 04:34:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 04:34:20 GMT
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
	-	`sha256:0eba1c9be4d292e332c2f27b821e199d8603b724238d9a4ce48c566533546298`  
		Last Modified: Thu, 22 Oct 2020 03:44:16 GMT  
		Size: 106.9 MB (106876307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d57e429df01b9589550363e9badf8beb2c0ef2cfb959fb7389948decaccc71f`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf71de68668ac772e9853d42397c63e34666b964b958c23d49616ecbd9df286`  
		Last Modified: Thu, 22 Oct 2020 04:35:15 GMT  
		Size: 8.3 MB (8309874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b116073137746923179401de3108b0ceda969a41fee25a4b097c75eaafee084`  
		Last Modified: Thu, 22 Oct 2020 04:35:14 GMT  
		Size: 1.4 MB (1407214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d809710fb5305cf38c3119a76bd45b286b83f7501326896adc101338a4766e`  
		Last Modified: Thu, 22 Oct 2020 04:35:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2f447ef196725a6fe1129ccca0b74d23ff3dfb38887d56e618348db89feae116
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114815426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b367cdbe3af19cc3dd00928134ec76ddeef267a733cb88a2e1c97b67a113b480`
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
# Thu, 22 Oct 2020 03:07:28 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 04:07:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 04:07:33 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 04:07:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 04:09:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 04:09:37 GMT
WORKDIR /go
# Thu, 22 Oct 2020 10:05:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 10:05:06 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 10:05:08 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 10:05:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 10:05:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 10:05:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 10:05:13 GMT
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
	-	`sha256:0861c41718d28217202ec1937beb9975a5bee4aec22544789a4941342423d823`  
		Last Modified: Thu, 22 Oct 2020 05:35:25 GMT  
		Size: 102.7 MB (102675647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189a4b66c7697ec4dec0236745f1b2130dd6699149d2259637327eef2d8fb5a3`  
		Last Modified: Thu, 22 Oct 2020 05:34:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43299b1fec8de48d0860d111e16df032ff921ceb1bfe97430ebe2d9c67900d99`  
		Last Modified: Thu, 22 Oct 2020 10:05:40 GMT  
		Size: 7.9 MB (7928833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4e67b21208cda0253a4fdeefdc15a2990ded4af282530e328cd7b48914ce8d`  
		Last Modified: Thu, 22 Oct 2020 10:05:38 GMT  
		Size: 1.3 MB (1327348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d25b580938f0aedbca674d485edf5de24f1e51289d0e2317ea8d1040f2fcaac`  
		Last Modified: Thu, 22 Oct 2020 10:05:38 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:53f07e930bd2ec03da216d3e8325f74985e425cfa28e027307b2165a68d918d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113627797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7140db1472303a8077c6b1e7cacc69b2d2594c3732b60b2a1c66257928694bd4`
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
# Thu, 22 Oct 2020 03:23:43 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 04:38:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 04:38:54 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 04:39:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 04:41:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 04:41:39 GMT
WORKDIR /go
# Thu, 22 Oct 2020 09:24:49 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 09:24:50 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 09:24:51 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 09:24:52 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 09:24:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 09:24:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 09:24:55 GMT
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
	-	`sha256:8cedb62f6546fc1b0d4fa80e293634cefa26d2336796ea8e8bc24eabc9bc501e`  
		Last Modified: Thu, 22 Oct 2020 06:00:08 GMT  
		Size: 102.5 MB (102470699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a88c985904d22a6adc07851b517bd17b6624e2b422ff3dfe8375de1283250d8`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc68f5c354cb3e9a5328b0f6341317092ad7a6081c8f1791c3857d479f79065`  
		Last Modified: Thu, 22 Oct 2020 09:25:24 GMT  
		Size: 7.1 MB (7144783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d905d9db6b8b7d05de2a2d569e2e8a9b617e197168db24c50a0fc2e6583f878`  
		Last Modified: Thu, 22 Oct 2020 09:25:24 GMT  
		Size: 1.3 MB (1325844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cb350ca3cb778c3ae223b0b0d844902b1ee234c91aa18341eaafc3a91cdc39`  
		Last Modified: Thu, 22 Oct 2020 09:25:22 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:33f8ff597086154bb625661b95eb1cf0ad74284a3fc00917506f2961ccc29a65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.0 MB (114950741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95c2f36f633ba51a79c3441793ba3bac5aa172347ccdbb8c8f371ce9e1e5fb41`
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
# Thu, 22 Oct 2020 04:10:13 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 04:15:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 04:15:31 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 04:15:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 04:17:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 04:17:40 GMT
WORKDIR /go
# Thu, 22 Oct 2020 09:30:37 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 09:30:38 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 09:30:45 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 09:30:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 09:30:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 09:30:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 09:30:59 GMT
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
	-	`sha256:5afe5f37f5b3016b6946fda75a1f4dce7778311971998bab26064ee548e69e57`  
		Last Modified: Thu, 22 Oct 2020 04:29:46 GMT  
		Size: 102.2 MB (102152165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d0fcabf3d036cdbe487c24ebdc36aa0cf4c2700b5b386791a3538d92071a62`  
		Last Modified: Thu, 22 Oct 2020 04:28:23 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466fde6265bf309aca5041a30a19ba0f889387ceb0872309caa82fd6531b221a`  
		Last Modified: Thu, 22 Oct 2020 09:31:34 GMT  
		Size: 8.5 MB (8499894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82672d1571ea79e8c88077d08e3c7022c89e0494a79368f22dd09e069761eeca`  
		Last Modified: Thu, 22 Oct 2020 09:31:32 GMT  
		Size: 1.3 MB (1310181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b29dbb8417e8cdce10eeeb84f0d7f37da96a00c256648362fd0a1130013462c`  
		Last Modified: Thu, 22 Oct 2020 09:31:32 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:1381ebb3e36c7f726363e75544a7cf23e07e34c50595cb35af607d6ead7655bf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.1 MB (114109814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8378d7f685f94342d985ca619645498434b64a6d62b7bf884dbb57030e7d923`
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
# Thu, 22 Oct 2020 13:27:55 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 13:30:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 13:30:31 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 13:30:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 13:30:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 13:30:50 GMT
WORKDIR /go
# Thu, 22 Oct 2020 13:45:58 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 13:46:02 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 13:46:10 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 13:46:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 13:46:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 13:46:34 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 13:46:37 GMT
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
	-	`sha256:a53757254f83d2b7412aa2718828ed0bd489d01d5bad2c6ee877672775244a8a`  
		Last Modified: Thu, 22 Oct 2020 13:36:50 GMT  
		Size: 100.8 MB (100814882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6876bebeafd85e7b46e88239c365eeec0a308353e7d1f7de434659ef597f889d`  
		Last Modified: Thu, 22 Oct 2020 13:36:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60beda9dadec93f6e90d3398b12787fc49427a3ba3a7e88e42e6105562016ec6`  
		Last Modified: Thu, 22 Oct 2020 13:48:15 GMT  
		Size: 8.9 MB (8920001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ca79d64160e09790e775af1b4204add8e6f21a3e837e1bd743c9b7b6b9c24a`  
		Last Modified: Thu, 22 Oct 2020 13:48:14 GMT  
		Size: 1.3 MB (1287791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7348aa6f5d47e3ce5091866c5cc3341d13a31faad6b1aa33e76e9432f45506a`  
		Last Modified: Thu, 22 Oct 2020 13:48:13 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:a8aa50ea100e687faa5739a6f62ec5843fc9846c874337726fed6ba09f3ac315
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118526471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7efeb3f913cdd9cdf7a017801f525a164c24a2efd93d1eb010477ca4094ac251`
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
# Thu, 22 Oct 2020 02:53:31 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 02:55:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 02:55:33 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 02:55:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 02:55:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 02:55:35 GMT
WORKDIR /go
# Thu, 22 Oct 2020 10:13:52 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 10:13:53 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 10:13:54 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 10:13:54 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 10:13:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 10:13:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 10:13:57 GMT
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
	-	`sha256:93a9f4b10b0ce05491e77b29b87fa3bbcbcd40e10a492d96185bf5ef0acc62f0`  
		Last Modified: Thu, 22 Oct 2020 02:58:45 GMT  
		Size: 105.9 MB (105937593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c973fb648f38c29beb5231f712f726631c6eb8fdaefbd4b7ac5408af2ea1a61`  
		Last Modified: Thu, 22 Oct 2020 02:58:32 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ff827958d5db211b007a45cc274d0658dcb49f4949f86888fa5f731d8df24a`  
		Last Modified: Thu, 22 Oct 2020 10:14:27 GMT  
		Size: 8.4 MB (8352218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36fa21e3b269069073c65c60c20545573892ddcd3d507593bc28a325da2b8c2`  
		Last Modified: Thu, 22 Oct 2020 10:14:26 GMT  
		Size: 1.4 MB (1388754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472fde2a1575da1d5a5924aab83ea94739ae66686513f4cfa7cd844707b59058`  
		Last Modified: Thu, 22 Oct 2020 10:14:26 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:ab8f8e005e8197265d91e6dcb9b94990e7b89b8474a015df00bc498851522a81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull caddy@sha256:5f0ba224d2ff94370fd2e10a05b2e06f062b1e9ba4278b62e9ecb99056ff4802
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2549102284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a10b666950b6ddd3242011e2bf926b6d52b2bb6f910ac359ac1b4b08e6db235c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 12:27:03 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Oct 2020 12:27:04 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Oct 2020 12:27:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Oct 2020 12:27:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Oct 2020 12:28:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Oct 2020 12:28:38 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Oct 2020 12:29:02 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 15 Oct 2020 01:14:39 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 15 Oct 2020 01:17:39 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1d579d0e980763f60bf43afb7c3783caf63433a485731ef4d2e262878d634b3f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 15 Oct 2020 01:17:40 GMT
WORKDIR C:\gopath
# Thu, 15 Oct 2020 02:32:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 15 Oct 2020 02:32:16 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 15 Oct 2020 02:32:17 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 15 Oct 2020 02:32:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 15 Oct 2020 02:32:40 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 15 Oct 2020 02:32:41 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23a75d88f9f5980bb112e2c28248975f107144d8d2e40dc4755e2a09f5e56df`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bea6d8b9d9b014ffa471b7bb8882ddb7e9d378ddcacc099f0710073bd6361b9`  
		Last Modified: Wed, 14 Oct 2020 12:50:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75c1905c0573cc5706bc066d23624f0e92a8871832c744fbe7eabdcbc6f8a85`  
		Last Modified: Wed, 14 Oct 2020 12:50:24 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938695376d9deeba8819539ff3245935c28f93229d1c332bb8b6a16e67013fbc`  
		Last Modified: Wed, 14 Oct 2020 12:50:23 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41106c6a476cf9666c6d8c3c853c982a841c29db05b3ef8a072baba537b6d74c`  
		Last Modified: Wed, 14 Oct 2020 12:50:48 GMT  
		Size: 34.3 MB (34312667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d6d6258831f87f3b455e6316e2bed430465a760272614de7cdd28c7c6e9f3e`  
		Last Modified: Wed, 14 Oct 2020 12:50:19 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e3f66638c4d5ce9adba16e49844f57efbab1d628d9d6c73133511b7c1c3892`  
		Last Modified: Wed, 14 Oct 2020 12:50:20 GMT  
		Size: 310.5 KB (310525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe34732f84b95b980d0ae0624ebae44818ef7879e34a9ffbebe752f1dcd4badf`  
		Last Modified: Thu, 15 Oct 2020 02:05:08 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a6c4c70f4e593c0500bebe3fa23edab8bd791805ab4a5edf34cb053b21264f`  
		Last Modified: Thu, 15 Oct 2020 02:05:35 GMT  
		Size: 138.6 MB (138590451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123678d8baa038225b16066bfa2f971f7454f2d5b16b95db1663954869cf837a`  
		Last Modified: Thu, 15 Oct 2020 02:05:07 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99abf6100e15da95d12aff85cd77f0adf4d96b7b1b2815445a9fc6f576c3df79`  
		Last Modified: Thu, 15 Oct 2020 02:35:13 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908a905e414249fe5a6b10921f1505b4e5edb7bad45fd2f70a3095f99e8d3929`  
		Last Modified: Thu, 15 Oct 2020 02:35:10 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beea46a5312f34364874857e7fdd21b76239ae4028aeabd8ef4e7092e536fda0`  
		Last Modified: Thu, 15 Oct 2020 02:35:09 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb245ad725b068d3bb29ee875394207d019d445c185bf1ca1ddd2ce1c62ce38`  
		Last Modified: Thu, 15 Oct 2020 02:35:10 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9cd8369d2f668d2d300f35c9d9ee98488040b7b695efbaadb1d3b76f314eac`  
		Last Modified: Thu, 15 Oct 2020 02:35:10 GMT  
		Size: 1.8 MB (1783668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798dfde6e8213d06ef180571d9c1956e9b42899062509ff88cfbc453b3ff9c37`  
		Last Modified: Thu, 15 Oct 2020 02:35:09 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:193e2b1f70d18f86f7e53052a5a343e8a9538646a3089c4eedf3e1441e7b1e4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64

### `caddy:2-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.3986; amd64

```console
$ docker pull caddy@sha256:8fea2fa2956f6e7eb56eb8f745fe7b6f4a7ccf45bd259d7a8cccb3d2c71f3c1f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5941324722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4f39f7f404783da13552d7024d9a3262d0d6a1834385977fb514556a43e41f9`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 12:31:45 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Oct 2020 12:31:46 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Oct 2020 12:31:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Oct 2020 12:31:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Oct 2020 12:33:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Oct 2020 12:33:58 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Oct 2020 12:35:13 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 15 Oct 2020 01:17:52 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 15 Oct 2020 01:21:40 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1d579d0e980763f60bf43afb7c3783caf63433a485731ef4d2e262878d634b3f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 15 Oct 2020 01:21:41 GMT
WORKDIR C:\gopath
# Thu, 15 Oct 2020 02:32:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 15 Oct 2020 02:32:47 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 15 Oct 2020 02:32:48 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 15 Oct 2020 02:32:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 15 Oct 2020 02:34:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 15 Oct 2020 02:34:06 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528ba1d9759adcc464112008fe49672e1f545981d69bab31186587ab32f92138`  
		Last Modified: Wed, 14 Oct 2020 12:51:33 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53bf4e6180661653575845d30a4d882dea92f395cb540b1cdf91170e9ee58731`  
		Last Modified: Wed, 14 Oct 2020 12:51:30 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e973f094614bb2cebe16df6f6004c05895ed077151aecdbbd0c476513054fc`  
		Last Modified: Wed, 14 Oct 2020 12:51:25 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1089b875ac355097876e23760dd2166f096a8645e312660ffd3c0e617a2df9a0`  
		Last Modified: Wed, 14 Oct 2020 12:51:29 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8934a016b666d0691307c6414d84c36eb82de4b2fc4d74dd04c75f632dc3a78c`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 35.0 MB (35016991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4d95d13c0a45aa19a623e51cb112530a589a3a4d15d5c119610f8196912fab`  
		Last Modified: Wed, 14 Oct 2020 12:51:20 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf8226941bb8f5af9f2be8fdb54da3e3caef344b0061a73e3debde23a55e98f`  
		Last Modified: Wed, 14 Oct 2020 12:51:24 GMT  
		Size: 9.9 MB (9870100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b8d8683ed903732b7672eb374d957e4ad20a8936cd48bc9a69059c19163325`  
		Last Modified: Thu, 15 Oct 2020 02:05:58 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38f6e003c1013456c5993d4c122314dab53690c52405c373b2055e636353e47`  
		Last Modified: Thu, 15 Oct 2020 02:06:27 GMT  
		Size: 143.8 MB (143758677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbc6767c79760c5d4cd356ae2dd0742f8d13be9298959aa3009b1e4d2c18cbc`  
		Last Modified: Thu, 15 Oct 2020 02:05:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba9f5f016316461f4d80f3defd59bad0cd10886ae46ef3ad8802facb8a3330b`  
		Last Modified: Thu, 15 Oct 2020 02:35:33 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b074f2cce57588dbf6e04970c0be7db19be264eee3f4bb3a7b4bbcf4fd717b95`  
		Last Modified: Thu, 15 Oct 2020 02:35:30 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b1d6dbe2c318375f7055dc79b3b4b44a06e13238cb914eddfb5cfa258f86c6`  
		Last Modified: Thu, 15 Oct 2020 02:35:30 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c349a444d08c6b059ed2430ee7e28766f5ac7a411eeadb73dad01e26fc70916`  
		Last Modified: Thu, 15 Oct 2020 02:35:30 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1bc4e5aa1948e251b46da1e6c6c5632371f1bf5a60c64269247ec5d348fb22`  
		Last Modified: Thu, 15 Oct 2020 02:35:33 GMT  
		Size: 11.3 MB (11312385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed394fa51b2433c7ce756430011e4cc52ac6d67198f2bf0ae8144eafa44a2a89`  
		Last Modified: Thu, 15 Oct 2020 02:35:31 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:0cc9e18409440159fbf2ac241bce180b0214fc5d2358aa87fedf1189394d7469
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.1518; amd64

```console
$ docker pull caddy@sha256:5b0edc0113282eff2b0b97cb2768aef9406975982b52b5801fe66a3b7e0f1f6b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2399991421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4a3be7f6340286c7cad100a7baf86ff095c7d81ce5c10b5c314e8d7e73a9ade`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 21:03:47 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Oct 2020 21:03:48 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 14 Oct 2020 21:04:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Oct 2020 21:04:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Oct 2020 21:04:21 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Oct 2020 21:04:22 GMT
VOLUME [c:/config]
# Wed, 14 Oct 2020 21:04:23 GMT
VOLUME [c:/data]
# Wed, 14 Oct 2020 21:04:24 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 14 Oct 2020 21:04:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Oct 2020 21:04:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Oct 2020 21:04:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Oct 2020 21:04:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Oct 2020 21:04:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Oct 2020 21:04:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Oct 2020 21:04:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Oct 2020 21:04:29 GMT
EXPOSE 80
# Wed, 14 Oct 2020 21:04:30 GMT
EXPOSE 443
# Wed, 14 Oct 2020 21:04:30 GMT
EXPOSE 2019
# Wed, 14 Oct 2020 21:04:46 GMT
RUN caddy version
# Wed, 14 Oct 2020 21:04:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590b685e6f8e8fa4cbca8ce94e257baf1c179f183afabfc59bdff4420027e080`  
		Last Modified: Wed, 14 Oct 2020 21:13:24 GMT  
		Size: 9.2 MB (9237870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8a16e6bfc40544aeeaa55e8406570aec66018352db80098da3663138201f74`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468f02630a43054839d6262fe9f0d41cdd551ab83bbbb35c26cd9ead72ce6985`  
		Last Modified: Wed, 14 Oct 2020 21:13:25 GMT  
		Size: 16.3 MB (16343904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcdb09f7b5a57cb7fce28be7e54975dfc770735e4570b259b9104ddc8421bbd`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4b2b1c53bbf344fa90b58a9d5ee4b990881289dde49074cecd1f0da649c20a`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01bade2ee2333f9cd004bd1812f0c1fc7f55b2297cf57b8343e17b48c9d3535`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b312fdc7f27df222f05918031d72e4457582b08c8fdeff7cde88a6a402b6f0c`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053d376e7f1eb8e50a394d7247f16006d36ae65144e75d37fe8bb0740d91695f`  
		Last Modified: Wed, 14 Oct 2020 21:13:18 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d88dd9c5821fcba44cce1002ed12b8702e0cbec6ee8d137cbec8e5bd145acd5`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca72f02c89a70e463873f7095a54263f02a7dc1fc35b8b3d92d0d6ed1114e1c3`  
		Last Modified: Wed, 14 Oct 2020 21:13:16 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744bfb9438a82d19472dbb92037ab018420b16a677b9451e9b92d13d9d4cc309`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab7908db3cd309e1cf3200fc5b51374d626702ea4ff411559cfa15da77b097d`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691b1b3fc24e5b473537703fcabf8cdc0acd56705ab671452b135de184ffbe0c`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba327018ef360de6c48ecbdb06f66a73defdb3996be6c2f17f0731514dbece5`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c122dffbcf7af8877cc67b8f468cd74a76d63a739b85f3ac429fb27794f724`  
		Last Modified: Wed, 14 Oct 2020 21:13:13 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbf77f12be69367c8fcf09b53209ec5b25083762192120e9ed3f8e429569a4f`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c631d9175a05b1f8c784df5ccc0daeda8990f4cfa0faebc76e525dc737e034`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b5835866e9c4e5a927e7b41da88a4c61a54547cc83fc91db1c1a43494bbac2`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13669d36e52f3d6963333d5102e23ad22fd5892d4fd1a9468f12194c39c2753`  
		Last Modified: Wed, 14 Oct 2020 21:13:11 GMT  
		Size: 299.0 KB (299047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f0e09c2bd5ebc6729c8f1d852f4adefae35e2335cd7dbbcc09c95205e95ab0`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.14393.3986; amd64

```console
$ docker pull caddy@sha256:4c7f9ebc39d2e00064b805df702d5364f55de8cb8cf5ae58d8e4f438988069e8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5773083905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0ce891f0605eaed2c51c683e9fe3d70f29bf6588b85b1f2be21dfcba2c4fb3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 21:06:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Oct 2020 21:06:25 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 14 Oct 2020 21:07:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Oct 2020 21:07:57 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Oct 2020 21:07:58 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Oct 2020 21:07:59 GMT
VOLUME [c:/config]
# Wed, 14 Oct 2020 21:08:00 GMT
VOLUME [c:/data]
# Wed, 14 Oct 2020 21:08:01 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 14 Oct 2020 21:08:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Oct 2020 21:08:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Oct 2020 21:08:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Oct 2020 21:08:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Oct 2020 21:08:05 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Oct 2020 21:08:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Oct 2020 21:08:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Oct 2020 21:08:08 GMT
EXPOSE 80
# Wed, 14 Oct 2020 21:08:08 GMT
EXPOSE 443
# Wed, 14 Oct 2020 21:08:09 GMT
EXPOSE 2019
# Wed, 14 Oct 2020 21:08:53 GMT
RUN caddy version
# Wed, 14 Oct 2020 21:08:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2b4a4f0660702b9f47920e1e7ea79666ac43584dadc8412d8a7b7eb0490a2c`  
		Last Modified: Wed, 14 Oct 2020 21:13:59 GMT  
		Size: 9.9 MB (9925104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3c401ae3441b3e5b7543d5482214980c1c14958e2713fee5966c2622a53963`  
		Last Modified: Wed, 14 Oct 2020 21:13:55 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffab013bf500710ef95125418f98138723e756c560a1de0145379662b77335db`  
		Last Modified: Wed, 14 Oct 2020 21:14:00 GMT  
		Size: 21.5 MB (21518510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcf1f0773bd9f450a654eb5dcecd55e2e3fe3ba01eb0dae7dbf27e84402a6be`  
		Last Modified: Wed, 14 Oct 2020 21:13:53 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7077da12d3b43ef9b9dad1d8c770898c3a0224a8a0a3b99dc4656cc594d09b62`  
		Last Modified: Wed, 14 Oct 2020 21:13:53 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3976aabb2b169dd3bb85d39e2473fe70f7f15de0124b56095dd3c25fbbc27c`  
		Last Modified: Wed, 14 Oct 2020 21:13:52 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e5576c4d0eac332d8332455193ed1057c55aa90bd5e9a6bca884a25623c3c8`  
		Last Modified: Wed, 14 Oct 2020 21:13:52 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7210dc7c5fabd3bf6636614bc150a0965808e559f2b293340b4d8e049a185684`  
		Last Modified: Wed, 14 Oct 2020 21:13:50 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7af1dab2b20db7484c30ac3175b1dc3b89884f843ece3209fdab4882f5e018`  
		Last Modified: Wed, 14 Oct 2020 21:13:49 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe18c02535b810df5a6916e6ffe0a4532c5a70dae17b5ce28956695be585480`  
		Last Modified: Wed, 14 Oct 2020 21:13:50 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb1797af36c3af3ecc1e7db5ddfdba44c6bfff97b0515b3463d0948fed92ac4`  
		Last Modified: Wed, 14 Oct 2020 21:13:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98a2d0f6d0934d8a3b866e68ca5e7775b2af52b170aa71f2113de2d32d532a3`  
		Last Modified: Wed, 14 Oct 2020 21:13:48 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f14b6955af73ac11170ddb2c596a1dd963ceafda86300b2de8466357d56aa4`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ce0d3817eff364f0101431f28cb70cde3766120bbe5fb10b53ebf59363136f`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dd973289c284ff507f57773413c00c41a54ad2015bafb509c68a044b609cda`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6c2b7b482e55dcb167623e29563231f659e1a523cb8f6e83423bb1d69a2014`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7811e07229200779f1a17a1899bf48c49f0250685f18fdffb38ee7c30ab779`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d7cb4258c8b7eab1c92df575a363d8685d8d783672e5256208f715c662b27b`  
		Last Modified: Wed, 14 Oct 2020 21:13:44 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ab63ba04ec1b983074014465794ebf2e437ec4c03997ac40e1be3a4abcce61`  
		Last Modified: Wed, 14 Oct 2020 21:13:44 GMT  
		Size: 268.2 KB (268209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac54f9c3e58e5d406091c73dec798c29e2ee3134663b63d3ddb4959f10f4f32`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:d720e5ab1579e03c0f86de11950434367743bdf8212a4501cd971c29d16942a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull caddy@sha256:5b0edc0113282eff2b0b97cb2768aef9406975982b52b5801fe66a3b7e0f1f6b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2399991421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4a3be7f6340286c7cad100a7baf86ff095c7d81ce5c10b5c314e8d7e73a9ade`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 21:03:47 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Oct 2020 21:03:48 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 14 Oct 2020 21:04:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Oct 2020 21:04:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Oct 2020 21:04:21 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Oct 2020 21:04:22 GMT
VOLUME [c:/config]
# Wed, 14 Oct 2020 21:04:23 GMT
VOLUME [c:/data]
# Wed, 14 Oct 2020 21:04:24 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 14 Oct 2020 21:04:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Oct 2020 21:04:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Oct 2020 21:04:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Oct 2020 21:04:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Oct 2020 21:04:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Oct 2020 21:04:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Oct 2020 21:04:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Oct 2020 21:04:29 GMT
EXPOSE 80
# Wed, 14 Oct 2020 21:04:30 GMT
EXPOSE 443
# Wed, 14 Oct 2020 21:04:30 GMT
EXPOSE 2019
# Wed, 14 Oct 2020 21:04:46 GMT
RUN caddy version
# Wed, 14 Oct 2020 21:04:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590b685e6f8e8fa4cbca8ce94e257baf1c179f183afabfc59bdff4420027e080`  
		Last Modified: Wed, 14 Oct 2020 21:13:24 GMT  
		Size: 9.2 MB (9237870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8a16e6bfc40544aeeaa55e8406570aec66018352db80098da3663138201f74`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468f02630a43054839d6262fe9f0d41cdd551ab83bbbb35c26cd9ead72ce6985`  
		Last Modified: Wed, 14 Oct 2020 21:13:25 GMT  
		Size: 16.3 MB (16343904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcdb09f7b5a57cb7fce28be7e54975dfc770735e4570b259b9104ddc8421bbd`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4b2b1c53bbf344fa90b58a9d5ee4b990881289dde49074cecd1f0da649c20a`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01bade2ee2333f9cd004bd1812f0c1fc7f55b2297cf57b8343e17b48c9d3535`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b312fdc7f27df222f05918031d72e4457582b08c8fdeff7cde88a6a402b6f0c`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053d376e7f1eb8e50a394d7247f16006d36ae65144e75d37fe8bb0740d91695f`  
		Last Modified: Wed, 14 Oct 2020 21:13:18 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d88dd9c5821fcba44cce1002ed12b8702e0cbec6ee8d137cbec8e5bd145acd5`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca72f02c89a70e463873f7095a54263f02a7dc1fc35b8b3d92d0d6ed1114e1c3`  
		Last Modified: Wed, 14 Oct 2020 21:13:16 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744bfb9438a82d19472dbb92037ab018420b16a677b9451e9b92d13d9d4cc309`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab7908db3cd309e1cf3200fc5b51374d626702ea4ff411559cfa15da77b097d`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691b1b3fc24e5b473537703fcabf8cdc0acd56705ab671452b135de184ffbe0c`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba327018ef360de6c48ecbdb06f66a73defdb3996be6c2f17f0731514dbece5`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c122dffbcf7af8877cc67b8f468cd74a76d63a739b85f3ac429fb27794f724`  
		Last Modified: Wed, 14 Oct 2020 21:13:13 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbf77f12be69367c8fcf09b53209ec5b25083762192120e9ed3f8e429569a4f`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c631d9175a05b1f8c784df5ccc0daeda8990f4cfa0faebc76e525dc737e034`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b5835866e9c4e5a927e7b41da88a4c61a54547cc83fc91db1c1a43494bbac2`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13669d36e52f3d6963333d5102e23ad22fd5892d4fd1a9468f12194c39c2753`  
		Last Modified: Wed, 14 Oct 2020 21:13:11 GMT  
		Size: 299.0 KB (299047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f0e09c2bd5ebc6729c8f1d852f4adefae35e2335cd7dbbcc09c95205e95ab0`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:155acd240efff18a38a7aff934be0f6976aeb1c76139025671c9833ed160c840
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64

### `caddy:2-windowsservercore-ltsc2016` - windows version 10.0.14393.3986; amd64

```console
$ docker pull caddy@sha256:4c7f9ebc39d2e00064b805df702d5364f55de8cb8cf5ae58d8e4f438988069e8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5773083905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0ce891f0605eaed2c51c683e9fe3d70f29bf6588b85b1f2be21dfcba2c4fb3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 21:06:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Oct 2020 21:06:25 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 14 Oct 2020 21:07:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Oct 2020 21:07:57 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Oct 2020 21:07:58 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Oct 2020 21:07:59 GMT
VOLUME [c:/config]
# Wed, 14 Oct 2020 21:08:00 GMT
VOLUME [c:/data]
# Wed, 14 Oct 2020 21:08:01 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 14 Oct 2020 21:08:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Oct 2020 21:08:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Oct 2020 21:08:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Oct 2020 21:08:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Oct 2020 21:08:05 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Oct 2020 21:08:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Oct 2020 21:08:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Oct 2020 21:08:08 GMT
EXPOSE 80
# Wed, 14 Oct 2020 21:08:08 GMT
EXPOSE 443
# Wed, 14 Oct 2020 21:08:09 GMT
EXPOSE 2019
# Wed, 14 Oct 2020 21:08:53 GMT
RUN caddy version
# Wed, 14 Oct 2020 21:08:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2b4a4f0660702b9f47920e1e7ea79666ac43584dadc8412d8a7b7eb0490a2c`  
		Last Modified: Wed, 14 Oct 2020 21:13:59 GMT  
		Size: 9.9 MB (9925104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3c401ae3441b3e5b7543d5482214980c1c14958e2713fee5966c2622a53963`  
		Last Modified: Wed, 14 Oct 2020 21:13:55 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffab013bf500710ef95125418f98138723e756c560a1de0145379662b77335db`  
		Last Modified: Wed, 14 Oct 2020 21:14:00 GMT  
		Size: 21.5 MB (21518510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcf1f0773bd9f450a654eb5dcecd55e2e3fe3ba01eb0dae7dbf27e84402a6be`  
		Last Modified: Wed, 14 Oct 2020 21:13:53 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7077da12d3b43ef9b9dad1d8c770898c3a0224a8a0a3b99dc4656cc594d09b62`  
		Last Modified: Wed, 14 Oct 2020 21:13:53 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3976aabb2b169dd3bb85d39e2473fe70f7f15de0124b56095dd3c25fbbc27c`  
		Last Modified: Wed, 14 Oct 2020 21:13:52 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e5576c4d0eac332d8332455193ed1057c55aa90bd5e9a6bca884a25623c3c8`  
		Last Modified: Wed, 14 Oct 2020 21:13:52 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7210dc7c5fabd3bf6636614bc150a0965808e559f2b293340b4d8e049a185684`  
		Last Modified: Wed, 14 Oct 2020 21:13:50 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7af1dab2b20db7484c30ac3175b1dc3b89884f843ece3209fdab4882f5e018`  
		Last Modified: Wed, 14 Oct 2020 21:13:49 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe18c02535b810df5a6916e6ffe0a4532c5a70dae17b5ce28956695be585480`  
		Last Modified: Wed, 14 Oct 2020 21:13:50 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb1797af36c3af3ecc1e7db5ddfdba44c6bfff97b0515b3463d0948fed92ac4`  
		Last Modified: Wed, 14 Oct 2020 21:13:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98a2d0f6d0934d8a3b866e68ca5e7775b2af52b170aa71f2113de2d32d532a3`  
		Last Modified: Wed, 14 Oct 2020 21:13:48 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f14b6955af73ac11170ddb2c596a1dd963ceafda86300b2de8466357d56aa4`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ce0d3817eff364f0101431f28cb70cde3766120bbe5fb10b53ebf59363136f`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dd973289c284ff507f57773413c00c41a54ad2015bafb509c68a044b609cda`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6c2b7b482e55dcb167623e29563231f659e1a523cb8f6e83423bb1d69a2014`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7811e07229200779f1a17a1899bf48c49f0250685f18fdffb38ee7c30ab779`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d7cb4258c8b7eab1c92df575a363d8685d8d783672e5256208f715c662b27b`  
		Last Modified: Wed, 14 Oct 2020 21:13:44 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ab63ba04ec1b983074014465794ebf2e437ec4c03997ac40e1be3a4abcce61`  
		Last Modified: Wed, 14 Oct 2020 21:13:44 GMT  
		Size: 268.2 KB (268209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac54f9c3e58e5d406091c73dec798c29e2ee3134663b63d3ddb4959f10f4f32`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.2 KB (1152 bytes)  
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
$ docker pull caddy@sha256:d1feb42feaf8542d7efe2afee44c2a57540f14deb3961b86aa0b7ee6de1b7c77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:b506e57149af1435025a622cd356fc93257f02130f1e721a1a067362b1f88ddd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.7 MB (119671750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05d3a71d119dcebe678d25c39ff3d11b63d842f1cd4756e133e9c3a4faa0fe38`
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
# Thu, 22 Oct 2020 03:34:57 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 03:37:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 03:37:52 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 03:37:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 03:37:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 03:37:54 GMT
WORKDIR /go
# Thu, 22 Oct 2020 04:34:16 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 04:34:16 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 04:34:16 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 04:34:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 04:34:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 04:34:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 04:34:20 GMT
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
	-	`sha256:0eba1c9be4d292e332c2f27b821e199d8603b724238d9a4ce48c566533546298`  
		Last Modified: Thu, 22 Oct 2020 03:44:16 GMT  
		Size: 106.9 MB (106876307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d57e429df01b9589550363e9badf8beb2c0ef2cfb959fb7389948decaccc71f`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf71de68668ac772e9853d42397c63e34666b964b958c23d49616ecbd9df286`  
		Last Modified: Thu, 22 Oct 2020 04:35:15 GMT  
		Size: 8.3 MB (8309874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b116073137746923179401de3108b0ceda969a41fee25a4b097c75eaafee084`  
		Last Modified: Thu, 22 Oct 2020 04:35:14 GMT  
		Size: 1.4 MB (1407214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d809710fb5305cf38c3119a76bd45b286b83f7501326896adc101338a4766e`  
		Last Modified: Thu, 22 Oct 2020 04:35:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2f447ef196725a6fe1129ccca0b74d23ff3dfb38887d56e618348db89feae116
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114815426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b367cdbe3af19cc3dd00928134ec76ddeef267a733cb88a2e1c97b67a113b480`
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
# Thu, 22 Oct 2020 03:07:28 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 04:07:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 04:07:33 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 04:07:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 04:09:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 04:09:37 GMT
WORKDIR /go
# Thu, 22 Oct 2020 10:05:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 10:05:06 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 10:05:08 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 10:05:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 10:05:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 10:05:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 10:05:13 GMT
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
	-	`sha256:0861c41718d28217202ec1937beb9975a5bee4aec22544789a4941342423d823`  
		Last Modified: Thu, 22 Oct 2020 05:35:25 GMT  
		Size: 102.7 MB (102675647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189a4b66c7697ec4dec0236745f1b2130dd6699149d2259637327eef2d8fb5a3`  
		Last Modified: Thu, 22 Oct 2020 05:34:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43299b1fec8de48d0860d111e16df032ff921ceb1bfe97430ebe2d9c67900d99`  
		Last Modified: Thu, 22 Oct 2020 10:05:40 GMT  
		Size: 7.9 MB (7928833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4e67b21208cda0253a4fdeefdc15a2990ded4af282530e328cd7b48914ce8d`  
		Last Modified: Thu, 22 Oct 2020 10:05:38 GMT  
		Size: 1.3 MB (1327348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d25b580938f0aedbca674d485edf5de24f1e51289d0e2317ea8d1040f2fcaac`  
		Last Modified: Thu, 22 Oct 2020 10:05:38 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:53f07e930bd2ec03da216d3e8325f74985e425cfa28e027307b2165a68d918d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113627797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7140db1472303a8077c6b1e7cacc69b2d2594c3732b60b2a1c66257928694bd4`
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
# Thu, 22 Oct 2020 03:23:43 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 04:38:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 04:38:54 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 04:39:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 04:41:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 04:41:39 GMT
WORKDIR /go
# Thu, 22 Oct 2020 09:24:49 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 09:24:50 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 09:24:51 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 09:24:52 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 09:24:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 09:24:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 09:24:55 GMT
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
	-	`sha256:8cedb62f6546fc1b0d4fa80e293634cefa26d2336796ea8e8bc24eabc9bc501e`  
		Last Modified: Thu, 22 Oct 2020 06:00:08 GMT  
		Size: 102.5 MB (102470699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a88c985904d22a6adc07851b517bd17b6624e2b422ff3dfe8375de1283250d8`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc68f5c354cb3e9a5328b0f6341317092ad7a6081c8f1791c3857d479f79065`  
		Last Modified: Thu, 22 Oct 2020 09:25:24 GMT  
		Size: 7.1 MB (7144783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d905d9db6b8b7d05de2a2d569e2e8a9b617e197168db24c50a0fc2e6583f878`  
		Last Modified: Thu, 22 Oct 2020 09:25:24 GMT  
		Size: 1.3 MB (1325844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cb350ca3cb778c3ae223b0b0d844902b1ee234c91aa18341eaafc3a91cdc39`  
		Last Modified: Thu, 22 Oct 2020 09:25:22 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:33f8ff597086154bb625661b95eb1cf0ad74284a3fc00917506f2961ccc29a65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.0 MB (114950741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95c2f36f633ba51a79c3441793ba3bac5aa172347ccdbb8c8f371ce9e1e5fb41`
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
# Thu, 22 Oct 2020 04:10:13 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 04:15:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 04:15:31 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 04:15:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 04:17:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 04:17:40 GMT
WORKDIR /go
# Thu, 22 Oct 2020 09:30:37 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 09:30:38 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 09:30:45 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 09:30:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 09:30:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 09:30:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 09:30:59 GMT
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
	-	`sha256:5afe5f37f5b3016b6946fda75a1f4dce7778311971998bab26064ee548e69e57`  
		Last Modified: Thu, 22 Oct 2020 04:29:46 GMT  
		Size: 102.2 MB (102152165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d0fcabf3d036cdbe487c24ebdc36aa0cf4c2700b5b386791a3538d92071a62`  
		Last Modified: Thu, 22 Oct 2020 04:28:23 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466fde6265bf309aca5041a30a19ba0f889387ceb0872309caa82fd6531b221a`  
		Last Modified: Thu, 22 Oct 2020 09:31:34 GMT  
		Size: 8.5 MB (8499894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82672d1571ea79e8c88077d08e3c7022c89e0494a79368f22dd09e069761eeca`  
		Last Modified: Thu, 22 Oct 2020 09:31:32 GMT  
		Size: 1.3 MB (1310181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b29dbb8417e8cdce10eeeb84f0d7f37da96a00c256648362fd0a1130013462c`  
		Last Modified: Thu, 22 Oct 2020 09:31:32 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:1381ebb3e36c7f726363e75544a7cf23e07e34c50595cb35af607d6ead7655bf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.1 MB (114109814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8378d7f685f94342d985ca619645498434b64a6d62b7bf884dbb57030e7d923`
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
# Thu, 22 Oct 2020 13:27:55 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 13:30:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 13:30:31 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 13:30:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 13:30:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 13:30:50 GMT
WORKDIR /go
# Thu, 22 Oct 2020 13:45:58 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 13:46:02 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 13:46:10 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 13:46:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 13:46:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 13:46:34 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 13:46:37 GMT
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
	-	`sha256:a53757254f83d2b7412aa2718828ed0bd489d01d5bad2c6ee877672775244a8a`  
		Last Modified: Thu, 22 Oct 2020 13:36:50 GMT  
		Size: 100.8 MB (100814882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6876bebeafd85e7b46e88239c365eeec0a308353e7d1f7de434659ef597f889d`  
		Last Modified: Thu, 22 Oct 2020 13:36:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60beda9dadec93f6e90d3398b12787fc49427a3ba3a7e88e42e6105562016ec6`  
		Last Modified: Thu, 22 Oct 2020 13:48:15 GMT  
		Size: 8.9 MB (8920001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ca79d64160e09790e775af1b4204add8e6f21a3e837e1bd743c9b7b6b9c24a`  
		Last Modified: Thu, 22 Oct 2020 13:48:14 GMT  
		Size: 1.3 MB (1287791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7348aa6f5d47e3ce5091866c5cc3341d13a31faad6b1aa33e76e9432f45506a`  
		Last Modified: Thu, 22 Oct 2020 13:48:13 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:a8aa50ea100e687faa5739a6f62ec5843fc9846c874337726fed6ba09f3ac315
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118526471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7efeb3f913cdd9cdf7a017801f525a164c24a2efd93d1eb010477ca4094ac251`
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
# Thu, 22 Oct 2020 02:53:31 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 02:55:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 02:55:33 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 02:55:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 02:55:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 02:55:35 GMT
WORKDIR /go
# Thu, 22 Oct 2020 10:13:52 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 10:13:53 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 10:13:54 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 10:13:54 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 10:13:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 10:13:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 10:13:57 GMT
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
	-	`sha256:93a9f4b10b0ce05491e77b29b87fa3bbcbcd40e10a492d96185bf5ef0acc62f0`  
		Last Modified: Thu, 22 Oct 2020 02:58:45 GMT  
		Size: 105.9 MB (105937593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c973fb648f38c29beb5231f712f726631c6eb8fdaefbd4b7ac5408af2ea1a61`  
		Last Modified: Thu, 22 Oct 2020 02:58:32 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ff827958d5db211b007a45cc274d0658dcb49f4949f86888fa5f731d8df24a`  
		Last Modified: Thu, 22 Oct 2020 10:14:27 GMT  
		Size: 8.4 MB (8352218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36fa21e3b269069073c65c60c20545573892ddcd3d507593bc28a325da2b8c2`  
		Last Modified: Thu, 22 Oct 2020 10:14:26 GMT  
		Size: 1.4 MB (1388754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472fde2a1575da1d5a5924aab83ea94739ae66686513f4cfa7cd844707b59058`  
		Last Modified: Thu, 22 Oct 2020 10:14:26 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.1518; amd64

```console
$ docker pull caddy@sha256:5f0ba224d2ff94370fd2e10a05b2e06f062b1e9ba4278b62e9ecb99056ff4802
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2549102284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a10b666950b6ddd3242011e2bf926b6d52b2bb6f910ac359ac1b4b08e6db235c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 12:27:03 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Oct 2020 12:27:04 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Oct 2020 12:27:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Oct 2020 12:27:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Oct 2020 12:28:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Oct 2020 12:28:38 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Oct 2020 12:29:02 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 15 Oct 2020 01:14:39 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 15 Oct 2020 01:17:39 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1d579d0e980763f60bf43afb7c3783caf63433a485731ef4d2e262878d634b3f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 15 Oct 2020 01:17:40 GMT
WORKDIR C:\gopath
# Thu, 15 Oct 2020 02:32:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 15 Oct 2020 02:32:16 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 15 Oct 2020 02:32:17 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 15 Oct 2020 02:32:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 15 Oct 2020 02:32:40 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 15 Oct 2020 02:32:41 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23a75d88f9f5980bb112e2c28248975f107144d8d2e40dc4755e2a09f5e56df`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bea6d8b9d9b014ffa471b7bb8882ddb7e9d378ddcacc099f0710073bd6361b9`  
		Last Modified: Wed, 14 Oct 2020 12:50:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75c1905c0573cc5706bc066d23624f0e92a8871832c744fbe7eabdcbc6f8a85`  
		Last Modified: Wed, 14 Oct 2020 12:50:24 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938695376d9deeba8819539ff3245935c28f93229d1c332bb8b6a16e67013fbc`  
		Last Modified: Wed, 14 Oct 2020 12:50:23 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41106c6a476cf9666c6d8c3c853c982a841c29db05b3ef8a072baba537b6d74c`  
		Last Modified: Wed, 14 Oct 2020 12:50:48 GMT  
		Size: 34.3 MB (34312667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d6d6258831f87f3b455e6316e2bed430465a760272614de7cdd28c7c6e9f3e`  
		Last Modified: Wed, 14 Oct 2020 12:50:19 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e3f66638c4d5ce9adba16e49844f57efbab1d628d9d6c73133511b7c1c3892`  
		Last Modified: Wed, 14 Oct 2020 12:50:20 GMT  
		Size: 310.5 KB (310525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe34732f84b95b980d0ae0624ebae44818ef7879e34a9ffbebe752f1dcd4badf`  
		Last Modified: Thu, 15 Oct 2020 02:05:08 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a6c4c70f4e593c0500bebe3fa23edab8bd791805ab4a5edf34cb053b21264f`  
		Last Modified: Thu, 15 Oct 2020 02:05:35 GMT  
		Size: 138.6 MB (138590451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123678d8baa038225b16066bfa2f971f7454f2d5b16b95db1663954869cf837a`  
		Last Modified: Thu, 15 Oct 2020 02:05:07 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99abf6100e15da95d12aff85cd77f0adf4d96b7b1b2815445a9fc6f576c3df79`  
		Last Modified: Thu, 15 Oct 2020 02:35:13 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908a905e414249fe5a6b10921f1505b4e5edb7bad45fd2f70a3095f99e8d3929`  
		Last Modified: Thu, 15 Oct 2020 02:35:10 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beea46a5312f34364874857e7fdd21b76239ae4028aeabd8ef4e7092e536fda0`  
		Last Modified: Thu, 15 Oct 2020 02:35:09 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb245ad725b068d3bb29ee875394207d019d445c185bf1ca1ddd2ce1c62ce38`  
		Last Modified: Thu, 15 Oct 2020 02:35:10 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9cd8369d2f668d2d300f35c9d9ee98488040b7b695efbaadb1d3b76f314eac`  
		Last Modified: Thu, 15 Oct 2020 02:35:10 GMT  
		Size: 1.8 MB (1783668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798dfde6e8213d06ef180571d9c1956e9b42899062509ff88cfbc453b3ff9c37`  
		Last Modified: Thu, 15 Oct 2020 02:35:09 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.14393.3986; amd64

```console
$ docker pull caddy@sha256:8fea2fa2956f6e7eb56eb8f745fe7b6f4a7ccf45bd259d7a8cccb3d2c71f3c1f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5941324722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4f39f7f404783da13552d7024d9a3262d0d6a1834385977fb514556a43e41f9`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 12:31:45 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Oct 2020 12:31:46 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Oct 2020 12:31:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Oct 2020 12:31:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Oct 2020 12:33:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Oct 2020 12:33:58 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Oct 2020 12:35:13 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 15 Oct 2020 01:17:52 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 15 Oct 2020 01:21:40 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1d579d0e980763f60bf43afb7c3783caf63433a485731ef4d2e262878d634b3f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 15 Oct 2020 01:21:41 GMT
WORKDIR C:\gopath
# Thu, 15 Oct 2020 02:32:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 15 Oct 2020 02:32:47 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 15 Oct 2020 02:32:48 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 15 Oct 2020 02:32:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 15 Oct 2020 02:34:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 15 Oct 2020 02:34:06 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528ba1d9759adcc464112008fe49672e1f545981d69bab31186587ab32f92138`  
		Last Modified: Wed, 14 Oct 2020 12:51:33 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53bf4e6180661653575845d30a4d882dea92f395cb540b1cdf91170e9ee58731`  
		Last Modified: Wed, 14 Oct 2020 12:51:30 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e973f094614bb2cebe16df6f6004c05895ed077151aecdbbd0c476513054fc`  
		Last Modified: Wed, 14 Oct 2020 12:51:25 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1089b875ac355097876e23760dd2166f096a8645e312660ffd3c0e617a2df9a0`  
		Last Modified: Wed, 14 Oct 2020 12:51:29 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8934a016b666d0691307c6414d84c36eb82de4b2fc4d74dd04c75f632dc3a78c`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 35.0 MB (35016991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4d95d13c0a45aa19a623e51cb112530a589a3a4d15d5c119610f8196912fab`  
		Last Modified: Wed, 14 Oct 2020 12:51:20 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf8226941bb8f5af9f2be8fdb54da3e3caef344b0061a73e3debde23a55e98f`  
		Last Modified: Wed, 14 Oct 2020 12:51:24 GMT  
		Size: 9.9 MB (9870100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b8d8683ed903732b7672eb374d957e4ad20a8936cd48bc9a69059c19163325`  
		Last Modified: Thu, 15 Oct 2020 02:05:58 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38f6e003c1013456c5993d4c122314dab53690c52405c373b2055e636353e47`  
		Last Modified: Thu, 15 Oct 2020 02:06:27 GMT  
		Size: 143.8 MB (143758677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbc6767c79760c5d4cd356ae2dd0742f8d13be9298959aa3009b1e4d2c18cbc`  
		Last Modified: Thu, 15 Oct 2020 02:05:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba9f5f016316461f4d80f3defd59bad0cd10886ae46ef3ad8802facb8a3330b`  
		Last Modified: Thu, 15 Oct 2020 02:35:33 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b074f2cce57588dbf6e04970c0be7db19be264eee3f4bb3a7b4bbcf4fd717b95`  
		Last Modified: Thu, 15 Oct 2020 02:35:30 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b1d6dbe2c318375f7055dc79b3b4b44a06e13238cb914eddfb5cfa258f86c6`  
		Last Modified: Thu, 15 Oct 2020 02:35:30 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c349a444d08c6b059ed2430ee7e28766f5ac7a411eeadb73dad01e26fc70916`  
		Last Modified: Thu, 15 Oct 2020 02:35:30 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1bc4e5aa1948e251b46da1e6c6c5632371f1bf5a60c64269247ec5d348fb22`  
		Last Modified: Thu, 15 Oct 2020 02:35:33 GMT  
		Size: 11.3 MB (11312385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed394fa51b2433c7ce756430011e4cc52ac6d67198f2bf0ae8144eafa44a2a89`  
		Last Modified: Thu, 15 Oct 2020 02:35:31 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:a42199f0a07411337da8367217434680136db2e93e04b596aa8d9399325f25f6
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
$ docker pull caddy@sha256:b506e57149af1435025a622cd356fc93257f02130f1e721a1a067362b1f88ddd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.7 MB (119671750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05d3a71d119dcebe678d25c39ff3d11b63d842f1cd4756e133e9c3a4faa0fe38`
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
# Thu, 22 Oct 2020 03:34:57 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 03:37:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 03:37:52 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 03:37:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 03:37:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 03:37:54 GMT
WORKDIR /go
# Thu, 22 Oct 2020 04:34:16 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 04:34:16 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 04:34:16 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 04:34:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 04:34:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 04:34:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 04:34:20 GMT
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
	-	`sha256:0eba1c9be4d292e332c2f27b821e199d8603b724238d9a4ce48c566533546298`  
		Last Modified: Thu, 22 Oct 2020 03:44:16 GMT  
		Size: 106.9 MB (106876307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d57e429df01b9589550363e9badf8beb2c0ef2cfb959fb7389948decaccc71f`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf71de68668ac772e9853d42397c63e34666b964b958c23d49616ecbd9df286`  
		Last Modified: Thu, 22 Oct 2020 04:35:15 GMT  
		Size: 8.3 MB (8309874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b116073137746923179401de3108b0ceda969a41fee25a4b097c75eaafee084`  
		Last Modified: Thu, 22 Oct 2020 04:35:14 GMT  
		Size: 1.4 MB (1407214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d809710fb5305cf38c3119a76bd45b286b83f7501326896adc101338a4766e`  
		Last Modified: Thu, 22 Oct 2020 04:35:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2f447ef196725a6fe1129ccca0b74d23ff3dfb38887d56e618348db89feae116
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114815426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b367cdbe3af19cc3dd00928134ec76ddeef267a733cb88a2e1c97b67a113b480`
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
# Thu, 22 Oct 2020 03:07:28 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 04:07:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 04:07:33 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 04:07:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 04:09:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 04:09:37 GMT
WORKDIR /go
# Thu, 22 Oct 2020 10:05:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 10:05:06 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 10:05:08 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 10:05:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 10:05:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 10:05:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 10:05:13 GMT
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
	-	`sha256:0861c41718d28217202ec1937beb9975a5bee4aec22544789a4941342423d823`  
		Last Modified: Thu, 22 Oct 2020 05:35:25 GMT  
		Size: 102.7 MB (102675647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189a4b66c7697ec4dec0236745f1b2130dd6699149d2259637327eef2d8fb5a3`  
		Last Modified: Thu, 22 Oct 2020 05:34:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43299b1fec8de48d0860d111e16df032ff921ceb1bfe97430ebe2d9c67900d99`  
		Last Modified: Thu, 22 Oct 2020 10:05:40 GMT  
		Size: 7.9 MB (7928833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4e67b21208cda0253a4fdeefdc15a2990ded4af282530e328cd7b48914ce8d`  
		Last Modified: Thu, 22 Oct 2020 10:05:38 GMT  
		Size: 1.3 MB (1327348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d25b580938f0aedbca674d485edf5de24f1e51289d0e2317ea8d1040f2fcaac`  
		Last Modified: Thu, 22 Oct 2020 10:05:38 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:53f07e930bd2ec03da216d3e8325f74985e425cfa28e027307b2165a68d918d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113627797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7140db1472303a8077c6b1e7cacc69b2d2594c3732b60b2a1c66257928694bd4`
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
# Thu, 22 Oct 2020 03:23:43 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 04:38:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 04:38:54 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 04:39:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 04:41:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 04:41:39 GMT
WORKDIR /go
# Thu, 22 Oct 2020 09:24:49 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 09:24:50 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 09:24:51 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 09:24:52 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 09:24:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 09:24:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 09:24:55 GMT
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
	-	`sha256:8cedb62f6546fc1b0d4fa80e293634cefa26d2336796ea8e8bc24eabc9bc501e`  
		Last Modified: Thu, 22 Oct 2020 06:00:08 GMT  
		Size: 102.5 MB (102470699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a88c985904d22a6adc07851b517bd17b6624e2b422ff3dfe8375de1283250d8`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc68f5c354cb3e9a5328b0f6341317092ad7a6081c8f1791c3857d479f79065`  
		Last Modified: Thu, 22 Oct 2020 09:25:24 GMT  
		Size: 7.1 MB (7144783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d905d9db6b8b7d05de2a2d569e2e8a9b617e197168db24c50a0fc2e6583f878`  
		Last Modified: Thu, 22 Oct 2020 09:25:24 GMT  
		Size: 1.3 MB (1325844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cb350ca3cb778c3ae223b0b0d844902b1ee234c91aa18341eaafc3a91cdc39`  
		Last Modified: Thu, 22 Oct 2020 09:25:22 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:33f8ff597086154bb625661b95eb1cf0ad74284a3fc00917506f2961ccc29a65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.0 MB (114950741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95c2f36f633ba51a79c3441793ba3bac5aa172347ccdbb8c8f371ce9e1e5fb41`
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
# Thu, 22 Oct 2020 04:10:13 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 04:15:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 04:15:31 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 04:15:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 04:17:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 04:17:40 GMT
WORKDIR /go
# Thu, 22 Oct 2020 09:30:37 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 09:30:38 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 09:30:45 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 09:30:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 09:30:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 09:30:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 09:30:59 GMT
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
	-	`sha256:5afe5f37f5b3016b6946fda75a1f4dce7778311971998bab26064ee548e69e57`  
		Last Modified: Thu, 22 Oct 2020 04:29:46 GMT  
		Size: 102.2 MB (102152165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d0fcabf3d036cdbe487c24ebdc36aa0cf4c2700b5b386791a3538d92071a62`  
		Last Modified: Thu, 22 Oct 2020 04:28:23 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466fde6265bf309aca5041a30a19ba0f889387ceb0872309caa82fd6531b221a`  
		Last Modified: Thu, 22 Oct 2020 09:31:34 GMT  
		Size: 8.5 MB (8499894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82672d1571ea79e8c88077d08e3c7022c89e0494a79368f22dd09e069761eeca`  
		Last Modified: Thu, 22 Oct 2020 09:31:32 GMT  
		Size: 1.3 MB (1310181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b29dbb8417e8cdce10eeeb84f0d7f37da96a00c256648362fd0a1130013462c`  
		Last Modified: Thu, 22 Oct 2020 09:31:32 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:1381ebb3e36c7f726363e75544a7cf23e07e34c50595cb35af607d6ead7655bf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.1 MB (114109814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8378d7f685f94342d985ca619645498434b64a6d62b7bf884dbb57030e7d923`
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
# Thu, 22 Oct 2020 13:27:55 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 13:30:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 13:30:31 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 13:30:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 13:30:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 13:30:50 GMT
WORKDIR /go
# Thu, 22 Oct 2020 13:45:58 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 13:46:02 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 13:46:10 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 13:46:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 13:46:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 13:46:34 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 13:46:37 GMT
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
	-	`sha256:a53757254f83d2b7412aa2718828ed0bd489d01d5bad2c6ee877672775244a8a`  
		Last Modified: Thu, 22 Oct 2020 13:36:50 GMT  
		Size: 100.8 MB (100814882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6876bebeafd85e7b46e88239c365eeec0a308353e7d1f7de434659ef597f889d`  
		Last Modified: Thu, 22 Oct 2020 13:36:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60beda9dadec93f6e90d3398b12787fc49427a3ba3a7e88e42e6105562016ec6`  
		Last Modified: Thu, 22 Oct 2020 13:48:15 GMT  
		Size: 8.9 MB (8920001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ca79d64160e09790e775af1b4204add8e6f21a3e837e1bd743c9b7b6b9c24a`  
		Last Modified: Thu, 22 Oct 2020 13:48:14 GMT  
		Size: 1.3 MB (1287791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7348aa6f5d47e3ce5091866c5cc3341d13a31faad6b1aa33e76e9432f45506a`  
		Last Modified: Thu, 22 Oct 2020 13:48:13 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:a8aa50ea100e687faa5739a6f62ec5843fc9846c874337726fed6ba09f3ac315
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118526471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7efeb3f913cdd9cdf7a017801f525a164c24a2efd93d1eb010477ca4094ac251`
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
# Thu, 22 Oct 2020 02:53:31 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 22 Oct 2020 02:55:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 	sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 22 Oct 2020 02:55:33 GMT
ENV GOPATH=/go
# Thu, 22 Oct 2020 02:55:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 02:55:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Oct 2020 02:55:35 GMT
WORKDIR /go
# Thu, 22 Oct 2020 10:13:52 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 22 Oct 2020 10:13:53 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 22 Oct 2020 10:13:54 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 10:13:54 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Oct 2020 10:13:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 22 Oct 2020 10:13:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 22 Oct 2020 10:13:57 GMT
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
	-	`sha256:93a9f4b10b0ce05491e77b29b87fa3bbcbcd40e10a492d96185bf5ef0acc62f0`  
		Last Modified: Thu, 22 Oct 2020 02:58:45 GMT  
		Size: 105.9 MB (105937593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c973fb648f38c29beb5231f712f726631c6eb8fdaefbd4b7ac5408af2ea1a61`  
		Last Modified: Thu, 22 Oct 2020 02:58:32 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ff827958d5db211b007a45cc274d0658dcb49f4949f86888fa5f731d8df24a`  
		Last Modified: Thu, 22 Oct 2020 10:14:27 GMT  
		Size: 8.4 MB (8352218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36fa21e3b269069073c65c60c20545573892ddcd3d507593bc28a325da2b8c2`  
		Last Modified: Thu, 22 Oct 2020 10:14:26 GMT  
		Size: 1.4 MB (1388754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472fde2a1575da1d5a5924aab83ea94739ae66686513f4cfa7cd844707b59058`  
		Last Modified: Thu, 22 Oct 2020 10:14:26 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:ab8f8e005e8197265d91e6dcb9b94990e7b89b8474a015df00bc498851522a81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull caddy@sha256:5f0ba224d2ff94370fd2e10a05b2e06f062b1e9ba4278b62e9ecb99056ff4802
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2549102284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a10b666950b6ddd3242011e2bf926b6d52b2bb6f910ac359ac1b4b08e6db235c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 12:27:03 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Oct 2020 12:27:04 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Oct 2020 12:27:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Oct 2020 12:27:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Oct 2020 12:28:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Oct 2020 12:28:38 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Oct 2020 12:29:02 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 15 Oct 2020 01:14:39 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 15 Oct 2020 01:17:39 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1d579d0e980763f60bf43afb7c3783caf63433a485731ef4d2e262878d634b3f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 15 Oct 2020 01:17:40 GMT
WORKDIR C:\gopath
# Thu, 15 Oct 2020 02:32:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 15 Oct 2020 02:32:16 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 15 Oct 2020 02:32:17 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 15 Oct 2020 02:32:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 15 Oct 2020 02:32:40 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 15 Oct 2020 02:32:41 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23a75d88f9f5980bb112e2c28248975f107144d8d2e40dc4755e2a09f5e56df`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bea6d8b9d9b014ffa471b7bb8882ddb7e9d378ddcacc099f0710073bd6361b9`  
		Last Modified: Wed, 14 Oct 2020 12:50:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75c1905c0573cc5706bc066d23624f0e92a8871832c744fbe7eabdcbc6f8a85`  
		Last Modified: Wed, 14 Oct 2020 12:50:24 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938695376d9deeba8819539ff3245935c28f93229d1c332bb8b6a16e67013fbc`  
		Last Modified: Wed, 14 Oct 2020 12:50:23 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41106c6a476cf9666c6d8c3c853c982a841c29db05b3ef8a072baba537b6d74c`  
		Last Modified: Wed, 14 Oct 2020 12:50:48 GMT  
		Size: 34.3 MB (34312667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d6d6258831f87f3b455e6316e2bed430465a760272614de7cdd28c7c6e9f3e`  
		Last Modified: Wed, 14 Oct 2020 12:50:19 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e3f66638c4d5ce9adba16e49844f57efbab1d628d9d6c73133511b7c1c3892`  
		Last Modified: Wed, 14 Oct 2020 12:50:20 GMT  
		Size: 310.5 KB (310525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe34732f84b95b980d0ae0624ebae44818ef7879e34a9ffbebe752f1dcd4badf`  
		Last Modified: Thu, 15 Oct 2020 02:05:08 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a6c4c70f4e593c0500bebe3fa23edab8bd791805ab4a5edf34cb053b21264f`  
		Last Modified: Thu, 15 Oct 2020 02:05:35 GMT  
		Size: 138.6 MB (138590451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123678d8baa038225b16066bfa2f971f7454f2d5b16b95db1663954869cf837a`  
		Last Modified: Thu, 15 Oct 2020 02:05:07 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99abf6100e15da95d12aff85cd77f0adf4d96b7b1b2815445a9fc6f576c3df79`  
		Last Modified: Thu, 15 Oct 2020 02:35:13 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908a905e414249fe5a6b10921f1505b4e5edb7bad45fd2f70a3095f99e8d3929`  
		Last Modified: Thu, 15 Oct 2020 02:35:10 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beea46a5312f34364874857e7fdd21b76239ae4028aeabd8ef4e7092e536fda0`  
		Last Modified: Thu, 15 Oct 2020 02:35:09 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb245ad725b068d3bb29ee875394207d019d445c185bf1ca1ddd2ce1c62ce38`  
		Last Modified: Thu, 15 Oct 2020 02:35:10 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9cd8369d2f668d2d300f35c9d9ee98488040b7b695efbaadb1d3b76f314eac`  
		Last Modified: Thu, 15 Oct 2020 02:35:10 GMT  
		Size: 1.8 MB (1783668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798dfde6e8213d06ef180571d9c1956e9b42899062509ff88cfbc453b3ff9c37`  
		Last Modified: Thu, 15 Oct 2020 02:35:09 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:193e2b1f70d18f86f7e53052a5a343e8a9538646a3089c4eedf3e1441e7b1e4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64

### `caddy:builder-windowsservercore-ltsc2016` - windows version 10.0.14393.3986; amd64

```console
$ docker pull caddy@sha256:8fea2fa2956f6e7eb56eb8f745fe7b6f4a7ccf45bd259d7a8cccb3d2c71f3c1f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5941324722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4f39f7f404783da13552d7024d9a3262d0d6a1834385977fb514556a43e41f9`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 12:31:45 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Oct 2020 12:31:46 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Oct 2020 12:31:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Oct 2020 12:31:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Oct 2020 12:33:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Oct 2020 12:33:58 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Oct 2020 12:35:13 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 15 Oct 2020 01:17:52 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 15 Oct 2020 01:21:40 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1d579d0e980763f60bf43afb7c3783caf63433a485731ef4d2e262878d634b3f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 15 Oct 2020 01:21:41 GMT
WORKDIR C:\gopath
# Thu, 15 Oct 2020 02:32:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 15 Oct 2020 02:32:47 GMT
ENV XCADDY_VERSION=v0.1.5
# Thu, 15 Oct 2020 02:32:48 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 15 Oct 2020 02:32:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 15 Oct 2020 02:34:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 15 Oct 2020 02:34:06 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528ba1d9759adcc464112008fe49672e1f545981d69bab31186587ab32f92138`  
		Last Modified: Wed, 14 Oct 2020 12:51:33 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53bf4e6180661653575845d30a4d882dea92f395cb540b1cdf91170e9ee58731`  
		Last Modified: Wed, 14 Oct 2020 12:51:30 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e973f094614bb2cebe16df6f6004c05895ed077151aecdbbd0c476513054fc`  
		Last Modified: Wed, 14 Oct 2020 12:51:25 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1089b875ac355097876e23760dd2166f096a8645e312660ffd3c0e617a2df9a0`  
		Last Modified: Wed, 14 Oct 2020 12:51:29 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8934a016b666d0691307c6414d84c36eb82de4b2fc4d74dd04c75f632dc3a78c`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 35.0 MB (35016991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4d95d13c0a45aa19a623e51cb112530a589a3a4d15d5c119610f8196912fab`  
		Last Modified: Wed, 14 Oct 2020 12:51:20 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf8226941bb8f5af9f2be8fdb54da3e3caef344b0061a73e3debde23a55e98f`  
		Last Modified: Wed, 14 Oct 2020 12:51:24 GMT  
		Size: 9.9 MB (9870100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b8d8683ed903732b7672eb374d957e4ad20a8936cd48bc9a69059c19163325`  
		Last Modified: Thu, 15 Oct 2020 02:05:58 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38f6e003c1013456c5993d4c122314dab53690c52405c373b2055e636353e47`  
		Last Modified: Thu, 15 Oct 2020 02:06:27 GMT  
		Size: 143.8 MB (143758677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbc6767c79760c5d4cd356ae2dd0742f8d13be9298959aa3009b1e4d2c18cbc`  
		Last Modified: Thu, 15 Oct 2020 02:05:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba9f5f016316461f4d80f3defd59bad0cd10886ae46ef3ad8802facb8a3330b`  
		Last Modified: Thu, 15 Oct 2020 02:35:33 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b074f2cce57588dbf6e04970c0be7db19be264eee3f4bb3a7b4bbcf4fd717b95`  
		Last Modified: Thu, 15 Oct 2020 02:35:30 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b1d6dbe2c318375f7055dc79b3b4b44a06e13238cb914eddfb5cfa258f86c6`  
		Last Modified: Thu, 15 Oct 2020 02:35:30 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c349a444d08c6b059ed2430ee7e28766f5ac7a411eeadb73dad01e26fc70916`  
		Last Modified: Thu, 15 Oct 2020 02:35:30 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1bc4e5aa1948e251b46da1e6c6c5632371f1bf5a60c64269247ec5d348fb22`  
		Last Modified: Thu, 15 Oct 2020 02:35:33 GMT  
		Size: 11.3 MB (11312385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed394fa51b2433c7ce756430011e4cc52ac6d67198f2bf0ae8144eafa44a2a89`  
		Last Modified: Thu, 15 Oct 2020 02:35:31 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:b44006ca7a107edd0fca2ff7a70cf75b81b20b61b722dff8a720364a3764ffd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

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

### `caddy:latest` - windows version 10.0.17763.1518; amd64

```console
$ docker pull caddy@sha256:5b0edc0113282eff2b0b97cb2768aef9406975982b52b5801fe66a3b7e0f1f6b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2399991421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4a3be7f6340286c7cad100a7baf86ff095c7d81ce5c10b5c314e8d7e73a9ade`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 21:03:47 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Oct 2020 21:03:48 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 14 Oct 2020 21:04:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Oct 2020 21:04:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Oct 2020 21:04:21 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Oct 2020 21:04:22 GMT
VOLUME [c:/config]
# Wed, 14 Oct 2020 21:04:23 GMT
VOLUME [c:/data]
# Wed, 14 Oct 2020 21:04:24 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 14 Oct 2020 21:04:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Oct 2020 21:04:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Oct 2020 21:04:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Oct 2020 21:04:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Oct 2020 21:04:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Oct 2020 21:04:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Oct 2020 21:04:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Oct 2020 21:04:29 GMT
EXPOSE 80
# Wed, 14 Oct 2020 21:04:30 GMT
EXPOSE 443
# Wed, 14 Oct 2020 21:04:30 GMT
EXPOSE 2019
# Wed, 14 Oct 2020 21:04:46 GMT
RUN caddy version
# Wed, 14 Oct 2020 21:04:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590b685e6f8e8fa4cbca8ce94e257baf1c179f183afabfc59bdff4420027e080`  
		Last Modified: Wed, 14 Oct 2020 21:13:24 GMT  
		Size: 9.2 MB (9237870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8a16e6bfc40544aeeaa55e8406570aec66018352db80098da3663138201f74`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468f02630a43054839d6262fe9f0d41cdd551ab83bbbb35c26cd9ead72ce6985`  
		Last Modified: Wed, 14 Oct 2020 21:13:25 GMT  
		Size: 16.3 MB (16343904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcdb09f7b5a57cb7fce28be7e54975dfc770735e4570b259b9104ddc8421bbd`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4b2b1c53bbf344fa90b58a9d5ee4b990881289dde49074cecd1f0da649c20a`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01bade2ee2333f9cd004bd1812f0c1fc7f55b2297cf57b8343e17b48c9d3535`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b312fdc7f27df222f05918031d72e4457582b08c8fdeff7cde88a6a402b6f0c`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053d376e7f1eb8e50a394d7247f16006d36ae65144e75d37fe8bb0740d91695f`  
		Last Modified: Wed, 14 Oct 2020 21:13:18 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d88dd9c5821fcba44cce1002ed12b8702e0cbec6ee8d137cbec8e5bd145acd5`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca72f02c89a70e463873f7095a54263f02a7dc1fc35b8b3d92d0d6ed1114e1c3`  
		Last Modified: Wed, 14 Oct 2020 21:13:16 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744bfb9438a82d19472dbb92037ab018420b16a677b9451e9b92d13d9d4cc309`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab7908db3cd309e1cf3200fc5b51374d626702ea4ff411559cfa15da77b097d`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691b1b3fc24e5b473537703fcabf8cdc0acd56705ab671452b135de184ffbe0c`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba327018ef360de6c48ecbdb06f66a73defdb3996be6c2f17f0731514dbece5`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c122dffbcf7af8877cc67b8f468cd74a76d63a739b85f3ac429fb27794f724`  
		Last Modified: Wed, 14 Oct 2020 21:13:13 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbf77f12be69367c8fcf09b53209ec5b25083762192120e9ed3f8e429569a4f`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c631d9175a05b1f8c784df5ccc0daeda8990f4cfa0faebc76e525dc737e034`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b5835866e9c4e5a927e7b41da88a4c61a54547cc83fc91db1c1a43494bbac2`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13669d36e52f3d6963333d5102e23ad22fd5892d4fd1a9468f12194c39c2753`  
		Last Modified: Wed, 14 Oct 2020 21:13:11 GMT  
		Size: 299.0 KB (299047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f0e09c2bd5ebc6729c8f1d852f4adefae35e2335cd7dbbcc09c95205e95ab0`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.14393.3986; amd64

```console
$ docker pull caddy@sha256:4c7f9ebc39d2e00064b805df702d5364f55de8cb8cf5ae58d8e4f438988069e8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5773083905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0ce891f0605eaed2c51c683e9fe3d70f29bf6588b85b1f2be21dfcba2c4fb3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 21:06:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Oct 2020 21:06:25 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 14 Oct 2020 21:07:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Oct 2020 21:07:57 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Oct 2020 21:07:58 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Oct 2020 21:07:59 GMT
VOLUME [c:/config]
# Wed, 14 Oct 2020 21:08:00 GMT
VOLUME [c:/data]
# Wed, 14 Oct 2020 21:08:01 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 14 Oct 2020 21:08:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Oct 2020 21:08:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Oct 2020 21:08:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Oct 2020 21:08:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Oct 2020 21:08:05 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Oct 2020 21:08:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Oct 2020 21:08:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Oct 2020 21:08:08 GMT
EXPOSE 80
# Wed, 14 Oct 2020 21:08:08 GMT
EXPOSE 443
# Wed, 14 Oct 2020 21:08:09 GMT
EXPOSE 2019
# Wed, 14 Oct 2020 21:08:53 GMT
RUN caddy version
# Wed, 14 Oct 2020 21:08:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2b4a4f0660702b9f47920e1e7ea79666ac43584dadc8412d8a7b7eb0490a2c`  
		Last Modified: Wed, 14 Oct 2020 21:13:59 GMT  
		Size: 9.9 MB (9925104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3c401ae3441b3e5b7543d5482214980c1c14958e2713fee5966c2622a53963`  
		Last Modified: Wed, 14 Oct 2020 21:13:55 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffab013bf500710ef95125418f98138723e756c560a1de0145379662b77335db`  
		Last Modified: Wed, 14 Oct 2020 21:14:00 GMT  
		Size: 21.5 MB (21518510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcf1f0773bd9f450a654eb5dcecd55e2e3fe3ba01eb0dae7dbf27e84402a6be`  
		Last Modified: Wed, 14 Oct 2020 21:13:53 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7077da12d3b43ef9b9dad1d8c770898c3a0224a8a0a3b99dc4656cc594d09b62`  
		Last Modified: Wed, 14 Oct 2020 21:13:53 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3976aabb2b169dd3bb85d39e2473fe70f7f15de0124b56095dd3c25fbbc27c`  
		Last Modified: Wed, 14 Oct 2020 21:13:52 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e5576c4d0eac332d8332455193ed1057c55aa90bd5e9a6bca884a25623c3c8`  
		Last Modified: Wed, 14 Oct 2020 21:13:52 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7210dc7c5fabd3bf6636614bc150a0965808e559f2b293340b4d8e049a185684`  
		Last Modified: Wed, 14 Oct 2020 21:13:50 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7af1dab2b20db7484c30ac3175b1dc3b89884f843ece3209fdab4882f5e018`  
		Last Modified: Wed, 14 Oct 2020 21:13:49 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe18c02535b810df5a6916e6ffe0a4532c5a70dae17b5ce28956695be585480`  
		Last Modified: Wed, 14 Oct 2020 21:13:50 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb1797af36c3af3ecc1e7db5ddfdba44c6bfff97b0515b3463d0948fed92ac4`  
		Last Modified: Wed, 14 Oct 2020 21:13:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98a2d0f6d0934d8a3b866e68ca5e7775b2af52b170aa71f2113de2d32d532a3`  
		Last Modified: Wed, 14 Oct 2020 21:13:48 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f14b6955af73ac11170ddb2c596a1dd963ceafda86300b2de8466357d56aa4`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ce0d3817eff364f0101431f28cb70cde3766120bbe5fb10b53ebf59363136f`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dd973289c284ff507f57773413c00c41a54ad2015bafb509c68a044b609cda`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6c2b7b482e55dcb167623e29563231f659e1a523cb8f6e83423bb1d69a2014`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7811e07229200779f1a17a1899bf48c49f0250685f18fdffb38ee7c30ab779`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d7cb4258c8b7eab1c92df575a363d8685d8d783672e5256208f715c662b27b`  
		Last Modified: Wed, 14 Oct 2020 21:13:44 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ab63ba04ec1b983074014465794ebf2e437ec4c03997ac40e1be3a4abcce61`  
		Last Modified: Wed, 14 Oct 2020 21:13:44 GMT  
		Size: 268.2 KB (268209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac54f9c3e58e5d406091c73dec798c29e2ee3134663b63d3ddb4959f10f4f32`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:0cc9e18409440159fbf2ac241bce180b0214fc5d2358aa87fedf1189394d7469
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.1518; amd64

```console
$ docker pull caddy@sha256:5b0edc0113282eff2b0b97cb2768aef9406975982b52b5801fe66a3b7e0f1f6b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2399991421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4a3be7f6340286c7cad100a7baf86ff095c7d81ce5c10b5c314e8d7e73a9ade`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 21:03:47 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Oct 2020 21:03:48 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 14 Oct 2020 21:04:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Oct 2020 21:04:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Oct 2020 21:04:21 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Oct 2020 21:04:22 GMT
VOLUME [c:/config]
# Wed, 14 Oct 2020 21:04:23 GMT
VOLUME [c:/data]
# Wed, 14 Oct 2020 21:04:24 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 14 Oct 2020 21:04:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Oct 2020 21:04:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Oct 2020 21:04:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Oct 2020 21:04:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Oct 2020 21:04:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Oct 2020 21:04:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Oct 2020 21:04:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Oct 2020 21:04:29 GMT
EXPOSE 80
# Wed, 14 Oct 2020 21:04:30 GMT
EXPOSE 443
# Wed, 14 Oct 2020 21:04:30 GMT
EXPOSE 2019
# Wed, 14 Oct 2020 21:04:46 GMT
RUN caddy version
# Wed, 14 Oct 2020 21:04:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590b685e6f8e8fa4cbca8ce94e257baf1c179f183afabfc59bdff4420027e080`  
		Last Modified: Wed, 14 Oct 2020 21:13:24 GMT  
		Size: 9.2 MB (9237870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8a16e6bfc40544aeeaa55e8406570aec66018352db80098da3663138201f74`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468f02630a43054839d6262fe9f0d41cdd551ab83bbbb35c26cd9ead72ce6985`  
		Last Modified: Wed, 14 Oct 2020 21:13:25 GMT  
		Size: 16.3 MB (16343904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcdb09f7b5a57cb7fce28be7e54975dfc770735e4570b259b9104ddc8421bbd`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4b2b1c53bbf344fa90b58a9d5ee4b990881289dde49074cecd1f0da649c20a`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01bade2ee2333f9cd004bd1812f0c1fc7f55b2297cf57b8343e17b48c9d3535`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b312fdc7f27df222f05918031d72e4457582b08c8fdeff7cde88a6a402b6f0c`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053d376e7f1eb8e50a394d7247f16006d36ae65144e75d37fe8bb0740d91695f`  
		Last Modified: Wed, 14 Oct 2020 21:13:18 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d88dd9c5821fcba44cce1002ed12b8702e0cbec6ee8d137cbec8e5bd145acd5`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca72f02c89a70e463873f7095a54263f02a7dc1fc35b8b3d92d0d6ed1114e1c3`  
		Last Modified: Wed, 14 Oct 2020 21:13:16 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744bfb9438a82d19472dbb92037ab018420b16a677b9451e9b92d13d9d4cc309`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab7908db3cd309e1cf3200fc5b51374d626702ea4ff411559cfa15da77b097d`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691b1b3fc24e5b473537703fcabf8cdc0acd56705ab671452b135de184ffbe0c`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba327018ef360de6c48ecbdb06f66a73defdb3996be6c2f17f0731514dbece5`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c122dffbcf7af8877cc67b8f468cd74a76d63a739b85f3ac429fb27794f724`  
		Last Modified: Wed, 14 Oct 2020 21:13:13 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbf77f12be69367c8fcf09b53209ec5b25083762192120e9ed3f8e429569a4f`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c631d9175a05b1f8c784df5ccc0daeda8990f4cfa0faebc76e525dc737e034`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b5835866e9c4e5a927e7b41da88a4c61a54547cc83fc91db1c1a43494bbac2`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13669d36e52f3d6963333d5102e23ad22fd5892d4fd1a9468f12194c39c2753`  
		Last Modified: Wed, 14 Oct 2020 21:13:11 GMT  
		Size: 299.0 KB (299047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f0e09c2bd5ebc6729c8f1d852f4adefae35e2335cd7dbbcc09c95205e95ab0`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.14393.3986; amd64

```console
$ docker pull caddy@sha256:4c7f9ebc39d2e00064b805df702d5364f55de8cb8cf5ae58d8e4f438988069e8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5773083905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0ce891f0605eaed2c51c683e9fe3d70f29bf6588b85b1f2be21dfcba2c4fb3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 21:06:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Oct 2020 21:06:25 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 14 Oct 2020 21:07:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Oct 2020 21:07:57 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Oct 2020 21:07:58 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Oct 2020 21:07:59 GMT
VOLUME [c:/config]
# Wed, 14 Oct 2020 21:08:00 GMT
VOLUME [c:/data]
# Wed, 14 Oct 2020 21:08:01 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 14 Oct 2020 21:08:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Oct 2020 21:08:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Oct 2020 21:08:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Oct 2020 21:08:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Oct 2020 21:08:05 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Oct 2020 21:08:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Oct 2020 21:08:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Oct 2020 21:08:08 GMT
EXPOSE 80
# Wed, 14 Oct 2020 21:08:08 GMT
EXPOSE 443
# Wed, 14 Oct 2020 21:08:09 GMT
EXPOSE 2019
# Wed, 14 Oct 2020 21:08:53 GMT
RUN caddy version
# Wed, 14 Oct 2020 21:08:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2b4a4f0660702b9f47920e1e7ea79666ac43584dadc8412d8a7b7eb0490a2c`  
		Last Modified: Wed, 14 Oct 2020 21:13:59 GMT  
		Size: 9.9 MB (9925104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3c401ae3441b3e5b7543d5482214980c1c14958e2713fee5966c2622a53963`  
		Last Modified: Wed, 14 Oct 2020 21:13:55 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffab013bf500710ef95125418f98138723e756c560a1de0145379662b77335db`  
		Last Modified: Wed, 14 Oct 2020 21:14:00 GMT  
		Size: 21.5 MB (21518510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcf1f0773bd9f450a654eb5dcecd55e2e3fe3ba01eb0dae7dbf27e84402a6be`  
		Last Modified: Wed, 14 Oct 2020 21:13:53 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7077da12d3b43ef9b9dad1d8c770898c3a0224a8a0a3b99dc4656cc594d09b62`  
		Last Modified: Wed, 14 Oct 2020 21:13:53 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3976aabb2b169dd3bb85d39e2473fe70f7f15de0124b56095dd3c25fbbc27c`  
		Last Modified: Wed, 14 Oct 2020 21:13:52 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e5576c4d0eac332d8332455193ed1057c55aa90bd5e9a6bca884a25623c3c8`  
		Last Modified: Wed, 14 Oct 2020 21:13:52 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7210dc7c5fabd3bf6636614bc150a0965808e559f2b293340b4d8e049a185684`  
		Last Modified: Wed, 14 Oct 2020 21:13:50 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7af1dab2b20db7484c30ac3175b1dc3b89884f843ece3209fdab4882f5e018`  
		Last Modified: Wed, 14 Oct 2020 21:13:49 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe18c02535b810df5a6916e6ffe0a4532c5a70dae17b5ce28956695be585480`  
		Last Modified: Wed, 14 Oct 2020 21:13:50 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb1797af36c3af3ecc1e7db5ddfdba44c6bfff97b0515b3463d0948fed92ac4`  
		Last Modified: Wed, 14 Oct 2020 21:13:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98a2d0f6d0934d8a3b866e68ca5e7775b2af52b170aa71f2113de2d32d532a3`  
		Last Modified: Wed, 14 Oct 2020 21:13:48 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f14b6955af73ac11170ddb2c596a1dd963ceafda86300b2de8466357d56aa4`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ce0d3817eff364f0101431f28cb70cde3766120bbe5fb10b53ebf59363136f`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dd973289c284ff507f57773413c00c41a54ad2015bafb509c68a044b609cda`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6c2b7b482e55dcb167623e29563231f659e1a523cb8f6e83423bb1d69a2014`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7811e07229200779f1a17a1899bf48c49f0250685f18fdffb38ee7c30ab779`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d7cb4258c8b7eab1c92df575a363d8685d8d783672e5256208f715c662b27b`  
		Last Modified: Wed, 14 Oct 2020 21:13:44 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ab63ba04ec1b983074014465794ebf2e437ec4c03997ac40e1be3a4abcce61`  
		Last Modified: Wed, 14 Oct 2020 21:13:44 GMT  
		Size: 268.2 KB (268209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac54f9c3e58e5d406091c73dec798c29e2ee3134663b63d3ddb4959f10f4f32`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:d720e5ab1579e03c0f86de11950434367743bdf8212a4501cd971c29d16942a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull caddy@sha256:5b0edc0113282eff2b0b97cb2768aef9406975982b52b5801fe66a3b7e0f1f6b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2399991421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4a3be7f6340286c7cad100a7baf86ff095c7d81ce5c10b5c314e8d7e73a9ade`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 21:03:47 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Oct 2020 21:03:48 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 14 Oct 2020 21:04:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Oct 2020 21:04:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Oct 2020 21:04:21 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Oct 2020 21:04:22 GMT
VOLUME [c:/config]
# Wed, 14 Oct 2020 21:04:23 GMT
VOLUME [c:/data]
# Wed, 14 Oct 2020 21:04:24 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 14 Oct 2020 21:04:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Oct 2020 21:04:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Oct 2020 21:04:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Oct 2020 21:04:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Oct 2020 21:04:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Oct 2020 21:04:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Oct 2020 21:04:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Oct 2020 21:04:29 GMT
EXPOSE 80
# Wed, 14 Oct 2020 21:04:30 GMT
EXPOSE 443
# Wed, 14 Oct 2020 21:04:30 GMT
EXPOSE 2019
# Wed, 14 Oct 2020 21:04:46 GMT
RUN caddy version
# Wed, 14 Oct 2020 21:04:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590b685e6f8e8fa4cbca8ce94e257baf1c179f183afabfc59bdff4420027e080`  
		Last Modified: Wed, 14 Oct 2020 21:13:24 GMT  
		Size: 9.2 MB (9237870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8a16e6bfc40544aeeaa55e8406570aec66018352db80098da3663138201f74`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468f02630a43054839d6262fe9f0d41cdd551ab83bbbb35c26cd9ead72ce6985`  
		Last Modified: Wed, 14 Oct 2020 21:13:25 GMT  
		Size: 16.3 MB (16343904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcdb09f7b5a57cb7fce28be7e54975dfc770735e4570b259b9104ddc8421bbd`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4b2b1c53bbf344fa90b58a9d5ee4b990881289dde49074cecd1f0da649c20a`  
		Last Modified: Wed, 14 Oct 2020 21:13:20 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01bade2ee2333f9cd004bd1812f0c1fc7f55b2297cf57b8343e17b48c9d3535`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b312fdc7f27df222f05918031d72e4457582b08c8fdeff7cde88a6a402b6f0c`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053d376e7f1eb8e50a394d7247f16006d36ae65144e75d37fe8bb0740d91695f`  
		Last Modified: Wed, 14 Oct 2020 21:13:18 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d88dd9c5821fcba44cce1002ed12b8702e0cbec6ee8d137cbec8e5bd145acd5`  
		Last Modified: Wed, 14 Oct 2020 21:13:17 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca72f02c89a70e463873f7095a54263f02a7dc1fc35b8b3d92d0d6ed1114e1c3`  
		Last Modified: Wed, 14 Oct 2020 21:13:16 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744bfb9438a82d19472dbb92037ab018420b16a677b9451e9b92d13d9d4cc309`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab7908db3cd309e1cf3200fc5b51374d626702ea4ff411559cfa15da77b097d`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691b1b3fc24e5b473537703fcabf8cdc0acd56705ab671452b135de184ffbe0c`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba327018ef360de6c48ecbdb06f66a73defdb3996be6c2f17f0731514dbece5`  
		Last Modified: Wed, 14 Oct 2020 21:13:14 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c122dffbcf7af8877cc67b8f468cd74a76d63a739b85f3ac429fb27794f724`  
		Last Modified: Wed, 14 Oct 2020 21:13:13 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbf77f12be69367c8fcf09b53209ec5b25083762192120e9ed3f8e429569a4f`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c631d9175a05b1f8c784df5ccc0daeda8990f4cfa0faebc76e525dc737e034`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b5835866e9c4e5a927e7b41da88a4c61a54547cc83fc91db1c1a43494bbac2`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13669d36e52f3d6963333d5102e23ad22fd5892d4fd1a9468f12194c39c2753`  
		Last Modified: Wed, 14 Oct 2020 21:13:11 GMT  
		Size: 299.0 KB (299047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f0e09c2bd5ebc6729c8f1d852f4adefae35e2335cd7dbbcc09c95205e95ab0`  
		Last Modified: Wed, 14 Oct 2020 21:13:10 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:155acd240efff18a38a7aff934be0f6976aeb1c76139025671c9833ed160c840
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64

### `caddy:windowsservercore-ltsc2016` - windows version 10.0.14393.3986; amd64

```console
$ docker pull caddy@sha256:4c7f9ebc39d2e00064b805df702d5364f55de8cb8cf5ae58d8e4f438988069e8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5773083905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0ce891f0605eaed2c51c683e9fe3d70f29bf6588b85b1f2be21dfcba2c4fb3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 21:06:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Oct 2020 21:06:25 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 14 Oct 2020 21:07:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Oct 2020 21:07:57 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Oct 2020 21:07:58 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Oct 2020 21:07:59 GMT
VOLUME [c:/config]
# Wed, 14 Oct 2020 21:08:00 GMT
VOLUME [c:/data]
# Wed, 14 Oct 2020 21:08:01 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 14 Oct 2020 21:08:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Oct 2020 21:08:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Oct 2020 21:08:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Oct 2020 21:08:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Oct 2020 21:08:05 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Oct 2020 21:08:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Oct 2020 21:08:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Oct 2020 21:08:08 GMT
EXPOSE 80
# Wed, 14 Oct 2020 21:08:08 GMT
EXPOSE 443
# Wed, 14 Oct 2020 21:08:09 GMT
EXPOSE 2019
# Wed, 14 Oct 2020 21:08:53 GMT
RUN caddy version
# Wed, 14 Oct 2020 21:08:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2b4a4f0660702b9f47920e1e7ea79666ac43584dadc8412d8a7b7eb0490a2c`  
		Last Modified: Wed, 14 Oct 2020 21:13:59 GMT  
		Size: 9.9 MB (9925104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3c401ae3441b3e5b7543d5482214980c1c14958e2713fee5966c2622a53963`  
		Last Modified: Wed, 14 Oct 2020 21:13:55 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffab013bf500710ef95125418f98138723e756c560a1de0145379662b77335db`  
		Last Modified: Wed, 14 Oct 2020 21:14:00 GMT  
		Size: 21.5 MB (21518510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcf1f0773bd9f450a654eb5dcecd55e2e3fe3ba01eb0dae7dbf27e84402a6be`  
		Last Modified: Wed, 14 Oct 2020 21:13:53 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7077da12d3b43ef9b9dad1d8c770898c3a0224a8a0a3b99dc4656cc594d09b62`  
		Last Modified: Wed, 14 Oct 2020 21:13:53 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3976aabb2b169dd3bb85d39e2473fe70f7f15de0124b56095dd3c25fbbc27c`  
		Last Modified: Wed, 14 Oct 2020 21:13:52 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e5576c4d0eac332d8332455193ed1057c55aa90bd5e9a6bca884a25623c3c8`  
		Last Modified: Wed, 14 Oct 2020 21:13:52 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7210dc7c5fabd3bf6636614bc150a0965808e559f2b293340b4d8e049a185684`  
		Last Modified: Wed, 14 Oct 2020 21:13:50 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7af1dab2b20db7484c30ac3175b1dc3b89884f843ece3209fdab4882f5e018`  
		Last Modified: Wed, 14 Oct 2020 21:13:49 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe18c02535b810df5a6916e6ffe0a4532c5a70dae17b5ce28956695be585480`  
		Last Modified: Wed, 14 Oct 2020 21:13:50 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb1797af36c3af3ecc1e7db5ddfdba44c6bfff97b0515b3463d0948fed92ac4`  
		Last Modified: Wed, 14 Oct 2020 21:13:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98a2d0f6d0934d8a3b866e68ca5e7775b2af52b170aa71f2113de2d32d532a3`  
		Last Modified: Wed, 14 Oct 2020 21:13:48 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f14b6955af73ac11170ddb2c596a1dd963ceafda86300b2de8466357d56aa4`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ce0d3817eff364f0101431f28cb70cde3766120bbe5fb10b53ebf59363136f`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dd973289c284ff507f57773413c00c41a54ad2015bafb509c68a044b609cda`  
		Last Modified: Wed, 14 Oct 2020 21:13:47 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6c2b7b482e55dcb167623e29563231f659e1a523cb8f6e83423bb1d69a2014`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7811e07229200779f1a17a1899bf48c49f0250685f18fdffb38ee7c30ab779`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d7cb4258c8b7eab1c92df575a363d8685d8d783672e5256208f715c662b27b`  
		Last Modified: Wed, 14 Oct 2020 21:13:44 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ab63ba04ec1b983074014465794ebf2e437ec4c03997ac40e1be3a4abcce61`  
		Last Modified: Wed, 14 Oct 2020 21:13:44 GMT  
		Size: 268.2 KB (268209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac54f9c3e58e5d406091c73dec798c29e2ee3134663b63d3ddb4959f10f4f32`  
		Last Modified: Wed, 14 Oct 2020 21:13:43 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
