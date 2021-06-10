<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `caddy`

-	[`caddy:2`](#caddy2)
-	[`caddy:2-alpine`](#caddy2-alpine)
-	[`caddy:2-builder`](#caddy2-builder)
-	[`caddy:2-builder-alpine`](#caddy2-builder-alpine)
-	[`caddy:2-builder-windowsservercore-1809`](#caddy2-builder-windowsservercore-1809)
-	[`caddy:2-builder-windowsservercore-ltsc2016`](#caddy2-builder-windowsservercore-ltsc2016)
-	[`caddy:2-windowsservercore`](#caddy2-windowsservercore)
-	[`caddy:2-windowsservercore-1809`](#caddy2-windowsservercore-1809)
-	[`caddy:2-windowsservercore-ltsc2016`](#caddy2-windowsservercore-ltsc2016)
-	[`caddy:2.3.0`](#caddy230)
-	[`caddy:2.3.0-alpine`](#caddy230-alpine)
-	[`caddy:2.3.0-builder`](#caddy230-builder)
-	[`caddy:2.3.0-builder-alpine`](#caddy230-builder-alpine)
-	[`caddy:2.3.0-builder-windowsservercore-1809`](#caddy230-builder-windowsservercore-1809)
-	[`caddy:2.3.0-builder-windowsservercore-ltsc2016`](#caddy230-builder-windowsservercore-ltsc2016)
-	[`caddy:2.3.0-windowsservercore`](#caddy230-windowsservercore)
-	[`caddy:2.3.0-windowsservercore-1809`](#caddy230-windowsservercore-1809)
-	[`caddy:2.3.0-windowsservercore-ltsc2016`](#caddy230-windowsservercore-ltsc2016)
-	[`caddy:2.4.1`](#caddy241)
-	[`caddy:2.4.1-alpine`](#caddy241-alpine)
-	[`caddy:2.4.1-builder`](#caddy241-builder)
-	[`caddy:2.4.1-builder-alpine`](#caddy241-builder-alpine)
-	[`caddy:2.4.1-builder-windowsservercore-1809`](#caddy241-builder-windowsservercore-1809)
-	[`caddy:2.4.1-builder-windowsservercore-ltsc2016`](#caddy241-builder-windowsservercore-ltsc2016)
-	[`caddy:2.4.1-windowsservercore`](#caddy241-windowsservercore)
-	[`caddy:2.4.1-windowsservercore-1809`](#caddy241-windowsservercore-1809)
-	[`caddy:2.4.1-windowsservercore-ltsc2016`](#caddy241-windowsservercore-ltsc2016)
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
$ docker pull caddy@sha256:8031d689a8e6f47dcc146121b75946348e8b2e94a183e92cac38a489f55759a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `caddy:2` - linux; amd64

```console
$ docker pull caddy@sha256:c3b2e52162bebaf3b0d128780b3bffc4aa9ccb6953953892dd9d31495e15dc55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14568035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b59636b1388443a36d8173a6ad50dbcf59de4b7786b8178ad9eb656ad6e9a387`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:11:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:04:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 24 May 2021 18:23:10 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:23:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 24 May 2021 18:23:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 24 May 2021 18:23:13 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 24 May 2021 18:23:14 GMT
ENV XDG_DATA_HOME=/data
# Mon, 24 May 2021 18:23:14 GMT
VOLUME [/config]
# Mon, 24 May 2021 18:23:14 GMT
VOLUME [/data]
# Mon, 24 May 2021 18:23:14 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:23:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:23:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:23:16 GMT
EXPOSE 80
# Mon, 24 May 2021 18:23:16 GMT
EXPOSE 443
# Mon, 24 May 2021 18:23:16 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:23:16 GMT
WORKDIR /srv
# Mon, 24 May 2021 18:23:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8294633c5b5606f8e98aaf81da701b7a7e2018dbf82355d1d73830c677034f19`  
		Last Modified: Wed, 14 Apr 2021 20:12:08 GMT  
		Size: 300.4 KB (300403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16798e0582fce7af9c2ba2c8ee4990d0fd1e58384e170ee9937486253d67bbf1`  
		Last Modified: Tue, 11 May 2021 01:05:00 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba0aa26d56032b74c8c88c24edc5a2f7987ea418aaa0966f93ab53c62802c2f`  
		Last Modified: Mon, 24 May 2021 18:23:47 GMT  
		Size: 11.4 MB (11449656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712687f6a8ba00b8b6cb95bad7426eb9964fff3de9f5a7f66dedf6310e8a8c01`  
		Last Modified: Mon, 24 May 2021 18:23:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:eea14e6e8e0ef54944ef2f6e1b6540a536661e033a1f216e92535b5741c2278e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13786866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e11afe23a7696f3f16192af7de16ece9c2dfb73868f2859b9dbacfe0e604fa4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 17:34:28 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 May 2021 17:34:30 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Wed, 26 May 2021 17:34:30 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 26 May 2021 17:34:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 May 2021 17:34:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 May 2021 17:34:33 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 May 2021 17:34:34 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 May 2021 17:34:34 GMT
VOLUME [/config]
# Wed, 26 May 2021 17:34:34 GMT
VOLUME [/data]
# Wed, 26 May 2021 17:34:34 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 26 May 2021 17:34:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 May 2021 17:34:34 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 May 2021 17:34:36 GMT
EXPOSE 80
# Wed, 26 May 2021 17:34:36 GMT
EXPOSE 443
# Wed, 26 May 2021 17:34:36 GMT
EXPOSE 2019
# Wed, 26 May 2021 17:34:36 GMT
WORKDIR /srv
# Wed, 26 May 2021 17:34:36 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c2672622a603ff8b0ed8517cfd5adb30b2b35ae40b42cd4ad0545dcb6d3b10`  
		Last Modified: Wed, 26 May 2021 17:36:11 GMT  
		Size: 300.5 KB (300528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b30604f35cc25a62ae1d71a50c6919ad28a2aa67bfd14bebc1984cec5b2c8b`  
		Last Modified: Wed, 26 May 2021 17:36:12 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7119340f7ca66a456adcbc374cbeb7e1c37c35867123bd3fac943aea26a813a8`  
		Last Modified: Wed, 26 May 2021 17:36:15 GMT  
		Size: 10.9 MB (10858201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392497979deecdb2075178245bdf58e8d1ce55c609d2b1320a869392bc007b3f`  
		Last Modified: Wed, 26 May 2021 17:36:12 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:ea6c90777b37ade094ce3f1f5d0efffe39519d18ec589fa4cfa2b6f0c5028e3a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13561305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8637a19be10382ee673bc51be71c9fa3ce23cfdcd0eb9d9bf8734147818227d4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 10:59:27 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 May 2021 10:59:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Wed, 26 May 2021 10:59:29 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 26 May 2021 10:59:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 May 2021 10:59:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 May 2021 10:59:32 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 May 2021 10:59:32 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 May 2021 10:59:32 GMT
VOLUME [/config]
# Wed, 26 May 2021 10:59:33 GMT
VOLUME [/data]
# Wed, 26 May 2021 10:59:33 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 26 May 2021 10:59:33 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 May 2021 10:59:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 May 2021 10:59:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 May 2021 10:59:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 May 2021 10:59:34 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 May 2021 10:59:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 May 2021 10:59:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 May 2021 10:59:34 GMT
EXPOSE 80
# Wed, 26 May 2021 10:59:35 GMT
EXPOSE 443
# Wed, 26 May 2021 10:59:35 GMT
EXPOSE 2019
# Wed, 26 May 2021 10:59:35 GMT
WORKDIR /srv
# Wed, 26 May 2021 10:59:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca051a8c4175c3d7d75c47c9a60045d2f5b7eb415ce35b56c99e9cab58ae3ba`  
		Last Modified: Wed, 26 May 2021 11:01:09 GMT  
		Size: 299.7 KB (299668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2db810fb832f7bd380a39ff7508fa03cc1854bdd51da4cfa239e07fe96fe4e`  
		Last Modified: Wed, 26 May 2021 11:01:09 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce092d490b7e90c7b37879314c23cb48b38be5392715e2d976bc99bbef8a230`  
		Last Modified: Wed, 26 May 2021 11:01:11 GMT  
		Size: 10.8 MB (10831485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb6eb70297874eea11cf38b8870aa1f896bfd6ec638fd6dc9177d7be039001b`  
		Last Modified: Wed, 26 May 2021 11:01:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:ad6d7adcc7d981edfcc5eb4bb42e1fc561b9d0301cadf2ccd920a4a98ae90387
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13415153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:383d427b090897c507d37417dfd21667985cf15a9e3e800b87c821eabe372bb6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 17:52:42 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 May 2021 17:52:43 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Wed, 26 May 2021 17:52:44 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 26 May 2021 17:52:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 May 2021 17:52:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 May 2021 17:52:47 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 May 2021 17:52:47 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 May 2021 17:52:47 GMT
VOLUME [/config]
# Wed, 26 May 2021 17:52:47 GMT
VOLUME [/data]
# Wed, 26 May 2021 17:52:47 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 May 2021 17:52:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 May 2021 17:52:49 GMT
EXPOSE 80
# Wed, 26 May 2021 17:52:49 GMT
EXPOSE 443
# Wed, 26 May 2021 17:52:49 GMT
EXPOSE 2019
# Wed, 26 May 2021 17:52:49 GMT
WORKDIR /srv
# Wed, 26 May 2021 17:52:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a305c6848b1bdb9c473c4a3128eff85e1604c1b2d0e78cef80874650b91a49`  
		Last Modified: Wed, 26 May 2021 17:53:57 GMT  
		Size: 300.6 KB (300633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2faea6afac2cf802bf88fd56ee1493ce97eca3a29920702a726ea8e5cd0ea3d`  
		Last Modified: Wed, 26 May 2021 17:53:57 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c196442e5472f13a88f63e7da52cbd15acf171b3d76e87cc47c3073ed0e95d`  
		Last Modified: Wed, 26 May 2021 17:53:59 GMT  
		Size: 10.4 MB (10396489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583f00c174c73f777e3d0cd263a593786c4c341cb20632fafb4246ac0f06f45b`  
		Last Modified: Wed, 26 May 2021 17:53:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:b767e2ec43a11bb1a211e3d7bc76c81d4a256f90084d5747367af6a9730e4f94
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13121818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f930dc44ddd7a57e1d48aaeed66a69653dc4d5c15bdae6c378273cb55287f07b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:12:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:17:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 24 May 2021 18:19:32 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:20:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 24 May 2021 18:20:18 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 24 May 2021 18:20:25 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 24 May 2021 18:20:32 GMT
ENV XDG_DATA_HOME=/data
# Mon, 24 May 2021 18:20:39 GMT
VOLUME [/config]
# Mon, 24 May 2021 18:20:45 GMT
VOLUME [/data]
# Mon, 24 May 2021 18:20:51 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:20:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:21:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:21:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:21:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:21:34 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:21:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:21:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:22:03 GMT
EXPOSE 80
# Mon, 24 May 2021 18:22:10 GMT
EXPOSE 443
# Mon, 24 May 2021 18:22:16 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:22:21 GMT
WORKDIR /srv
# Mon, 24 May 2021 18:22:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25908330df11bb7bc2ed71aa9b4de279db5492df2b03ced3f6650b25821c4584`  
		Last Modified: Wed, 14 Apr 2021 22:16:00 GMT  
		Size: 302.6 KB (302554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a224581e3ba4733f37686f5a5d5375019f9126a0ded6ed20f13e09e898dc735e`  
		Last Modified: Tue, 11 May 2021 01:20:08 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c6214f82b33045060ad6f882d1ed7a5779be7a0883c4da8306ab03e9e2623c`  
		Last Modified: Mon, 24 May 2021 18:23:37 GMT  
		Size: 10.0 MB (10000116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52a67b9935763896cc7c3386cd93b5f7fbc80093549e39f460dc7e170f679f4`  
		Last Modified: Mon, 24 May 2021 18:23:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:40e8d6bc1ad5c4c4f902426841f39a594dd3842c212bed7ecbb66f312b5a4f6e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13938687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c9fccd235488bb04e0075ea4a47a8c102dce45c98cbba05e4d7d0d0ebb13b1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:07:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 10 May 2021 23:41:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 24 May 2021 17:41:40 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 17:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 24 May 2021 17:41:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 24 May 2021 17:41:48 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 24 May 2021 17:41:48 GMT
ENV XDG_DATA_HOME=/data
# Mon, 24 May 2021 17:41:49 GMT
VOLUME [/config]
# Mon, 24 May 2021 17:41:50 GMT
VOLUME [/data]
# Mon, 24 May 2021 17:41:50 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 17:41:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 17:41:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 17:41:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 17:41:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 17:41:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 17:41:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 17:41:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 17:41:55 GMT
EXPOSE 80
# Mon, 24 May 2021 17:41:56 GMT
EXPOSE 443
# Mon, 24 May 2021 17:41:57 GMT
EXPOSE 2019
# Mon, 24 May 2021 17:41:57 GMT
WORKDIR /srv
# Mon, 24 May 2021 17:41:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db3c8b812fcb0d1bfd42c16c2e9ac68f4f3006382c5362e969d1c9eb3a9fab5`  
		Last Modified: Wed, 14 Apr 2021 20:08:26 GMT  
		Size: 300.8 KB (300847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba030675d7bb5bc251d93896d2c81ed8a2f4f4ef2e8e84ad7dfdce9886387c`  
		Last Modified: Mon, 10 May 2021 23:42:29 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03e81629e078650b941a4beb267a6755133e90fa22a688bffb5df188e069c55`  
		Last Modified: Mon, 24 May 2021 17:42:37 GMT  
		Size: 11.0 MB (11029189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbee1e7ec347a65e5e78b46b8fe541241e3f6c13a468785945abd0aaba24545`  
		Last Modified: Mon, 24 May 2021 17:42:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:d4a3e0eabf14e4f98a9bcf5eada28d1443573b082afe95028d548d5b88a2b33e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2654170862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:736d3aa581b715efdf7c0431ebfbaed21b664091d8e8f7e4595c5f9dabbd2acb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 12:10:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:08:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Jun 2021 20:08:07 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:08:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Jun 2021 20:08:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Jun 2021 20:08:49 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Jun 2021 20:08:51 GMT
VOLUME [c:/config]
# Wed, 09 Jun 2021 20:08:53 GMT
VOLUME [c:/data]
# Wed, 09 Jun 2021 20:08:55 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 09 Jun 2021 20:08:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Jun 2021 20:09:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Jun 2021 20:09:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Jun 2021 20:09:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Jun 2021 20:09:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Jun 2021 20:09:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Jun 2021 20:09:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Jun 2021 20:09:14 GMT
EXPOSE 80
# Wed, 09 Jun 2021 20:09:17 GMT
EXPOSE 443
# Wed, 09 Jun 2021 20:09:19 GMT
EXPOSE 2019
# Wed, 09 Jun 2021 20:09:41 GMT
RUN caddy version
# Wed, 09 Jun 2021 20:09:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7863ef96846d497ea06fe442ea13dcecaf5c248ce238c69800475281a4fa848e`  
		Last Modified: Wed, 09 Jun 2021 12:20:41 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dc18d712eacfb666370e311daaf51e09fc2f76ca762e4592e149fbe6aba561`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 361.4 KB (361380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b774f6019fa0c611532d02bdf31c54e9da56fe2330e3e0745538ef036cfb87`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e977598d13d0ee9ae780f2cf34706c57e810301d20d9fc8286ad9390b9166b`  
		Last Modified: Wed, 09 Jun 2021 20:19:37 GMT  
		Size: 11.9 MB (11906202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7361692fe34486902f2dd9f69cc3bce54c4cb8c5c86ed80a0d75033f25ae5213`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35d39d3918ab9262122b494a653aec25e76a65396f9198d7be955cb9c26c6f3`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66891a50a919af8d3cb83358a7f8d33b2055c143bd3499cc431fd32d053ed393`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519d446a1689a5424a77bf1cbf0f00153b28c6eff9ee22f0f88e0e32b3f6bda3`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534ea2eef93aa67b4ac4bfb48ac5498fa33b02d0b88b9ae60b8ae159addacecc`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19fc40bc9ade11a1755b185c529e961b474d959d45a44b1b1ab5f12e3d17863a`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ef9960b6bac284e65c351bc447bb8931486a0c1c3ee68c9e5a62828b4ae0e`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cfda8707421463aa0f297ce5d4ac3a615f60caf56e6e69a299caa08a04f7da`  
		Last Modified: Wed, 09 Jun 2021 20:19:29 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa0c9ece6e3482cf3ffc8d9a087d113db0f7c249f59bcf06f3ffc65c5e4bce0`  
		Last Modified: Wed, 09 Jun 2021 20:19:29 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6614223fb410a8262956f73a038f6d79b67d5976fe8740b21dfa2121a9cbd7f2`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f354857e070035731eb660ec35ff9f8549b6cc79211bab40ae642d9875f98f8b`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc94f29a4cb79013fce0bf1a5776868fa31912b598231e46883a114d86f712d3`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e536fde913e2e2d5ae24846adca32195330a9be6e7d1c3180ce7ac6bc6a35ae1`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b11db027637bf7abeec6bbcd83920c4eb7c291aeeae4d2886a1563bf41289a6`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3a70d973d27d739faae877290b3184bee11c706ebd4bfa515d180fba88ef0f`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc7b3e3d99424f8d3737a4502a6f50767ae25b699a315155b98700af682b64f`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 292.6 KB (292631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d435932a64bec158a6193fa4a31a1b38e446ec9f63c0b6be3282c3acf3288949`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:e7e7af29e7917229552a0c802147dba99fb7a1427b84296a2c60ea7e19cbcb0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278267906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7184db699efd0a2ce0077179784cc7277e5faa7d07534ea1ce32d61d7f46ebc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 12:41:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:11:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Jun 2021 20:11:30 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:13:06 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Jun 2021 20:13:09 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Jun 2021 20:13:11 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Jun 2021 20:13:15 GMT
VOLUME [c:/config]
# Wed, 09 Jun 2021 20:13:18 GMT
VOLUME [c:/data]
# Wed, 09 Jun 2021 20:13:20 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 09 Jun 2021 20:13:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Jun 2021 20:13:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Jun 2021 20:13:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Jun 2021 20:13:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Jun 2021 20:13:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Jun 2021 20:13:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Jun 2021 20:13:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Jun 2021 20:13:40 GMT
EXPOSE 80
# Wed, 09 Jun 2021 20:13:42 GMT
EXPOSE 443
# Wed, 09 Jun 2021 20:13:45 GMT
EXPOSE 2019
# Wed, 09 Jun 2021 20:14:40 GMT
RUN caddy version
# Wed, 09 Jun 2021 20:14:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c82e82e95dbad4ccc260b42e03767eb07222e2f00ec57a69b3c87b17da1d2fd3`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a28e390d3b8e7b9369b102914eaee6e1fa0d14eb258b628be67f99f32f06f81`  
		Last Modified: Wed, 09 Jun 2021 20:20:01 GMT  
		Size: 357.4 KB (357370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7f07987f083e935103f83e47894b93aceaf05d1ded81dd09eb0bc3c8e45af`  
		Last Modified: Wed, 09 Jun 2021 20:20:01 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e65ddfdcdd60907208873b2a532cc58bc0f57d144430cef2c7630e80e4fd1e`  
		Last Modified: Wed, 09 Jun 2021 20:20:05 GMT  
		Size: 11.9 MB (11896985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58e4679b7ef7e1b9d82f44a6b5055c6916801193550bcce3ce390851224c736`  
		Last Modified: Wed, 09 Jun 2021 20:20:00 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107d803623512ea83de929509cc68f334261f2018c60bde60a99eadd0c2b179`  
		Last Modified: Wed, 09 Jun 2021 20:20:00 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f757538ddb020d145715a4890594958e741fe98366f1a58314361e5a8a3487`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462510ee9cb1c642e2804f8f607f02ccc5c31b63c956b9394bf38c5041b10d8b`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e87709f8365472aa7278651dacfc7eee93b24859a494cf6904b4f7ce80df0a`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5439b862b8218f1d7e0e0269efdbed614475ffbdcbaac06a3953f80b07677a1a`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1950c17917c025587fa23872145ee00eaaa11939dc87314c1aa74119db642d`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84164685053ad8b12a46e198ec2e93143d1df956bbbd4af76c88d0f549031c60`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103b7e93d2e2faefef7bd14bc00910442ce8da843f4fb726e2dba2d97752ddc9`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046d1e0cd75d46944ff833afe00c5dc9835ec1eb72876965a98a1488778910a6`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593a0ce075f6e5e07785dd7cd14aa1c274339da4d6f80495f0d1a85fabdef5db`  
		Last Modified: Wed, 09 Jun 2021 20:19:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14f5cdc43c91f65e6c5879691adc6e392d353807b27465a9b270fe7a06da51c`  
		Last Modified: Wed, 09 Jun 2021 20:19:55 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd488f5f58644d68e5103098932448a58d05a716861b26bf33376e75ad27e61`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c218cc3caa4b354c536ad99d30753a6eb41c52a58c52aafc0655a8482382a07`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3dad29a1e0241680f68697c2b0dbca8e85d0084faef4bdd3e66c8294be80671`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daeda652af05f03b2ec029aa5caa6b49d533546fa8347f5b1db003e8a83a7c30`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 260.8 KB (260840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9779c5588bf525e972d3b02ecaeeee32f3939ef8d54e8a16c52e0e62804e2e42`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:48e775e759b55c34afd4293c6ec80650a45754a193c8eaa62c6fcddb6f599d45
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
$ docker pull caddy@sha256:c3b2e52162bebaf3b0d128780b3bffc4aa9ccb6953953892dd9d31495e15dc55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14568035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b59636b1388443a36d8173a6ad50dbcf59de4b7786b8178ad9eb656ad6e9a387`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:11:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:04:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 24 May 2021 18:23:10 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:23:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 24 May 2021 18:23:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 24 May 2021 18:23:13 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 24 May 2021 18:23:14 GMT
ENV XDG_DATA_HOME=/data
# Mon, 24 May 2021 18:23:14 GMT
VOLUME [/config]
# Mon, 24 May 2021 18:23:14 GMT
VOLUME [/data]
# Mon, 24 May 2021 18:23:14 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:23:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:23:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:23:16 GMT
EXPOSE 80
# Mon, 24 May 2021 18:23:16 GMT
EXPOSE 443
# Mon, 24 May 2021 18:23:16 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:23:16 GMT
WORKDIR /srv
# Mon, 24 May 2021 18:23:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8294633c5b5606f8e98aaf81da701b7a7e2018dbf82355d1d73830c677034f19`  
		Last Modified: Wed, 14 Apr 2021 20:12:08 GMT  
		Size: 300.4 KB (300403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16798e0582fce7af9c2ba2c8ee4990d0fd1e58384e170ee9937486253d67bbf1`  
		Last Modified: Tue, 11 May 2021 01:05:00 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba0aa26d56032b74c8c88c24edc5a2f7987ea418aaa0966f93ab53c62802c2f`  
		Last Modified: Mon, 24 May 2021 18:23:47 GMT  
		Size: 11.4 MB (11449656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712687f6a8ba00b8b6cb95bad7426eb9964fff3de9f5a7f66dedf6310e8a8c01`  
		Last Modified: Mon, 24 May 2021 18:23:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:eea14e6e8e0ef54944ef2f6e1b6540a536661e033a1f216e92535b5741c2278e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13786866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e11afe23a7696f3f16192af7de16ece9c2dfb73868f2859b9dbacfe0e604fa4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 17:34:28 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 May 2021 17:34:30 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Wed, 26 May 2021 17:34:30 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 26 May 2021 17:34:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 May 2021 17:34:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 May 2021 17:34:33 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 May 2021 17:34:34 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 May 2021 17:34:34 GMT
VOLUME [/config]
# Wed, 26 May 2021 17:34:34 GMT
VOLUME [/data]
# Wed, 26 May 2021 17:34:34 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 26 May 2021 17:34:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 May 2021 17:34:34 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 May 2021 17:34:36 GMT
EXPOSE 80
# Wed, 26 May 2021 17:34:36 GMT
EXPOSE 443
# Wed, 26 May 2021 17:34:36 GMT
EXPOSE 2019
# Wed, 26 May 2021 17:34:36 GMT
WORKDIR /srv
# Wed, 26 May 2021 17:34:36 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c2672622a603ff8b0ed8517cfd5adb30b2b35ae40b42cd4ad0545dcb6d3b10`  
		Last Modified: Wed, 26 May 2021 17:36:11 GMT  
		Size: 300.5 KB (300528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b30604f35cc25a62ae1d71a50c6919ad28a2aa67bfd14bebc1984cec5b2c8b`  
		Last Modified: Wed, 26 May 2021 17:36:12 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7119340f7ca66a456adcbc374cbeb7e1c37c35867123bd3fac943aea26a813a8`  
		Last Modified: Wed, 26 May 2021 17:36:15 GMT  
		Size: 10.9 MB (10858201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392497979deecdb2075178245bdf58e8d1ce55c609d2b1320a869392bc007b3f`  
		Last Modified: Wed, 26 May 2021 17:36:12 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:ea6c90777b37ade094ce3f1f5d0efffe39519d18ec589fa4cfa2b6f0c5028e3a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13561305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8637a19be10382ee673bc51be71c9fa3ce23cfdcd0eb9d9bf8734147818227d4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 10:59:27 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 May 2021 10:59:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Wed, 26 May 2021 10:59:29 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 26 May 2021 10:59:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 May 2021 10:59:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 May 2021 10:59:32 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 May 2021 10:59:32 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 May 2021 10:59:32 GMT
VOLUME [/config]
# Wed, 26 May 2021 10:59:33 GMT
VOLUME [/data]
# Wed, 26 May 2021 10:59:33 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 26 May 2021 10:59:33 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 May 2021 10:59:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 May 2021 10:59:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 May 2021 10:59:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 May 2021 10:59:34 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 May 2021 10:59:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 May 2021 10:59:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 May 2021 10:59:34 GMT
EXPOSE 80
# Wed, 26 May 2021 10:59:35 GMT
EXPOSE 443
# Wed, 26 May 2021 10:59:35 GMT
EXPOSE 2019
# Wed, 26 May 2021 10:59:35 GMT
WORKDIR /srv
# Wed, 26 May 2021 10:59:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca051a8c4175c3d7d75c47c9a60045d2f5b7eb415ce35b56c99e9cab58ae3ba`  
		Last Modified: Wed, 26 May 2021 11:01:09 GMT  
		Size: 299.7 KB (299668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2db810fb832f7bd380a39ff7508fa03cc1854bdd51da4cfa239e07fe96fe4e`  
		Last Modified: Wed, 26 May 2021 11:01:09 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce092d490b7e90c7b37879314c23cb48b38be5392715e2d976bc99bbef8a230`  
		Last Modified: Wed, 26 May 2021 11:01:11 GMT  
		Size: 10.8 MB (10831485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb6eb70297874eea11cf38b8870aa1f896bfd6ec638fd6dc9177d7be039001b`  
		Last Modified: Wed, 26 May 2021 11:01:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:ad6d7adcc7d981edfcc5eb4bb42e1fc561b9d0301cadf2ccd920a4a98ae90387
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13415153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:383d427b090897c507d37417dfd21667985cf15a9e3e800b87c821eabe372bb6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 17:52:42 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 May 2021 17:52:43 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Wed, 26 May 2021 17:52:44 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 26 May 2021 17:52:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 May 2021 17:52:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 May 2021 17:52:47 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 May 2021 17:52:47 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 May 2021 17:52:47 GMT
VOLUME [/config]
# Wed, 26 May 2021 17:52:47 GMT
VOLUME [/data]
# Wed, 26 May 2021 17:52:47 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 May 2021 17:52:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 May 2021 17:52:49 GMT
EXPOSE 80
# Wed, 26 May 2021 17:52:49 GMT
EXPOSE 443
# Wed, 26 May 2021 17:52:49 GMT
EXPOSE 2019
# Wed, 26 May 2021 17:52:49 GMT
WORKDIR /srv
# Wed, 26 May 2021 17:52:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a305c6848b1bdb9c473c4a3128eff85e1604c1b2d0e78cef80874650b91a49`  
		Last Modified: Wed, 26 May 2021 17:53:57 GMT  
		Size: 300.6 KB (300633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2faea6afac2cf802bf88fd56ee1493ce97eca3a29920702a726ea8e5cd0ea3d`  
		Last Modified: Wed, 26 May 2021 17:53:57 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c196442e5472f13a88f63e7da52cbd15acf171b3d76e87cc47c3073ed0e95d`  
		Last Modified: Wed, 26 May 2021 17:53:59 GMT  
		Size: 10.4 MB (10396489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583f00c174c73f777e3d0cd263a593786c4c341cb20632fafb4246ac0f06f45b`  
		Last Modified: Wed, 26 May 2021 17:53:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:b767e2ec43a11bb1a211e3d7bc76c81d4a256f90084d5747367af6a9730e4f94
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13121818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f930dc44ddd7a57e1d48aaeed66a69653dc4d5c15bdae6c378273cb55287f07b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:12:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:17:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 24 May 2021 18:19:32 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:20:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 24 May 2021 18:20:18 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 24 May 2021 18:20:25 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 24 May 2021 18:20:32 GMT
ENV XDG_DATA_HOME=/data
# Mon, 24 May 2021 18:20:39 GMT
VOLUME [/config]
# Mon, 24 May 2021 18:20:45 GMT
VOLUME [/data]
# Mon, 24 May 2021 18:20:51 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:20:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:21:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:21:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:21:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:21:34 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:21:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:21:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:22:03 GMT
EXPOSE 80
# Mon, 24 May 2021 18:22:10 GMT
EXPOSE 443
# Mon, 24 May 2021 18:22:16 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:22:21 GMT
WORKDIR /srv
# Mon, 24 May 2021 18:22:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25908330df11bb7bc2ed71aa9b4de279db5492df2b03ced3f6650b25821c4584`  
		Last Modified: Wed, 14 Apr 2021 22:16:00 GMT  
		Size: 302.6 KB (302554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a224581e3ba4733f37686f5a5d5375019f9126a0ded6ed20f13e09e898dc735e`  
		Last Modified: Tue, 11 May 2021 01:20:08 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c6214f82b33045060ad6f882d1ed7a5779be7a0883c4da8306ab03e9e2623c`  
		Last Modified: Mon, 24 May 2021 18:23:37 GMT  
		Size: 10.0 MB (10000116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52a67b9935763896cc7c3386cd93b5f7fbc80093549e39f460dc7e170f679f4`  
		Last Modified: Mon, 24 May 2021 18:23:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:40e8d6bc1ad5c4c4f902426841f39a594dd3842c212bed7ecbb66f312b5a4f6e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13938687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c9fccd235488bb04e0075ea4a47a8c102dce45c98cbba05e4d7d0d0ebb13b1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:07:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 10 May 2021 23:41:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 24 May 2021 17:41:40 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 17:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 24 May 2021 17:41:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 24 May 2021 17:41:48 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 24 May 2021 17:41:48 GMT
ENV XDG_DATA_HOME=/data
# Mon, 24 May 2021 17:41:49 GMT
VOLUME [/config]
# Mon, 24 May 2021 17:41:50 GMT
VOLUME [/data]
# Mon, 24 May 2021 17:41:50 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 17:41:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 17:41:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 17:41:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 17:41:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 17:41:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 17:41:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 17:41:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 17:41:55 GMT
EXPOSE 80
# Mon, 24 May 2021 17:41:56 GMT
EXPOSE 443
# Mon, 24 May 2021 17:41:57 GMT
EXPOSE 2019
# Mon, 24 May 2021 17:41:57 GMT
WORKDIR /srv
# Mon, 24 May 2021 17:41:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db3c8b812fcb0d1bfd42c16c2e9ac68f4f3006382c5362e969d1c9eb3a9fab5`  
		Last Modified: Wed, 14 Apr 2021 20:08:26 GMT  
		Size: 300.8 KB (300847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba030675d7bb5bc251d93896d2c81ed8a2f4f4ef2e8e84ad7dfdce9886387c`  
		Last Modified: Mon, 10 May 2021 23:42:29 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03e81629e078650b941a4beb267a6755133e90fa22a688bffb5df188e069c55`  
		Last Modified: Mon, 24 May 2021 17:42:37 GMT  
		Size: 11.0 MB (11029189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbee1e7ec347a65e5e78b46b8fe541241e3f6c13a468785945abd0aaba24545`  
		Last Modified: Mon, 24 May 2021 17:42:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:7e7f52b8b3e06a36bc4b32d552b0b2b30dc863461d3250a691fae68fc89c841b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:acb1d8e470fc9d3be900f5a534a57d59d7e827ad2a4fabbedbacde1d08e850ee
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116540780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eafee2350c73e5c74f40dc4ff4146d3ac64f52d221205b317621567780641a34`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:27:12 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 21:27:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 21:27:13 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:46:27 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 01:48:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 01:48:48 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 01:48:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:48:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 01:48:50 GMT
WORKDIR /go
# Fri, 04 Jun 2021 02:18:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 02:18:24 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 02:18:25 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 02:18:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 02:18:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 02:18:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 02:18:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adcc1eea9eeabb6de296adb3e0c1b0722cf13251ff3e4e2d0a5f7ed8e3d48342`  
		Last Modified: Wed, 14 Apr 2021 21:35:06 GMT  
		Size: 281.3 KB (281269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4ab2625f07be8d5c6e48046a05ff3ecc7f374b794a926fb62247b66b511909`  
		Last Modified: Wed, 14 Apr 2021 21:35:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689510d40a2658530c96a39b304e1561733255af89b84ce6de9f489b3ca1a281`  
		Last Modified: Fri, 04 Jun 2021 01:59:43 GMT  
		Size: 105.7 MB (105740137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4d89f102e3b1bb1c586ebf1bf8ab36d3a58ed7793fdb0f6ceca00bc2b177cd`  
		Last Modified: Fri, 04 Jun 2021 01:59:25 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44fa7996470329a7e8174cb5cbaa52ade2eb5fffabe426b05cab3d2c904e6e0`  
		Last Modified: Fri, 04 Jun 2021 02:19:02 GMT  
		Size: 6.4 MB (6395534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26081f37d859cc0d0f0882b13352f2ef140940d73620b130154c91355054b525`  
		Last Modified: Fri, 04 Jun 2021 02:19:02 GMT  
		Size: 1.3 MB (1311156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0133abdd19ffca66008a8732eca2edf1f571ed52fe2b3d873ed8158282f9f7`  
		Last Modified: Fri, 04 Jun 2021 02:19:01 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:9c6cfad074c68103b20a26d1f2da9f0f8f22b5406a356e5696e1856cf3e5c332
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112301607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfd32aee08fd69ca7dcd229bd475cce45176a90ef6154a872d01333b97e2119c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Fri, 04 Jun 2021 05:29:59 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 04 Jun 2021 05:30:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 04 Jun 2021 05:30:00 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 05:30:00 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 05:32:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 05:33:00 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 05:33:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 05:33:01 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 05:33:01 GMT
WORKDIR /go
# Fri, 04 Jun 2021 07:35:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 07:35:01 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 07:35:01 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 07:35:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 07:35:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 07:35:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 07:35:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90c33f298071ceb1106bce90623a7fe87a3be8510fe9512966f1a7bc5625a47`  
		Last Modified: Fri, 04 Jun 2021 05:41:55 GMT  
		Size: 281.4 KB (281382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f381ff0ec8799fc86bf65aba1711ab973cc107a53a6d134a9a0ba3267477a0fb`  
		Last Modified: Fri, 04 Jun 2021 05:41:55 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d5ab13bd0ab2cb8b8b4b1e08587ddb255e3d3bd2cebd7fcb8ba562bb0974d5`  
		Last Modified: Fri, 04 Jun 2021 05:42:20 GMT  
		Size: 101.9 MB (101944742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2d1d4b06a01686239e04dc869317cdd368448fe45334d9838856be1d149dae`  
		Last Modified: Fri, 04 Jun 2021 05:41:55 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fad5cba6f9b7a0e238d430bcd3ce8b3fc12e6bdc8cdb46008ce5a932e27f229`  
		Last Modified: Fri, 04 Jun 2021 07:36:16 GMT  
		Size: 6.2 MB (6230964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed25c6ff0ab0732ac72d5202c79100508522040b20b4ef01be1fb5e20210ae85`  
		Last Modified: Fri, 04 Jun 2021 07:36:15 GMT  
		Size: 1.2 MB (1221675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c309325d1d11d3a67efbffdd774a27af11a477b9ab43b25e95912d6d72b5c652`  
		Last Modified: Fri, 04 Jun 2021 07:36:15 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:3ce06d10a24fe566699c8997bc0c089e851e46c0f69fa0fff18d0085b4346289
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111232949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cde3b1d7cb6f225fb3b4f3064f07e8f9186fcbff0ecb697e5aa10d00899ea6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 27 May 2021 15:06:45 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 27 May 2021 15:06:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 May 2021 15:06:46 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 07:52:57 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 07:55:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 07:55:34 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 07:55:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 07:55:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 07:55:36 GMT
WORKDIR /go
# Fri, 04 Jun 2021 12:06:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 12:06:59 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 12:06:59 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 12:06:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 12:07:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 12:07:01 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 12:07:01 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7339ea1d6bf57b602a207a1e2f24e2f2d6d0fef53ac31afc17a550368c53e63b`  
		Last Modified: Thu, 27 May 2021 15:19:37 GMT  
		Size: 280.5 KB (280537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c586fedb7a1526f50c1bb5ccadd41167254abbdf9cc445264c5a2cda55bff7f3`  
		Last Modified: Thu, 27 May 2021 15:19:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac424f1791899264fd7faf16b2b868022b332df5c89c65ab7bd4da634a0debcc`  
		Last Modified: Fri, 04 Jun 2021 08:07:59 GMT  
		Size: 101.7 MB (101746953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ea8b8d5ee549723867d0f8a4a54e81bc6e8cffef6b2e29cd0efa53f44d75ae`  
		Last Modified: Fri, 04 Jun 2021 08:07:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73f5e95932571acfe6d65aba85701fb9e0a60e6aef82a4d1eeeeab75717fb1`  
		Last Modified: Fri, 04 Jun 2021 12:08:13 GMT  
		Size: 5.6 MB (5561103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c649a927d5a9a52469a77c3ba79e77cc5b94865a1f8d1085843dbd50573897e3`  
		Last Modified: Fri, 04 Jun 2021 12:08:13 GMT  
		Size: 1.2 MB (1219497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7604724e4d7dadae83d4d023c9f2101e6dcd59c058928794c12cc23a4f34d7f`  
		Last Modified: Fri, 04 Jun 2021 12:08:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5dc91099db737a46c5bb7ca6fe3c0174e49874c492ff48e5eac5fc30a579864b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111775816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73671d0a54a8053b75985bb11523edbe1e3877082dede6664d842d058fc6048b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 27 May 2021 22:17:28 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 27 May 2021 22:17:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 May 2021 22:17:29 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 04:00:14 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 04:01:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 04:01:36 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 04:01:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 04:01:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 04:01:37 GMT
WORKDIR /go
# Fri, 04 Jun 2021 07:44:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 07:44:36 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 07:44:36 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 07:44:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 07:44:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 07:44:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 07:44:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3088b5b3c5c0fab79ca41c188d3696a5053778b6c7d602b2aea8084c094608d1`  
		Last Modified: Thu, 27 May 2021 22:26:43 GMT  
		Size: 281.5 KB (281495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7225fbf94c881dc50b56f5430522fbde8891efa801909d5d9f06261d839cc5`  
		Last Modified: Thu, 27 May 2021 22:26:43 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba82ee9f976e7f9d818f11b866566f142f7ceddface2c0d3d5fe3a6920cc659d`  
		Last Modified: Fri, 04 Jun 2021 04:09:30 GMT  
		Size: 101.1 MB (101096027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506bd15cee9f23181bcd604afe8ec2b150b0321d4d0e741e272734456560caac`  
		Last Modified: Fri, 04 Jun 2021 04:09:12 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83fba387ff0d0e9e65223a37bf6a1e09e7e24774a900e99f743e8c3d455f4fdb`  
		Last Modified: Fri, 04 Jun 2021 07:45:32 GMT  
		Size: 6.5 MB (6484015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84ec75c54b55467ea07ae1ace7ace92b52355954733f1ecbd86d26937d03364`  
		Last Modified: Fri, 04 Jun 2021 07:45:31 GMT  
		Size: 1.2 MB (1201540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91117b691ccdbc0552460233c27811b1de617ff3bc78eac7af1f1f70d7b6f6cb`  
		Last Modified: Fri, 04 Jun 2021 07:45:31 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:7f735b71e3863db84fafaaef6c3299cd3f902d9d99504589d7d8b77ed30fdd1b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110613992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ead49008853a08fc29f3178cf58d7cfcb85b1d9dd361879df0f96cf640dcc94`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:53:57 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 22:54:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:54:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 03:07:09 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 03:08:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 03:09:08 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 03:09:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 03:09:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 03:09:30 GMT
WORKDIR /go
# Fri, 04 Jun 2021 09:16:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 09:16:18 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 09:16:26 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 09:16:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 09:16:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 09:16:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 09:16:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf726c40dc4802009a4b6f0f7947c86242c2c078623e8f1f21343864093b3a9`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 283.4 KB (283413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c17712dac96942b05a27f88ea5346bd57b4cabdb33c153562ef144635225b3`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6104245b6f3bb2cd73fecb2ee6ef3347bedc6f588475449849c4229c3321eb8`  
		Last Modified: Fri, 04 Jun 2021 03:20:31 GMT  
		Size: 99.5 MB (99515576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c228774385f5c8b0c6ad74f4b22b8976926d85634278c36ba33b49f23ac5154`  
		Last Modified: Fri, 04 Jun 2021 03:20:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af27e8f9d4959b48b81f61cb0d645eccfd256ee74635e0396fac0b732c0e57b`  
		Last Modified: Fri, 04 Jun 2021 09:17:36 GMT  
		Size: 6.8 MB (6830629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d43d75e1cc7759d079bd9ad4389f4cd3b79a036ff24add605969b915d46114`  
		Last Modified: Fri, 04 Jun 2021 09:17:35 GMT  
		Size: 1.2 MB (1170519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd193d55e35894d2beb5854ebb790227fb34a033785effbaa520604e248480c`  
		Last Modified: Fri, 04 Jun 2021 09:17:35 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:bb5f24094fadd35d4c5940a0c1f143d212544334b9bce93de93677dbabe4db16
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115475353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23250df470a63b89f2a4832f806630ba5002e9595baed80673428d73b9b8e8a9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:45:11 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:45:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:45:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:26:42 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 01:28:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 01:28:34 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 01:28:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:28:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 01:28:36 GMT
WORKDIR /go
# Fri, 04 Jun 2021 03:02:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 03:02:56 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 03:02:56 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 03:02:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 03:02:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 03:03:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 03:03:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc746875ae346ee6ec3c9080f8a7a50bef3899ea9d5ae9dac45a81bfe861c9d`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 281.7 KB (281708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0242688236000dd8f33d16f89f36da3ef1bb2a7a32bb59a7eb97a18ed3d5158`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0ff47eca4941b373fedcfb40530f4d5ef82aed9a9b83bd7fa6cee6546112fd`  
		Last Modified: Fri, 04 Jun 2021 01:37:12 GMT  
		Size: 104.8 MB (104846719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6991fc153a27c9de6b023272f31bf22b708f788131bd628abeb30592007377a8`  
		Last Modified: Fri, 04 Jun 2021 01:36:59 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b452ba9be082c7a2255414c44dde4b275a327b14d24e947901062089bd7ebf43`  
		Last Modified: Fri, 04 Jun 2021 03:03:37 GMT  
		Size: 6.5 MB (6479039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507d613df3c6f7ea5929ebfe6205e87ae1b89cd044677a765da66d135bb7ef57`  
		Last Modified: Fri, 04 Jun 2021 03:03:37 GMT  
		Size: 1.3 MB (1264524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd9e1c527bba47d9aa0c07957cb156d2c1d205ca81c81e8b00b5b9c0330290b`  
		Last Modified: Fri, 04 Jun 2021 03:03:36 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:0cba0bbebbf26fbfe27a39006a093cfb426976baff4e8c3ec906a2a229be9e69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2808421770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c51b9b016f1a3599a109e39809816252f59ecd94d60ef1b7043ab7404059d79`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 12:10:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 12:37:22 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Jun 2021 12:37:25 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Jun 2021 12:37:29 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Jun 2021 12:37:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Jun 2021 12:38:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:38:25 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Jun 2021 12:38:51 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Jun 2021 12:38:53 GMT
ENV GOLANG_VERSION=1.16.5
# Wed, 09 Jun 2021 12:41:22 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:41:27 GMT
WORKDIR C:\gopath
# Wed, 09 Jun 2021 20:15:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:15:04 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 09 Jun 2021 20:15:06 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:15:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Jun 2021 20:15:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Jun 2021 20:15:46 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7863ef96846d497ea06fe442ea13dcecaf5c248ce238c69800475281a4fa848e`  
		Last Modified: Wed, 09 Jun 2021 12:20:41 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f985a0b4390580a94aa3cbc8ecb01fc33805bb3304c4217dc5ec9fb6626011ca`  
		Last Modified: Wed, 09 Jun 2021 13:03:26 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5adf5cc2989b1cf730e7993bd088f778b31b33bac78f6d9c133226f7bcf4a6`  
		Last Modified: Wed, 09 Jun 2021 13:03:24 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480b981517ab26b6ee7e090e51d040995ac5a6a55410880ea3f0c8255dada3bc`  
		Last Modified: Wed, 09 Jun 2021 13:03:24 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a372a8dcfb8f1152565f4b8c928c202db247ddc21fd9a35838a2278c65ff6f`  
		Last Modified: Wed, 09 Jun 2021 13:03:23 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97090ffba94bc8afc85a54e404c8aca13253969fe01c8b0ac1f8ce3a0b909953`  
		Last Modified: Wed, 09 Jun 2021 13:03:53 GMT  
		Size: 25.4 MB (25445694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb1c026791860f230531a960e59a35d86f3ae617c5b6ad60155718694ed3720`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fca536252ace3ea8e08bcd38a313ad63d7d308f4a1d24734c324d191b65647`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 314.6 KB (314587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3865edd5ab3e6e2858d35fea90d96f24eb95579b3bb7f95674954df09b428a8e`  
		Last Modified: Wed, 09 Jun 2021 13:03:20 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424a1b81819edd902af8893d485a39318ee4023db4db6f9c73ebb8470a5c2310`  
		Last Modified: Wed, 09 Jun 2021 13:03:58 GMT  
		Size: 139.4 MB (139355479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f54cc4fcf8b7300908d2cb4aa6dbfe433cc614c35c200ca655b96d576a40412`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 1.6 KB (1596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ae8d8d0f1afc3ddbfe8673534bd1ae7afdf7662fb5fd73ef017088a251e15c`  
		Last Modified: Wed, 09 Jun 2021 20:20:23 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761852a93f82584033e99d58efb7a7e5fad44135d49f23090e1217932f809891`  
		Last Modified: Wed, 09 Jun 2021 20:20:20 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f24be856334e97a03392fc575807609b5afd8808514d9ca8305700e72834ea`  
		Last Modified: Wed, 09 Jun 2021 20:20:20 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047b293c2c055e53ea3099cdc7cd511d55cb43391cbcfd34e0c3a96ac1d179ca`  
		Last Modified: Wed, 09 Jun 2021 20:20:20 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2806e8d39eec5d338e88005243d0a11fcb7c24dab13df4ee3c5ce9ee0266dd9`  
		Last Modified: Wed, 09 Jun 2021 20:20:21 GMT  
		Size: 1.7 MB (1703136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de952f0fc6af6d7eea8c8d4d424cf97622e0b2628a32387976f4dc8df54efb8`  
		Last Modified: Wed, 09 Jun 2021 20:20:20 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:4481a6011b8d50eca815372f7a8f28afaae493233d49d4ec20b3d3a5abf93fc7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6437000457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4919458e8d791f772cd7dd820598edd51cc401fa898c7e4ddddc19e6bb2890fe`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 12:41:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 12:41:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Jun 2021 12:41:43 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Jun 2021 12:41:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Jun 2021 12:41:49 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Jun 2021 12:44:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:44:27 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Jun 2021 12:45:49 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Jun 2021 12:45:51 GMT
ENV GOLANG_VERSION=1.16.5
# Wed, 09 Jun 2021 12:49:20 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:49:24 GMT
WORKDIR C:\gopath
# Wed, 09 Jun 2021 20:15:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:15:56 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 09 Jun 2021 20:15:59 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:16:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Jun 2021 20:17:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Jun 2021 20:17:28 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c82e82e95dbad4ccc260b42e03767eb07222e2f00ec57a69b3c87b17da1d2fd3`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a881968e28f8c2900b00800a0de406d0e98740558d9564ad738d053e63d9a1e`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab71df915cf7ac4c559039a917269e11faab2d0e6862a01408431df7fb40362f`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82ce560dcbc3235ed87d6c938aa761616dbd299188ae53a51a266eb37f381f6`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bee5ea2f89fe3f3e514b8dfcd823da340447b633c6048e00773d1c30fbbc0e9`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad71deb840b73610184070ebc7c566bd1dac9cc309d53679460697243bab7640`  
		Last Modified: Wed, 09 Jun 2021 13:04:50 GMT  
		Size: 25.4 MB (25441204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16f2a89ed7a230471eb96b67829deb255795564010b0ff2de47179cdfdec1d0`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cc755175ec255452c16e1e41cc78a8cd719d65f70221e7d128c1dc18eec8f2`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 307.7 KB (307689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d153904f724dbfda646a6c5ccdc1eed2545cf7777c8650461abdedafe75bc693`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ec88320a2e6bf1cfef8856b9271f7d2fa4d2ae8e0eb5b9a44175d04a725631`  
		Last Modified: Wed, 09 Jun 2021 13:04:58 GMT  
		Size: 143.8 MB (143821249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419b516d300f276d9a3f98a1d2c47394abb00b15edeaadcb2f5d0ecee3380f14`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 1.6 KB (1576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d420a2d4c5bca557510bd5eaeea0268b05bb6e61104acea0af1e28c7537c8352`  
		Last Modified: Wed, 09 Jun 2021 20:20:41 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06bf21d106193b12d0b9a688698ec718f7fb4514f317565933b89f22da0d1de`  
		Last Modified: Wed, 09 Jun 2021 20:20:38 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64471c2fb9e42024fce3859860cf6a05f584b8c21ff5c776f7c285588f1117fc`  
		Last Modified: Wed, 09 Jun 2021 20:20:38 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f2c847c9bab79f9970336a628d5b7948504e3f2a67f95cac9a1a3f12132673`  
		Last Modified: Wed, 09 Jun 2021 20:20:38 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae1157ef3d362883b0503349e9d7cb6d729fa420af63a826262dca25f7a9fc`  
		Last Modified: Wed, 09 Jun 2021 20:20:39 GMT  
		Size: 1.7 MB (1684468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e122b3fd6e41cb67b3d9b46e55753aa37f1f60c2de7fab150181822a556d2791`  
		Last Modified: Wed, 09 Jun 2021 20:20:38 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:4b4685dba38126a1d8dc692a9cc3f60e145e085f5f2a132b32bdbbcec0109a55
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
$ docker pull caddy@sha256:acb1d8e470fc9d3be900f5a534a57d59d7e827ad2a4fabbedbacde1d08e850ee
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116540780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eafee2350c73e5c74f40dc4ff4146d3ac64f52d221205b317621567780641a34`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:27:12 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 21:27:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 21:27:13 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:46:27 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 01:48:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 01:48:48 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 01:48:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:48:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 01:48:50 GMT
WORKDIR /go
# Fri, 04 Jun 2021 02:18:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 02:18:24 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 02:18:25 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 02:18:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 02:18:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 02:18:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 02:18:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adcc1eea9eeabb6de296adb3e0c1b0722cf13251ff3e4e2d0a5f7ed8e3d48342`  
		Last Modified: Wed, 14 Apr 2021 21:35:06 GMT  
		Size: 281.3 KB (281269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4ab2625f07be8d5c6e48046a05ff3ecc7f374b794a926fb62247b66b511909`  
		Last Modified: Wed, 14 Apr 2021 21:35:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689510d40a2658530c96a39b304e1561733255af89b84ce6de9f489b3ca1a281`  
		Last Modified: Fri, 04 Jun 2021 01:59:43 GMT  
		Size: 105.7 MB (105740137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4d89f102e3b1bb1c586ebf1bf8ab36d3a58ed7793fdb0f6ceca00bc2b177cd`  
		Last Modified: Fri, 04 Jun 2021 01:59:25 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44fa7996470329a7e8174cb5cbaa52ade2eb5fffabe426b05cab3d2c904e6e0`  
		Last Modified: Fri, 04 Jun 2021 02:19:02 GMT  
		Size: 6.4 MB (6395534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26081f37d859cc0d0f0882b13352f2ef140940d73620b130154c91355054b525`  
		Last Modified: Fri, 04 Jun 2021 02:19:02 GMT  
		Size: 1.3 MB (1311156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0133abdd19ffca66008a8732eca2edf1f571ed52fe2b3d873ed8158282f9f7`  
		Last Modified: Fri, 04 Jun 2021 02:19:01 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:9c6cfad074c68103b20a26d1f2da9f0f8f22b5406a356e5696e1856cf3e5c332
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112301607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfd32aee08fd69ca7dcd229bd475cce45176a90ef6154a872d01333b97e2119c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Fri, 04 Jun 2021 05:29:59 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 04 Jun 2021 05:30:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 04 Jun 2021 05:30:00 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 05:30:00 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 05:32:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 05:33:00 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 05:33:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 05:33:01 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 05:33:01 GMT
WORKDIR /go
# Fri, 04 Jun 2021 07:35:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 07:35:01 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 07:35:01 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 07:35:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 07:35:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 07:35:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 07:35:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90c33f298071ceb1106bce90623a7fe87a3be8510fe9512966f1a7bc5625a47`  
		Last Modified: Fri, 04 Jun 2021 05:41:55 GMT  
		Size: 281.4 KB (281382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f381ff0ec8799fc86bf65aba1711ab973cc107a53a6d134a9a0ba3267477a0fb`  
		Last Modified: Fri, 04 Jun 2021 05:41:55 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d5ab13bd0ab2cb8b8b4b1e08587ddb255e3d3bd2cebd7fcb8ba562bb0974d5`  
		Last Modified: Fri, 04 Jun 2021 05:42:20 GMT  
		Size: 101.9 MB (101944742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2d1d4b06a01686239e04dc869317cdd368448fe45334d9838856be1d149dae`  
		Last Modified: Fri, 04 Jun 2021 05:41:55 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fad5cba6f9b7a0e238d430bcd3ce8b3fc12e6bdc8cdb46008ce5a932e27f229`  
		Last Modified: Fri, 04 Jun 2021 07:36:16 GMT  
		Size: 6.2 MB (6230964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed25c6ff0ab0732ac72d5202c79100508522040b20b4ef01be1fb5e20210ae85`  
		Last Modified: Fri, 04 Jun 2021 07:36:15 GMT  
		Size: 1.2 MB (1221675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c309325d1d11d3a67efbffdd774a27af11a477b9ab43b25e95912d6d72b5c652`  
		Last Modified: Fri, 04 Jun 2021 07:36:15 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:3ce06d10a24fe566699c8997bc0c089e851e46c0f69fa0fff18d0085b4346289
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111232949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cde3b1d7cb6f225fb3b4f3064f07e8f9186fcbff0ecb697e5aa10d00899ea6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 27 May 2021 15:06:45 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 27 May 2021 15:06:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 May 2021 15:06:46 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 07:52:57 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 07:55:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 07:55:34 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 07:55:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 07:55:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 07:55:36 GMT
WORKDIR /go
# Fri, 04 Jun 2021 12:06:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 12:06:59 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 12:06:59 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 12:06:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 12:07:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 12:07:01 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 12:07:01 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7339ea1d6bf57b602a207a1e2f24e2f2d6d0fef53ac31afc17a550368c53e63b`  
		Last Modified: Thu, 27 May 2021 15:19:37 GMT  
		Size: 280.5 KB (280537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c586fedb7a1526f50c1bb5ccadd41167254abbdf9cc445264c5a2cda55bff7f3`  
		Last Modified: Thu, 27 May 2021 15:19:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac424f1791899264fd7faf16b2b868022b332df5c89c65ab7bd4da634a0debcc`  
		Last Modified: Fri, 04 Jun 2021 08:07:59 GMT  
		Size: 101.7 MB (101746953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ea8b8d5ee549723867d0f8a4a54e81bc6e8cffef6b2e29cd0efa53f44d75ae`  
		Last Modified: Fri, 04 Jun 2021 08:07:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73f5e95932571acfe6d65aba85701fb9e0a60e6aef82a4d1eeeeab75717fb1`  
		Last Modified: Fri, 04 Jun 2021 12:08:13 GMT  
		Size: 5.6 MB (5561103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c649a927d5a9a52469a77c3ba79e77cc5b94865a1f8d1085843dbd50573897e3`  
		Last Modified: Fri, 04 Jun 2021 12:08:13 GMT  
		Size: 1.2 MB (1219497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7604724e4d7dadae83d4d023c9f2101e6dcd59c058928794c12cc23a4f34d7f`  
		Last Modified: Fri, 04 Jun 2021 12:08:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5dc91099db737a46c5bb7ca6fe3c0174e49874c492ff48e5eac5fc30a579864b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111775816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73671d0a54a8053b75985bb11523edbe1e3877082dede6664d842d058fc6048b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 27 May 2021 22:17:28 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 27 May 2021 22:17:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 May 2021 22:17:29 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 04:00:14 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 04:01:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 04:01:36 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 04:01:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 04:01:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 04:01:37 GMT
WORKDIR /go
# Fri, 04 Jun 2021 07:44:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 07:44:36 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 07:44:36 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 07:44:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 07:44:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 07:44:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 07:44:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3088b5b3c5c0fab79ca41c188d3696a5053778b6c7d602b2aea8084c094608d1`  
		Last Modified: Thu, 27 May 2021 22:26:43 GMT  
		Size: 281.5 KB (281495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7225fbf94c881dc50b56f5430522fbde8891efa801909d5d9f06261d839cc5`  
		Last Modified: Thu, 27 May 2021 22:26:43 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba82ee9f976e7f9d818f11b866566f142f7ceddface2c0d3d5fe3a6920cc659d`  
		Last Modified: Fri, 04 Jun 2021 04:09:30 GMT  
		Size: 101.1 MB (101096027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506bd15cee9f23181bcd604afe8ec2b150b0321d4d0e741e272734456560caac`  
		Last Modified: Fri, 04 Jun 2021 04:09:12 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83fba387ff0d0e9e65223a37bf6a1e09e7e24774a900e99f743e8c3d455f4fdb`  
		Last Modified: Fri, 04 Jun 2021 07:45:32 GMT  
		Size: 6.5 MB (6484015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84ec75c54b55467ea07ae1ace7ace92b52355954733f1ecbd86d26937d03364`  
		Last Modified: Fri, 04 Jun 2021 07:45:31 GMT  
		Size: 1.2 MB (1201540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91117b691ccdbc0552460233c27811b1de617ff3bc78eac7af1f1f70d7b6f6cb`  
		Last Modified: Fri, 04 Jun 2021 07:45:31 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:7f735b71e3863db84fafaaef6c3299cd3f902d9d99504589d7d8b77ed30fdd1b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110613992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ead49008853a08fc29f3178cf58d7cfcb85b1d9dd361879df0f96cf640dcc94`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:53:57 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 22:54:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:54:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 03:07:09 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 03:08:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 03:09:08 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 03:09:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 03:09:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 03:09:30 GMT
WORKDIR /go
# Fri, 04 Jun 2021 09:16:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 09:16:18 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 09:16:26 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 09:16:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 09:16:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 09:16:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 09:16:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf726c40dc4802009a4b6f0f7947c86242c2c078623e8f1f21343864093b3a9`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 283.4 KB (283413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c17712dac96942b05a27f88ea5346bd57b4cabdb33c153562ef144635225b3`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6104245b6f3bb2cd73fecb2ee6ef3347bedc6f588475449849c4229c3321eb8`  
		Last Modified: Fri, 04 Jun 2021 03:20:31 GMT  
		Size: 99.5 MB (99515576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c228774385f5c8b0c6ad74f4b22b8976926d85634278c36ba33b49f23ac5154`  
		Last Modified: Fri, 04 Jun 2021 03:20:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af27e8f9d4959b48b81f61cb0d645eccfd256ee74635e0396fac0b732c0e57b`  
		Last Modified: Fri, 04 Jun 2021 09:17:36 GMT  
		Size: 6.8 MB (6830629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d43d75e1cc7759d079bd9ad4389f4cd3b79a036ff24add605969b915d46114`  
		Last Modified: Fri, 04 Jun 2021 09:17:35 GMT  
		Size: 1.2 MB (1170519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd193d55e35894d2beb5854ebb790227fb34a033785effbaa520604e248480c`  
		Last Modified: Fri, 04 Jun 2021 09:17:35 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:bb5f24094fadd35d4c5940a0c1f143d212544334b9bce93de93677dbabe4db16
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115475353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23250df470a63b89f2a4832f806630ba5002e9595baed80673428d73b9b8e8a9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:45:11 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:45:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:45:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:26:42 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 01:28:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 01:28:34 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 01:28:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:28:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 01:28:36 GMT
WORKDIR /go
# Fri, 04 Jun 2021 03:02:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 03:02:56 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 03:02:56 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 03:02:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 03:02:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 03:03:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 03:03:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc746875ae346ee6ec3c9080f8a7a50bef3899ea9d5ae9dac45a81bfe861c9d`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 281.7 KB (281708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0242688236000dd8f33d16f89f36da3ef1bb2a7a32bb59a7eb97a18ed3d5158`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0ff47eca4941b373fedcfb40530f4d5ef82aed9a9b83bd7fa6cee6546112fd`  
		Last Modified: Fri, 04 Jun 2021 01:37:12 GMT  
		Size: 104.8 MB (104846719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6991fc153a27c9de6b023272f31bf22b708f788131bd628abeb30592007377a8`  
		Last Modified: Fri, 04 Jun 2021 01:36:59 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b452ba9be082c7a2255414c44dde4b275a327b14d24e947901062089bd7ebf43`  
		Last Modified: Fri, 04 Jun 2021 03:03:37 GMT  
		Size: 6.5 MB (6479039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507d613df3c6f7ea5929ebfe6205e87ae1b89cd044677a765da66d135bb7ef57`  
		Last Modified: Fri, 04 Jun 2021 03:03:37 GMT  
		Size: 1.3 MB (1264524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd9e1c527bba47d9aa0c07957cb156d2c1d205ca81c81e8b00b5b9c0330290b`  
		Last Modified: Fri, 04 Jun 2021 03:03:36 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:5c8e1831e4df2e628cf1bf9d35260d624c1b15d27abfac59a5431f15f3d0a66a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:0cba0bbebbf26fbfe27a39006a093cfb426976baff4e8c3ec906a2a229be9e69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2808421770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c51b9b016f1a3599a109e39809816252f59ecd94d60ef1b7043ab7404059d79`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 12:10:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 12:37:22 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Jun 2021 12:37:25 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Jun 2021 12:37:29 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Jun 2021 12:37:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Jun 2021 12:38:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:38:25 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Jun 2021 12:38:51 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Jun 2021 12:38:53 GMT
ENV GOLANG_VERSION=1.16.5
# Wed, 09 Jun 2021 12:41:22 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:41:27 GMT
WORKDIR C:\gopath
# Wed, 09 Jun 2021 20:15:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:15:04 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 09 Jun 2021 20:15:06 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:15:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Jun 2021 20:15:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Jun 2021 20:15:46 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7863ef96846d497ea06fe442ea13dcecaf5c248ce238c69800475281a4fa848e`  
		Last Modified: Wed, 09 Jun 2021 12:20:41 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f985a0b4390580a94aa3cbc8ecb01fc33805bb3304c4217dc5ec9fb6626011ca`  
		Last Modified: Wed, 09 Jun 2021 13:03:26 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5adf5cc2989b1cf730e7993bd088f778b31b33bac78f6d9c133226f7bcf4a6`  
		Last Modified: Wed, 09 Jun 2021 13:03:24 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480b981517ab26b6ee7e090e51d040995ac5a6a55410880ea3f0c8255dada3bc`  
		Last Modified: Wed, 09 Jun 2021 13:03:24 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a372a8dcfb8f1152565f4b8c928c202db247ddc21fd9a35838a2278c65ff6f`  
		Last Modified: Wed, 09 Jun 2021 13:03:23 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97090ffba94bc8afc85a54e404c8aca13253969fe01c8b0ac1f8ce3a0b909953`  
		Last Modified: Wed, 09 Jun 2021 13:03:53 GMT  
		Size: 25.4 MB (25445694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb1c026791860f230531a960e59a35d86f3ae617c5b6ad60155718694ed3720`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fca536252ace3ea8e08bcd38a313ad63d7d308f4a1d24734c324d191b65647`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 314.6 KB (314587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3865edd5ab3e6e2858d35fea90d96f24eb95579b3bb7f95674954df09b428a8e`  
		Last Modified: Wed, 09 Jun 2021 13:03:20 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424a1b81819edd902af8893d485a39318ee4023db4db6f9c73ebb8470a5c2310`  
		Last Modified: Wed, 09 Jun 2021 13:03:58 GMT  
		Size: 139.4 MB (139355479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f54cc4fcf8b7300908d2cb4aa6dbfe433cc614c35c200ca655b96d576a40412`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 1.6 KB (1596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ae8d8d0f1afc3ddbfe8673534bd1ae7afdf7662fb5fd73ef017088a251e15c`  
		Last Modified: Wed, 09 Jun 2021 20:20:23 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761852a93f82584033e99d58efb7a7e5fad44135d49f23090e1217932f809891`  
		Last Modified: Wed, 09 Jun 2021 20:20:20 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f24be856334e97a03392fc575807609b5afd8808514d9ca8305700e72834ea`  
		Last Modified: Wed, 09 Jun 2021 20:20:20 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047b293c2c055e53ea3099cdc7cd511d55cb43391cbcfd34e0c3a96ac1d179ca`  
		Last Modified: Wed, 09 Jun 2021 20:20:20 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2806e8d39eec5d338e88005243d0a11fcb7c24dab13df4ee3c5ce9ee0266dd9`  
		Last Modified: Wed, 09 Jun 2021 20:20:21 GMT  
		Size: 1.7 MB (1703136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de952f0fc6af6d7eea8c8d4d424cf97622e0b2628a32387976f4dc8df54efb8`  
		Last Modified: Wed, 09 Jun 2021 20:20:20 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:be2e88c1df8f07111be41e7303360a3a48b2c80edee366850af00d9df909afdb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `caddy:2-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:4481a6011b8d50eca815372f7a8f28afaae493233d49d4ec20b3d3a5abf93fc7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6437000457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4919458e8d791f772cd7dd820598edd51cc401fa898c7e4ddddc19e6bb2890fe`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 12:41:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 12:41:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Jun 2021 12:41:43 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Jun 2021 12:41:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Jun 2021 12:41:49 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Jun 2021 12:44:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:44:27 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Jun 2021 12:45:49 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Jun 2021 12:45:51 GMT
ENV GOLANG_VERSION=1.16.5
# Wed, 09 Jun 2021 12:49:20 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:49:24 GMT
WORKDIR C:\gopath
# Wed, 09 Jun 2021 20:15:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:15:56 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 09 Jun 2021 20:15:59 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:16:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Jun 2021 20:17:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Jun 2021 20:17:28 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c82e82e95dbad4ccc260b42e03767eb07222e2f00ec57a69b3c87b17da1d2fd3`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a881968e28f8c2900b00800a0de406d0e98740558d9564ad738d053e63d9a1e`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab71df915cf7ac4c559039a917269e11faab2d0e6862a01408431df7fb40362f`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82ce560dcbc3235ed87d6c938aa761616dbd299188ae53a51a266eb37f381f6`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bee5ea2f89fe3f3e514b8dfcd823da340447b633c6048e00773d1c30fbbc0e9`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad71deb840b73610184070ebc7c566bd1dac9cc309d53679460697243bab7640`  
		Last Modified: Wed, 09 Jun 2021 13:04:50 GMT  
		Size: 25.4 MB (25441204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16f2a89ed7a230471eb96b67829deb255795564010b0ff2de47179cdfdec1d0`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cc755175ec255452c16e1e41cc78a8cd719d65f70221e7d128c1dc18eec8f2`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 307.7 KB (307689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d153904f724dbfda646a6c5ccdc1eed2545cf7777c8650461abdedafe75bc693`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ec88320a2e6bf1cfef8856b9271f7d2fa4d2ae8e0eb5b9a44175d04a725631`  
		Last Modified: Wed, 09 Jun 2021 13:04:58 GMT  
		Size: 143.8 MB (143821249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419b516d300f276d9a3f98a1d2c47394abb00b15edeaadcb2f5d0ecee3380f14`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 1.6 KB (1576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d420a2d4c5bca557510bd5eaeea0268b05bb6e61104acea0af1e28c7537c8352`  
		Last Modified: Wed, 09 Jun 2021 20:20:41 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06bf21d106193b12d0b9a688698ec718f7fb4514f317565933b89f22da0d1de`  
		Last Modified: Wed, 09 Jun 2021 20:20:38 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64471c2fb9e42024fce3859860cf6a05f584b8c21ff5c776f7c285588f1117fc`  
		Last Modified: Wed, 09 Jun 2021 20:20:38 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f2c847c9bab79f9970336a628d5b7948504e3f2a67f95cac9a1a3f12132673`  
		Last Modified: Wed, 09 Jun 2021 20:20:38 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae1157ef3d362883b0503349e9d7cb6d729fa420af63a826262dca25f7a9fc`  
		Last Modified: Wed, 09 Jun 2021 20:20:39 GMT  
		Size: 1.7 MB (1684468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e122b3fd6e41cb67b3d9b46e55753aa37f1f60c2de7fab150181822a556d2791`  
		Last Modified: Wed, 09 Jun 2021 20:20:38 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:3f315a56b68ba9264142c6087b0db8f08492d6a8f90e8f16604e23920a1753fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:d4a3e0eabf14e4f98a9bcf5eada28d1443573b082afe95028d548d5b88a2b33e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2654170862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:736d3aa581b715efdf7c0431ebfbaed21b664091d8e8f7e4595c5f9dabbd2acb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 12:10:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:08:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Jun 2021 20:08:07 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:08:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Jun 2021 20:08:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Jun 2021 20:08:49 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Jun 2021 20:08:51 GMT
VOLUME [c:/config]
# Wed, 09 Jun 2021 20:08:53 GMT
VOLUME [c:/data]
# Wed, 09 Jun 2021 20:08:55 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 09 Jun 2021 20:08:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Jun 2021 20:09:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Jun 2021 20:09:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Jun 2021 20:09:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Jun 2021 20:09:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Jun 2021 20:09:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Jun 2021 20:09:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Jun 2021 20:09:14 GMT
EXPOSE 80
# Wed, 09 Jun 2021 20:09:17 GMT
EXPOSE 443
# Wed, 09 Jun 2021 20:09:19 GMT
EXPOSE 2019
# Wed, 09 Jun 2021 20:09:41 GMT
RUN caddy version
# Wed, 09 Jun 2021 20:09:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7863ef96846d497ea06fe442ea13dcecaf5c248ce238c69800475281a4fa848e`  
		Last Modified: Wed, 09 Jun 2021 12:20:41 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dc18d712eacfb666370e311daaf51e09fc2f76ca762e4592e149fbe6aba561`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 361.4 KB (361380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b774f6019fa0c611532d02bdf31c54e9da56fe2330e3e0745538ef036cfb87`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e977598d13d0ee9ae780f2cf34706c57e810301d20d9fc8286ad9390b9166b`  
		Last Modified: Wed, 09 Jun 2021 20:19:37 GMT  
		Size: 11.9 MB (11906202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7361692fe34486902f2dd9f69cc3bce54c4cb8c5c86ed80a0d75033f25ae5213`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35d39d3918ab9262122b494a653aec25e76a65396f9198d7be955cb9c26c6f3`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66891a50a919af8d3cb83358a7f8d33b2055c143bd3499cc431fd32d053ed393`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519d446a1689a5424a77bf1cbf0f00153b28c6eff9ee22f0f88e0e32b3f6bda3`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534ea2eef93aa67b4ac4bfb48ac5498fa33b02d0b88b9ae60b8ae159addacecc`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19fc40bc9ade11a1755b185c529e961b474d959d45a44b1b1ab5f12e3d17863a`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ef9960b6bac284e65c351bc447bb8931486a0c1c3ee68c9e5a62828b4ae0e`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cfda8707421463aa0f297ce5d4ac3a615f60caf56e6e69a299caa08a04f7da`  
		Last Modified: Wed, 09 Jun 2021 20:19:29 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa0c9ece6e3482cf3ffc8d9a087d113db0f7c249f59bcf06f3ffc65c5e4bce0`  
		Last Modified: Wed, 09 Jun 2021 20:19:29 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6614223fb410a8262956f73a038f6d79b67d5976fe8740b21dfa2121a9cbd7f2`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f354857e070035731eb660ec35ff9f8549b6cc79211bab40ae642d9875f98f8b`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc94f29a4cb79013fce0bf1a5776868fa31912b598231e46883a114d86f712d3`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e536fde913e2e2d5ae24846adca32195330a9be6e7d1c3180ce7ac6bc6a35ae1`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b11db027637bf7abeec6bbcd83920c4eb7c291aeeae4d2886a1563bf41289a6`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3a70d973d27d739faae877290b3184bee11c706ebd4bfa515d180fba88ef0f`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc7b3e3d99424f8d3737a4502a6f50767ae25b699a315155b98700af682b64f`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 292.6 KB (292631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d435932a64bec158a6193fa4a31a1b38e446ec9f63c0b6be3282c3acf3288949`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:e7e7af29e7917229552a0c802147dba99fb7a1427b84296a2c60ea7e19cbcb0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278267906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7184db699efd0a2ce0077179784cc7277e5faa7d07534ea1ce32d61d7f46ebc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 12:41:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:11:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Jun 2021 20:11:30 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:13:06 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Jun 2021 20:13:09 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Jun 2021 20:13:11 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Jun 2021 20:13:15 GMT
VOLUME [c:/config]
# Wed, 09 Jun 2021 20:13:18 GMT
VOLUME [c:/data]
# Wed, 09 Jun 2021 20:13:20 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 09 Jun 2021 20:13:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Jun 2021 20:13:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Jun 2021 20:13:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Jun 2021 20:13:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Jun 2021 20:13:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Jun 2021 20:13:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Jun 2021 20:13:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Jun 2021 20:13:40 GMT
EXPOSE 80
# Wed, 09 Jun 2021 20:13:42 GMT
EXPOSE 443
# Wed, 09 Jun 2021 20:13:45 GMT
EXPOSE 2019
# Wed, 09 Jun 2021 20:14:40 GMT
RUN caddy version
# Wed, 09 Jun 2021 20:14:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c82e82e95dbad4ccc260b42e03767eb07222e2f00ec57a69b3c87b17da1d2fd3`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a28e390d3b8e7b9369b102914eaee6e1fa0d14eb258b628be67f99f32f06f81`  
		Last Modified: Wed, 09 Jun 2021 20:20:01 GMT  
		Size: 357.4 KB (357370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7f07987f083e935103f83e47894b93aceaf05d1ded81dd09eb0bc3c8e45af`  
		Last Modified: Wed, 09 Jun 2021 20:20:01 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e65ddfdcdd60907208873b2a532cc58bc0f57d144430cef2c7630e80e4fd1e`  
		Last Modified: Wed, 09 Jun 2021 20:20:05 GMT  
		Size: 11.9 MB (11896985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58e4679b7ef7e1b9d82f44a6b5055c6916801193550bcce3ce390851224c736`  
		Last Modified: Wed, 09 Jun 2021 20:20:00 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107d803623512ea83de929509cc68f334261f2018c60bde60a99eadd0c2b179`  
		Last Modified: Wed, 09 Jun 2021 20:20:00 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f757538ddb020d145715a4890594958e741fe98366f1a58314361e5a8a3487`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462510ee9cb1c642e2804f8f607f02ccc5c31b63c956b9394bf38c5041b10d8b`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e87709f8365472aa7278651dacfc7eee93b24859a494cf6904b4f7ce80df0a`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5439b862b8218f1d7e0e0269efdbed614475ffbdcbaac06a3953f80b07677a1a`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1950c17917c025587fa23872145ee00eaaa11939dc87314c1aa74119db642d`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84164685053ad8b12a46e198ec2e93143d1df956bbbd4af76c88d0f549031c60`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103b7e93d2e2faefef7bd14bc00910442ce8da843f4fb726e2dba2d97752ddc9`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046d1e0cd75d46944ff833afe00c5dc9835ec1eb72876965a98a1488778910a6`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593a0ce075f6e5e07785dd7cd14aa1c274339da4d6f80495f0d1a85fabdef5db`  
		Last Modified: Wed, 09 Jun 2021 20:19:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14f5cdc43c91f65e6c5879691adc6e392d353807b27465a9b270fe7a06da51c`  
		Last Modified: Wed, 09 Jun 2021 20:19:55 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd488f5f58644d68e5103098932448a58d05a716861b26bf33376e75ad27e61`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c218cc3caa4b354c536ad99d30753a6eb41c52a58c52aafc0655a8482382a07`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3dad29a1e0241680f68697c2b0dbca8e85d0084faef4bdd3e66c8294be80671`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daeda652af05f03b2ec029aa5caa6b49d533546fa8347f5b1db003e8a83a7c30`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 260.8 KB (260840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9779c5588bf525e972d3b02ecaeeee32f3939ef8d54e8a16c52e0e62804e2e42`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:699404cfeaf1b53b36b5cad0c6d2fe8858034adb85e80f41f14f9fbe13a22366
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:d4a3e0eabf14e4f98a9bcf5eada28d1443573b082afe95028d548d5b88a2b33e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2654170862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:736d3aa581b715efdf7c0431ebfbaed21b664091d8e8f7e4595c5f9dabbd2acb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 12:10:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:08:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Jun 2021 20:08:07 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:08:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Jun 2021 20:08:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Jun 2021 20:08:49 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Jun 2021 20:08:51 GMT
VOLUME [c:/config]
# Wed, 09 Jun 2021 20:08:53 GMT
VOLUME [c:/data]
# Wed, 09 Jun 2021 20:08:55 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 09 Jun 2021 20:08:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Jun 2021 20:09:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Jun 2021 20:09:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Jun 2021 20:09:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Jun 2021 20:09:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Jun 2021 20:09:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Jun 2021 20:09:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Jun 2021 20:09:14 GMT
EXPOSE 80
# Wed, 09 Jun 2021 20:09:17 GMT
EXPOSE 443
# Wed, 09 Jun 2021 20:09:19 GMT
EXPOSE 2019
# Wed, 09 Jun 2021 20:09:41 GMT
RUN caddy version
# Wed, 09 Jun 2021 20:09:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7863ef96846d497ea06fe442ea13dcecaf5c248ce238c69800475281a4fa848e`  
		Last Modified: Wed, 09 Jun 2021 12:20:41 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dc18d712eacfb666370e311daaf51e09fc2f76ca762e4592e149fbe6aba561`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 361.4 KB (361380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b774f6019fa0c611532d02bdf31c54e9da56fe2330e3e0745538ef036cfb87`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e977598d13d0ee9ae780f2cf34706c57e810301d20d9fc8286ad9390b9166b`  
		Last Modified: Wed, 09 Jun 2021 20:19:37 GMT  
		Size: 11.9 MB (11906202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7361692fe34486902f2dd9f69cc3bce54c4cb8c5c86ed80a0d75033f25ae5213`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35d39d3918ab9262122b494a653aec25e76a65396f9198d7be955cb9c26c6f3`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66891a50a919af8d3cb83358a7f8d33b2055c143bd3499cc431fd32d053ed393`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519d446a1689a5424a77bf1cbf0f00153b28c6eff9ee22f0f88e0e32b3f6bda3`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534ea2eef93aa67b4ac4bfb48ac5498fa33b02d0b88b9ae60b8ae159addacecc`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19fc40bc9ade11a1755b185c529e961b474d959d45a44b1b1ab5f12e3d17863a`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ef9960b6bac284e65c351bc447bb8931486a0c1c3ee68c9e5a62828b4ae0e`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cfda8707421463aa0f297ce5d4ac3a615f60caf56e6e69a299caa08a04f7da`  
		Last Modified: Wed, 09 Jun 2021 20:19:29 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa0c9ece6e3482cf3ffc8d9a087d113db0f7c249f59bcf06f3ffc65c5e4bce0`  
		Last Modified: Wed, 09 Jun 2021 20:19:29 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6614223fb410a8262956f73a038f6d79b67d5976fe8740b21dfa2121a9cbd7f2`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f354857e070035731eb660ec35ff9f8549b6cc79211bab40ae642d9875f98f8b`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc94f29a4cb79013fce0bf1a5776868fa31912b598231e46883a114d86f712d3`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e536fde913e2e2d5ae24846adca32195330a9be6e7d1c3180ce7ac6bc6a35ae1`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b11db027637bf7abeec6bbcd83920c4eb7c291aeeae4d2886a1563bf41289a6`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3a70d973d27d739faae877290b3184bee11c706ebd4bfa515d180fba88ef0f`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc7b3e3d99424f8d3737a4502a6f50767ae25b699a315155b98700af682b64f`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 292.6 KB (292631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d435932a64bec158a6193fa4a31a1b38e446ec9f63c0b6be3282c3acf3288949`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:f07a9aef54a1c73076c58ba7037c8840b67601723e6dbf534878e515d02f519d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `caddy:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:e7e7af29e7917229552a0c802147dba99fb7a1427b84296a2c60ea7e19cbcb0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278267906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7184db699efd0a2ce0077179784cc7277e5faa7d07534ea1ce32d61d7f46ebc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 12:41:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:11:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Jun 2021 20:11:30 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:13:06 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Jun 2021 20:13:09 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Jun 2021 20:13:11 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Jun 2021 20:13:15 GMT
VOLUME [c:/config]
# Wed, 09 Jun 2021 20:13:18 GMT
VOLUME [c:/data]
# Wed, 09 Jun 2021 20:13:20 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 09 Jun 2021 20:13:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Jun 2021 20:13:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Jun 2021 20:13:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Jun 2021 20:13:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Jun 2021 20:13:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Jun 2021 20:13:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Jun 2021 20:13:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Jun 2021 20:13:40 GMT
EXPOSE 80
# Wed, 09 Jun 2021 20:13:42 GMT
EXPOSE 443
# Wed, 09 Jun 2021 20:13:45 GMT
EXPOSE 2019
# Wed, 09 Jun 2021 20:14:40 GMT
RUN caddy version
# Wed, 09 Jun 2021 20:14:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c82e82e95dbad4ccc260b42e03767eb07222e2f00ec57a69b3c87b17da1d2fd3`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a28e390d3b8e7b9369b102914eaee6e1fa0d14eb258b628be67f99f32f06f81`  
		Last Modified: Wed, 09 Jun 2021 20:20:01 GMT  
		Size: 357.4 KB (357370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7f07987f083e935103f83e47894b93aceaf05d1ded81dd09eb0bc3c8e45af`  
		Last Modified: Wed, 09 Jun 2021 20:20:01 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e65ddfdcdd60907208873b2a532cc58bc0f57d144430cef2c7630e80e4fd1e`  
		Last Modified: Wed, 09 Jun 2021 20:20:05 GMT  
		Size: 11.9 MB (11896985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58e4679b7ef7e1b9d82f44a6b5055c6916801193550bcce3ce390851224c736`  
		Last Modified: Wed, 09 Jun 2021 20:20:00 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107d803623512ea83de929509cc68f334261f2018c60bde60a99eadd0c2b179`  
		Last Modified: Wed, 09 Jun 2021 20:20:00 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f757538ddb020d145715a4890594958e741fe98366f1a58314361e5a8a3487`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462510ee9cb1c642e2804f8f607f02ccc5c31b63c956b9394bf38c5041b10d8b`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e87709f8365472aa7278651dacfc7eee93b24859a494cf6904b4f7ce80df0a`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5439b862b8218f1d7e0e0269efdbed614475ffbdcbaac06a3953f80b07677a1a`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1950c17917c025587fa23872145ee00eaaa11939dc87314c1aa74119db642d`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84164685053ad8b12a46e198ec2e93143d1df956bbbd4af76c88d0f549031c60`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103b7e93d2e2faefef7bd14bc00910442ce8da843f4fb726e2dba2d97752ddc9`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046d1e0cd75d46944ff833afe00c5dc9835ec1eb72876965a98a1488778910a6`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593a0ce075f6e5e07785dd7cd14aa1c274339da4d6f80495f0d1a85fabdef5db`  
		Last Modified: Wed, 09 Jun 2021 20:19:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14f5cdc43c91f65e6c5879691adc6e392d353807b27465a9b270fe7a06da51c`  
		Last Modified: Wed, 09 Jun 2021 20:19:55 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd488f5f58644d68e5103098932448a58d05a716861b26bf33376e75ad27e61`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c218cc3caa4b354c536ad99d30753a6eb41c52a58c52aafc0655a8482382a07`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3dad29a1e0241680f68697c2b0dbca8e85d0084faef4bdd3e66c8294be80671`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daeda652af05f03b2ec029aa5caa6b49d533546fa8347f5b1db003e8a83a7c30`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 260.8 KB (260840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9779c5588bf525e972d3b02ecaeeee32f3939ef8d54e8a16c52e0e62804e2e42`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0`

```console
$ docker pull caddy@sha256:48a10ed3e4c20797a6260e6fe5fc07d966b19b644101380b829f9306b713d424
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `caddy:2.3.0` - linux; amd64

```console
$ docker pull caddy@sha256:6fbf52298c46c55c572670b5395ecaee5d399338003c9bb4e4abed875c542f4f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14728953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7395cc3713b2ca5574a9b4aafc468a1533d16582efe47dcab74ed547540d698a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:10:47 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 14 Apr 2021 20:10:49 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 14 Apr 2021 20:10:49 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 14 Apr 2021 20:10:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 14 Apr 2021 20:10:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:10:53 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 14 Apr 2021 20:10:53 GMT
ENV XDG_DATA_HOME=/data
# Wed, 14 Apr 2021 20:10:53 GMT
VOLUME [/config]
# Wed, 14 Apr 2021 20:10:54 GMT
VOLUME [/data]
# Wed, 14 Apr 2021 20:10:54 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 14 Apr 2021 20:10:54 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Apr 2021 20:10:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Apr 2021 20:10:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Apr 2021 20:10:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Apr 2021 20:10:55 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Apr 2021 20:10:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Apr 2021 20:10:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Apr 2021 20:10:55 GMT
EXPOSE 80
# Wed, 14 Apr 2021 20:10:56 GMT
EXPOSE 443
# Wed, 14 Apr 2021 20:10:56 GMT
EXPOSE 2019
# Wed, 14 Apr 2021 20:10:56 GMT
WORKDIR /srv
# Wed, 14 Apr 2021 20:10:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7a0cd9cca5be9b30bbc70611052d1456502e1f338ce4b14946233b21cd6a9a`  
		Last Modified: Wed, 14 Apr 2021 20:11:46 GMT  
		Size: 300.0 KB (300016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5666523658a43fbbdff6b8fca498a988f4dcecc3ce027f1701414658c21d4ea`  
		Last Modified: Wed, 14 Apr 2021 20:11:46 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b097228407f13a161f68b188b0a4f255855b64d84e7b076745a744d5aa7ed8cf`  
		Last Modified: Wed, 14 Apr 2021 20:11:49 GMT  
		Size: 11.6 MB (11622383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40682d93cc09b4592a1b9c08d48d0a956b5eef4f123d80d1a12942482edb6aab`  
		Last Modified: Wed, 14 Apr 2021 20:11:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - linux; arm variant v6

```console
$ docker pull caddy@sha256:9bce30e38cfc52503c61076f36ffb5a114edfd0fccce6a14ca1d4a5b05fe0396
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13856198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:724dcdf3c72bd742f2159fc9b2c06ae63fdea026a3ea29ce6fd62be584970ab0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 17:34:00 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 May 2021 17:34:02 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 26 May 2021 17:34:02 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 26 May 2021 17:34:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 May 2021 17:34:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 May 2021 17:34:06 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 May 2021 17:34:06 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 May 2021 17:34:06 GMT
VOLUME [/config]
# Wed, 26 May 2021 17:34:06 GMT
VOLUME [/data]
# Wed, 26 May 2021 17:34:07 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 26 May 2021 17:34:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 May 2021 17:34:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 May 2021 17:34:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 May 2021 17:34:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 May 2021 17:34:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 May 2021 17:34:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 May 2021 17:34:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 May 2021 17:34:08 GMT
EXPOSE 80
# Wed, 26 May 2021 17:34:08 GMT
EXPOSE 443
# Wed, 26 May 2021 17:34:09 GMT
EXPOSE 2019
# Wed, 26 May 2021 17:34:09 GMT
WORKDIR /srv
# Wed, 26 May 2021 17:34:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66bf1e8e942074f0918055d1c8d4f5a37fc49f60d51d7dac8c99158b12f08c4`  
		Last Modified: Wed, 26 May 2021 17:35:48 GMT  
		Size: 300.1 KB (300124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728011a3ed68cd5a75f232f50e1795a6d970d61319a6bea12257efee2a8bfd8c`  
		Last Modified: Wed, 26 May 2021 17:35:48 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dacf38e2c4ebd5e9273dce56badd353c0a118e64e791cbe420684640a1ddf43`  
		Last Modified: Wed, 26 May 2021 17:35:51 GMT  
		Size: 10.9 MB (10944837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03cebcee786bfd2aeeb61bef69129c600f6a3f2e64e7a2f3947e6ca44d2d3dce`  
		Last Modified: Wed, 26 May 2021 17:35:48 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - linux; arm variant v7

```console
$ docker pull caddy@sha256:89f8b58c0d64c909b42b314e21f4f528fb26ad089fec1074351931df1275356d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13639720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b469699d596090e1892422cdf20a628940d2e2f648deccc309ac35a78ee90b05`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:50 GMT
ADD file:d844cc7b5e00fb62be39d903a2fb4a08f700e75112c8eef1f31101e846ed010d in / 
# Wed, 14 Apr 2021 18:57:52 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 10:59:00 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 May 2021 10:59:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 26 May 2021 10:59:01 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 26 May 2021 10:59:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 May 2021 10:59:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 May 2021 10:59:05 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 May 2021 10:59:05 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 May 2021 10:59:05 GMT
VOLUME [/config]
# Wed, 26 May 2021 10:59:05 GMT
VOLUME [/data]
# Wed, 26 May 2021 10:59:06 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 26 May 2021 10:59:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 May 2021 10:59:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 May 2021 10:59:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 May 2021 10:59:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 May 2021 10:59:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 May 2021 10:59:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 May 2021 10:59:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 May 2021 10:59:07 GMT
EXPOSE 80
# Wed, 26 May 2021 10:59:07 GMT
EXPOSE 443
# Wed, 26 May 2021 10:59:08 GMT
EXPOSE 2019
# Wed, 26 May 2021 10:59:08 GMT
WORKDIR /srv
# Wed, 26 May 2021 10:59:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:420c7481a3a76d5d12df768d2745ddbe40357df0af780c756a5a7d1f2a43d288`  
		Last Modified: Wed, 14 Apr 2021 18:58:46 GMT  
		Size: 2.4 MB (2409178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0027272d49af15ac9da258452a72131dcd85952f239e74d30e358b8005a8607f`  
		Last Modified: Wed, 26 May 2021 11:00:47 GMT  
		Size: 299.2 KB (299220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71820726ccd35446fc10d44070097f472327e9635d95fb0d177f8abfee34feb`  
		Last Modified: Wed, 26 May 2021 11:00:46 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9292ed2f8935f81e87fa79d852cf50391442db2bb9d03b2fd1864a31534f48ef`  
		Last Modified: Wed, 26 May 2021 11:00:49 GMT  
		Size: 10.9 MB (10925340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1658488c9f4af8634b62e103ebaaea5157a1160842f29aae2d356eb5bb8830`  
		Last Modified: Wed, 26 May 2021 11:00:46 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:93350eef41de8b474813be3ca07152dced05c0933bfac5a737c76793814bda09
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13615998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:361d35420e6c676e639a224453ed118b1289bd104e1c690ed159511809d6f0e4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 17:52:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 May 2021 17:52:21 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 26 May 2021 17:52:21 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 26 May 2021 17:52:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 May 2021 17:52:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 May 2021 17:52:24 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 May 2021 17:52:24 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 May 2021 17:52:24 GMT
VOLUME [/config]
# Wed, 26 May 2021 17:52:25 GMT
VOLUME [/data]
# Wed, 26 May 2021 17:52:25 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 26 May 2021 17:52:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 May 2021 17:52:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 May 2021 17:52:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 May 2021 17:52:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 May 2021 17:52:26 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 May 2021 17:52:26 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 May 2021 17:52:26 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 May 2021 17:52:26 GMT
EXPOSE 80
# Wed, 26 May 2021 17:52:27 GMT
EXPOSE 443
# Wed, 26 May 2021 17:52:27 GMT
EXPOSE 2019
# Wed, 26 May 2021 17:52:27 GMT
WORKDIR /srv
# Wed, 26 May 2021 17:52:27 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f34966f2b5bfb527f382b2cae307edda8f0d3f1bbef6b306bc4b51ee1e2e583`  
		Last Modified: Wed, 26 May 2021 17:53:38 GMT  
		Size: 300.3 KB (300334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ac5551bf8db11fbc1e883d20dd979eda8d251add9211302ecc3206cf314861`  
		Last Modified: Wed, 26 May 2021 17:53:38 GMT  
		Size: 5.8 KB (5836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00979462742e469d07bcfc93a948e429e5af5c907d8bde9bc300557c946b08ce`  
		Last Modified: Wed, 26 May 2021 17:53:40 GMT  
		Size: 10.6 MB (10598981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308da36143fee886a490420bfb231382978fc3c615e083345e0b56e835f14b07`  
		Last Modified: Wed, 26 May 2021 17:53:37 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - linux; ppc64le

```console
$ docker pull caddy@sha256:f551e1db7910e2d5235d303760aff5b514fc6e8b49d8d67d434bb23c40ac25db
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13356454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:982bd235f46e537404cdab42c3dfb3d0058f97ed5d7984f2e71ad8734adcc6a8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:09:04 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 14 Apr 2021 22:09:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 14 Apr 2021 22:09:24 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 14 Apr 2021 22:09:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 14 Apr 2021 22:09:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:09:56 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 14 Apr 2021 22:10:01 GMT
ENV XDG_DATA_HOME=/data
# Wed, 14 Apr 2021 22:10:06 GMT
VOLUME [/config]
# Wed, 14 Apr 2021 22:10:15 GMT
VOLUME [/data]
# Wed, 14 Apr 2021 22:10:22 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 14 Apr 2021 22:10:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Apr 2021 22:10:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Apr 2021 22:10:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Apr 2021 22:10:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Apr 2021 22:10:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Apr 2021 22:11:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Apr 2021 22:11:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Apr 2021 22:11:14 GMT
EXPOSE 80
# Wed, 14 Apr 2021 22:11:20 GMT
EXPOSE 443
# Wed, 14 Apr 2021 22:11:27 GMT
EXPOSE 2019
# Wed, 14 Apr 2021 22:11:35 GMT
WORKDIR /srv
# Wed, 14 Apr 2021 22:11:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d93dd31358a6e859a05bb506b946720f02c7ec7969776d811b20eaaa84508cd7`  
		Last Modified: Wed, 14 Apr 2021 22:15:41 GMT  
		Size: 302.3 KB (302339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8077b8c9cca163d9a34281a866cf5fe991ff8c160ebd1ab1b617c6b722ec690`  
		Last Modified: Wed, 14 Apr 2021 22:15:41 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55884816b8eca8150db9473989410e372c69c5431deb51a6cacd029895cf3dd6`  
		Last Modified: Wed, 14 Apr 2021 22:15:43 GMT  
		Size: 10.2 MB (10241380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51efee06e0a650ff5f146fc54a695d4bf2b44e19da18120fdc494982d52cdd62`  
		Last Modified: Wed, 14 Apr 2021 22:15:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - linux; s390x

```console
$ docker pull caddy@sha256:68aaf625a22bff4e71edf895129baa2d562765c24ac81a5c68aff2995ebf89c2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14146947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbfd454f0dfa64ee1a952f9ed74a3f3bda3688a9565f062c3ea37e48b54eb210`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:07:21 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 14 Apr 2021 20:07:22 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 14 Apr 2021 20:07:22 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 14 Apr 2021 20:07:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 14 Apr 2021 20:07:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:07:26 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 14 Apr 2021 20:07:27 GMT
ENV XDG_DATA_HOME=/data
# Wed, 14 Apr 2021 20:07:27 GMT
VOLUME [/config]
# Wed, 14 Apr 2021 20:07:27 GMT
VOLUME [/data]
# Wed, 14 Apr 2021 20:07:27 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 14 Apr 2021 20:07:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Apr 2021 20:07:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Apr 2021 20:07:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Apr 2021 20:07:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Apr 2021 20:07:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Apr 2021 20:07:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Apr 2021 20:07:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Apr 2021 20:07:29 GMT
EXPOSE 80
# Wed, 14 Apr 2021 20:07:29 GMT
EXPOSE 443
# Wed, 14 Apr 2021 20:07:29 GMT
EXPOSE 2019
# Wed, 14 Apr 2021 20:07:30 GMT
WORKDIR /srv
# Wed, 14 Apr 2021 20:07:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dab58470b754d248933aa56b48394e3ee4db4561d430d23ea378f0371ca59cb`  
		Last Modified: Wed, 14 Apr 2021 20:08:16 GMT  
		Size: 300.5 KB (300471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd514b608428ea44dae7dc67e641a276593e7715178d86d7702153521de849d7`  
		Last Modified: Wed, 14 Apr 2021 20:08:16 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a437814dab55b178c71f55598a70d0b532b3f645bdeb43e89244a6ebcde01446`  
		Last Modified: Wed, 14 Apr 2021 20:08:18 GMT  
		Size: 11.3 MB (11272061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412be9af105c69ee35fec76e8c0dbde8c8ba61c774b7d354e9c9fc8f538e8155`  
		Last Modified: Wed, 14 Apr 2021 20:08:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:abfb982cd83fb9b806ec5efc924058a088a526547c8994c5a38ffaf05cd1a2e4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2654306673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9adcb39b5c8fc517d2f7805d6b1b9aba540a058014b0636d515b0cc29c63fb7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 12:10:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 19:58:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Jun 2021 19:58:06 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 09 Jun 2021 19:58:45 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Jun 2021 19:58:47 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Jun 2021 19:58:49 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Jun 2021 19:58:52 GMT
VOLUME [c:/config]
# Wed, 09 Jun 2021 19:58:54 GMT
VOLUME [c:/data]
# Wed, 09 Jun 2021 19:58:57 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 09 Jun 2021 19:58:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Jun 2021 19:59:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Jun 2021 19:59:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Jun 2021 19:59:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Jun 2021 19:59:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Jun 2021 19:59:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Jun 2021 19:59:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Jun 2021 19:59:15 GMT
EXPOSE 80
# Wed, 09 Jun 2021 19:59:17 GMT
EXPOSE 443
# Wed, 09 Jun 2021 19:59:20 GMT
EXPOSE 2019
# Wed, 09 Jun 2021 19:59:41 GMT
RUN caddy version
# Wed, 09 Jun 2021 19:59:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7863ef96846d497ea06fe442ea13dcecaf5c248ce238c69800475281a4fa848e`  
		Last Modified: Wed, 09 Jun 2021 12:20:41 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7d9ebdfbbf3d1e8112e1cb391db31904536061de5256556e771e9969f203b0`  
		Last Modified: Wed, 09 Jun 2021 20:18:20 GMT  
		Size: 361.6 KB (361645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8897f927c230372062964e749dc71a1079d44309ded3bfaca335b559fe2e58`  
		Last Modified: Wed, 09 Jun 2021 20:18:19 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd2185358235294396b61f1daa54f4b588dae132c10145e26e1aa27403e3e57`  
		Last Modified: Wed, 09 Jun 2021 20:18:33 GMT  
		Size: 12.0 MB (12042056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c556a340c4eb84af59ae068dc4578b860ee79b4018d7266a2c47ef8c8552667`  
		Last Modified: Wed, 09 Jun 2021 20:18:19 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b6f691ea8f2966736d5e44aaeeb20e8f173b2a817f4e821f4f8130910c87b1`  
		Last Modified: Wed, 09 Jun 2021 20:18:18 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53652087525344ae336288573310ddb36a768d2c3b1c668536776ca777535ee`  
		Last Modified: Wed, 09 Jun 2021 20:18:17 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e7823b092ee21c368597d091df167f1ee6a0d457f8ce4cfbd1ca5f610f94d8`  
		Last Modified: Wed, 09 Jun 2021 20:18:16 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebc12b375fa0cebfe64352b7506467d6b3bc204dfe4b02bd50fe16832efcfb0`  
		Last Modified: Wed, 09 Jun 2021 20:18:16 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d7680a122b7c72ed29d1b997262311532fa6db08032bd46444d052e36180d8`  
		Last Modified: Wed, 09 Jun 2021 20:18:16 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6703c8f9c1144cfa310b45884ed415026ea0c81f8f45be2351681aa578cee675`  
		Last Modified: Wed, 09 Jun 2021 20:18:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7741bb8d10925c9dc4507da771fb2d6b0fb41d41999608c705667c82b2ed24a`  
		Last Modified: Wed, 09 Jun 2021 20:18:14 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52ab324f35848d4e4a9bb7a49ca222ae128927d3dae72baee1b3e8309c0c516`  
		Last Modified: Wed, 09 Jun 2021 20:18:13 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614f13023b6134592bf80f195a24148dbcd9c6d85ce74b0a6e01fd8ac21af258`  
		Last Modified: Wed, 09 Jun 2021 20:18:13 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec077e1f7b7042bcaac19c45da37857a07fad1bc03946731d8647e25c6894e0`  
		Last Modified: Wed, 09 Jun 2021 20:18:13 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cf69b06a4d52b3c8b6d2c62b7655fcc045a248904be961434d6486822c2cdf`  
		Last Modified: Wed, 09 Jun 2021 20:18:13 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f643524a9a79dcaa3ae3723d70eff0a06ac5278102c91270cc69dac606cbbd`  
		Last Modified: Wed, 09 Jun 2021 20:18:11 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734615d480107ad568078168de5289e7dacb0f451e185d6f28db22ffd9f6f38d`  
		Last Modified: Wed, 09 Jun 2021 20:18:10 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6e6c4e82d321ceb042388a4b32b9f8491a91e5060c2ad66b82c194e9ef2ba2`  
		Last Modified: Wed, 09 Jun 2021 20:18:11 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7c66662d27b64b2b1cb6c5b01c8f552366559fa3373e6d1d2c184fdc0378b3`  
		Last Modified: Wed, 09 Jun 2021 20:18:11 GMT  
		Size: 292.5 KB (292467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9442f528e1f1b1935332a277492e8f047fe6a0b2eef98d62cde1fe286d16fb`  
		Last Modified: Wed, 09 Jun 2021 20:18:11 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:36ebdab9cdd78892ba6e1c23096ead371830033af55ae4beff4a0f094f99bbb1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278410557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef0074d1abe6f6b4fc4f63ee29ba68462abe0043cf344dc84e4a1ff8100147d3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 12:41:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:01:17 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Jun 2021 20:01:19 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 09 Jun 2021 20:02:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Jun 2021 20:02:51 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Jun 2021 20:02:53 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Jun 2021 20:02:56 GMT
VOLUME [c:/config]
# Wed, 09 Jun 2021 20:02:58 GMT
VOLUME [c:/data]
# Wed, 09 Jun 2021 20:03:00 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 09 Jun 2021 20:03:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Jun 2021 20:03:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Jun 2021 20:03:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Jun 2021 20:03:11 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Jun 2021 20:03:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Jun 2021 20:03:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Jun 2021 20:03:19 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Jun 2021 20:03:22 GMT
EXPOSE 80
# Wed, 09 Jun 2021 20:03:24 GMT
EXPOSE 443
# Wed, 09 Jun 2021 20:03:27 GMT
EXPOSE 2019
# Wed, 09 Jun 2021 20:04:20 GMT
RUN caddy version
# Wed, 09 Jun 2021 20:04:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c82e82e95dbad4ccc260b42e03767eb07222e2f00ec57a69b3c87b17da1d2fd3`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7186c10d925bf51b7a0347cc44d9ccaaa700dd33c15bace64af437d839c08afc`  
		Last Modified: Wed, 09 Jun 2021 20:18:49 GMT  
		Size: 361.3 KB (361336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1a2b2e25a8e63c3ba5cf619d40f3daf10176d34ef1d5c6c74a617222e995bb`  
		Last Modified: Wed, 09 Jun 2021 20:18:49 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548bb9bdcebdb55c9c2a25ff1dd2962e5df2cee757f77d0b3c522d4f65983347`  
		Last Modified: Wed, 09 Jun 2021 20:18:52 GMT  
		Size: 12.0 MB (12034364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32ac36259028a1154879df59cb600b66fa7c5041ae6b274f385b96b28556bf1`  
		Last Modified: Wed, 09 Jun 2021 20:18:48 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1b36eb1530660082da73324bc94be1f00ba9b5d1e4be1d71199da3862a8a1c`  
		Last Modified: Wed, 09 Jun 2021 20:18:49 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8438aefe94f1d735ca92a8acfb9324000bf1f7fe4262886fa0b2df71d9e3c6bd`  
		Last Modified: Wed, 09 Jun 2021 20:18:46 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5bdad10cdbc7d78ee974dc7eec9a6345eb611f3a88ba9feed472596cc16454`  
		Last Modified: Wed, 09 Jun 2021 20:18:46 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3b6c63126e2060df917222ab905391a0f9fc0435f083aac9e843280d7afa7e`  
		Last Modified: Wed, 09 Jun 2021 20:18:46 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e412d17bbc625e61917a3fb903d8c775ddd693e84f4f6e6e1a53513f721ce4d8`  
		Last Modified: Wed, 09 Jun 2021 20:18:46 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cf08f45398baf12ebb8841e1c35678c167ce40ff7e83f9dd26a18ebd421ecc`  
		Last Modified: Wed, 09 Jun 2021 20:18:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570549f521be576d96b6d437a1a9004acaca2113f13ff43c879183db63e7eabd`  
		Last Modified: Wed, 09 Jun 2021 20:18:44 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d3ae1448bd25d3230e37d601c19abc7d1a2318b9ec037ffbd6d73927587b0a`  
		Last Modified: Wed, 09 Jun 2021 20:18:43 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944473f314aecab72089d844d05e1dd74b01454e2695396b5859dc9a6a9e07ea`  
		Last Modified: Wed, 09 Jun 2021 20:18:43 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a0802196eafa3eaeb45d12be27ffb7ce40038a96de352a11a5ffca06bcac50`  
		Last Modified: Wed, 09 Jun 2021 20:18:43 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:619af6b5ed093c9982004d31fd110fef2f317361602c32d65b453a6696db7808`  
		Last Modified: Wed, 09 Jun 2021 20:18:43 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79b4eac4f34750a41ea7faf4ee96b53b82bcf7e59cf8dac12c9dfc0d7606c7b`  
		Last Modified: Wed, 09 Jun 2021 20:18:41 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850ec4f3db9855738633574af9754a365fd845298867d1284d06ecd491ff6ea0`  
		Last Modified: Wed, 09 Jun 2021 20:18:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8dd45a07a5c2ce9a15b4a257361bd6508f013393bf9dc4bcc2f74cd1117ea13`  
		Last Modified: Wed, 09 Jun 2021 20:18:41 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cf05ec484a7aed9f1a8719d84b10aff6c29802fb4f68ddc16c0fde6495b93b`  
		Last Modified: Wed, 09 Jun 2021 20:18:41 GMT  
		Size: 262.0 KB (262013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4419e3710f83c624955a0392e5ffdfb1bda977c25ce5b407d4d6e9ca90396f`  
		Last Modified: Wed, 09 Jun 2021 20:18:41 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-alpine`

```console
$ docker pull caddy@sha256:efcc3a05635ff2c48f11d9497009d37c0ae939d471c27297e02fbd0b53e8befc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.3.0-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:6fbf52298c46c55c572670b5395ecaee5d399338003c9bb4e4abed875c542f4f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14728953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7395cc3713b2ca5574a9b4aafc468a1533d16582efe47dcab74ed547540d698a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:10:47 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 14 Apr 2021 20:10:49 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 14 Apr 2021 20:10:49 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 14 Apr 2021 20:10:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 14 Apr 2021 20:10:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:10:53 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 14 Apr 2021 20:10:53 GMT
ENV XDG_DATA_HOME=/data
# Wed, 14 Apr 2021 20:10:53 GMT
VOLUME [/config]
# Wed, 14 Apr 2021 20:10:54 GMT
VOLUME [/data]
# Wed, 14 Apr 2021 20:10:54 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 14 Apr 2021 20:10:54 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Apr 2021 20:10:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Apr 2021 20:10:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Apr 2021 20:10:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Apr 2021 20:10:55 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Apr 2021 20:10:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Apr 2021 20:10:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Apr 2021 20:10:55 GMT
EXPOSE 80
# Wed, 14 Apr 2021 20:10:56 GMT
EXPOSE 443
# Wed, 14 Apr 2021 20:10:56 GMT
EXPOSE 2019
# Wed, 14 Apr 2021 20:10:56 GMT
WORKDIR /srv
# Wed, 14 Apr 2021 20:10:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7a0cd9cca5be9b30bbc70611052d1456502e1f338ce4b14946233b21cd6a9a`  
		Last Modified: Wed, 14 Apr 2021 20:11:46 GMT  
		Size: 300.0 KB (300016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5666523658a43fbbdff6b8fca498a988f4dcecc3ce027f1701414658c21d4ea`  
		Last Modified: Wed, 14 Apr 2021 20:11:46 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b097228407f13a161f68b188b0a4f255855b64d84e7b076745a744d5aa7ed8cf`  
		Last Modified: Wed, 14 Apr 2021 20:11:49 GMT  
		Size: 11.6 MB (11622383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40682d93cc09b4592a1b9c08d48d0a956b5eef4f123d80d1a12942482edb6aab`  
		Last Modified: Wed, 14 Apr 2021 20:11:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:9bce30e38cfc52503c61076f36ffb5a114edfd0fccce6a14ca1d4a5b05fe0396
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13856198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:724dcdf3c72bd742f2159fc9b2c06ae63fdea026a3ea29ce6fd62be584970ab0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 17:34:00 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 May 2021 17:34:02 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 26 May 2021 17:34:02 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 26 May 2021 17:34:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 May 2021 17:34:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 May 2021 17:34:06 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 May 2021 17:34:06 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 May 2021 17:34:06 GMT
VOLUME [/config]
# Wed, 26 May 2021 17:34:06 GMT
VOLUME [/data]
# Wed, 26 May 2021 17:34:07 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 26 May 2021 17:34:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 May 2021 17:34:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 May 2021 17:34:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 May 2021 17:34:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 May 2021 17:34:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 May 2021 17:34:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 May 2021 17:34:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 May 2021 17:34:08 GMT
EXPOSE 80
# Wed, 26 May 2021 17:34:08 GMT
EXPOSE 443
# Wed, 26 May 2021 17:34:09 GMT
EXPOSE 2019
# Wed, 26 May 2021 17:34:09 GMT
WORKDIR /srv
# Wed, 26 May 2021 17:34:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66bf1e8e942074f0918055d1c8d4f5a37fc49f60d51d7dac8c99158b12f08c4`  
		Last Modified: Wed, 26 May 2021 17:35:48 GMT  
		Size: 300.1 KB (300124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728011a3ed68cd5a75f232f50e1795a6d970d61319a6bea12257efee2a8bfd8c`  
		Last Modified: Wed, 26 May 2021 17:35:48 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dacf38e2c4ebd5e9273dce56badd353c0a118e64e791cbe420684640a1ddf43`  
		Last Modified: Wed, 26 May 2021 17:35:51 GMT  
		Size: 10.9 MB (10944837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03cebcee786bfd2aeeb61bef69129c600f6a3f2e64e7a2f3947e6ca44d2d3dce`  
		Last Modified: Wed, 26 May 2021 17:35:48 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:89f8b58c0d64c909b42b314e21f4f528fb26ad089fec1074351931df1275356d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13639720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b469699d596090e1892422cdf20a628940d2e2f648deccc309ac35a78ee90b05`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:50 GMT
ADD file:d844cc7b5e00fb62be39d903a2fb4a08f700e75112c8eef1f31101e846ed010d in / 
# Wed, 14 Apr 2021 18:57:52 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 10:59:00 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 May 2021 10:59:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 26 May 2021 10:59:01 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 26 May 2021 10:59:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 May 2021 10:59:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 May 2021 10:59:05 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 May 2021 10:59:05 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 May 2021 10:59:05 GMT
VOLUME [/config]
# Wed, 26 May 2021 10:59:05 GMT
VOLUME [/data]
# Wed, 26 May 2021 10:59:06 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 26 May 2021 10:59:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 May 2021 10:59:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 May 2021 10:59:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 May 2021 10:59:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 May 2021 10:59:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 May 2021 10:59:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 May 2021 10:59:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 May 2021 10:59:07 GMT
EXPOSE 80
# Wed, 26 May 2021 10:59:07 GMT
EXPOSE 443
# Wed, 26 May 2021 10:59:08 GMT
EXPOSE 2019
# Wed, 26 May 2021 10:59:08 GMT
WORKDIR /srv
# Wed, 26 May 2021 10:59:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:420c7481a3a76d5d12df768d2745ddbe40357df0af780c756a5a7d1f2a43d288`  
		Last Modified: Wed, 14 Apr 2021 18:58:46 GMT  
		Size: 2.4 MB (2409178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0027272d49af15ac9da258452a72131dcd85952f239e74d30e358b8005a8607f`  
		Last Modified: Wed, 26 May 2021 11:00:47 GMT  
		Size: 299.2 KB (299220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71820726ccd35446fc10d44070097f472327e9635d95fb0d177f8abfee34feb`  
		Last Modified: Wed, 26 May 2021 11:00:46 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9292ed2f8935f81e87fa79d852cf50391442db2bb9d03b2fd1864a31534f48ef`  
		Last Modified: Wed, 26 May 2021 11:00:49 GMT  
		Size: 10.9 MB (10925340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1658488c9f4af8634b62e103ebaaea5157a1160842f29aae2d356eb5bb8830`  
		Last Modified: Wed, 26 May 2021 11:00:46 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:93350eef41de8b474813be3ca07152dced05c0933bfac5a737c76793814bda09
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13615998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:361d35420e6c676e639a224453ed118b1289bd104e1c690ed159511809d6f0e4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 17:52:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 May 2021 17:52:21 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 26 May 2021 17:52:21 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 26 May 2021 17:52:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 May 2021 17:52:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 May 2021 17:52:24 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 May 2021 17:52:24 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 May 2021 17:52:24 GMT
VOLUME [/config]
# Wed, 26 May 2021 17:52:25 GMT
VOLUME [/data]
# Wed, 26 May 2021 17:52:25 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 26 May 2021 17:52:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 May 2021 17:52:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 May 2021 17:52:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 May 2021 17:52:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 May 2021 17:52:26 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 May 2021 17:52:26 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 May 2021 17:52:26 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 May 2021 17:52:26 GMT
EXPOSE 80
# Wed, 26 May 2021 17:52:27 GMT
EXPOSE 443
# Wed, 26 May 2021 17:52:27 GMT
EXPOSE 2019
# Wed, 26 May 2021 17:52:27 GMT
WORKDIR /srv
# Wed, 26 May 2021 17:52:27 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f34966f2b5bfb527f382b2cae307edda8f0d3f1bbef6b306bc4b51ee1e2e583`  
		Last Modified: Wed, 26 May 2021 17:53:38 GMT  
		Size: 300.3 KB (300334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ac5551bf8db11fbc1e883d20dd979eda8d251add9211302ecc3206cf314861`  
		Last Modified: Wed, 26 May 2021 17:53:38 GMT  
		Size: 5.8 KB (5836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00979462742e469d07bcfc93a948e429e5af5c907d8bde9bc300557c946b08ce`  
		Last Modified: Wed, 26 May 2021 17:53:40 GMT  
		Size: 10.6 MB (10598981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308da36143fee886a490420bfb231382978fc3c615e083345e0b56e835f14b07`  
		Last Modified: Wed, 26 May 2021 17:53:37 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:f551e1db7910e2d5235d303760aff5b514fc6e8b49d8d67d434bb23c40ac25db
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13356454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:982bd235f46e537404cdab42c3dfb3d0058f97ed5d7984f2e71ad8734adcc6a8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:09:04 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 14 Apr 2021 22:09:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 14 Apr 2021 22:09:24 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 14 Apr 2021 22:09:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 14 Apr 2021 22:09:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:09:56 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 14 Apr 2021 22:10:01 GMT
ENV XDG_DATA_HOME=/data
# Wed, 14 Apr 2021 22:10:06 GMT
VOLUME [/config]
# Wed, 14 Apr 2021 22:10:15 GMT
VOLUME [/data]
# Wed, 14 Apr 2021 22:10:22 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 14 Apr 2021 22:10:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Apr 2021 22:10:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Apr 2021 22:10:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Apr 2021 22:10:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Apr 2021 22:10:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Apr 2021 22:11:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Apr 2021 22:11:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Apr 2021 22:11:14 GMT
EXPOSE 80
# Wed, 14 Apr 2021 22:11:20 GMT
EXPOSE 443
# Wed, 14 Apr 2021 22:11:27 GMT
EXPOSE 2019
# Wed, 14 Apr 2021 22:11:35 GMT
WORKDIR /srv
# Wed, 14 Apr 2021 22:11:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d93dd31358a6e859a05bb506b946720f02c7ec7969776d811b20eaaa84508cd7`  
		Last Modified: Wed, 14 Apr 2021 22:15:41 GMT  
		Size: 302.3 KB (302339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8077b8c9cca163d9a34281a866cf5fe991ff8c160ebd1ab1b617c6b722ec690`  
		Last Modified: Wed, 14 Apr 2021 22:15:41 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55884816b8eca8150db9473989410e372c69c5431deb51a6cacd029895cf3dd6`  
		Last Modified: Wed, 14 Apr 2021 22:15:43 GMT  
		Size: 10.2 MB (10241380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51efee06e0a650ff5f146fc54a695d4bf2b44e19da18120fdc494982d52cdd62`  
		Last Modified: Wed, 14 Apr 2021 22:15:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:68aaf625a22bff4e71edf895129baa2d562765c24ac81a5c68aff2995ebf89c2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14146947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbfd454f0dfa64ee1a952f9ed74a3f3bda3688a9565f062c3ea37e48b54eb210`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:07:21 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 14 Apr 2021 20:07:22 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 14 Apr 2021 20:07:22 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 14 Apr 2021 20:07:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 14 Apr 2021 20:07:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:07:26 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 14 Apr 2021 20:07:27 GMT
ENV XDG_DATA_HOME=/data
# Wed, 14 Apr 2021 20:07:27 GMT
VOLUME [/config]
# Wed, 14 Apr 2021 20:07:27 GMT
VOLUME [/data]
# Wed, 14 Apr 2021 20:07:27 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 14 Apr 2021 20:07:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Apr 2021 20:07:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Apr 2021 20:07:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Apr 2021 20:07:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Apr 2021 20:07:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Apr 2021 20:07:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Apr 2021 20:07:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Apr 2021 20:07:29 GMT
EXPOSE 80
# Wed, 14 Apr 2021 20:07:29 GMT
EXPOSE 443
# Wed, 14 Apr 2021 20:07:29 GMT
EXPOSE 2019
# Wed, 14 Apr 2021 20:07:30 GMT
WORKDIR /srv
# Wed, 14 Apr 2021 20:07:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dab58470b754d248933aa56b48394e3ee4db4561d430d23ea378f0371ca59cb`  
		Last Modified: Wed, 14 Apr 2021 20:08:16 GMT  
		Size: 300.5 KB (300471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd514b608428ea44dae7dc67e641a276593e7715178d86d7702153521de849d7`  
		Last Modified: Wed, 14 Apr 2021 20:08:16 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a437814dab55b178c71f55598a70d0b532b3f645bdeb43e89244a6ebcde01446`  
		Last Modified: Wed, 14 Apr 2021 20:08:18 GMT  
		Size: 11.3 MB (11272061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412be9af105c69ee35fec76e8c0dbde8c8ba61c774b7d354e9c9fc8f538e8155`  
		Last Modified: Wed, 14 Apr 2021 20:08:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder`

```console
$ docker pull caddy@sha256:f2e0674b5ff224796aa0b3c39f6216a1e4c906671cf01b04465846a99ccbc6fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `caddy:2.3.0-builder` - linux; amd64

```console
$ docker pull caddy@sha256:dab101574c292c0d5a14303c3ce32bae72eb8857c50b7e299b3530d344e6fed6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.6 MB (119568982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee8999d0d30aa3a7e51a63c8a14259957c2cab78a79cfab7ba724b086b0e5342`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:29:08 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 21:29:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 21:29:09 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:54:37 GMT
ENV GOLANG_VERSION=1.15.13
# Fri, 04 Jun 2021 01:57:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.13.src.tar.gz'; 	sha256='99069e7223479cce4553f84f874b9345f6f4045f27cf5089489b546da619a244'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 01:57:11 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 01:57:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:57:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 01:57:13 GMT
WORKDIR /go
# Fri, 04 Jun 2021 02:18:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 02:18:14 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 02:18:14 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 04 Jun 2021 02:18:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 02:18:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 02:18:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 02:18:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22b54d2d4342f88201f48db57cae1f7edbacae870ee13d7962f999edd7529a9`  
		Last Modified: Wed, 14 Apr 2021 21:35:49 GMT  
		Size: 280.9 KB (280879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5898d3d0f1f95fd666f764bf918c1656be6169868335cb63bc428a5ef47cf32`  
		Last Modified: Wed, 14 Apr 2021 21:35:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c99558b793b186fdd5d335e6642493bc781ec856990676f2aa1040aa8046e4`  
		Last Modified: Fri, 04 Jun 2021 02:02:37 GMT  
		Size: 106.8 MB (106843700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44852843fdfff71fde889e1298b44f2e751d2dad991e004b6c007bc5580e1c1`  
		Last Modified: Fri, 04 Jun 2021 02:02:21 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae07c7aa4b2dcad677739da03d767f61de42cb72ead8912eeb925f37a13b1193`  
		Last Modified: Fri, 04 Jun 2021 02:18:52 GMT  
		Size: 8.3 MB (8331955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0cad1e66e51a5d6782deb26c50ba2b3d134c67be71ef764b259bb4399350da`  
		Last Modified: Fri, 04 Jun 2021 02:18:51 GMT  
		Size: 1.3 MB (1311165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e95219338eb895044e0c7b46a36673ecfb6c7960f9d919b2bb8b5dc841df9c5`  
		Last Modified: Fri, 04 Jun 2021 02:18:50 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:139376881376df2fe2a3da6e16c17bdd48e36658cc1c6fbcfe4e0c967224a212
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114757182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4ee37aecc47e0516f1b490b09eab0796ee617588a5e20ff0852be69eebbb363`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Fri, 04 Jun 2021 05:33:14 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 04 Jun 2021 05:33:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 04 Jun 2021 05:33:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 05:38:27 GMT
ENV GOLANG_VERSION=1.15.13
# Fri, 04 Jun 2021 05:40:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.13.src.tar.gz'; 	sha256='99069e7223479cce4553f84f874b9345f6f4045f27cf5089489b546da619a244'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 05:40:34 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 05:40:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 05:40:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 05:40:35 GMT
WORKDIR /go
# Fri, 04 Jun 2021 07:34:41 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 07:34:41 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 07:34:41 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 04 Jun 2021 07:34:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 07:34:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 07:34:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 07:34:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0f71b059ed1f15e0cc291db3b05bcfb952a7022c5bfa0bf773b2f6983e398b`  
		Last Modified: Fri, 04 Jun 2021 05:42:59 GMT  
		Size: 281.0 KB (280983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87127e5e091b2d254a8912384687cbf5d69306db1707819e5f76b5e05dd9a1b4`  
		Last Modified: Fri, 04 Jun 2021 05:42:58 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e963d6e47b2151caafd1927d686104933962877494bcc22e3fb3249c477762a1`  
		Last Modified: Fri, 04 Jun 2021 05:44:53 GMT  
		Size: 102.7 MB (102699043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9d8b7cc7a1890bcfc729fd083d1daa52371cb91eed35a4e842f82644a711bd`  
		Last Modified: Fri, 04 Jun 2021 05:44:29 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9e4da3952cac7bb181c6b0c631042c1836b9f2be2b9b1272e90c6f23ff65c2`  
		Last Modified: Fri, 04 Jun 2021 07:36:03 GMT  
		Size: 7.9 MB (7949520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30879094b25ff7449882d81e6d800cc31a2fe2de7f8f2295519c5e4dec3e9ef5`  
		Last Modified: Fri, 04 Jun 2021 07:36:02 GMT  
		Size: 1.2 MB (1221669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22684bcb87ba66404655ff19b80727faaa37346a298de5d567f63efb0327213c`  
		Last Modified: Fri, 04 Jun 2021 07:36:01 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:5af5fe8420ba660cd383117d1acec755b1aad2c0a227f8c991a03a9594974d32
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113558218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:474422d99714149054f45e3107a2cac4a1b7cdef7daefd32d7bde19f2664c549`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:50 GMT
ADD file:d844cc7b5e00fb62be39d903a2fb4a08f700e75112c8eef1f31101e846ed010d in / 
# Wed, 14 Apr 2021 18:57:52 GMT
CMD ["/bin/sh"]
# Thu, 27 May 2021 15:09:03 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 27 May 2021 15:09:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 May 2021 15:09:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 08:01:55 GMT
ENV GOLANG_VERSION=1.15.13
# Fri, 04 Jun 2021 08:04:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.13.src.tar.gz'; 	sha256='99069e7223479cce4553f84f874b9345f6f4045f27cf5089489b546da619a244'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 08:04:11 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 08:04:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 08:04:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 08:04:12 GMT
WORKDIR /go
# Fri, 04 Jun 2021 12:06:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 12:06:39 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 12:06:39 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 04 Jun 2021 12:06:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 12:06:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 12:06:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 12:06:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:420c7481a3a76d5d12df768d2745ddbe40357df0af780c756a5a7d1f2a43d288`  
		Last Modified: Wed, 14 Apr 2021 18:58:46 GMT  
		Size: 2.4 MB (2409178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ab4a5418648c6773cb5cf767263feab5cf1fa07373a09a69f446dd7aaa539b`  
		Last Modified: Thu, 27 May 2021 15:20:37 GMT  
		Size: 280.1 KB (280079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6deabb5f1fcb454ad8c41d861ec0a41200d384f180ca61119f9fab681ed68250`  
		Last Modified: Thu, 27 May 2021 15:20:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2215ded1a734bfbdd3d5e4eaf3d0e3691e77b38b3057fd380864340445b8bf`  
		Last Modified: Fri, 04 Jun 2021 08:11:33 GMT  
		Size: 102.5 MB (102487784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ec40919aef15b57a662e569f74515e88b908bcfb4dfcdb17d91625c5290726`  
		Last Modified: Fri, 04 Jun 2021 08:11:12 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec5a7ea5b2c21a3e443898514bc524f3f23ab950ade795f1df31cf76fdd6b22`  
		Last Modified: Fri, 04 Jun 2021 12:08:00 GMT  
		Size: 7.2 MB (7160966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f19d42e06034ec74676218691e3db95aa7097eb72af1c0fe1a5c39e530b0851`  
		Last Modified: Fri, 04 Jun 2021 12:08:00 GMT  
		Size: 1.2 MB (1219497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872a6ef6240ce0d9dfa07531a4b5a7c002ac114311f0eab02483f885659cdce9`  
		Last Modified: Fri, 04 Jun 2021 12:07:59 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b7435ba85c2ee6e57c08831d747a35228c9e53a8d41da561a225e720b6cb47fd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.9 MB (114883293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cae71db43f70b8321c53c1501961405528d00efdd0bd4528b562f0d00637780a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Thu, 27 May 2021 22:19:09 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 27 May 2021 22:19:10 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 May 2021 22:19:10 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 04:05:25 GMT
ENV GOLANG_VERSION=1.15.13
# Fri, 04 Jun 2021 04:06:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.13.src.tar.gz'; 	sha256='99069e7223479cce4553f84f874b9345f6f4045f27cf5089489b546da619a244'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 04:06:41 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 04:06:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 04:06:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 04:06:42 GMT
WORKDIR /go
# Fri, 04 Jun 2021 07:44:21 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 07:44:21 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 07:44:21 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 04 Jun 2021 07:44:21 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 07:44:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 07:44:23 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 07:44:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26465e32a6e291788c9b2b4432f0af63dfdd04bca2e8ae847bde572f42a733e`  
		Last Modified: Thu, 27 May 2021 22:27:30 GMT  
		Size: 281.2 KB (281222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f49142a29a82917f9eaa023b07c8ff867cb284239fcf5a248503f7dbd3e9dc`  
		Last Modified: Thu, 27 May 2021 22:27:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c02e755f48b045d2d9ccf36f177cdc1ea3ca2d66545cf7399532c6d24914130`  
		Last Modified: Fri, 04 Jun 2021 04:12:27 GMT  
		Size: 102.2 MB (102163909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd0c443e99d28e248deea2844ce8931bded714c432b52006463aa81dc8678c9`  
		Last Modified: Fri, 04 Jun 2021 04:12:11 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2879229c89c929c6535fc7271571dfc9cb5a7b354d3a9558001d2902a59b4c37`  
		Last Modified: Fri, 04 Jun 2021 07:45:20 GMT  
		Size: 8.5 MB (8525213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0582c1d82b9024cb3014c9e2a9913f8730361484ef5a3bc76614a494ce409266`  
		Last Modified: Fri, 04 Jun 2021 07:45:19 GMT  
		Size: 1.2 MB (1201540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcecedb55f3f4e2eaad4d4cb69f285c2530d6e5f7565393b1a66382aed52255`  
		Last Modified: Fri, 04 Jun 2021 07:45:19 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:a13494cb32e9c1946f08c311cfc34e843d2a5e6ec9914c0f09fca6667f621f4f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (114044306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1202e79e8aed4d2f61956225ac808df484b1b18e200d9f35227417153904b82d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:57:05 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 22:57:14 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:57:16 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 03:16:08 GMT
ENV GOLANG_VERSION=1.15.13
# Fri, 04 Jun 2021 03:17:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.13.src.tar.gz'; 	sha256='99069e7223479cce4553f84f874b9345f6f4045f27cf5089489b546da619a244'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 03:17:59 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 03:18:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 03:18:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 03:18:18 GMT
WORKDIR /go
# Fri, 04 Jun 2021 09:15:08 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 09:15:13 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 09:15:17 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 04 Jun 2021 09:15:21 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 09:15:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 09:15:42 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 09:15:48 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9dca7bf08f7e7ef8f1c651b5ba53ba748e66f5a75400b38f67596867bfae4e2`  
		Last Modified: Wed, 14 Apr 2021 23:06:16 GMT  
		Size: 283.2 KB (283201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d495ca184c89fdc74ec1ec1cc670ff41be844b29174141c4602ac1400b0645`  
		Last Modified: Wed, 14 Apr 2021 23:06:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94361d968b03698b28db36d34acbfb4ff0167913d3b4f90425cf82efbafc0be0`  
		Last Modified: Fri, 04 Jun 2021 03:22:53 GMT  
		Size: 100.8 MB (100837387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99dbe45fcc235f0e65a2ef4455216291ab98ff390c8939346c3eaed17c4c3593`  
		Last Modified: Fri, 04 Jun 2021 03:22:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8559c83e92fcaeaf72f49b67bc868da2ae4ea20ec33c802cb0c8f7c4d0d248`  
		Last Modified: Fri, 04 Jun 2021 09:17:21 GMT  
		Size: 8.9 MB (8945743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5b75d2fee0a0feec48567db1bc22b7f21a5f82a11cda54c6d60333056cc10e`  
		Last Modified: Fri, 04 Jun 2021 09:17:19 GMT  
		Size: 1.2 MB (1170511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865517bf89f30406db0377785eea441afe7d5b59f4833b257819ce92a1e42033`  
		Last Modified: Fri, 04 Jun 2021 09:17:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; s390x

```console
$ docker pull caddy@sha256:a84536ef2787b6f223b60ca90d63c9f77bdf5e5c097ab1849cff15618bf30a2f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118462986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1442ae1cc6855fa1d225d092fb9dfac2623a9b6cf3d5c72d161dbd67a80ac4cc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:46:59 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:47:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:47:00 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:34:05 GMT
ENV GOLANG_VERSION=1.15.13
# Fri, 04 Jun 2021 01:35:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.13.src.tar.gz'; 	sha256='99069e7223479cce4553f84f874b9345f6f4045f27cf5089489b546da619a244'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 01:35:59 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 01:36:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:36:01 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 01:36:02 GMT
WORKDIR /go
# Fri, 04 Jun 2021 03:02:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 03:02:36 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 03:02:36 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 04 Jun 2021 03:02:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 03:02:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 03:02:40 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 03:02:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c29c45d0e43ef7a36e47dfc16916a076f7ba26b656842380c26207ad30f5c8b`  
		Last Modified: Wed, 14 Apr 2021 20:52:52 GMT  
		Size: 281.3 KB (281343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f1645d6cbfccd2924337f37dc819e7edc27989ead8bc679441954a0e483c24`  
		Last Modified: Wed, 14 Apr 2021 20:52:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53aee8604eb1ebe4c56ab2f95d15cb45f8a4c77eaa029d741e0e07ea915abc4`  
		Last Modified: Fri, 04 Jun 2021 01:38:46 GMT  
		Size: 106.0 MB (105974260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6263fcbd0a56cefc3ece1f23cfa8ff1282289b4f5d6a227fb6da67eaa138d149`  
		Last Modified: Fri, 04 Jun 2021 01:38:32 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67b4a845632dc7d71ea69a707e32ddc43979ac1f162bb3f2cc42caff6c44263`  
		Last Modified: Fri, 04 Jun 2021 03:03:30 GMT  
		Size: 8.4 MB (8373722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a9df4c1026221cf717ece5510b70a3052332c5d9752feb88d1ce930469afa9`  
		Last Modified: Fri, 04 Jun 2021 03:03:29 GMT  
		Size: 1.3 MB (1264520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd366a4f6c048395918a673e86dcfdf2d9dd40ff31135dea0dbb6f45dd09630f`  
		Last Modified: Fri, 04 Jun 2021 03:03:29 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:ff63dc4220acbee19d46f1f90c520215272ef626904177e8e3ab902f20d24166
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2803206746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21b3c0e5af19fe63d09f877bf0873c7d246d73f0976972cfbc101873ce7dcc12`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 12:10:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 12:37:22 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Jun 2021 12:37:25 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Jun 2021 12:37:29 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Jun 2021 12:37:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Jun 2021 12:38:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:38:25 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Jun 2021 12:38:51 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Jun 2021 12:53:05 GMT
ENV GOLANG_VERSION=1.15.13
# Wed, 09 Jun 2021 12:55:41 GMT
RUN $url = 'https://dl.google.com/go/go1.15.13.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'd1cf76a11bbd5158715a3e3b6b7f0c623f5472f7c0e654c858913b74b09e7e81'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:55:45 GMT
WORKDIR C:\gopath
# Wed, 09 Jun 2021 20:04:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:04:46 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 09 Jun 2021 20:04:48 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 09 Jun 2021 20:04:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Jun 2021 20:05:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Jun 2021 20:05:28 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7863ef96846d497ea06fe442ea13dcecaf5c248ce238c69800475281a4fa848e`  
		Last Modified: Wed, 09 Jun 2021 12:20:41 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f985a0b4390580a94aa3cbc8ecb01fc33805bb3304c4217dc5ec9fb6626011ca`  
		Last Modified: Wed, 09 Jun 2021 13:03:26 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5adf5cc2989b1cf730e7993bd088f778b31b33bac78f6d9c133226f7bcf4a6`  
		Last Modified: Wed, 09 Jun 2021 13:03:24 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480b981517ab26b6ee7e090e51d040995ac5a6a55410880ea3f0c8255dada3bc`  
		Last Modified: Wed, 09 Jun 2021 13:03:24 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a372a8dcfb8f1152565f4b8c928c202db247ddc21fd9a35838a2278c65ff6f`  
		Last Modified: Wed, 09 Jun 2021 13:03:23 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97090ffba94bc8afc85a54e404c8aca13253969fe01c8b0ac1f8ce3a0b909953`  
		Last Modified: Wed, 09 Jun 2021 13:03:53 GMT  
		Size: 25.4 MB (25445694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb1c026791860f230531a960e59a35d86f3ae617c5b6ad60155718694ed3720`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fca536252ace3ea8e08bcd38a313ad63d7d308f4a1d24734c324d191b65647`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 314.6 KB (314587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df4120010f40b960e19d8764ed02a2c890105b59db267006c2ee33b36ebd799`  
		Last Modified: Wed, 09 Jun 2021 13:06:07 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d6cfa07b19fb56bb08eb291e20f7d66b837a46601dd5ea63f6ed2b427aed8`  
		Last Modified: Wed, 09 Jun 2021 13:08:40 GMT  
		Size: 134.1 MB (134140046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9808910afde2fc505754150e5a7934f9c7d181da0b7d471269697a72a340f0`  
		Last Modified: Wed, 09 Jun 2021 13:06:06 GMT  
		Size: 1.6 KB (1571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03572753f10e009566b7c8d906b8f261b3dd7d8453d1ea0732cc5333eb31df8a`  
		Last Modified: Wed, 09 Jun 2021 20:19:03 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb91931265afabdffe4a61e87f2a4d7fd7bd14eac6eb2f94afd65a926c2d20d`  
		Last Modified: Wed, 09 Jun 2021 20:19:00 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b248330835a77d664e76e0592db9df4e6973e2a874095e9d691d1a4c0945b74f`  
		Last Modified: Wed, 09 Jun 2021 20:19:00 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206fab654f0a9901f88fd5484a15829b0a8110eeca91ce298545782a5e4d162f`  
		Last Modified: Wed, 09 Jun 2021 20:19:00 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8408058ce0608cb19abc856081e565fe4efed434eef85087476e216af95a9a92`  
		Last Modified: Wed, 09 Jun 2021 20:19:01 GMT  
		Size: 1.7 MB (1703393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01fa1130849879916d58b2f96e9054df0a56422f138b0323a1de772c5896421`  
		Last Modified: Wed, 09 Jun 2021 20:19:00 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:c8115755d722963e20128d1dc1005ed730f2d565f341347cdc210b98a9f9406c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6431784335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cc7e9dfce803d295ef74ddcfdb048cf4b0c534e21f6fae7a1136e474470534e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 12:41:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 12:41:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Jun 2021 12:41:43 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Jun 2021 12:41:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Jun 2021 12:41:49 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Jun 2021 12:44:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:44:27 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Jun 2021 12:45:49 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Jun 2021 12:56:02 GMT
ENV GOLANG_VERSION=1.15.13
# Wed, 09 Jun 2021 12:59:45 GMT
RUN $url = 'https://dl.google.com/go/go1.15.13.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'd1cf76a11bbd5158715a3e3b6b7f0c623f5472f7c0e654c858913b74b09e7e81'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:59:49 GMT
WORKDIR C:\gopath
# Wed, 09 Jun 2021 20:05:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:05:38 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 09 Jun 2021 20:05:42 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 09 Jun 2021 20:05:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Jun 2021 20:07:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Jun 2021 20:07:23 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c82e82e95dbad4ccc260b42e03767eb07222e2f00ec57a69b3c87b17da1d2fd3`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a881968e28f8c2900b00800a0de406d0e98740558d9564ad738d053e63d9a1e`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab71df915cf7ac4c559039a917269e11faab2d0e6862a01408431df7fb40362f`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82ce560dcbc3235ed87d6c938aa761616dbd299188ae53a51a266eb37f381f6`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bee5ea2f89fe3f3e514b8dfcd823da340447b633c6048e00773d1c30fbbc0e9`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad71deb840b73610184070ebc7c566bd1dac9cc309d53679460697243bab7640`  
		Last Modified: Wed, 09 Jun 2021 13:04:50 GMT  
		Size: 25.4 MB (25441204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16f2a89ed7a230471eb96b67829deb255795564010b0ff2de47179cdfdec1d0`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cc755175ec255452c16e1e41cc78a8cd719d65f70221e7d128c1dc18eec8f2`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 307.7 KB (307689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cb64eb99938376ba010bc236c996c172af200b15dce04ab461c156248269b7`  
		Last Modified: Wed, 09 Jun 2021 13:08:50 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f13f4dbf7582b2566a28473ffdc0850d8cd490cfb0d5e13568bc3d104aa1b9c`  
		Last Modified: Wed, 09 Jun 2021 13:11:32 GMT  
		Size: 138.6 MB (138598442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e2567bd998dd047ec27020dd4b6cc678d9f5e5c4c30ba2aeb4bbed135c6507`  
		Last Modified: Wed, 09 Jun 2021 13:08:50 GMT  
		Size: 1.6 KB (1574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd54a3680618246bc4f7a44ac005d9f63292e795ccdcf18cad2265cfa6eb2aa8`  
		Last Modified: Wed, 09 Jun 2021 20:19:16 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0003b3b81fea490ce3d717180fb612decca6b6c5e8924bc88cf3ba681e3858`  
		Last Modified: Wed, 09 Jun 2021 20:19:13 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4888eaf97833d4a8959b4c814e970d541992014645e85fe0f20f34ceb58f27ed`  
		Last Modified: Wed, 09 Jun 2021 20:19:13 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce0cc57747c2565c9825fc51e64e37b374745c15a1ce914f5a24eb25eff252d`  
		Last Modified: Wed, 09 Jun 2021 20:19:13 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def326ce00fc8a710eb36bffbf156cd48ba97585363cb5cf0df0693211058690`  
		Last Modified: Wed, 09 Jun 2021 20:19:16 GMT  
		Size: 1.7 MB (1691133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740e3a80e946b7578215b57f455cdd284a951e5970e8423b1dc5d2bb21241258`  
		Last Modified: Wed, 09 Jun 2021 20:19:13 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder-alpine`

```console
$ docker pull caddy@sha256:8bc9fa7153dcb813a5683403971ee57fc991f4109bdf420225929ecaf512a062
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.3.0-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:dab101574c292c0d5a14303c3ce32bae72eb8857c50b7e299b3530d344e6fed6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.6 MB (119568982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee8999d0d30aa3a7e51a63c8a14259957c2cab78a79cfab7ba724b086b0e5342`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:29:08 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 21:29:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 21:29:09 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:54:37 GMT
ENV GOLANG_VERSION=1.15.13
# Fri, 04 Jun 2021 01:57:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.13.src.tar.gz'; 	sha256='99069e7223479cce4553f84f874b9345f6f4045f27cf5089489b546da619a244'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 01:57:11 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 01:57:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:57:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 01:57:13 GMT
WORKDIR /go
# Fri, 04 Jun 2021 02:18:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 02:18:14 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 02:18:14 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 04 Jun 2021 02:18:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 02:18:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 02:18:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 02:18:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22b54d2d4342f88201f48db57cae1f7edbacae870ee13d7962f999edd7529a9`  
		Last Modified: Wed, 14 Apr 2021 21:35:49 GMT  
		Size: 280.9 KB (280879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5898d3d0f1f95fd666f764bf918c1656be6169868335cb63bc428a5ef47cf32`  
		Last Modified: Wed, 14 Apr 2021 21:35:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c99558b793b186fdd5d335e6642493bc781ec856990676f2aa1040aa8046e4`  
		Last Modified: Fri, 04 Jun 2021 02:02:37 GMT  
		Size: 106.8 MB (106843700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44852843fdfff71fde889e1298b44f2e751d2dad991e004b6c007bc5580e1c1`  
		Last Modified: Fri, 04 Jun 2021 02:02:21 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae07c7aa4b2dcad677739da03d767f61de42cb72ead8912eeb925f37a13b1193`  
		Last Modified: Fri, 04 Jun 2021 02:18:52 GMT  
		Size: 8.3 MB (8331955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0cad1e66e51a5d6782deb26c50ba2b3d134c67be71ef764b259bb4399350da`  
		Last Modified: Fri, 04 Jun 2021 02:18:51 GMT  
		Size: 1.3 MB (1311165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e95219338eb895044e0c7b46a36673ecfb6c7960f9d919b2bb8b5dc841df9c5`  
		Last Modified: Fri, 04 Jun 2021 02:18:50 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:139376881376df2fe2a3da6e16c17bdd48e36658cc1c6fbcfe4e0c967224a212
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114757182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4ee37aecc47e0516f1b490b09eab0796ee617588a5e20ff0852be69eebbb363`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Fri, 04 Jun 2021 05:33:14 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 04 Jun 2021 05:33:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 04 Jun 2021 05:33:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 05:38:27 GMT
ENV GOLANG_VERSION=1.15.13
# Fri, 04 Jun 2021 05:40:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.13.src.tar.gz'; 	sha256='99069e7223479cce4553f84f874b9345f6f4045f27cf5089489b546da619a244'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 05:40:34 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 05:40:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 05:40:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 05:40:35 GMT
WORKDIR /go
# Fri, 04 Jun 2021 07:34:41 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 07:34:41 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 07:34:41 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 04 Jun 2021 07:34:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 07:34:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 07:34:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 07:34:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0f71b059ed1f15e0cc291db3b05bcfb952a7022c5bfa0bf773b2f6983e398b`  
		Last Modified: Fri, 04 Jun 2021 05:42:59 GMT  
		Size: 281.0 KB (280983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87127e5e091b2d254a8912384687cbf5d69306db1707819e5f76b5e05dd9a1b4`  
		Last Modified: Fri, 04 Jun 2021 05:42:58 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e963d6e47b2151caafd1927d686104933962877494bcc22e3fb3249c477762a1`  
		Last Modified: Fri, 04 Jun 2021 05:44:53 GMT  
		Size: 102.7 MB (102699043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9d8b7cc7a1890bcfc729fd083d1daa52371cb91eed35a4e842f82644a711bd`  
		Last Modified: Fri, 04 Jun 2021 05:44:29 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9e4da3952cac7bb181c6b0c631042c1836b9f2be2b9b1272e90c6f23ff65c2`  
		Last Modified: Fri, 04 Jun 2021 07:36:03 GMT  
		Size: 7.9 MB (7949520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30879094b25ff7449882d81e6d800cc31a2fe2de7f8f2295519c5e4dec3e9ef5`  
		Last Modified: Fri, 04 Jun 2021 07:36:02 GMT  
		Size: 1.2 MB (1221669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22684bcb87ba66404655ff19b80727faaa37346a298de5d567f63efb0327213c`  
		Last Modified: Fri, 04 Jun 2021 07:36:01 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:5af5fe8420ba660cd383117d1acec755b1aad2c0a227f8c991a03a9594974d32
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113558218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:474422d99714149054f45e3107a2cac4a1b7cdef7daefd32d7bde19f2664c549`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:50 GMT
ADD file:d844cc7b5e00fb62be39d903a2fb4a08f700e75112c8eef1f31101e846ed010d in / 
# Wed, 14 Apr 2021 18:57:52 GMT
CMD ["/bin/sh"]
# Thu, 27 May 2021 15:09:03 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 27 May 2021 15:09:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 May 2021 15:09:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 08:01:55 GMT
ENV GOLANG_VERSION=1.15.13
# Fri, 04 Jun 2021 08:04:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.13.src.tar.gz'; 	sha256='99069e7223479cce4553f84f874b9345f6f4045f27cf5089489b546da619a244'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 08:04:11 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 08:04:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 08:04:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 08:04:12 GMT
WORKDIR /go
# Fri, 04 Jun 2021 12:06:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 12:06:39 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 12:06:39 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 04 Jun 2021 12:06:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 12:06:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 12:06:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 12:06:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:420c7481a3a76d5d12df768d2745ddbe40357df0af780c756a5a7d1f2a43d288`  
		Last Modified: Wed, 14 Apr 2021 18:58:46 GMT  
		Size: 2.4 MB (2409178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ab4a5418648c6773cb5cf767263feab5cf1fa07373a09a69f446dd7aaa539b`  
		Last Modified: Thu, 27 May 2021 15:20:37 GMT  
		Size: 280.1 KB (280079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6deabb5f1fcb454ad8c41d861ec0a41200d384f180ca61119f9fab681ed68250`  
		Last Modified: Thu, 27 May 2021 15:20:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2215ded1a734bfbdd3d5e4eaf3d0e3691e77b38b3057fd380864340445b8bf`  
		Last Modified: Fri, 04 Jun 2021 08:11:33 GMT  
		Size: 102.5 MB (102487784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ec40919aef15b57a662e569f74515e88b908bcfb4dfcdb17d91625c5290726`  
		Last Modified: Fri, 04 Jun 2021 08:11:12 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec5a7ea5b2c21a3e443898514bc524f3f23ab950ade795f1df31cf76fdd6b22`  
		Last Modified: Fri, 04 Jun 2021 12:08:00 GMT  
		Size: 7.2 MB (7160966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f19d42e06034ec74676218691e3db95aa7097eb72af1c0fe1a5c39e530b0851`  
		Last Modified: Fri, 04 Jun 2021 12:08:00 GMT  
		Size: 1.2 MB (1219497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872a6ef6240ce0d9dfa07531a4b5a7c002ac114311f0eab02483f885659cdce9`  
		Last Modified: Fri, 04 Jun 2021 12:07:59 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b7435ba85c2ee6e57c08831d747a35228c9e53a8d41da561a225e720b6cb47fd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.9 MB (114883293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cae71db43f70b8321c53c1501961405528d00efdd0bd4528b562f0d00637780a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Thu, 27 May 2021 22:19:09 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 27 May 2021 22:19:10 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 May 2021 22:19:10 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 04:05:25 GMT
ENV GOLANG_VERSION=1.15.13
# Fri, 04 Jun 2021 04:06:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.13.src.tar.gz'; 	sha256='99069e7223479cce4553f84f874b9345f6f4045f27cf5089489b546da619a244'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 04:06:41 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 04:06:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 04:06:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 04:06:42 GMT
WORKDIR /go
# Fri, 04 Jun 2021 07:44:21 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 07:44:21 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 07:44:21 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 04 Jun 2021 07:44:21 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 07:44:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 07:44:23 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 07:44:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26465e32a6e291788c9b2b4432f0af63dfdd04bca2e8ae847bde572f42a733e`  
		Last Modified: Thu, 27 May 2021 22:27:30 GMT  
		Size: 281.2 KB (281222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f49142a29a82917f9eaa023b07c8ff867cb284239fcf5a248503f7dbd3e9dc`  
		Last Modified: Thu, 27 May 2021 22:27:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c02e755f48b045d2d9ccf36f177cdc1ea3ca2d66545cf7399532c6d24914130`  
		Last Modified: Fri, 04 Jun 2021 04:12:27 GMT  
		Size: 102.2 MB (102163909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd0c443e99d28e248deea2844ce8931bded714c432b52006463aa81dc8678c9`  
		Last Modified: Fri, 04 Jun 2021 04:12:11 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2879229c89c929c6535fc7271571dfc9cb5a7b354d3a9558001d2902a59b4c37`  
		Last Modified: Fri, 04 Jun 2021 07:45:20 GMT  
		Size: 8.5 MB (8525213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0582c1d82b9024cb3014c9e2a9913f8730361484ef5a3bc76614a494ce409266`  
		Last Modified: Fri, 04 Jun 2021 07:45:19 GMT  
		Size: 1.2 MB (1201540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcecedb55f3f4e2eaad4d4cb69f285c2530d6e5f7565393b1a66382aed52255`  
		Last Modified: Fri, 04 Jun 2021 07:45:19 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:a13494cb32e9c1946f08c311cfc34e843d2a5e6ec9914c0f09fca6667f621f4f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (114044306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1202e79e8aed4d2f61956225ac808df484b1b18e200d9f35227417153904b82d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:57:05 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 22:57:14 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:57:16 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 03:16:08 GMT
ENV GOLANG_VERSION=1.15.13
# Fri, 04 Jun 2021 03:17:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.13.src.tar.gz'; 	sha256='99069e7223479cce4553f84f874b9345f6f4045f27cf5089489b546da619a244'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 03:17:59 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 03:18:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 03:18:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 03:18:18 GMT
WORKDIR /go
# Fri, 04 Jun 2021 09:15:08 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 09:15:13 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 09:15:17 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 04 Jun 2021 09:15:21 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 09:15:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 09:15:42 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 09:15:48 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9dca7bf08f7e7ef8f1c651b5ba53ba748e66f5a75400b38f67596867bfae4e2`  
		Last Modified: Wed, 14 Apr 2021 23:06:16 GMT  
		Size: 283.2 KB (283201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d495ca184c89fdc74ec1ec1cc670ff41be844b29174141c4602ac1400b0645`  
		Last Modified: Wed, 14 Apr 2021 23:06:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94361d968b03698b28db36d34acbfb4ff0167913d3b4f90425cf82efbafc0be0`  
		Last Modified: Fri, 04 Jun 2021 03:22:53 GMT  
		Size: 100.8 MB (100837387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99dbe45fcc235f0e65a2ef4455216291ab98ff390c8939346c3eaed17c4c3593`  
		Last Modified: Fri, 04 Jun 2021 03:22:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8559c83e92fcaeaf72f49b67bc868da2ae4ea20ec33c802cb0c8f7c4d0d248`  
		Last Modified: Fri, 04 Jun 2021 09:17:21 GMT  
		Size: 8.9 MB (8945743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5b75d2fee0a0feec48567db1bc22b7f21a5f82a11cda54c6d60333056cc10e`  
		Last Modified: Fri, 04 Jun 2021 09:17:19 GMT  
		Size: 1.2 MB (1170511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865517bf89f30406db0377785eea441afe7d5b59f4833b257819ce92a1e42033`  
		Last Modified: Fri, 04 Jun 2021 09:17:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:a84536ef2787b6f223b60ca90d63c9f77bdf5e5c097ab1849cff15618bf30a2f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118462986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1442ae1cc6855fa1d225d092fb9dfac2623a9b6cf3d5c72d161dbd67a80ac4cc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:46:59 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:47:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:47:00 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:34:05 GMT
ENV GOLANG_VERSION=1.15.13
# Fri, 04 Jun 2021 01:35:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.13.src.tar.gz'; 	sha256='99069e7223479cce4553f84f874b9345f6f4045f27cf5089489b546da619a244'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 01:35:59 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 01:36:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:36:01 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 01:36:02 GMT
WORKDIR /go
# Fri, 04 Jun 2021 03:02:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 03:02:36 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 03:02:36 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 04 Jun 2021 03:02:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 03:02:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 03:02:40 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 03:02:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c29c45d0e43ef7a36e47dfc16916a076f7ba26b656842380c26207ad30f5c8b`  
		Last Modified: Wed, 14 Apr 2021 20:52:52 GMT  
		Size: 281.3 KB (281343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f1645d6cbfccd2924337f37dc819e7edc27989ead8bc679441954a0e483c24`  
		Last Modified: Wed, 14 Apr 2021 20:52:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53aee8604eb1ebe4c56ab2f95d15cb45f8a4c77eaa029d741e0e07ea915abc4`  
		Last Modified: Fri, 04 Jun 2021 01:38:46 GMT  
		Size: 106.0 MB (105974260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6263fcbd0a56cefc3ece1f23cfa8ff1282289b4f5d6a227fb6da67eaa138d149`  
		Last Modified: Fri, 04 Jun 2021 01:38:32 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67b4a845632dc7d71ea69a707e32ddc43979ac1f162bb3f2cc42caff6c44263`  
		Last Modified: Fri, 04 Jun 2021 03:03:30 GMT  
		Size: 8.4 MB (8373722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a9df4c1026221cf717ece5510b70a3052332c5d9752feb88d1ce930469afa9`  
		Last Modified: Fri, 04 Jun 2021 03:03:29 GMT  
		Size: 1.3 MB (1264520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd366a4f6c048395918a673e86dcfdf2d9dd40ff31135dea0dbb6f45dd09630f`  
		Last Modified: Fri, 04 Jun 2021 03:03:29 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:e2bf592f6ca97b63bdc20d11a4f7bcb7d32af5607e79f5efe625351446c6bc06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `caddy:2.3.0-builder-windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:ff63dc4220acbee19d46f1f90c520215272ef626904177e8e3ab902f20d24166
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2803206746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21b3c0e5af19fe63d09f877bf0873c7d246d73f0976972cfbc101873ce7dcc12`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 12:10:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 12:37:22 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Jun 2021 12:37:25 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Jun 2021 12:37:29 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Jun 2021 12:37:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Jun 2021 12:38:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:38:25 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Jun 2021 12:38:51 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Jun 2021 12:53:05 GMT
ENV GOLANG_VERSION=1.15.13
# Wed, 09 Jun 2021 12:55:41 GMT
RUN $url = 'https://dl.google.com/go/go1.15.13.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'd1cf76a11bbd5158715a3e3b6b7f0c623f5472f7c0e654c858913b74b09e7e81'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:55:45 GMT
WORKDIR C:\gopath
# Wed, 09 Jun 2021 20:04:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:04:46 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 09 Jun 2021 20:04:48 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 09 Jun 2021 20:04:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Jun 2021 20:05:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Jun 2021 20:05:28 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7863ef96846d497ea06fe442ea13dcecaf5c248ce238c69800475281a4fa848e`  
		Last Modified: Wed, 09 Jun 2021 12:20:41 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f985a0b4390580a94aa3cbc8ecb01fc33805bb3304c4217dc5ec9fb6626011ca`  
		Last Modified: Wed, 09 Jun 2021 13:03:26 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5adf5cc2989b1cf730e7993bd088f778b31b33bac78f6d9c133226f7bcf4a6`  
		Last Modified: Wed, 09 Jun 2021 13:03:24 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480b981517ab26b6ee7e090e51d040995ac5a6a55410880ea3f0c8255dada3bc`  
		Last Modified: Wed, 09 Jun 2021 13:03:24 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a372a8dcfb8f1152565f4b8c928c202db247ddc21fd9a35838a2278c65ff6f`  
		Last Modified: Wed, 09 Jun 2021 13:03:23 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97090ffba94bc8afc85a54e404c8aca13253969fe01c8b0ac1f8ce3a0b909953`  
		Last Modified: Wed, 09 Jun 2021 13:03:53 GMT  
		Size: 25.4 MB (25445694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb1c026791860f230531a960e59a35d86f3ae617c5b6ad60155718694ed3720`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fca536252ace3ea8e08bcd38a313ad63d7d308f4a1d24734c324d191b65647`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 314.6 KB (314587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df4120010f40b960e19d8764ed02a2c890105b59db267006c2ee33b36ebd799`  
		Last Modified: Wed, 09 Jun 2021 13:06:07 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d6cfa07b19fb56bb08eb291e20f7d66b837a46601dd5ea63f6ed2b427aed8`  
		Last Modified: Wed, 09 Jun 2021 13:08:40 GMT  
		Size: 134.1 MB (134140046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9808910afde2fc505754150e5a7934f9c7d181da0b7d471269697a72a340f0`  
		Last Modified: Wed, 09 Jun 2021 13:06:06 GMT  
		Size: 1.6 KB (1571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03572753f10e009566b7c8d906b8f261b3dd7d8453d1ea0732cc5333eb31df8a`  
		Last Modified: Wed, 09 Jun 2021 20:19:03 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb91931265afabdffe4a61e87f2a4d7fd7bd14eac6eb2f94afd65a926c2d20d`  
		Last Modified: Wed, 09 Jun 2021 20:19:00 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b248330835a77d664e76e0592db9df4e6973e2a874095e9d691d1a4c0945b74f`  
		Last Modified: Wed, 09 Jun 2021 20:19:00 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206fab654f0a9901f88fd5484a15829b0a8110eeca91ce298545782a5e4d162f`  
		Last Modified: Wed, 09 Jun 2021 20:19:00 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8408058ce0608cb19abc856081e565fe4efed434eef85087476e216af95a9a92`  
		Last Modified: Wed, 09 Jun 2021 20:19:01 GMT  
		Size: 1.7 MB (1703393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01fa1130849879916d58b2f96e9054df0a56422f138b0323a1de772c5896421`  
		Last Modified: Wed, 09 Jun 2021 20:19:00 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:edbe9afe8273b506e1b71574f39698c9e176279bfa6081812e1e26ed1cc7107a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `caddy:2.3.0-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:c8115755d722963e20128d1dc1005ed730f2d565f341347cdc210b98a9f9406c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6431784335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cc7e9dfce803d295ef74ddcfdb048cf4b0c534e21f6fae7a1136e474470534e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 12:41:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 12:41:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Jun 2021 12:41:43 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Jun 2021 12:41:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Jun 2021 12:41:49 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Jun 2021 12:44:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:44:27 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Jun 2021 12:45:49 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Jun 2021 12:56:02 GMT
ENV GOLANG_VERSION=1.15.13
# Wed, 09 Jun 2021 12:59:45 GMT
RUN $url = 'https://dl.google.com/go/go1.15.13.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'd1cf76a11bbd5158715a3e3b6b7f0c623f5472f7c0e654c858913b74b09e7e81'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:59:49 GMT
WORKDIR C:\gopath
# Wed, 09 Jun 2021 20:05:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:05:38 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 09 Jun 2021 20:05:42 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 09 Jun 2021 20:05:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Jun 2021 20:07:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Jun 2021 20:07:23 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c82e82e95dbad4ccc260b42e03767eb07222e2f00ec57a69b3c87b17da1d2fd3`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a881968e28f8c2900b00800a0de406d0e98740558d9564ad738d053e63d9a1e`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab71df915cf7ac4c559039a917269e11faab2d0e6862a01408431df7fb40362f`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82ce560dcbc3235ed87d6c938aa761616dbd299188ae53a51a266eb37f381f6`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bee5ea2f89fe3f3e514b8dfcd823da340447b633c6048e00773d1c30fbbc0e9`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad71deb840b73610184070ebc7c566bd1dac9cc309d53679460697243bab7640`  
		Last Modified: Wed, 09 Jun 2021 13:04:50 GMT  
		Size: 25.4 MB (25441204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16f2a89ed7a230471eb96b67829deb255795564010b0ff2de47179cdfdec1d0`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cc755175ec255452c16e1e41cc78a8cd719d65f70221e7d128c1dc18eec8f2`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 307.7 KB (307689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cb64eb99938376ba010bc236c996c172af200b15dce04ab461c156248269b7`  
		Last Modified: Wed, 09 Jun 2021 13:08:50 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f13f4dbf7582b2566a28473ffdc0850d8cd490cfb0d5e13568bc3d104aa1b9c`  
		Last Modified: Wed, 09 Jun 2021 13:11:32 GMT  
		Size: 138.6 MB (138598442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e2567bd998dd047ec27020dd4b6cc678d9f5e5c4c30ba2aeb4bbed135c6507`  
		Last Modified: Wed, 09 Jun 2021 13:08:50 GMT  
		Size: 1.6 KB (1574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd54a3680618246bc4f7a44ac005d9f63292e795ccdcf18cad2265cfa6eb2aa8`  
		Last Modified: Wed, 09 Jun 2021 20:19:16 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0003b3b81fea490ce3d717180fb612decca6b6c5e8924bc88cf3ba681e3858`  
		Last Modified: Wed, 09 Jun 2021 20:19:13 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4888eaf97833d4a8959b4c814e970d541992014645e85fe0f20f34ceb58f27ed`  
		Last Modified: Wed, 09 Jun 2021 20:19:13 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce0cc57747c2565c9825fc51e64e37b374745c15a1ce914f5a24eb25eff252d`  
		Last Modified: Wed, 09 Jun 2021 20:19:13 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def326ce00fc8a710eb36bffbf156cd48ba97585363cb5cf0df0693211058690`  
		Last Modified: Wed, 09 Jun 2021 20:19:16 GMT  
		Size: 1.7 MB (1691133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740e3a80e946b7578215b57f455cdd284a951e5970e8423b1dc5d2bb21241258`  
		Last Modified: Wed, 09 Jun 2021 20:19:13 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-windowsservercore`

```console
$ docker pull caddy@sha256:15d7c29dd7b38e74e3eefe924c32ae6b0d0ac40b1f36a748e152ce116d1e8307
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `caddy:2.3.0-windowsservercore` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:abfb982cd83fb9b806ec5efc924058a088a526547c8994c5a38ffaf05cd1a2e4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2654306673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9adcb39b5c8fc517d2f7805d6b1b9aba540a058014b0636d515b0cc29c63fb7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 12:10:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 19:58:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Jun 2021 19:58:06 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 09 Jun 2021 19:58:45 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Jun 2021 19:58:47 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Jun 2021 19:58:49 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Jun 2021 19:58:52 GMT
VOLUME [c:/config]
# Wed, 09 Jun 2021 19:58:54 GMT
VOLUME [c:/data]
# Wed, 09 Jun 2021 19:58:57 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 09 Jun 2021 19:58:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Jun 2021 19:59:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Jun 2021 19:59:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Jun 2021 19:59:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Jun 2021 19:59:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Jun 2021 19:59:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Jun 2021 19:59:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Jun 2021 19:59:15 GMT
EXPOSE 80
# Wed, 09 Jun 2021 19:59:17 GMT
EXPOSE 443
# Wed, 09 Jun 2021 19:59:20 GMT
EXPOSE 2019
# Wed, 09 Jun 2021 19:59:41 GMT
RUN caddy version
# Wed, 09 Jun 2021 19:59:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7863ef96846d497ea06fe442ea13dcecaf5c248ce238c69800475281a4fa848e`  
		Last Modified: Wed, 09 Jun 2021 12:20:41 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7d9ebdfbbf3d1e8112e1cb391db31904536061de5256556e771e9969f203b0`  
		Last Modified: Wed, 09 Jun 2021 20:18:20 GMT  
		Size: 361.6 KB (361645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8897f927c230372062964e749dc71a1079d44309ded3bfaca335b559fe2e58`  
		Last Modified: Wed, 09 Jun 2021 20:18:19 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd2185358235294396b61f1daa54f4b588dae132c10145e26e1aa27403e3e57`  
		Last Modified: Wed, 09 Jun 2021 20:18:33 GMT  
		Size: 12.0 MB (12042056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c556a340c4eb84af59ae068dc4578b860ee79b4018d7266a2c47ef8c8552667`  
		Last Modified: Wed, 09 Jun 2021 20:18:19 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b6f691ea8f2966736d5e44aaeeb20e8f173b2a817f4e821f4f8130910c87b1`  
		Last Modified: Wed, 09 Jun 2021 20:18:18 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53652087525344ae336288573310ddb36a768d2c3b1c668536776ca777535ee`  
		Last Modified: Wed, 09 Jun 2021 20:18:17 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e7823b092ee21c368597d091df167f1ee6a0d457f8ce4cfbd1ca5f610f94d8`  
		Last Modified: Wed, 09 Jun 2021 20:18:16 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebc12b375fa0cebfe64352b7506467d6b3bc204dfe4b02bd50fe16832efcfb0`  
		Last Modified: Wed, 09 Jun 2021 20:18:16 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d7680a122b7c72ed29d1b997262311532fa6db08032bd46444d052e36180d8`  
		Last Modified: Wed, 09 Jun 2021 20:18:16 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6703c8f9c1144cfa310b45884ed415026ea0c81f8f45be2351681aa578cee675`  
		Last Modified: Wed, 09 Jun 2021 20:18:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7741bb8d10925c9dc4507da771fb2d6b0fb41d41999608c705667c82b2ed24a`  
		Last Modified: Wed, 09 Jun 2021 20:18:14 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52ab324f35848d4e4a9bb7a49ca222ae128927d3dae72baee1b3e8309c0c516`  
		Last Modified: Wed, 09 Jun 2021 20:18:13 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614f13023b6134592bf80f195a24148dbcd9c6d85ce74b0a6e01fd8ac21af258`  
		Last Modified: Wed, 09 Jun 2021 20:18:13 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec077e1f7b7042bcaac19c45da37857a07fad1bc03946731d8647e25c6894e0`  
		Last Modified: Wed, 09 Jun 2021 20:18:13 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cf69b06a4d52b3c8b6d2c62b7655fcc045a248904be961434d6486822c2cdf`  
		Last Modified: Wed, 09 Jun 2021 20:18:13 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f643524a9a79dcaa3ae3723d70eff0a06ac5278102c91270cc69dac606cbbd`  
		Last Modified: Wed, 09 Jun 2021 20:18:11 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734615d480107ad568078168de5289e7dacb0f451e185d6f28db22ffd9f6f38d`  
		Last Modified: Wed, 09 Jun 2021 20:18:10 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6e6c4e82d321ceb042388a4b32b9f8491a91e5060c2ad66b82c194e9ef2ba2`  
		Last Modified: Wed, 09 Jun 2021 20:18:11 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7c66662d27b64b2b1cb6c5b01c8f552366559fa3373e6d1d2c184fdc0378b3`  
		Last Modified: Wed, 09 Jun 2021 20:18:11 GMT  
		Size: 292.5 KB (292467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9442f528e1f1b1935332a277492e8f047fe6a0b2eef98d62cde1fe286d16fb`  
		Last Modified: Wed, 09 Jun 2021 20:18:11 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-windowsservercore` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:36ebdab9cdd78892ba6e1c23096ead371830033af55ae4beff4a0f094f99bbb1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278410557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef0074d1abe6f6b4fc4f63ee29ba68462abe0043cf344dc84e4a1ff8100147d3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 12:41:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:01:17 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Jun 2021 20:01:19 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 09 Jun 2021 20:02:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Jun 2021 20:02:51 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Jun 2021 20:02:53 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Jun 2021 20:02:56 GMT
VOLUME [c:/config]
# Wed, 09 Jun 2021 20:02:58 GMT
VOLUME [c:/data]
# Wed, 09 Jun 2021 20:03:00 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 09 Jun 2021 20:03:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Jun 2021 20:03:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Jun 2021 20:03:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Jun 2021 20:03:11 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Jun 2021 20:03:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Jun 2021 20:03:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Jun 2021 20:03:19 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Jun 2021 20:03:22 GMT
EXPOSE 80
# Wed, 09 Jun 2021 20:03:24 GMT
EXPOSE 443
# Wed, 09 Jun 2021 20:03:27 GMT
EXPOSE 2019
# Wed, 09 Jun 2021 20:04:20 GMT
RUN caddy version
# Wed, 09 Jun 2021 20:04:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c82e82e95dbad4ccc260b42e03767eb07222e2f00ec57a69b3c87b17da1d2fd3`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7186c10d925bf51b7a0347cc44d9ccaaa700dd33c15bace64af437d839c08afc`  
		Last Modified: Wed, 09 Jun 2021 20:18:49 GMT  
		Size: 361.3 KB (361336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1a2b2e25a8e63c3ba5cf619d40f3daf10176d34ef1d5c6c74a617222e995bb`  
		Last Modified: Wed, 09 Jun 2021 20:18:49 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548bb9bdcebdb55c9c2a25ff1dd2962e5df2cee757f77d0b3c522d4f65983347`  
		Last Modified: Wed, 09 Jun 2021 20:18:52 GMT  
		Size: 12.0 MB (12034364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32ac36259028a1154879df59cb600b66fa7c5041ae6b274f385b96b28556bf1`  
		Last Modified: Wed, 09 Jun 2021 20:18:48 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1b36eb1530660082da73324bc94be1f00ba9b5d1e4be1d71199da3862a8a1c`  
		Last Modified: Wed, 09 Jun 2021 20:18:49 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8438aefe94f1d735ca92a8acfb9324000bf1f7fe4262886fa0b2df71d9e3c6bd`  
		Last Modified: Wed, 09 Jun 2021 20:18:46 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5bdad10cdbc7d78ee974dc7eec9a6345eb611f3a88ba9feed472596cc16454`  
		Last Modified: Wed, 09 Jun 2021 20:18:46 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3b6c63126e2060df917222ab905391a0f9fc0435f083aac9e843280d7afa7e`  
		Last Modified: Wed, 09 Jun 2021 20:18:46 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e412d17bbc625e61917a3fb903d8c775ddd693e84f4f6e6e1a53513f721ce4d8`  
		Last Modified: Wed, 09 Jun 2021 20:18:46 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cf08f45398baf12ebb8841e1c35678c167ce40ff7e83f9dd26a18ebd421ecc`  
		Last Modified: Wed, 09 Jun 2021 20:18:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570549f521be576d96b6d437a1a9004acaca2113f13ff43c879183db63e7eabd`  
		Last Modified: Wed, 09 Jun 2021 20:18:44 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d3ae1448bd25d3230e37d601c19abc7d1a2318b9ec037ffbd6d73927587b0a`  
		Last Modified: Wed, 09 Jun 2021 20:18:43 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944473f314aecab72089d844d05e1dd74b01454e2695396b5859dc9a6a9e07ea`  
		Last Modified: Wed, 09 Jun 2021 20:18:43 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a0802196eafa3eaeb45d12be27ffb7ce40038a96de352a11a5ffca06bcac50`  
		Last Modified: Wed, 09 Jun 2021 20:18:43 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:619af6b5ed093c9982004d31fd110fef2f317361602c32d65b453a6696db7808`  
		Last Modified: Wed, 09 Jun 2021 20:18:43 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79b4eac4f34750a41ea7faf4ee96b53b82bcf7e59cf8dac12c9dfc0d7606c7b`  
		Last Modified: Wed, 09 Jun 2021 20:18:41 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850ec4f3db9855738633574af9754a365fd845298867d1284d06ecd491ff6ea0`  
		Last Modified: Wed, 09 Jun 2021 20:18:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8dd45a07a5c2ce9a15b4a257361bd6508f013393bf9dc4bcc2f74cd1117ea13`  
		Last Modified: Wed, 09 Jun 2021 20:18:41 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cf05ec484a7aed9f1a8719d84b10aff6c29802fb4f68ddc16c0fde6495b93b`  
		Last Modified: Wed, 09 Jun 2021 20:18:41 GMT  
		Size: 262.0 KB (262013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4419e3710f83c624955a0392e5ffdfb1bda977c25ce5b407d4d6e9ca90396f`  
		Last Modified: Wed, 09 Jun 2021 20:18:41 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-windowsservercore-1809`

```console
$ docker pull caddy@sha256:1c304c34b529be6a6dca737117cc44beac0a630ca3a4cb0e7c3cd0fff81cb728
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `caddy:2.3.0-windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:abfb982cd83fb9b806ec5efc924058a088a526547c8994c5a38ffaf05cd1a2e4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2654306673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9adcb39b5c8fc517d2f7805d6b1b9aba540a058014b0636d515b0cc29c63fb7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 12:10:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 19:58:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Jun 2021 19:58:06 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 09 Jun 2021 19:58:45 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Jun 2021 19:58:47 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Jun 2021 19:58:49 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Jun 2021 19:58:52 GMT
VOLUME [c:/config]
# Wed, 09 Jun 2021 19:58:54 GMT
VOLUME [c:/data]
# Wed, 09 Jun 2021 19:58:57 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 09 Jun 2021 19:58:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Jun 2021 19:59:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Jun 2021 19:59:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Jun 2021 19:59:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Jun 2021 19:59:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Jun 2021 19:59:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Jun 2021 19:59:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Jun 2021 19:59:15 GMT
EXPOSE 80
# Wed, 09 Jun 2021 19:59:17 GMT
EXPOSE 443
# Wed, 09 Jun 2021 19:59:20 GMT
EXPOSE 2019
# Wed, 09 Jun 2021 19:59:41 GMT
RUN caddy version
# Wed, 09 Jun 2021 19:59:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7863ef96846d497ea06fe442ea13dcecaf5c248ce238c69800475281a4fa848e`  
		Last Modified: Wed, 09 Jun 2021 12:20:41 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7d9ebdfbbf3d1e8112e1cb391db31904536061de5256556e771e9969f203b0`  
		Last Modified: Wed, 09 Jun 2021 20:18:20 GMT  
		Size: 361.6 KB (361645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8897f927c230372062964e749dc71a1079d44309ded3bfaca335b559fe2e58`  
		Last Modified: Wed, 09 Jun 2021 20:18:19 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd2185358235294396b61f1daa54f4b588dae132c10145e26e1aa27403e3e57`  
		Last Modified: Wed, 09 Jun 2021 20:18:33 GMT  
		Size: 12.0 MB (12042056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c556a340c4eb84af59ae068dc4578b860ee79b4018d7266a2c47ef8c8552667`  
		Last Modified: Wed, 09 Jun 2021 20:18:19 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b6f691ea8f2966736d5e44aaeeb20e8f173b2a817f4e821f4f8130910c87b1`  
		Last Modified: Wed, 09 Jun 2021 20:18:18 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53652087525344ae336288573310ddb36a768d2c3b1c668536776ca777535ee`  
		Last Modified: Wed, 09 Jun 2021 20:18:17 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e7823b092ee21c368597d091df167f1ee6a0d457f8ce4cfbd1ca5f610f94d8`  
		Last Modified: Wed, 09 Jun 2021 20:18:16 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebc12b375fa0cebfe64352b7506467d6b3bc204dfe4b02bd50fe16832efcfb0`  
		Last Modified: Wed, 09 Jun 2021 20:18:16 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d7680a122b7c72ed29d1b997262311532fa6db08032bd46444d052e36180d8`  
		Last Modified: Wed, 09 Jun 2021 20:18:16 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6703c8f9c1144cfa310b45884ed415026ea0c81f8f45be2351681aa578cee675`  
		Last Modified: Wed, 09 Jun 2021 20:18:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7741bb8d10925c9dc4507da771fb2d6b0fb41d41999608c705667c82b2ed24a`  
		Last Modified: Wed, 09 Jun 2021 20:18:14 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52ab324f35848d4e4a9bb7a49ca222ae128927d3dae72baee1b3e8309c0c516`  
		Last Modified: Wed, 09 Jun 2021 20:18:13 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614f13023b6134592bf80f195a24148dbcd9c6d85ce74b0a6e01fd8ac21af258`  
		Last Modified: Wed, 09 Jun 2021 20:18:13 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec077e1f7b7042bcaac19c45da37857a07fad1bc03946731d8647e25c6894e0`  
		Last Modified: Wed, 09 Jun 2021 20:18:13 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cf69b06a4d52b3c8b6d2c62b7655fcc045a248904be961434d6486822c2cdf`  
		Last Modified: Wed, 09 Jun 2021 20:18:13 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f643524a9a79dcaa3ae3723d70eff0a06ac5278102c91270cc69dac606cbbd`  
		Last Modified: Wed, 09 Jun 2021 20:18:11 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734615d480107ad568078168de5289e7dacb0f451e185d6f28db22ffd9f6f38d`  
		Last Modified: Wed, 09 Jun 2021 20:18:10 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6e6c4e82d321ceb042388a4b32b9f8491a91e5060c2ad66b82c194e9ef2ba2`  
		Last Modified: Wed, 09 Jun 2021 20:18:11 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7c66662d27b64b2b1cb6c5b01c8f552366559fa3373e6d1d2c184fdc0378b3`  
		Last Modified: Wed, 09 Jun 2021 20:18:11 GMT  
		Size: 292.5 KB (292467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9442f528e1f1b1935332a277492e8f047fe6a0b2eef98d62cde1fe286d16fb`  
		Last Modified: Wed, 09 Jun 2021 20:18:11 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:c727c466c6db11e0f1f1879bd7898f8569033ccf85054b310cbd882647d7e6e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `caddy:2.3.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:36ebdab9cdd78892ba6e1c23096ead371830033af55ae4beff4a0f094f99bbb1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278410557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef0074d1abe6f6b4fc4f63ee29ba68462abe0043cf344dc84e4a1ff8100147d3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 12:41:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:01:17 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Jun 2021 20:01:19 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 09 Jun 2021 20:02:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Jun 2021 20:02:51 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Jun 2021 20:02:53 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Jun 2021 20:02:56 GMT
VOLUME [c:/config]
# Wed, 09 Jun 2021 20:02:58 GMT
VOLUME [c:/data]
# Wed, 09 Jun 2021 20:03:00 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 09 Jun 2021 20:03:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Jun 2021 20:03:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Jun 2021 20:03:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Jun 2021 20:03:11 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Jun 2021 20:03:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Jun 2021 20:03:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Jun 2021 20:03:19 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Jun 2021 20:03:22 GMT
EXPOSE 80
# Wed, 09 Jun 2021 20:03:24 GMT
EXPOSE 443
# Wed, 09 Jun 2021 20:03:27 GMT
EXPOSE 2019
# Wed, 09 Jun 2021 20:04:20 GMT
RUN caddy version
# Wed, 09 Jun 2021 20:04:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c82e82e95dbad4ccc260b42e03767eb07222e2f00ec57a69b3c87b17da1d2fd3`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7186c10d925bf51b7a0347cc44d9ccaaa700dd33c15bace64af437d839c08afc`  
		Last Modified: Wed, 09 Jun 2021 20:18:49 GMT  
		Size: 361.3 KB (361336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1a2b2e25a8e63c3ba5cf619d40f3daf10176d34ef1d5c6c74a617222e995bb`  
		Last Modified: Wed, 09 Jun 2021 20:18:49 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548bb9bdcebdb55c9c2a25ff1dd2962e5df2cee757f77d0b3c522d4f65983347`  
		Last Modified: Wed, 09 Jun 2021 20:18:52 GMT  
		Size: 12.0 MB (12034364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32ac36259028a1154879df59cb600b66fa7c5041ae6b274f385b96b28556bf1`  
		Last Modified: Wed, 09 Jun 2021 20:18:48 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1b36eb1530660082da73324bc94be1f00ba9b5d1e4be1d71199da3862a8a1c`  
		Last Modified: Wed, 09 Jun 2021 20:18:49 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8438aefe94f1d735ca92a8acfb9324000bf1f7fe4262886fa0b2df71d9e3c6bd`  
		Last Modified: Wed, 09 Jun 2021 20:18:46 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5bdad10cdbc7d78ee974dc7eec9a6345eb611f3a88ba9feed472596cc16454`  
		Last Modified: Wed, 09 Jun 2021 20:18:46 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3b6c63126e2060df917222ab905391a0f9fc0435f083aac9e843280d7afa7e`  
		Last Modified: Wed, 09 Jun 2021 20:18:46 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e412d17bbc625e61917a3fb903d8c775ddd693e84f4f6e6e1a53513f721ce4d8`  
		Last Modified: Wed, 09 Jun 2021 20:18:46 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cf08f45398baf12ebb8841e1c35678c167ce40ff7e83f9dd26a18ebd421ecc`  
		Last Modified: Wed, 09 Jun 2021 20:18:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570549f521be576d96b6d437a1a9004acaca2113f13ff43c879183db63e7eabd`  
		Last Modified: Wed, 09 Jun 2021 20:18:44 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d3ae1448bd25d3230e37d601c19abc7d1a2318b9ec037ffbd6d73927587b0a`  
		Last Modified: Wed, 09 Jun 2021 20:18:43 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944473f314aecab72089d844d05e1dd74b01454e2695396b5859dc9a6a9e07ea`  
		Last Modified: Wed, 09 Jun 2021 20:18:43 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a0802196eafa3eaeb45d12be27ffb7ce40038a96de352a11a5ffca06bcac50`  
		Last Modified: Wed, 09 Jun 2021 20:18:43 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:619af6b5ed093c9982004d31fd110fef2f317361602c32d65b453a6696db7808`  
		Last Modified: Wed, 09 Jun 2021 20:18:43 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79b4eac4f34750a41ea7faf4ee96b53b82bcf7e59cf8dac12c9dfc0d7606c7b`  
		Last Modified: Wed, 09 Jun 2021 20:18:41 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850ec4f3db9855738633574af9754a365fd845298867d1284d06ecd491ff6ea0`  
		Last Modified: Wed, 09 Jun 2021 20:18:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8dd45a07a5c2ce9a15b4a257361bd6508f013393bf9dc4bcc2f74cd1117ea13`  
		Last Modified: Wed, 09 Jun 2021 20:18:41 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cf05ec484a7aed9f1a8719d84b10aff6c29802fb4f68ddc16c0fde6495b93b`  
		Last Modified: Wed, 09 Jun 2021 20:18:41 GMT  
		Size: 262.0 KB (262013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4419e3710f83c624955a0392e5ffdfb1bda977c25ce5b407d4d6e9ca90396f`  
		Last Modified: Wed, 09 Jun 2021 20:18:41 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.1`

```console
$ docker pull caddy@sha256:8031d689a8e6f47dcc146121b75946348e8b2e94a183e92cac38a489f55759a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `caddy:2.4.1` - linux; amd64

```console
$ docker pull caddy@sha256:c3b2e52162bebaf3b0d128780b3bffc4aa9ccb6953953892dd9d31495e15dc55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14568035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b59636b1388443a36d8173a6ad50dbcf59de4b7786b8178ad9eb656ad6e9a387`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:11:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:04:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 24 May 2021 18:23:10 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:23:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 24 May 2021 18:23:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 24 May 2021 18:23:13 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 24 May 2021 18:23:14 GMT
ENV XDG_DATA_HOME=/data
# Mon, 24 May 2021 18:23:14 GMT
VOLUME [/config]
# Mon, 24 May 2021 18:23:14 GMT
VOLUME [/data]
# Mon, 24 May 2021 18:23:14 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:23:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:23:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:23:16 GMT
EXPOSE 80
# Mon, 24 May 2021 18:23:16 GMT
EXPOSE 443
# Mon, 24 May 2021 18:23:16 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:23:16 GMT
WORKDIR /srv
# Mon, 24 May 2021 18:23:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8294633c5b5606f8e98aaf81da701b7a7e2018dbf82355d1d73830c677034f19`  
		Last Modified: Wed, 14 Apr 2021 20:12:08 GMT  
		Size: 300.4 KB (300403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16798e0582fce7af9c2ba2c8ee4990d0fd1e58384e170ee9937486253d67bbf1`  
		Last Modified: Tue, 11 May 2021 01:05:00 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba0aa26d56032b74c8c88c24edc5a2f7987ea418aaa0966f93ab53c62802c2f`  
		Last Modified: Mon, 24 May 2021 18:23:47 GMT  
		Size: 11.4 MB (11449656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712687f6a8ba00b8b6cb95bad7426eb9964fff3de9f5a7f66dedf6310e8a8c01`  
		Last Modified: Mon, 24 May 2021 18:23:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1` - linux; arm variant v6

```console
$ docker pull caddy@sha256:eea14e6e8e0ef54944ef2f6e1b6540a536661e033a1f216e92535b5741c2278e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13786866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e11afe23a7696f3f16192af7de16ece9c2dfb73868f2859b9dbacfe0e604fa4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 17:34:28 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 May 2021 17:34:30 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Wed, 26 May 2021 17:34:30 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 26 May 2021 17:34:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 May 2021 17:34:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 May 2021 17:34:33 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 May 2021 17:34:34 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 May 2021 17:34:34 GMT
VOLUME [/config]
# Wed, 26 May 2021 17:34:34 GMT
VOLUME [/data]
# Wed, 26 May 2021 17:34:34 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 26 May 2021 17:34:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 May 2021 17:34:34 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 May 2021 17:34:36 GMT
EXPOSE 80
# Wed, 26 May 2021 17:34:36 GMT
EXPOSE 443
# Wed, 26 May 2021 17:34:36 GMT
EXPOSE 2019
# Wed, 26 May 2021 17:34:36 GMT
WORKDIR /srv
# Wed, 26 May 2021 17:34:36 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c2672622a603ff8b0ed8517cfd5adb30b2b35ae40b42cd4ad0545dcb6d3b10`  
		Last Modified: Wed, 26 May 2021 17:36:11 GMT  
		Size: 300.5 KB (300528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b30604f35cc25a62ae1d71a50c6919ad28a2aa67bfd14bebc1984cec5b2c8b`  
		Last Modified: Wed, 26 May 2021 17:36:12 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7119340f7ca66a456adcbc374cbeb7e1c37c35867123bd3fac943aea26a813a8`  
		Last Modified: Wed, 26 May 2021 17:36:15 GMT  
		Size: 10.9 MB (10858201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392497979deecdb2075178245bdf58e8d1ce55c609d2b1320a869392bc007b3f`  
		Last Modified: Wed, 26 May 2021 17:36:12 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1` - linux; arm variant v7

```console
$ docker pull caddy@sha256:ea6c90777b37ade094ce3f1f5d0efffe39519d18ec589fa4cfa2b6f0c5028e3a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13561305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8637a19be10382ee673bc51be71c9fa3ce23cfdcd0eb9d9bf8734147818227d4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 10:59:27 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 May 2021 10:59:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Wed, 26 May 2021 10:59:29 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 26 May 2021 10:59:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 May 2021 10:59:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 May 2021 10:59:32 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 May 2021 10:59:32 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 May 2021 10:59:32 GMT
VOLUME [/config]
# Wed, 26 May 2021 10:59:33 GMT
VOLUME [/data]
# Wed, 26 May 2021 10:59:33 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 26 May 2021 10:59:33 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 May 2021 10:59:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 May 2021 10:59:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 May 2021 10:59:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 May 2021 10:59:34 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 May 2021 10:59:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 May 2021 10:59:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 May 2021 10:59:34 GMT
EXPOSE 80
# Wed, 26 May 2021 10:59:35 GMT
EXPOSE 443
# Wed, 26 May 2021 10:59:35 GMT
EXPOSE 2019
# Wed, 26 May 2021 10:59:35 GMT
WORKDIR /srv
# Wed, 26 May 2021 10:59:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca051a8c4175c3d7d75c47c9a60045d2f5b7eb415ce35b56c99e9cab58ae3ba`  
		Last Modified: Wed, 26 May 2021 11:01:09 GMT  
		Size: 299.7 KB (299668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2db810fb832f7bd380a39ff7508fa03cc1854bdd51da4cfa239e07fe96fe4e`  
		Last Modified: Wed, 26 May 2021 11:01:09 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce092d490b7e90c7b37879314c23cb48b38be5392715e2d976bc99bbef8a230`  
		Last Modified: Wed, 26 May 2021 11:01:11 GMT  
		Size: 10.8 MB (10831485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb6eb70297874eea11cf38b8870aa1f896bfd6ec638fd6dc9177d7be039001b`  
		Last Modified: Wed, 26 May 2021 11:01:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:ad6d7adcc7d981edfcc5eb4bb42e1fc561b9d0301cadf2ccd920a4a98ae90387
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13415153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:383d427b090897c507d37417dfd21667985cf15a9e3e800b87c821eabe372bb6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 17:52:42 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 May 2021 17:52:43 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Wed, 26 May 2021 17:52:44 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 26 May 2021 17:52:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 May 2021 17:52:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 May 2021 17:52:47 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 May 2021 17:52:47 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 May 2021 17:52:47 GMT
VOLUME [/config]
# Wed, 26 May 2021 17:52:47 GMT
VOLUME [/data]
# Wed, 26 May 2021 17:52:47 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 May 2021 17:52:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 May 2021 17:52:49 GMT
EXPOSE 80
# Wed, 26 May 2021 17:52:49 GMT
EXPOSE 443
# Wed, 26 May 2021 17:52:49 GMT
EXPOSE 2019
# Wed, 26 May 2021 17:52:49 GMT
WORKDIR /srv
# Wed, 26 May 2021 17:52:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a305c6848b1bdb9c473c4a3128eff85e1604c1b2d0e78cef80874650b91a49`  
		Last Modified: Wed, 26 May 2021 17:53:57 GMT  
		Size: 300.6 KB (300633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2faea6afac2cf802bf88fd56ee1493ce97eca3a29920702a726ea8e5cd0ea3d`  
		Last Modified: Wed, 26 May 2021 17:53:57 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c196442e5472f13a88f63e7da52cbd15acf171b3d76e87cc47c3073ed0e95d`  
		Last Modified: Wed, 26 May 2021 17:53:59 GMT  
		Size: 10.4 MB (10396489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583f00c174c73f777e3d0cd263a593786c4c341cb20632fafb4246ac0f06f45b`  
		Last Modified: Wed, 26 May 2021 17:53:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1` - linux; ppc64le

```console
$ docker pull caddy@sha256:b767e2ec43a11bb1a211e3d7bc76c81d4a256f90084d5747367af6a9730e4f94
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13121818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f930dc44ddd7a57e1d48aaeed66a69653dc4d5c15bdae6c378273cb55287f07b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:12:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:17:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 24 May 2021 18:19:32 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:20:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 24 May 2021 18:20:18 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 24 May 2021 18:20:25 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 24 May 2021 18:20:32 GMT
ENV XDG_DATA_HOME=/data
# Mon, 24 May 2021 18:20:39 GMT
VOLUME [/config]
# Mon, 24 May 2021 18:20:45 GMT
VOLUME [/data]
# Mon, 24 May 2021 18:20:51 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:20:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:21:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:21:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:21:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:21:34 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:21:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:21:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:22:03 GMT
EXPOSE 80
# Mon, 24 May 2021 18:22:10 GMT
EXPOSE 443
# Mon, 24 May 2021 18:22:16 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:22:21 GMT
WORKDIR /srv
# Mon, 24 May 2021 18:22:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25908330df11bb7bc2ed71aa9b4de279db5492df2b03ced3f6650b25821c4584`  
		Last Modified: Wed, 14 Apr 2021 22:16:00 GMT  
		Size: 302.6 KB (302554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a224581e3ba4733f37686f5a5d5375019f9126a0ded6ed20f13e09e898dc735e`  
		Last Modified: Tue, 11 May 2021 01:20:08 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c6214f82b33045060ad6f882d1ed7a5779be7a0883c4da8306ab03e9e2623c`  
		Last Modified: Mon, 24 May 2021 18:23:37 GMT  
		Size: 10.0 MB (10000116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52a67b9935763896cc7c3386cd93b5f7fbc80093549e39f460dc7e170f679f4`  
		Last Modified: Mon, 24 May 2021 18:23:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1` - linux; s390x

```console
$ docker pull caddy@sha256:40e8d6bc1ad5c4c4f902426841f39a594dd3842c212bed7ecbb66f312b5a4f6e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13938687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c9fccd235488bb04e0075ea4a47a8c102dce45c98cbba05e4d7d0d0ebb13b1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:07:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 10 May 2021 23:41:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 24 May 2021 17:41:40 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 17:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 24 May 2021 17:41:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 24 May 2021 17:41:48 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 24 May 2021 17:41:48 GMT
ENV XDG_DATA_HOME=/data
# Mon, 24 May 2021 17:41:49 GMT
VOLUME [/config]
# Mon, 24 May 2021 17:41:50 GMT
VOLUME [/data]
# Mon, 24 May 2021 17:41:50 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 17:41:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 17:41:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 17:41:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 17:41:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 17:41:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 17:41:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 17:41:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 17:41:55 GMT
EXPOSE 80
# Mon, 24 May 2021 17:41:56 GMT
EXPOSE 443
# Mon, 24 May 2021 17:41:57 GMT
EXPOSE 2019
# Mon, 24 May 2021 17:41:57 GMT
WORKDIR /srv
# Mon, 24 May 2021 17:41:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db3c8b812fcb0d1bfd42c16c2e9ac68f4f3006382c5362e969d1c9eb3a9fab5`  
		Last Modified: Wed, 14 Apr 2021 20:08:26 GMT  
		Size: 300.8 KB (300847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba030675d7bb5bc251d93896d2c81ed8a2f4f4ef2e8e84ad7dfdce9886387c`  
		Last Modified: Mon, 10 May 2021 23:42:29 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03e81629e078650b941a4beb267a6755133e90fa22a688bffb5df188e069c55`  
		Last Modified: Mon, 24 May 2021 17:42:37 GMT  
		Size: 11.0 MB (11029189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbee1e7ec347a65e5e78b46b8fe541241e3f6c13a468785945abd0aaba24545`  
		Last Modified: Mon, 24 May 2021 17:42:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:d4a3e0eabf14e4f98a9bcf5eada28d1443573b082afe95028d548d5b88a2b33e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2654170862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:736d3aa581b715efdf7c0431ebfbaed21b664091d8e8f7e4595c5f9dabbd2acb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 12:10:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:08:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Jun 2021 20:08:07 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:08:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Jun 2021 20:08:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Jun 2021 20:08:49 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Jun 2021 20:08:51 GMT
VOLUME [c:/config]
# Wed, 09 Jun 2021 20:08:53 GMT
VOLUME [c:/data]
# Wed, 09 Jun 2021 20:08:55 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 09 Jun 2021 20:08:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Jun 2021 20:09:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Jun 2021 20:09:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Jun 2021 20:09:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Jun 2021 20:09:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Jun 2021 20:09:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Jun 2021 20:09:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Jun 2021 20:09:14 GMT
EXPOSE 80
# Wed, 09 Jun 2021 20:09:17 GMT
EXPOSE 443
# Wed, 09 Jun 2021 20:09:19 GMT
EXPOSE 2019
# Wed, 09 Jun 2021 20:09:41 GMT
RUN caddy version
# Wed, 09 Jun 2021 20:09:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7863ef96846d497ea06fe442ea13dcecaf5c248ce238c69800475281a4fa848e`  
		Last Modified: Wed, 09 Jun 2021 12:20:41 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dc18d712eacfb666370e311daaf51e09fc2f76ca762e4592e149fbe6aba561`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 361.4 KB (361380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b774f6019fa0c611532d02bdf31c54e9da56fe2330e3e0745538ef036cfb87`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e977598d13d0ee9ae780f2cf34706c57e810301d20d9fc8286ad9390b9166b`  
		Last Modified: Wed, 09 Jun 2021 20:19:37 GMT  
		Size: 11.9 MB (11906202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7361692fe34486902f2dd9f69cc3bce54c4cb8c5c86ed80a0d75033f25ae5213`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35d39d3918ab9262122b494a653aec25e76a65396f9198d7be955cb9c26c6f3`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66891a50a919af8d3cb83358a7f8d33b2055c143bd3499cc431fd32d053ed393`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519d446a1689a5424a77bf1cbf0f00153b28c6eff9ee22f0f88e0e32b3f6bda3`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534ea2eef93aa67b4ac4bfb48ac5498fa33b02d0b88b9ae60b8ae159addacecc`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19fc40bc9ade11a1755b185c529e961b474d959d45a44b1b1ab5f12e3d17863a`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ef9960b6bac284e65c351bc447bb8931486a0c1c3ee68c9e5a62828b4ae0e`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cfda8707421463aa0f297ce5d4ac3a615f60caf56e6e69a299caa08a04f7da`  
		Last Modified: Wed, 09 Jun 2021 20:19:29 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa0c9ece6e3482cf3ffc8d9a087d113db0f7c249f59bcf06f3ffc65c5e4bce0`  
		Last Modified: Wed, 09 Jun 2021 20:19:29 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6614223fb410a8262956f73a038f6d79b67d5976fe8740b21dfa2121a9cbd7f2`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f354857e070035731eb660ec35ff9f8549b6cc79211bab40ae642d9875f98f8b`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc94f29a4cb79013fce0bf1a5776868fa31912b598231e46883a114d86f712d3`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e536fde913e2e2d5ae24846adca32195330a9be6e7d1c3180ce7ac6bc6a35ae1`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b11db027637bf7abeec6bbcd83920c4eb7c291aeeae4d2886a1563bf41289a6`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3a70d973d27d739faae877290b3184bee11c706ebd4bfa515d180fba88ef0f`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc7b3e3d99424f8d3737a4502a6f50767ae25b699a315155b98700af682b64f`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 292.6 KB (292631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d435932a64bec158a6193fa4a31a1b38e446ec9f63c0b6be3282c3acf3288949`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:e7e7af29e7917229552a0c802147dba99fb7a1427b84296a2c60ea7e19cbcb0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278267906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7184db699efd0a2ce0077179784cc7277e5faa7d07534ea1ce32d61d7f46ebc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 12:41:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:11:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Jun 2021 20:11:30 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:13:06 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Jun 2021 20:13:09 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Jun 2021 20:13:11 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Jun 2021 20:13:15 GMT
VOLUME [c:/config]
# Wed, 09 Jun 2021 20:13:18 GMT
VOLUME [c:/data]
# Wed, 09 Jun 2021 20:13:20 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 09 Jun 2021 20:13:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Jun 2021 20:13:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Jun 2021 20:13:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Jun 2021 20:13:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Jun 2021 20:13:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Jun 2021 20:13:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Jun 2021 20:13:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Jun 2021 20:13:40 GMT
EXPOSE 80
# Wed, 09 Jun 2021 20:13:42 GMT
EXPOSE 443
# Wed, 09 Jun 2021 20:13:45 GMT
EXPOSE 2019
# Wed, 09 Jun 2021 20:14:40 GMT
RUN caddy version
# Wed, 09 Jun 2021 20:14:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c82e82e95dbad4ccc260b42e03767eb07222e2f00ec57a69b3c87b17da1d2fd3`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a28e390d3b8e7b9369b102914eaee6e1fa0d14eb258b628be67f99f32f06f81`  
		Last Modified: Wed, 09 Jun 2021 20:20:01 GMT  
		Size: 357.4 KB (357370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7f07987f083e935103f83e47894b93aceaf05d1ded81dd09eb0bc3c8e45af`  
		Last Modified: Wed, 09 Jun 2021 20:20:01 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e65ddfdcdd60907208873b2a532cc58bc0f57d144430cef2c7630e80e4fd1e`  
		Last Modified: Wed, 09 Jun 2021 20:20:05 GMT  
		Size: 11.9 MB (11896985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58e4679b7ef7e1b9d82f44a6b5055c6916801193550bcce3ce390851224c736`  
		Last Modified: Wed, 09 Jun 2021 20:20:00 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107d803623512ea83de929509cc68f334261f2018c60bde60a99eadd0c2b179`  
		Last Modified: Wed, 09 Jun 2021 20:20:00 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f757538ddb020d145715a4890594958e741fe98366f1a58314361e5a8a3487`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462510ee9cb1c642e2804f8f607f02ccc5c31b63c956b9394bf38c5041b10d8b`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e87709f8365472aa7278651dacfc7eee93b24859a494cf6904b4f7ce80df0a`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5439b862b8218f1d7e0e0269efdbed614475ffbdcbaac06a3953f80b07677a1a`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1950c17917c025587fa23872145ee00eaaa11939dc87314c1aa74119db642d`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84164685053ad8b12a46e198ec2e93143d1df956bbbd4af76c88d0f549031c60`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103b7e93d2e2faefef7bd14bc00910442ce8da843f4fb726e2dba2d97752ddc9`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046d1e0cd75d46944ff833afe00c5dc9835ec1eb72876965a98a1488778910a6`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593a0ce075f6e5e07785dd7cd14aa1c274339da4d6f80495f0d1a85fabdef5db`  
		Last Modified: Wed, 09 Jun 2021 20:19:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14f5cdc43c91f65e6c5879691adc6e392d353807b27465a9b270fe7a06da51c`  
		Last Modified: Wed, 09 Jun 2021 20:19:55 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd488f5f58644d68e5103098932448a58d05a716861b26bf33376e75ad27e61`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c218cc3caa4b354c536ad99d30753a6eb41c52a58c52aafc0655a8482382a07`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3dad29a1e0241680f68697c2b0dbca8e85d0084faef4bdd3e66c8294be80671`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daeda652af05f03b2ec029aa5caa6b49d533546fa8347f5b1db003e8a83a7c30`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 260.8 KB (260840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9779c5588bf525e972d3b02ecaeeee32f3939ef8d54e8a16c52e0e62804e2e42`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.1-alpine`

```console
$ docker pull caddy@sha256:48e775e759b55c34afd4293c6ec80650a45754a193c8eaa62c6fcddb6f599d45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.4.1-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:c3b2e52162bebaf3b0d128780b3bffc4aa9ccb6953953892dd9d31495e15dc55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14568035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b59636b1388443a36d8173a6ad50dbcf59de4b7786b8178ad9eb656ad6e9a387`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:11:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:04:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 24 May 2021 18:23:10 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:23:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 24 May 2021 18:23:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 24 May 2021 18:23:13 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 24 May 2021 18:23:14 GMT
ENV XDG_DATA_HOME=/data
# Mon, 24 May 2021 18:23:14 GMT
VOLUME [/config]
# Mon, 24 May 2021 18:23:14 GMT
VOLUME [/data]
# Mon, 24 May 2021 18:23:14 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:23:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:23:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:23:16 GMT
EXPOSE 80
# Mon, 24 May 2021 18:23:16 GMT
EXPOSE 443
# Mon, 24 May 2021 18:23:16 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:23:16 GMT
WORKDIR /srv
# Mon, 24 May 2021 18:23:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8294633c5b5606f8e98aaf81da701b7a7e2018dbf82355d1d73830c677034f19`  
		Last Modified: Wed, 14 Apr 2021 20:12:08 GMT  
		Size: 300.4 KB (300403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16798e0582fce7af9c2ba2c8ee4990d0fd1e58384e170ee9937486253d67bbf1`  
		Last Modified: Tue, 11 May 2021 01:05:00 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba0aa26d56032b74c8c88c24edc5a2f7987ea418aaa0966f93ab53c62802c2f`  
		Last Modified: Mon, 24 May 2021 18:23:47 GMT  
		Size: 11.4 MB (11449656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712687f6a8ba00b8b6cb95bad7426eb9964fff3de9f5a7f66dedf6310e8a8c01`  
		Last Modified: Mon, 24 May 2021 18:23:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:eea14e6e8e0ef54944ef2f6e1b6540a536661e033a1f216e92535b5741c2278e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13786866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e11afe23a7696f3f16192af7de16ece9c2dfb73868f2859b9dbacfe0e604fa4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 17:34:28 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 May 2021 17:34:30 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Wed, 26 May 2021 17:34:30 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 26 May 2021 17:34:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 May 2021 17:34:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 May 2021 17:34:33 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 May 2021 17:34:34 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 May 2021 17:34:34 GMT
VOLUME [/config]
# Wed, 26 May 2021 17:34:34 GMT
VOLUME [/data]
# Wed, 26 May 2021 17:34:34 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 26 May 2021 17:34:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 May 2021 17:34:34 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 May 2021 17:34:36 GMT
EXPOSE 80
# Wed, 26 May 2021 17:34:36 GMT
EXPOSE 443
# Wed, 26 May 2021 17:34:36 GMT
EXPOSE 2019
# Wed, 26 May 2021 17:34:36 GMT
WORKDIR /srv
# Wed, 26 May 2021 17:34:36 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c2672622a603ff8b0ed8517cfd5adb30b2b35ae40b42cd4ad0545dcb6d3b10`  
		Last Modified: Wed, 26 May 2021 17:36:11 GMT  
		Size: 300.5 KB (300528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b30604f35cc25a62ae1d71a50c6919ad28a2aa67bfd14bebc1984cec5b2c8b`  
		Last Modified: Wed, 26 May 2021 17:36:12 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7119340f7ca66a456adcbc374cbeb7e1c37c35867123bd3fac943aea26a813a8`  
		Last Modified: Wed, 26 May 2021 17:36:15 GMT  
		Size: 10.9 MB (10858201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392497979deecdb2075178245bdf58e8d1ce55c609d2b1320a869392bc007b3f`  
		Last Modified: Wed, 26 May 2021 17:36:12 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:ea6c90777b37ade094ce3f1f5d0efffe39519d18ec589fa4cfa2b6f0c5028e3a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13561305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8637a19be10382ee673bc51be71c9fa3ce23cfdcd0eb9d9bf8734147818227d4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 10:59:27 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 May 2021 10:59:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Wed, 26 May 2021 10:59:29 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 26 May 2021 10:59:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 May 2021 10:59:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 May 2021 10:59:32 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 May 2021 10:59:32 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 May 2021 10:59:32 GMT
VOLUME [/config]
# Wed, 26 May 2021 10:59:33 GMT
VOLUME [/data]
# Wed, 26 May 2021 10:59:33 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 26 May 2021 10:59:33 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 May 2021 10:59:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 May 2021 10:59:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 May 2021 10:59:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 May 2021 10:59:34 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 May 2021 10:59:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 May 2021 10:59:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 May 2021 10:59:34 GMT
EXPOSE 80
# Wed, 26 May 2021 10:59:35 GMT
EXPOSE 443
# Wed, 26 May 2021 10:59:35 GMT
EXPOSE 2019
# Wed, 26 May 2021 10:59:35 GMT
WORKDIR /srv
# Wed, 26 May 2021 10:59:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca051a8c4175c3d7d75c47c9a60045d2f5b7eb415ce35b56c99e9cab58ae3ba`  
		Last Modified: Wed, 26 May 2021 11:01:09 GMT  
		Size: 299.7 KB (299668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2db810fb832f7bd380a39ff7508fa03cc1854bdd51da4cfa239e07fe96fe4e`  
		Last Modified: Wed, 26 May 2021 11:01:09 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce092d490b7e90c7b37879314c23cb48b38be5392715e2d976bc99bbef8a230`  
		Last Modified: Wed, 26 May 2021 11:01:11 GMT  
		Size: 10.8 MB (10831485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb6eb70297874eea11cf38b8870aa1f896bfd6ec638fd6dc9177d7be039001b`  
		Last Modified: Wed, 26 May 2021 11:01:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:ad6d7adcc7d981edfcc5eb4bb42e1fc561b9d0301cadf2ccd920a4a98ae90387
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13415153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:383d427b090897c507d37417dfd21667985cf15a9e3e800b87c821eabe372bb6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 17:52:42 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 May 2021 17:52:43 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Wed, 26 May 2021 17:52:44 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 26 May 2021 17:52:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 May 2021 17:52:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 May 2021 17:52:47 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 May 2021 17:52:47 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 May 2021 17:52:47 GMT
VOLUME [/config]
# Wed, 26 May 2021 17:52:47 GMT
VOLUME [/data]
# Wed, 26 May 2021 17:52:47 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 May 2021 17:52:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 May 2021 17:52:49 GMT
EXPOSE 80
# Wed, 26 May 2021 17:52:49 GMT
EXPOSE 443
# Wed, 26 May 2021 17:52:49 GMT
EXPOSE 2019
# Wed, 26 May 2021 17:52:49 GMT
WORKDIR /srv
# Wed, 26 May 2021 17:52:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a305c6848b1bdb9c473c4a3128eff85e1604c1b2d0e78cef80874650b91a49`  
		Last Modified: Wed, 26 May 2021 17:53:57 GMT  
		Size: 300.6 KB (300633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2faea6afac2cf802bf88fd56ee1493ce97eca3a29920702a726ea8e5cd0ea3d`  
		Last Modified: Wed, 26 May 2021 17:53:57 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c196442e5472f13a88f63e7da52cbd15acf171b3d76e87cc47c3073ed0e95d`  
		Last Modified: Wed, 26 May 2021 17:53:59 GMT  
		Size: 10.4 MB (10396489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583f00c174c73f777e3d0cd263a593786c4c341cb20632fafb4246ac0f06f45b`  
		Last Modified: Wed, 26 May 2021 17:53:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:b767e2ec43a11bb1a211e3d7bc76c81d4a256f90084d5747367af6a9730e4f94
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13121818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f930dc44ddd7a57e1d48aaeed66a69653dc4d5c15bdae6c378273cb55287f07b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:12:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:17:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 24 May 2021 18:19:32 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:20:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 24 May 2021 18:20:18 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 24 May 2021 18:20:25 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 24 May 2021 18:20:32 GMT
ENV XDG_DATA_HOME=/data
# Mon, 24 May 2021 18:20:39 GMT
VOLUME [/config]
# Mon, 24 May 2021 18:20:45 GMT
VOLUME [/data]
# Mon, 24 May 2021 18:20:51 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:20:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:21:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:21:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:21:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:21:34 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:21:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:21:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:22:03 GMT
EXPOSE 80
# Mon, 24 May 2021 18:22:10 GMT
EXPOSE 443
# Mon, 24 May 2021 18:22:16 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:22:21 GMT
WORKDIR /srv
# Mon, 24 May 2021 18:22:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25908330df11bb7bc2ed71aa9b4de279db5492df2b03ced3f6650b25821c4584`  
		Last Modified: Wed, 14 Apr 2021 22:16:00 GMT  
		Size: 302.6 KB (302554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a224581e3ba4733f37686f5a5d5375019f9126a0ded6ed20f13e09e898dc735e`  
		Last Modified: Tue, 11 May 2021 01:20:08 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c6214f82b33045060ad6f882d1ed7a5779be7a0883c4da8306ab03e9e2623c`  
		Last Modified: Mon, 24 May 2021 18:23:37 GMT  
		Size: 10.0 MB (10000116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52a67b9935763896cc7c3386cd93b5f7fbc80093549e39f460dc7e170f679f4`  
		Last Modified: Mon, 24 May 2021 18:23:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:40e8d6bc1ad5c4c4f902426841f39a594dd3842c212bed7ecbb66f312b5a4f6e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13938687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c9fccd235488bb04e0075ea4a47a8c102dce45c98cbba05e4d7d0d0ebb13b1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:07:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 10 May 2021 23:41:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 24 May 2021 17:41:40 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 17:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 24 May 2021 17:41:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 24 May 2021 17:41:48 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 24 May 2021 17:41:48 GMT
ENV XDG_DATA_HOME=/data
# Mon, 24 May 2021 17:41:49 GMT
VOLUME [/config]
# Mon, 24 May 2021 17:41:50 GMT
VOLUME [/data]
# Mon, 24 May 2021 17:41:50 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 17:41:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 17:41:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 17:41:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 17:41:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 17:41:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 17:41:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 17:41:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 17:41:55 GMT
EXPOSE 80
# Mon, 24 May 2021 17:41:56 GMT
EXPOSE 443
# Mon, 24 May 2021 17:41:57 GMT
EXPOSE 2019
# Mon, 24 May 2021 17:41:57 GMT
WORKDIR /srv
# Mon, 24 May 2021 17:41:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db3c8b812fcb0d1bfd42c16c2e9ac68f4f3006382c5362e969d1c9eb3a9fab5`  
		Last Modified: Wed, 14 Apr 2021 20:08:26 GMT  
		Size: 300.8 KB (300847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba030675d7bb5bc251d93896d2c81ed8a2f4f4ef2e8e84ad7dfdce9886387c`  
		Last Modified: Mon, 10 May 2021 23:42:29 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03e81629e078650b941a4beb267a6755133e90fa22a688bffb5df188e069c55`  
		Last Modified: Mon, 24 May 2021 17:42:37 GMT  
		Size: 11.0 MB (11029189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbee1e7ec347a65e5e78b46b8fe541241e3f6c13a468785945abd0aaba24545`  
		Last Modified: Mon, 24 May 2021 17:42:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.1-builder`

```console
$ docker pull caddy@sha256:7e7f52b8b3e06a36bc4b32d552b0b2b30dc863461d3250a691fae68fc89c841b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `caddy:2.4.1-builder` - linux; amd64

```console
$ docker pull caddy@sha256:acb1d8e470fc9d3be900f5a534a57d59d7e827ad2a4fabbedbacde1d08e850ee
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116540780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eafee2350c73e5c74f40dc4ff4146d3ac64f52d221205b317621567780641a34`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:27:12 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 21:27:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 21:27:13 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:46:27 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 01:48:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 01:48:48 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 01:48:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:48:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 01:48:50 GMT
WORKDIR /go
# Fri, 04 Jun 2021 02:18:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 02:18:24 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 02:18:25 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 02:18:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 02:18:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 02:18:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 02:18:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adcc1eea9eeabb6de296adb3e0c1b0722cf13251ff3e4e2d0a5f7ed8e3d48342`  
		Last Modified: Wed, 14 Apr 2021 21:35:06 GMT  
		Size: 281.3 KB (281269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4ab2625f07be8d5c6e48046a05ff3ecc7f374b794a926fb62247b66b511909`  
		Last Modified: Wed, 14 Apr 2021 21:35:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689510d40a2658530c96a39b304e1561733255af89b84ce6de9f489b3ca1a281`  
		Last Modified: Fri, 04 Jun 2021 01:59:43 GMT  
		Size: 105.7 MB (105740137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4d89f102e3b1bb1c586ebf1bf8ab36d3a58ed7793fdb0f6ceca00bc2b177cd`  
		Last Modified: Fri, 04 Jun 2021 01:59:25 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44fa7996470329a7e8174cb5cbaa52ade2eb5fffabe426b05cab3d2c904e6e0`  
		Last Modified: Fri, 04 Jun 2021 02:19:02 GMT  
		Size: 6.4 MB (6395534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26081f37d859cc0d0f0882b13352f2ef140940d73620b130154c91355054b525`  
		Last Modified: Fri, 04 Jun 2021 02:19:02 GMT  
		Size: 1.3 MB (1311156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0133abdd19ffca66008a8732eca2edf1f571ed52fe2b3d873ed8158282f9f7`  
		Last Modified: Fri, 04 Jun 2021 02:19:01 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:9c6cfad074c68103b20a26d1f2da9f0f8f22b5406a356e5696e1856cf3e5c332
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112301607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfd32aee08fd69ca7dcd229bd475cce45176a90ef6154a872d01333b97e2119c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Fri, 04 Jun 2021 05:29:59 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 04 Jun 2021 05:30:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 04 Jun 2021 05:30:00 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 05:30:00 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 05:32:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 05:33:00 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 05:33:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 05:33:01 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 05:33:01 GMT
WORKDIR /go
# Fri, 04 Jun 2021 07:35:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 07:35:01 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 07:35:01 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 07:35:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 07:35:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 07:35:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 07:35:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90c33f298071ceb1106bce90623a7fe87a3be8510fe9512966f1a7bc5625a47`  
		Last Modified: Fri, 04 Jun 2021 05:41:55 GMT  
		Size: 281.4 KB (281382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f381ff0ec8799fc86bf65aba1711ab973cc107a53a6d134a9a0ba3267477a0fb`  
		Last Modified: Fri, 04 Jun 2021 05:41:55 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d5ab13bd0ab2cb8b8b4b1e08587ddb255e3d3bd2cebd7fcb8ba562bb0974d5`  
		Last Modified: Fri, 04 Jun 2021 05:42:20 GMT  
		Size: 101.9 MB (101944742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2d1d4b06a01686239e04dc869317cdd368448fe45334d9838856be1d149dae`  
		Last Modified: Fri, 04 Jun 2021 05:41:55 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fad5cba6f9b7a0e238d430bcd3ce8b3fc12e6bdc8cdb46008ce5a932e27f229`  
		Last Modified: Fri, 04 Jun 2021 07:36:16 GMT  
		Size: 6.2 MB (6230964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed25c6ff0ab0732ac72d5202c79100508522040b20b4ef01be1fb5e20210ae85`  
		Last Modified: Fri, 04 Jun 2021 07:36:15 GMT  
		Size: 1.2 MB (1221675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c309325d1d11d3a67efbffdd774a27af11a477b9ab43b25e95912d6d72b5c652`  
		Last Modified: Fri, 04 Jun 2021 07:36:15 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:3ce06d10a24fe566699c8997bc0c089e851e46c0f69fa0fff18d0085b4346289
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111232949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cde3b1d7cb6f225fb3b4f3064f07e8f9186fcbff0ecb697e5aa10d00899ea6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 27 May 2021 15:06:45 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 27 May 2021 15:06:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 May 2021 15:06:46 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 07:52:57 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 07:55:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 07:55:34 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 07:55:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 07:55:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 07:55:36 GMT
WORKDIR /go
# Fri, 04 Jun 2021 12:06:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 12:06:59 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 12:06:59 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 12:06:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 12:07:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 12:07:01 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 12:07:01 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7339ea1d6bf57b602a207a1e2f24e2f2d6d0fef53ac31afc17a550368c53e63b`  
		Last Modified: Thu, 27 May 2021 15:19:37 GMT  
		Size: 280.5 KB (280537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c586fedb7a1526f50c1bb5ccadd41167254abbdf9cc445264c5a2cda55bff7f3`  
		Last Modified: Thu, 27 May 2021 15:19:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac424f1791899264fd7faf16b2b868022b332df5c89c65ab7bd4da634a0debcc`  
		Last Modified: Fri, 04 Jun 2021 08:07:59 GMT  
		Size: 101.7 MB (101746953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ea8b8d5ee549723867d0f8a4a54e81bc6e8cffef6b2e29cd0efa53f44d75ae`  
		Last Modified: Fri, 04 Jun 2021 08:07:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73f5e95932571acfe6d65aba85701fb9e0a60e6aef82a4d1eeeeab75717fb1`  
		Last Modified: Fri, 04 Jun 2021 12:08:13 GMT  
		Size: 5.6 MB (5561103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c649a927d5a9a52469a77c3ba79e77cc5b94865a1f8d1085843dbd50573897e3`  
		Last Modified: Fri, 04 Jun 2021 12:08:13 GMT  
		Size: 1.2 MB (1219497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7604724e4d7dadae83d4d023c9f2101e6dcd59c058928794c12cc23a4f34d7f`  
		Last Modified: Fri, 04 Jun 2021 12:08:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5dc91099db737a46c5bb7ca6fe3c0174e49874c492ff48e5eac5fc30a579864b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111775816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73671d0a54a8053b75985bb11523edbe1e3877082dede6664d842d058fc6048b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 27 May 2021 22:17:28 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 27 May 2021 22:17:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 May 2021 22:17:29 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 04:00:14 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 04:01:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 04:01:36 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 04:01:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 04:01:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 04:01:37 GMT
WORKDIR /go
# Fri, 04 Jun 2021 07:44:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 07:44:36 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 07:44:36 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 07:44:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 07:44:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 07:44:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 07:44:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3088b5b3c5c0fab79ca41c188d3696a5053778b6c7d602b2aea8084c094608d1`  
		Last Modified: Thu, 27 May 2021 22:26:43 GMT  
		Size: 281.5 KB (281495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7225fbf94c881dc50b56f5430522fbde8891efa801909d5d9f06261d839cc5`  
		Last Modified: Thu, 27 May 2021 22:26:43 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba82ee9f976e7f9d818f11b866566f142f7ceddface2c0d3d5fe3a6920cc659d`  
		Last Modified: Fri, 04 Jun 2021 04:09:30 GMT  
		Size: 101.1 MB (101096027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506bd15cee9f23181bcd604afe8ec2b150b0321d4d0e741e272734456560caac`  
		Last Modified: Fri, 04 Jun 2021 04:09:12 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83fba387ff0d0e9e65223a37bf6a1e09e7e24774a900e99f743e8c3d455f4fdb`  
		Last Modified: Fri, 04 Jun 2021 07:45:32 GMT  
		Size: 6.5 MB (6484015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84ec75c54b55467ea07ae1ace7ace92b52355954733f1ecbd86d26937d03364`  
		Last Modified: Fri, 04 Jun 2021 07:45:31 GMT  
		Size: 1.2 MB (1201540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91117b691ccdbc0552460233c27811b1de617ff3bc78eac7af1f1f70d7b6f6cb`  
		Last Modified: Fri, 04 Jun 2021 07:45:31 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:7f735b71e3863db84fafaaef6c3299cd3f902d9d99504589d7d8b77ed30fdd1b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110613992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ead49008853a08fc29f3178cf58d7cfcb85b1d9dd361879df0f96cf640dcc94`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:53:57 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 22:54:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:54:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 03:07:09 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 03:08:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 03:09:08 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 03:09:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 03:09:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 03:09:30 GMT
WORKDIR /go
# Fri, 04 Jun 2021 09:16:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 09:16:18 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 09:16:26 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 09:16:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 09:16:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 09:16:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 09:16:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf726c40dc4802009a4b6f0f7947c86242c2c078623e8f1f21343864093b3a9`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 283.4 KB (283413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c17712dac96942b05a27f88ea5346bd57b4cabdb33c153562ef144635225b3`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6104245b6f3bb2cd73fecb2ee6ef3347bedc6f588475449849c4229c3321eb8`  
		Last Modified: Fri, 04 Jun 2021 03:20:31 GMT  
		Size: 99.5 MB (99515576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c228774385f5c8b0c6ad74f4b22b8976926d85634278c36ba33b49f23ac5154`  
		Last Modified: Fri, 04 Jun 2021 03:20:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af27e8f9d4959b48b81f61cb0d645eccfd256ee74635e0396fac0b732c0e57b`  
		Last Modified: Fri, 04 Jun 2021 09:17:36 GMT  
		Size: 6.8 MB (6830629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d43d75e1cc7759d079bd9ad4389f4cd3b79a036ff24add605969b915d46114`  
		Last Modified: Fri, 04 Jun 2021 09:17:35 GMT  
		Size: 1.2 MB (1170519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd193d55e35894d2beb5854ebb790227fb34a033785effbaa520604e248480c`  
		Last Modified: Fri, 04 Jun 2021 09:17:35 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1-builder` - linux; s390x

```console
$ docker pull caddy@sha256:bb5f24094fadd35d4c5940a0c1f143d212544334b9bce93de93677dbabe4db16
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115475353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23250df470a63b89f2a4832f806630ba5002e9595baed80673428d73b9b8e8a9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:45:11 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:45:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:45:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:26:42 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 01:28:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 01:28:34 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 01:28:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:28:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 01:28:36 GMT
WORKDIR /go
# Fri, 04 Jun 2021 03:02:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 03:02:56 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 03:02:56 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 03:02:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 03:02:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 03:03:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 03:03:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc746875ae346ee6ec3c9080f8a7a50bef3899ea9d5ae9dac45a81bfe861c9d`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 281.7 KB (281708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0242688236000dd8f33d16f89f36da3ef1bb2a7a32bb59a7eb97a18ed3d5158`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0ff47eca4941b373fedcfb40530f4d5ef82aed9a9b83bd7fa6cee6546112fd`  
		Last Modified: Fri, 04 Jun 2021 01:37:12 GMT  
		Size: 104.8 MB (104846719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6991fc153a27c9de6b023272f31bf22b708f788131bd628abeb30592007377a8`  
		Last Modified: Fri, 04 Jun 2021 01:36:59 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b452ba9be082c7a2255414c44dde4b275a327b14d24e947901062089bd7ebf43`  
		Last Modified: Fri, 04 Jun 2021 03:03:37 GMT  
		Size: 6.5 MB (6479039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507d613df3c6f7ea5929ebfe6205e87ae1b89cd044677a765da66d135bb7ef57`  
		Last Modified: Fri, 04 Jun 2021 03:03:37 GMT  
		Size: 1.3 MB (1264524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd9e1c527bba47d9aa0c07957cb156d2c1d205ca81c81e8b00b5b9c0330290b`  
		Last Modified: Fri, 04 Jun 2021 03:03:36 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1-builder` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:0cba0bbebbf26fbfe27a39006a093cfb426976baff4e8c3ec906a2a229be9e69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2808421770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c51b9b016f1a3599a109e39809816252f59ecd94d60ef1b7043ab7404059d79`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 12:10:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 12:37:22 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Jun 2021 12:37:25 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Jun 2021 12:37:29 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Jun 2021 12:37:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Jun 2021 12:38:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:38:25 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Jun 2021 12:38:51 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Jun 2021 12:38:53 GMT
ENV GOLANG_VERSION=1.16.5
# Wed, 09 Jun 2021 12:41:22 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:41:27 GMT
WORKDIR C:\gopath
# Wed, 09 Jun 2021 20:15:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:15:04 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 09 Jun 2021 20:15:06 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:15:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Jun 2021 20:15:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Jun 2021 20:15:46 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7863ef96846d497ea06fe442ea13dcecaf5c248ce238c69800475281a4fa848e`  
		Last Modified: Wed, 09 Jun 2021 12:20:41 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f985a0b4390580a94aa3cbc8ecb01fc33805bb3304c4217dc5ec9fb6626011ca`  
		Last Modified: Wed, 09 Jun 2021 13:03:26 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5adf5cc2989b1cf730e7993bd088f778b31b33bac78f6d9c133226f7bcf4a6`  
		Last Modified: Wed, 09 Jun 2021 13:03:24 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480b981517ab26b6ee7e090e51d040995ac5a6a55410880ea3f0c8255dada3bc`  
		Last Modified: Wed, 09 Jun 2021 13:03:24 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a372a8dcfb8f1152565f4b8c928c202db247ddc21fd9a35838a2278c65ff6f`  
		Last Modified: Wed, 09 Jun 2021 13:03:23 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97090ffba94bc8afc85a54e404c8aca13253969fe01c8b0ac1f8ce3a0b909953`  
		Last Modified: Wed, 09 Jun 2021 13:03:53 GMT  
		Size: 25.4 MB (25445694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb1c026791860f230531a960e59a35d86f3ae617c5b6ad60155718694ed3720`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fca536252ace3ea8e08bcd38a313ad63d7d308f4a1d24734c324d191b65647`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 314.6 KB (314587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3865edd5ab3e6e2858d35fea90d96f24eb95579b3bb7f95674954df09b428a8e`  
		Last Modified: Wed, 09 Jun 2021 13:03:20 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424a1b81819edd902af8893d485a39318ee4023db4db6f9c73ebb8470a5c2310`  
		Last Modified: Wed, 09 Jun 2021 13:03:58 GMT  
		Size: 139.4 MB (139355479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f54cc4fcf8b7300908d2cb4aa6dbfe433cc614c35c200ca655b96d576a40412`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 1.6 KB (1596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ae8d8d0f1afc3ddbfe8673534bd1ae7afdf7662fb5fd73ef017088a251e15c`  
		Last Modified: Wed, 09 Jun 2021 20:20:23 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761852a93f82584033e99d58efb7a7e5fad44135d49f23090e1217932f809891`  
		Last Modified: Wed, 09 Jun 2021 20:20:20 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f24be856334e97a03392fc575807609b5afd8808514d9ca8305700e72834ea`  
		Last Modified: Wed, 09 Jun 2021 20:20:20 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047b293c2c055e53ea3099cdc7cd511d55cb43391cbcfd34e0c3a96ac1d179ca`  
		Last Modified: Wed, 09 Jun 2021 20:20:20 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2806e8d39eec5d338e88005243d0a11fcb7c24dab13df4ee3c5ce9ee0266dd9`  
		Last Modified: Wed, 09 Jun 2021 20:20:21 GMT  
		Size: 1.7 MB (1703136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de952f0fc6af6d7eea8c8d4d424cf97622e0b2628a32387976f4dc8df54efb8`  
		Last Modified: Wed, 09 Jun 2021 20:20:20 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1-builder` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:4481a6011b8d50eca815372f7a8f28afaae493233d49d4ec20b3d3a5abf93fc7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6437000457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4919458e8d791f772cd7dd820598edd51cc401fa898c7e4ddddc19e6bb2890fe`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 12:41:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 12:41:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Jun 2021 12:41:43 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Jun 2021 12:41:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Jun 2021 12:41:49 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Jun 2021 12:44:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:44:27 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Jun 2021 12:45:49 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Jun 2021 12:45:51 GMT
ENV GOLANG_VERSION=1.16.5
# Wed, 09 Jun 2021 12:49:20 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:49:24 GMT
WORKDIR C:\gopath
# Wed, 09 Jun 2021 20:15:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:15:56 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 09 Jun 2021 20:15:59 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:16:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Jun 2021 20:17:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Jun 2021 20:17:28 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c82e82e95dbad4ccc260b42e03767eb07222e2f00ec57a69b3c87b17da1d2fd3`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a881968e28f8c2900b00800a0de406d0e98740558d9564ad738d053e63d9a1e`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab71df915cf7ac4c559039a917269e11faab2d0e6862a01408431df7fb40362f`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82ce560dcbc3235ed87d6c938aa761616dbd299188ae53a51a266eb37f381f6`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bee5ea2f89fe3f3e514b8dfcd823da340447b633c6048e00773d1c30fbbc0e9`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad71deb840b73610184070ebc7c566bd1dac9cc309d53679460697243bab7640`  
		Last Modified: Wed, 09 Jun 2021 13:04:50 GMT  
		Size: 25.4 MB (25441204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16f2a89ed7a230471eb96b67829deb255795564010b0ff2de47179cdfdec1d0`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cc755175ec255452c16e1e41cc78a8cd719d65f70221e7d128c1dc18eec8f2`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 307.7 KB (307689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d153904f724dbfda646a6c5ccdc1eed2545cf7777c8650461abdedafe75bc693`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ec88320a2e6bf1cfef8856b9271f7d2fa4d2ae8e0eb5b9a44175d04a725631`  
		Last Modified: Wed, 09 Jun 2021 13:04:58 GMT  
		Size: 143.8 MB (143821249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419b516d300f276d9a3f98a1d2c47394abb00b15edeaadcb2f5d0ecee3380f14`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 1.6 KB (1576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d420a2d4c5bca557510bd5eaeea0268b05bb6e61104acea0af1e28c7537c8352`  
		Last Modified: Wed, 09 Jun 2021 20:20:41 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06bf21d106193b12d0b9a688698ec718f7fb4514f317565933b89f22da0d1de`  
		Last Modified: Wed, 09 Jun 2021 20:20:38 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64471c2fb9e42024fce3859860cf6a05f584b8c21ff5c776f7c285588f1117fc`  
		Last Modified: Wed, 09 Jun 2021 20:20:38 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f2c847c9bab79f9970336a628d5b7948504e3f2a67f95cac9a1a3f12132673`  
		Last Modified: Wed, 09 Jun 2021 20:20:38 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae1157ef3d362883b0503349e9d7cb6d729fa420af63a826262dca25f7a9fc`  
		Last Modified: Wed, 09 Jun 2021 20:20:39 GMT  
		Size: 1.7 MB (1684468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e122b3fd6e41cb67b3d9b46e55753aa37f1f60c2de7fab150181822a556d2791`  
		Last Modified: Wed, 09 Jun 2021 20:20:38 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.1-builder-alpine`

```console
$ docker pull caddy@sha256:4b4685dba38126a1d8dc692a9cc3f60e145e085f5f2a132b32bdbbcec0109a55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.4.1-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:acb1d8e470fc9d3be900f5a534a57d59d7e827ad2a4fabbedbacde1d08e850ee
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116540780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eafee2350c73e5c74f40dc4ff4146d3ac64f52d221205b317621567780641a34`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:27:12 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 21:27:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 21:27:13 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:46:27 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 01:48:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 01:48:48 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 01:48:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:48:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 01:48:50 GMT
WORKDIR /go
# Fri, 04 Jun 2021 02:18:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 02:18:24 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 02:18:25 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 02:18:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 02:18:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 02:18:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 02:18:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adcc1eea9eeabb6de296adb3e0c1b0722cf13251ff3e4e2d0a5f7ed8e3d48342`  
		Last Modified: Wed, 14 Apr 2021 21:35:06 GMT  
		Size: 281.3 KB (281269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4ab2625f07be8d5c6e48046a05ff3ecc7f374b794a926fb62247b66b511909`  
		Last Modified: Wed, 14 Apr 2021 21:35:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689510d40a2658530c96a39b304e1561733255af89b84ce6de9f489b3ca1a281`  
		Last Modified: Fri, 04 Jun 2021 01:59:43 GMT  
		Size: 105.7 MB (105740137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4d89f102e3b1bb1c586ebf1bf8ab36d3a58ed7793fdb0f6ceca00bc2b177cd`  
		Last Modified: Fri, 04 Jun 2021 01:59:25 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44fa7996470329a7e8174cb5cbaa52ade2eb5fffabe426b05cab3d2c904e6e0`  
		Last Modified: Fri, 04 Jun 2021 02:19:02 GMT  
		Size: 6.4 MB (6395534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26081f37d859cc0d0f0882b13352f2ef140940d73620b130154c91355054b525`  
		Last Modified: Fri, 04 Jun 2021 02:19:02 GMT  
		Size: 1.3 MB (1311156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0133abdd19ffca66008a8732eca2edf1f571ed52fe2b3d873ed8158282f9f7`  
		Last Modified: Fri, 04 Jun 2021 02:19:01 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:9c6cfad074c68103b20a26d1f2da9f0f8f22b5406a356e5696e1856cf3e5c332
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112301607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfd32aee08fd69ca7dcd229bd475cce45176a90ef6154a872d01333b97e2119c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Fri, 04 Jun 2021 05:29:59 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 04 Jun 2021 05:30:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 04 Jun 2021 05:30:00 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 05:30:00 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 05:32:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 05:33:00 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 05:33:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 05:33:01 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 05:33:01 GMT
WORKDIR /go
# Fri, 04 Jun 2021 07:35:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 07:35:01 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 07:35:01 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 07:35:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 07:35:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 07:35:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 07:35:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90c33f298071ceb1106bce90623a7fe87a3be8510fe9512966f1a7bc5625a47`  
		Last Modified: Fri, 04 Jun 2021 05:41:55 GMT  
		Size: 281.4 KB (281382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f381ff0ec8799fc86bf65aba1711ab973cc107a53a6d134a9a0ba3267477a0fb`  
		Last Modified: Fri, 04 Jun 2021 05:41:55 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d5ab13bd0ab2cb8b8b4b1e08587ddb255e3d3bd2cebd7fcb8ba562bb0974d5`  
		Last Modified: Fri, 04 Jun 2021 05:42:20 GMT  
		Size: 101.9 MB (101944742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2d1d4b06a01686239e04dc869317cdd368448fe45334d9838856be1d149dae`  
		Last Modified: Fri, 04 Jun 2021 05:41:55 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fad5cba6f9b7a0e238d430bcd3ce8b3fc12e6bdc8cdb46008ce5a932e27f229`  
		Last Modified: Fri, 04 Jun 2021 07:36:16 GMT  
		Size: 6.2 MB (6230964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed25c6ff0ab0732ac72d5202c79100508522040b20b4ef01be1fb5e20210ae85`  
		Last Modified: Fri, 04 Jun 2021 07:36:15 GMT  
		Size: 1.2 MB (1221675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c309325d1d11d3a67efbffdd774a27af11a477b9ab43b25e95912d6d72b5c652`  
		Last Modified: Fri, 04 Jun 2021 07:36:15 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:3ce06d10a24fe566699c8997bc0c089e851e46c0f69fa0fff18d0085b4346289
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111232949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cde3b1d7cb6f225fb3b4f3064f07e8f9186fcbff0ecb697e5aa10d00899ea6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 27 May 2021 15:06:45 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 27 May 2021 15:06:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 May 2021 15:06:46 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 07:52:57 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 07:55:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 07:55:34 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 07:55:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 07:55:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 07:55:36 GMT
WORKDIR /go
# Fri, 04 Jun 2021 12:06:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 12:06:59 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 12:06:59 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 12:06:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 12:07:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 12:07:01 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 12:07:01 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7339ea1d6bf57b602a207a1e2f24e2f2d6d0fef53ac31afc17a550368c53e63b`  
		Last Modified: Thu, 27 May 2021 15:19:37 GMT  
		Size: 280.5 KB (280537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c586fedb7a1526f50c1bb5ccadd41167254abbdf9cc445264c5a2cda55bff7f3`  
		Last Modified: Thu, 27 May 2021 15:19:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac424f1791899264fd7faf16b2b868022b332df5c89c65ab7bd4da634a0debcc`  
		Last Modified: Fri, 04 Jun 2021 08:07:59 GMT  
		Size: 101.7 MB (101746953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ea8b8d5ee549723867d0f8a4a54e81bc6e8cffef6b2e29cd0efa53f44d75ae`  
		Last Modified: Fri, 04 Jun 2021 08:07:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73f5e95932571acfe6d65aba85701fb9e0a60e6aef82a4d1eeeeab75717fb1`  
		Last Modified: Fri, 04 Jun 2021 12:08:13 GMT  
		Size: 5.6 MB (5561103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c649a927d5a9a52469a77c3ba79e77cc5b94865a1f8d1085843dbd50573897e3`  
		Last Modified: Fri, 04 Jun 2021 12:08:13 GMT  
		Size: 1.2 MB (1219497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7604724e4d7dadae83d4d023c9f2101e6dcd59c058928794c12cc23a4f34d7f`  
		Last Modified: Fri, 04 Jun 2021 12:08:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5dc91099db737a46c5bb7ca6fe3c0174e49874c492ff48e5eac5fc30a579864b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111775816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73671d0a54a8053b75985bb11523edbe1e3877082dede6664d842d058fc6048b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 27 May 2021 22:17:28 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 27 May 2021 22:17:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 May 2021 22:17:29 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 04:00:14 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 04:01:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 04:01:36 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 04:01:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 04:01:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 04:01:37 GMT
WORKDIR /go
# Fri, 04 Jun 2021 07:44:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 07:44:36 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 07:44:36 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 07:44:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 07:44:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 07:44:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 07:44:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3088b5b3c5c0fab79ca41c188d3696a5053778b6c7d602b2aea8084c094608d1`  
		Last Modified: Thu, 27 May 2021 22:26:43 GMT  
		Size: 281.5 KB (281495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7225fbf94c881dc50b56f5430522fbde8891efa801909d5d9f06261d839cc5`  
		Last Modified: Thu, 27 May 2021 22:26:43 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba82ee9f976e7f9d818f11b866566f142f7ceddface2c0d3d5fe3a6920cc659d`  
		Last Modified: Fri, 04 Jun 2021 04:09:30 GMT  
		Size: 101.1 MB (101096027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506bd15cee9f23181bcd604afe8ec2b150b0321d4d0e741e272734456560caac`  
		Last Modified: Fri, 04 Jun 2021 04:09:12 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83fba387ff0d0e9e65223a37bf6a1e09e7e24774a900e99f743e8c3d455f4fdb`  
		Last Modified: Fri, 04 Jun 2021 07:45:32 GMT  
		Size: 6.5 MB (6484015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84ec75c54b55467ea07ae1ace7ace92b52355954733f1ecbd86d26937d03364`  
		Last Modified: Fri, 04 Jun 2021 07:45:31 GMT  
		Size: 1.2 MB (1201540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91117b691ccdbc0552460233c27811b1de617ff3bc78eac7af1f1f70d7b6f6cb`  
		Last Modified: Fri, 04 Jun 2021 07:45:31 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:7f735b71e3863db84fafaaef6c3299cd3f902d9d99504589d7d8b77ed30fdd1b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110613992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ead49008853a08fc29f3178cf58d7cfcb85b1d9dd361879df0f96cf640dcc94`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:53:57 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 22:54:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:54:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 03:07:09 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 03:08:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 03:09:08 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 03:09:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 03:09:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 03:09:30 GMT
WORKDIR /go
# Fri, 04 Jun 2021 09:16:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 09:16:18 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 09:16:26 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 09:16:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 09:16:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 09:16:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 09:16:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf726c40dc4802009a4b6f0f7947c86242c2c078623e8f1f21343864093b3a9`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 283.4 KB (283413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c17712dac96942b05a27f88ea5346bd57b4cabdb33c153562ef144635225b3`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6104245b6f3bb2cd73fecb2ee6ef3347bedc6f588475449849c4229c3321eb8`  
		Last Modified: Fri, 04 Jun 2021 03:20:31 GMT  
		Size: 99.5 MB (99515576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c228774385f5c8b0c6ad74f4b22b8976926d85634278c36ba33b49f23ac5154`  
		Last Modified: Fri, 04 Jun 2021 03:20:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af27e8f9d4959b48b81f61cb0d645eccfd256ee74635e0396fac0b732c0e57b`  
		Last Modified: Fri, 04 Jun 2021 09:17:36 GMT  
		Size: 6.8 MB (6830629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d43d75e1cc7759d079bd9ad4389f4cd3b79a036ff24add605969b915d46114`  
		Last Modified: Fri, 04 Jun 2021 09:17:35 GMT  
		Size: 1.2 MB (1170519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd193d55e35894d2beb5854ebb790227fb34a033785effbaa520604e248480c`  
		Last Modified: Fri, 04 Jun 2021 09:17:35 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:bb5f24094fadd35d4c5940a0c1f143d212544334b9bce93de93677dbabe4db16
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115475353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23250df470a63b89f2a4832f806630ba5002e9595baed80673428d73b9b8e8a9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:45:11 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:45:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:45:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:26:42 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 01:28:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 01:28:34 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 01:28:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:28:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 01:28:36 GMT
WORKDIR /go
# Fri, 04 Jun 2021 03:02:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 03:02:56 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 03:02:56 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 03:02:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 03:02:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 03:03:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 03:03:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc746875ae346ee6ec3c9080f8a7a50bef3899ea9d5ae9dac45a81bfe861c9d`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 281.7 KB (281708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0242688236000dd8f33d16f89f36da3ef1bb2a7a32bb59a7eb97a18ed3d5158`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0ff47eca4941b373fedcfb40530f4d5ef82aed9a9b83bd7fa6cee6546112fd`  
		Last Modified: Fri, 04 Jun 2021 01:37:12 GMT  
		Size: 104.8 MB (104846719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6991fc153a27c9de6b023272f31bf22b708f788131bd628abeb30592007377a8`  
		Last Modified: Fri, 04 Jun 2021 01:36:59 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b452ba9be082c7a2255414c44dde4b275a327b14d24e947901062089bd7ebf43`  
		Last Modified: Fri, 04 Jun 2021 03:03:37 GMT  
		Size: 6.5 MB (6479039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507d613df3c6f7ea5929ebfe6205e87ae1b89cd044677a765da66d135bb7ef57`  
		Last Modified: Fri, 04 Jun 2021 03:03:37 GMT  
		Size: 1.3 MB (1264524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd9e1c527bba47d9aa0c07957cb156d2c1d205ca81c81e8b00b5b9c0330290b`  
		Last Modified: Fri, 04 Jun 2021 03:03:36 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.1-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:5c8e1831e4df2e628cf1bf9d35260d624c1b15d27abfac59a5431f15f3d0a66a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `caddy:2.4.1-builder-windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:0cba0bbebbf26fbfe27a39006a093cfb426976baff4e8c3ec906a2a229be9e69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2808421770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c51b9b016f1a3599a109e39809816252f59ecd94d60ef1b7043ab7404059d79`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 12:10:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 12:37:22 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Jun 2021 12:37:25 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Jun 2021 12:37:29 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Jun 2021 12:37:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Jun 2021 12:38:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:38:25 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Jun 2021 12:38:51 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Jun 2021 12:38:53 GMT
ENV GOLANG_VERSION=1.16.5
# Wed, 09 Jun 2021 12:41:22 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:41:27 GMT
WORKDIR C:\gopath
# Wed, 09 Jun 2021 20:15:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:15:04 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 09 Jun 2021 20:15:06 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:15:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Jun 2021 20:15:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Jun 2021 20:15:46 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7863ef96846d497ea06fe442ea13dcecaf5c248ce238c69800475281a4fa848e`  
		Last Modified: Wed, 09 Jun 2021 12:20:41 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f985a0b4390580a94aa3cbc8ecb01fc33805bb3304c4217dc5ec9fb6626011ca`  
		Last Modified: Wed, 09 Jun 2021 13:03:26 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5adf5cc2989b1cf730e7993bd088f778b31b33bac78f6d9c133226f7bcf4a6`  
		Last Modified: Wed, 09 Jun 2021 13:03:24 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480b981517ab26b6ee7e090e51d040995ac5a6a55410880ea3f0c8255dada3bc`  
		Last Modified: Wed, 09 Jun 2021 13:03:24 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a372a8dcfb8f1152565f4b8c928c202db247ddc21fd9a35838a2278c65ff6f`  
		Last Modified: Wed, 09 Jun 2021 13:03:23 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97090ffba94bc8afc85a54e404c8aca13253969fe01c8b0ac1f8ce3a0b909953`  
		Last Modified: Wed, 09 Jun 2021 13:03:53 GMT  
		Size: 25.4 MB (25445694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb1c026791860f230531a960e59a35d86f3ae617c5b6ad60155718694ed3720`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fca536252ace3ea8e08bcd38a313ad63d7d308f4a1d24734c324d191b65647`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 314.6 KB (314587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3865edd5ab3e6e2858d35fea90d96f24eb95579b3bb7f95674954df09b428a8e`  
		Last Modified: Wed, 09 Jun 2021 13:03:20 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424a1b81819edd902af8893d485a39318ee4023db4db6f9c73ebb8470a5c2310`  
		Last Modified: Wed, 09 Jun 2021 13:03:58 GMT  
		Size: 139.4 MB (139355479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f54cc4fcf8b7300908d2cb4aa6dbfe433cc614c35c200ca655b96d576a40412`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 1.6 KB (1596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ae8d8d0f1afc3ddbfe8673534bd1ae7afdf7662fb5fd73ef017088a251e15c`  
		Last Modified: Wed, 09 Jun 2021 20:20:23 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761852a93f82584033e99d58efb7a7e5fad44135d49f23090e1217932f809891`  
		Last Modified: Wed, 09 Jun 2021 20:20:20 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f24be856334e97a03392fc575807609b5afd8808514d9ca8305700e72834ea`  
		Last Modified: Wed, 09 Jun 2021 20:20:20 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047b293c2c055e53ea3099cdc7cd511d55cb43391cbcfd34e0c3a96ac1d179ca`  
		Last Modified: Wed, 09 Jun 2021 20:20:20 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2806e8d39eec5d338e88005243d0a11fcb7c24dab13df4ee3c5ce9ee0266dd9`  
		Last Modified: Wed, 09 Jun 2021 20:20:21 GMT  
		Size: 1.7 MB (1703136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de952f0fc6af6d7eea8c8d4d424cf97622e0b2628a32387976f4dc8df54efb8`  
		Last Modified: Wed, 09 Jun 2021 20:20:20 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.1-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:be2e88c1df8f07111be41e7303360a3a48b2c80edee366850af00d9df909afdb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `caddy:2.4.1-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:4481a6011b8d50eca815372f7a8f28afaae493233d49d4ec20b3d3a5abf93fc7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6437000457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4919458e8d791f772cd7dd820598edd51cc401fa898c7e4ddddc19e6bb2890fe`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 12:41:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 12:41:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Jun 2021 12:41:43 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Jun 2021 12:41:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Jun 2021 12:41:49 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Jun 2021 12:44:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:44:27 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Jun 2021 12:45:49 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Jun 2021 12:45:51 GMT
ENV GOLANG_VERSION=1.16.5
# Wed, 09 Jun 2021 12:49:20 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:49:24 GMT
WORKDIR C:\gopath
# Wed, 09 Jun 2021 20:15:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:15:56 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 09 Jun 2021 20:15:59 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:16:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Jun 2021 20:17:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Jun 2021 20:17:28 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c82e82e95dbad4ccc260b42e03767eb07222e2f00ec57a69b3c87b17da1d2fd3`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a881968e28f8c2900b00800a0de406d0e98740558d9564ad738d053e63d9a1e`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab71df915cf7ac4c559039a917269e11faab2d0e6862a01408431df7fb40362f`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82ce560dcbc3235ed87d6c938aa761616dbd299188ae53a51a266eb37f381f6`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bee5ea2f89fe3f3e514b8dfcd823da340447b633c6048e00773d1c30fbbc0e9`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad71deb840b73610184070ebc7c566bd1dac9cc309d53679460697243bab7640`  
		Last Modified: Wed, 09 Jun 2021 13:04:50 GMT  
		Size: 25.4 MB (25441204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16f2a89ed7a230471eb96b67829deb255795564010b0ff2de47179cdfdec1d0`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cc755175ec255452c16e1e41cc78a8cd719d65f70221e7d128c1dc18eec8f2`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 307.7 KB (307689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d153904f724dbfda646a6c5ccdc1eed2545cf7777c8650461abdedafe75bc693`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ec88320a2e6bf1cfef8856b9271f7d2fa4d2ae8e0eb5b9a44175d04a725631`  
		Last Modified: Wed, 09 Jun 2021 13:04:58 GMT  
		Size: 143.8 MB (143821249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419b516d300f276d9a3f98a1d2c47394abb00b15edeaadcb2f5d0ecee3380f14`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 1.6 KB (1576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d420a2d4c5bca557510bd5eaeea0268b05bb6e61104acea0af1e28c7537c8352`  
		Last Modified: Wed, 09 Jun 2021 20:20:41 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06bf21d106193b12d0b9a688698ec718f7fb4514f317565933b89f22da0d1de`  
		Last Modified: Wed, 09 Jun 2021 20:20:38 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64471c2fb9e42024fce3859860cf6a05f584b8c21ff5c776f7c285588f1117fc`  
		Last Modified: Wed, 09 Jun 2021 20:20:38 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f2c847c9bab79f9970336a628d5b7948504e3f2a67f95cac9a1a3f12132673`  
		Last Modified: Wed, 09 Jun 2021 20:20:38 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae1157ef3d362883b0503349e9d7cb6d729fa420af63a826262dca25f7a9fc`  
		Last Modified: Wed, 09 Jun 2021 20:20:39 GMT  
		Size: 1.7 MB (1684468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e122b3fd6e41cb67b3d9b46e55753aa37f1f60c2de7fab150181822a556d2791`  
		Last Modified: Wed, 09 Jun 2021 20:20:38 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.1-windowsservercore`

```console
$ docker pull caddy@sha256:3f315a56b68ba9264142c6087b0db8f08492d6a8f90e8f16604e23920a1753fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `caddy:2.4.1-windowsservercore` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:d4a3e0eabf14e4f98a9bcf5eada28d1443573b082afe95028d548d5b88a2b33e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2654170862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:736d3aa581b715efdf7c0431ebfbaed21b664091d8e8f7e4595c5f9dabbd2acb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 12:10:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:08:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Jun 2021 20:08:07 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:08:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Jun 2021 20:08:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Jun 2021 20:08:49 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Jun 2021 20:08:51 GMT
VOLUME [c:/config]
# Wed, 09 Jun 2021 20:08:53 GMT
VOLUME [c:/data]
# Wed, 09 Jun 2021 20:08:55 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 09 Jun 2021 20:08:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Jun 2021 20:09:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Jun 2021 20:09:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Jun 2021 20:09:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Jun 2021 20:09:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Jun 2021 20:09:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Jun 2021 20:09:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Jun 2021 20:09:14 GMT
EXPOSE 80
# Wed, 09 Jun 2021 20:09:17 GMT
EXPOSE 443
# Wed, 09 Jun 2021 20:09:19 GMT
EXPOSE 2019
# Wed, 09 Jun 2021 20:09:41 GMT
RUN caddy version
# Wed, 09 Jun 2021 20:09:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7863ef96846d497ea06fe442ea13dcecaf5c248ce238c69800475281a4fa848e`  
		Last Modified: Wed, 09 Jun 2021 12:20:41 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dc18d712eacfb666370e311daaf51e09fc2f76ca762e4592e149fbe6aba561`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 361.4 KB (361380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b774f6019fa0c611532d02bdf31c54e9da56fe2330e3e0745538ef036cfb87`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e977598d13d0ee9ae780f2cf34706c57e810301d20d9fc8286ad9390b9166b`  
		Last Modified: Wed, 09 Jun 2021 20:19:37 GMT  
		Size: 11.9 MB (11906202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7361692fe34486902f2dd9f69cc3bce54c4cb8c5c86ed80a0d75033f25ae5213`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35d39d3918ab9262122b494a653aec25e76a65396f9198d7be955cb9c26c6f3`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66891a50a919af8d3cb83358a7f8d33b2055c143bd3499cc431fd32d053ed393`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519d446a1689a5424a77bf1cbf0f00153b28c6eff9ee22f0f88e0e32b3f6bda3`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534ea2eef93aa67b4ac4bfb48ac5498fa33b02d0b88b9ae60b8ae159addacecc`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19fc40bc9ade11a1755b185c529e961b474d959d45a44b1b1ab5f12e3d17863a`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ef9960b6bac284e65c351bc447bb8931486a0c1c3ee68c9e5a62828b4ae0e`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cfda8707421463aa0f297ce5d4ac3a615f60caf56e6e69a299caa08a04f7da`  
		Last Modified: Wed, 09 Jun 2021 20:19:29 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa0c9ece6e3482cf3ffc8d9a087d113db0f7c249f59bcf06f3ffc65c5e4bce0`  
		Last Modified: Wed, 09 Jun 2021 20:19:29 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6614223fb410a8262956f73a038f6d79b67d5976fe8740b21dfa2121a9cbd7f2`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f354857e070035731eb660ec35ff9f8549b6cc79211bab40ae642d9875f98f8b`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc94f29a4cb79013fce0bf1a5776868fa31912b598231e46883a114d86f712d3`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e536fde913e2e2d5ae24846adca32195330a9be6e7d1c3180ce7ac6bc6a35ae1`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b11db027637bf7abeec6bbcd83920c4eb7c291aeeae4d2886a1563bf41289a6`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3a70d973d27d739faae877290b3184bee11c706ebd4bfa515d180fba88ef0f`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc7b3e3d99424f8d3737a4502a6f50767ae25b699a315155b98700af682b64f`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 292.6 KB (292631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d435932a64bec158a6193fa4a31a1b38e446ec9f63c0b6be3282c3acf3288949`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1-windowsservercore` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:e7e7af29e7917229552a0c802147dba99fb7a1427b84296a2c60ea7e19cbcb0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278267906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7184db699efd0a2ce0077179784cc7277e5faa7d07534ea1ce32d61d7f46ebc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 12:41:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:11:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Jun 2021 20:11:30 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:13:06 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Jun 2021 20:13:09 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Jun 2021 20:13:11 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Jun 2021 20:13:15 GMT
VOLUME [c:/config]
# Wed, 09 Jun 2021 20:13:18 GMT
VOLUME [c:/data]
# Wed, 09 Jun 2021 20:13:20 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 09 Jun 2021 20:13:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Jun 2021 20:13:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Jun 2021 20:13:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Jun 2021 20:13:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Jun 2021 20:13:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Jun 2021 20:13:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Jun 2021 20:13:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Jun 2021 20:13:40 GMT
EXPOSE 80
# Wed, 09 Jun 2021 20:13:42 GMT
EXPOSE 443
# Wed, 09 Jun 2021 20:13:45 GMT
EXPOSE 2019
# Wed, 09 Jun 2021 20:14:40 GMT
RUN caddy version
# Wed, 09 Jun 2021 20:14:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c82e82e95dbad4ccc260b42e03767eb07222e2f00ec57a69b3c87b17da1d2fd3`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a28e390d3b8e7b9369b102914eaee6e1fa0d14eb258b628be67f99f32f06f81`  
		Last Modified: Wed, 09 Jun 2021 20:20:01 GMT  
		Size: 357.4 KB (357370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7f07987f083e935103f83e47894b93aceaf05d1ded81dd09eb0bc3c8e45af`  
		Last Modified: Wed, 09 Jun 2021 20:20:01 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e65ddfdcdd60907208873b2a532cc58bc0f57d144430cef2c7630e80e4fd1e`  
		Last Modified: Wed, 09 Jun 2021 20:20:05 GMT  
		Size: 11.9 MB (11896985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58e4679b7ef7e1b9d82f44a6b5055c6916801193550bcce3ce390851224c736`  
		Last Modified: Wed, 09 Jun 2021 20:20:00 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107d803623512ea83de929509cc68f334261f2018c60bde60a99eadd0c2b179`  
		Last Modified: Wed, 09 Jun 2021 20:20:00 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f757538ddb020d145715a4890594958e741fe98366f1a58314361e5a8a3487`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462510ee9cb1c642e2804f8f607f02ccc5c31b63c956b9394bf38c5041b10d8b`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e87709f8365472aa7278651dacfc7eee93b24859a494cf6904b4f7ce80df0a`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5439b862b8218f1d7e0e0269efdbed614475ffbdcbaac06a3953f80b07677a1a`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1950c17917c025587fa23872145ee00eaaa11939dc87314c1aa74119db642d`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84164685053ad8b12a46e198ec2e93143d1df956bbbd4af76c88d0f549031c60`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103b7e93d2e2faefef7bd14bc00910442ce8da843f4fb726e2dba2d97752ddc9`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046d1e0cd75d46944ff833afe00c5dc9835ec1eb72876965a98a1488778910a6`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593a0ce075f6e5e07785dd7cd14aa1c274339da4d6f80495f0d1a85fabdef5db`  
		Last Modified: Wed, 09 Jun 2021 20:19:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14f5cdc43c91f65e6c5879691adc6e392d353807b27465a9b270fe7a06da51c`  
		Last Modified: Wed, 09 Jun 2021 20:19:55 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd488f5f58644d68e5103098932448a58d05a716861b26bf33376e75ad27e61`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c218cc3caa4b354c536ad99d30753a6eb41c52a58c52aafc0655a8482382a07`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3dad29a1e0241680f68697c2b0dbca8e85d0084faef4bdd3e66c8294be80671`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daeda652af05f03b2ec029aa5caa6b49d533546fa8347f5b1db003e8a83a7c30`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 260.8 KB (260840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9779c5588bf525e972d3b02ecaeeee32f3939ef8d54e8a16c52e0e62804e2e42`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.1-windowsservercore-1809`

```console
$ docker pull caddy@sha256:699404cfeaf1b53b36b5cad0c6d2fe8858034adb85e80f41f14f9fbe13a22366
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `caddy:2.4.1-windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:d4a3e0eabf14e4f98a9bcf5eada28d1443573b082afe95028d548d5b88a2b33e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2654170862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:736d3aa581b715efdf7c0431ebfbaed21b664091d8e8f7e4595c5f9dabbd2acb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 12:10:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:08:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Jun 2021 20:08:07 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:08:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Jun 2021 20:08:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Jun 2021 20:08:49 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Jun 2021 20:08:51 GMT
VOLUME [c:/config]
# Wed, 09 Jun 2021 20:08:53 GMT
VOLUME [c:/data]
# Wed, 09 Jun 2021 20:08:55 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 09 Jun 2021 20:08:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Jun 2021 20:09:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Jun 2021 20:09:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Jun 2021 20:09:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Jun 2021 20:09:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Jun 2021 20:09:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Jun 2021 20:09:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Jun 2021 20:09:14 GMT
EXPOSE 80
# Wed, 09 Jun 2021 20:09:17 GMT
EXPOSE 443
# Wed, 09 Jun 2021 20:09:19 GMT
EXPOSE 2019
# Wed, 09 Jun 2021 20:09:41 GMT
RUN caddy version
# Wed, 09 Jun 2021 20:09:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7863ef96846d497ea06fe442ea13dcecaf5c248ce238c69800475281a4fa848e`  
		Last Modified: Wed, 09 Jun 2021 12:20:41 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dc18d712eacfb666370e311daaf51e09fc2f76ca762e4592e149fbe6aba561`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 361.4 KB (361380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b774f6019fa0c611532d02bdf31c54e9da56fe2330e3e0745538ef036cfb87`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e977598d13d0ee9ae780f2cf34706c57e810301d20d9fc8286ad9390b9166b`  
		Last Modified: Wed, 09 Jun 2021 20:19:37 GMT  
		Size: 11.9 MB (11906202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7361692fe34486902f2dd9f69cc3bce54c4cb8c5c86ed80a0d75033f25ae5213`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35d39d3918ab9262122b494a653aec25e76a65396f9198d7be955cb9c26c6f3`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66891a50a919af8d3cb83358a7f8d33b2055c143bd3499cc431fd32d053ed393`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519d446a1689a5424a77bf1cbf0f00153b28c6eff9ee22f0f88e0e32b3f6bda3`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534ea2eef93aa67b4ac4bfb48ac5498fa33b02d0b88b9ae60b8ae159addacecc`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19fc40bc9ade11a1755b185c529e961b474d959d45a44b1b1ab5f12e3d17863a`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ef9960b6bac284e65c351bc447bb8931486a0c1c3ee68c9e5a62828b4ae0e`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cfda8707421463aa0f297ce5d4ac3a615f60caf56e6e69a299caa08a04f7da`  
		Last Modified: Wed, 09 Jun 2021 20:19:29 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa0c9ece6e3482cf3ffc8d9a087d113db0f7c249f59bcf06f3ffc65c5e4bce0`  
		Last Modified: Wed, 09 Jun 2021 20:19:29 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6614223fb410a8262956f73a038f6d79b67d5976fe8740b21dfa2121a9cbd7f2`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f354857e070035731eb660ec35ff9f8549b6cc79211bab40ae642d9875f98f8b`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc94f29a4cb79013fce0bf1a5776868fa31912b598231e46883a114d86f712d3`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e536fde913e2e2d5ae24846adca32195330a9be6e7d1c3180ce7ac6bc6a35ae1`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b11db027637bf7abeec6bbcd83920c4eb7c291aeeae4d2886a1563bf41289a6`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3a70d973d27d739faae877290b3184bee11c706ebd4bfa515d180fba88ef0f`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc7b3e3d99424f8d3737a4502a6f50767ae25b699a315155b98700af682b64f`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 292.6 KB (292631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d435932a64bec158a6193fa4a31a1b38e446ec9f63c0b6be3282c3acf3288949`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.1-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:f07a9aef54a1c73076c58ba7037c8840b67601723e6dbf534878e515d02f519d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `caddy:2.4.1-windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:e7e7af29e7917229552a0c802147dba99fb7a1427b84296a2c60ea7e19cbcb0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278267906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7184db699efd0a2ce0077179784cc7277e5faa7d07534ea1ce32d61d7f46ebc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 12:41:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:11:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Jun 2021 20:11:30 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:13:06 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Jun 2021 20:13:09 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Jun 2021 20:13:11 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Jun 2021 20:13:15 GMT
VOLUME [c:/config]
# Wed, 09 Jun 2021 20:13:18 GMT
VOLUME [c:/data]
# Wed, 09 Jun 2021 20:13:20 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 09 Jun 2021 20:13:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Jun 2021 20:13:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Jun 2021 20:13:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Jun 2021 20:13:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Jun 2021 20:13:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Jun 2021 20:13:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Jun 2021 20:13:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Jun 2021 20:13:40 GMT
EXPOSE 80
# Wed, 09 Jun 2021 20:13:42 GMT
EXPOSE 443
# Wed, 09 Jun 2021 20:13:45 GMT
EXPOSE 2019
# Wed, 09 Jun 2021 20:14:40 GMT
RUN caddy version
# Wed, 09 Jun 2021 20:14:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c82e82e95dbad4ccc260b42e03767eb07222e2f00ec57a69b3c87b17da1d2fd3`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a28e390d3b8e7b9369b102914eaee6e1fa0d14eb258b628be67f99f32f06f81`  
		Last Modified: Wed, 09 Jun 2021 20:20:01 GMT  
		Size: 357.4 KB (357370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7f07987f083e935103f83e47894b93aceaf05d1ded81dd09eb0bc3c8e45af`  
		Last Modified: Wed, 09 Jun 2021 20:20:01 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e65ddfdcdd60907208873b2a532cc58bc0f57d144430cef2c7630e80e4fd1e`  
		Last Modified: Wed, 09 Jun 2021 20:20:05 GMT  
		Size: 11.9 MB (11896985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58e4679b7ef7e1b9d82f44a6b5055c6916801193550bcce3ce390851224c736`  
		Last Modified: Wed, 09 Jun 2021 20:20:00 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107d803623512ea83de929509cc68f334261f2018c60bde60a99eadd0c2b179`  
		Last Modified: Wed, 09 Jun 2021 20:20:00 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f757538ddb020d145715a4890594958e741fe98366f1a58314361e5a8a3487`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462510ee9cb1c642e2804f8f607f02ccc5c31b63c956b9394bf38c5041b10d8b`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e87709f8365472aa7278651dacfc7eee93b24859a494cf6904b4f7ce80df0a`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5439b862b8218f1d7e0e0269efdbed614475ffbdcbaac06a3953f80b07677a1a`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1950c17917c025587fa23872145ee00eaaa11939dc87314c1aa74119db642d`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84164685053ad8b12a46e198ec2e93143d1df956bbbd4af76c88d0f549031c60`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103b7e93d2e2faefef7bd14bc00910442ce8da843f4fb726e2dba2d97752ddc9`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046d1e0cd75d46944ff833afe00c5dc9835ec1eb72876965a98a1488778910a6`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593a0ce075f6e5e07785dd7cd14aa1c274339da4d6f80495f0d1a85fabdef5db`  
		Last Modified: Wed, 09 Jun 2021 20:19:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14f5cdc43c91f65e6c5879691adc6e392d353807b27465a9b270fe7a06da51c`  
		Last Modified: Wed, 09 Jun 2021 20:19:55 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd488f5f58644d68e5103098932448a58d05a716861b26bf33376e75ad27e61`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c218cc3caa4b354c536ad99d30753a6eb41c52a58c52aafc0655a8482382a07`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3dad29a1e0241680f68697c2b0dbca8e85d0084faef4bdd3e66c8294be80671`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daeda652af05f03b2ec029aa5caa6b49d533546fa8347f5b1db003e8a83a7c30`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 260.8 KB (260840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9779c5588bf525e972d3b02ecaeeee32f3939ef8d54e8a16c52e0e62804e2e42`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:48e775e759b55c34afd4293c6ec80650a45754a193c8eaa62c6fcddb6f599d45
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
$ docker pull caddy@sha256:c3b2e52162bebaf3b0d128780b3bffc4aa9ccb6953953892dd9d31495e15dc55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14568035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b59636b1388443a36d8173a6ad50dbcf59de4b7786b8178ad9eb656ad6e9a387`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:11:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:04:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 24 May 2021 18:23:10 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:23:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 24 May 2021 18:23:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 24 May 2021 18:23:13 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 24 May 2021 18:23:14 GMT
ENV XDG_DATA_HOME=/data
# Mon, 24 May 2021 18:23:14 GMT
VOLUME [/config]
# Mon, 24 May 2021 18:23:14 GMT
VOLUME [/data]
# Mon, 24 May 2021 18:23:14 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:23:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:23:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:23:16 GMT
EXPOSE 80
# Mon, 24 May 2021 18:23:16 GMT
EXPOSE 443
# Mon, 24 May 2021 18:23:16 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:23:16 GMT
WORKDIR /srv
# Mon, 24 May 2021 18:23:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8294633c5b5606f8e98aaf81da701b7a7e2018dbf82355d1d73830c677034f19`  
		Last Modified: Wed, 14 Apr 2021 20:12:08 GMT  
		Size: 300.4 KB (300403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16798e0582fce7af9c2ba2c8ee4990d0fd1e58384e170ee9937486253d67bbf1`  
		Last Modified: Tue, 11 May 2021 01:05:00 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba0aa26d56032b74c8c88c24edc5a2f7987ea418aaa0966f93ab53c62802c2f`  
		Last Modified: Mon, 24 May 2021 18:23:47 GMT  
		Size: 11.4 MB (11449656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712687f6a8ba00b8b6cb95bad7426eb9964fff3de9f5a7f66dedf6310e8a8c01`  
		Last Modified: Mon, 24 May 2021 18:23:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:eea14e6e8e0ef54944ef2f6e1b6540a536661e033a1f216e92535b5741c2278e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13786866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e11afe23a7696f3f16192af7de16ece9c2dfb73868f2859b9dbacfe0e604fa4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 17:34:28 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 May 2021 17:34:30 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Wed, 26 May 2021 17:34:30 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 26 May 2021 17:34:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 May 2021 17:34:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 May 2021 17:34:33 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 May 2021 17:34:34 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 May 2021 17:34:34 GMT
VOLUME [/config]
# Wed, 26 May 2021 17:34:34 GMT
VOLUME [/data]
# Wed, 26 May 2021 17:34:34 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 26 May 2021 17:34:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 May 2021 17:34:34 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 May 2021 17:34:36 GMT
EXPOSE 80
# Wed, 26 May 2021 17:34:36 GMT
EXPOSE 443
# Wed, 26 May 2021 17:34:36 GMT
EXPOSE 2019
# Wed, 26 May 2021 17:34:36 GMT
WORKDIR /srv
# Wed, 26 May 2021 17:34:36 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c2672622a603ff8b0ed8517cfd5adb30b2b35ae40b42cd4ad0545dcb6d3b10`  
		Last Modified: Wed, 26 May 2021 17:36:11 GMT  
		Size: 300.5 KB (300528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b30604f35cc25a62ae1d71a50c6919ad28a2aa67bfd14bebc1984cec5b2c8b`  
		Last Modified: Wed, 26 May 2021 17:36:12 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7119340f7ca66a456adcbc374cbeb7e1c37c35867123bd3fac943aea26a813a8`  
		Last Modified: Wed, 26 May 2021 17:36:15 GMT  
		Size: 10.9 MB (10858201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392497979deecdb2075178245bdf58e8d1ce55c609d2b1320a869392bc007b3f`  
		Last Modified: Wed, 26 May 2021 17:36:12 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:ea6c90777b37ade094ce3f1f5d0efffe39519d18ec589fa4cfa2b6f0c5028e3a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13561305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8637a19be10382ee673bc51be71c9fa3ce23cfdcd0eb9d9bf8734147818227d4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 10:59:27 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 May 2021 10:59:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Wed, 26 May 2021 10:59:29 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 26 May 2021 10:59:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 May 2021 10:59:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 May 2021 10:59:32 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 May 2021 10:59:32 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 May 2021 10:59:32 GMT
VOLUME [/config]
# Wed, 26 May 2021 10:59:33 GMT
VOLUME [/data]
# Wed, 26 May 2021 10:59:33 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 26 May 2021 10:59:33 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 May 2021 10:59:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 May 2021 10:59:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 May 2021 10:59:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 May 2021 10:59:34 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 May 2021 10:59:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 May 2021 10:59:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 May 2021 10:59:34 GMT
EXPOSE 80
# Wed, 26 May 2021 10:59:35 GMT
EXPOSE 443
# Wed, 26 May 2021 10:59:35 GMT
EXPOSE 2019
# Wed, 26 May 2021 10:59:35 GMT
WORKDIR /srv
# Wed, 26 May 2021 10:59:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca051a8c4175c3d7d75c47c9a60045d2f5b7eb415ce35b56c99e9cab58ae3ba`  
		Last Modified: Wed, 26 May 2021 11:01:09 GMT  
		Size: 299.7 KB (299668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2db810fb832f7bd380a39ff7508fa03cc1854bdd51da4cfa239e07fe96fe4e`  
		Last Modified: Wed, 26 May 2021 11:01:09 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce092d490b7e90c7b37879314c23cb48b38be5392715e2d976bc99bbef8a230`  
		Last Modified: Wed, 26 May 2021 11:01:11 GMT  
		Size: 10.8 MB (10831485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb6eb70297874eea11cf38b8870aa1f896bfd6ec638fd6dc9177d7be039001b`  
		Last Modified: Wed, 26 May 2021 11:01:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:ad6d7adcc7d981edfcc5eb4bb42e1fc561b9d0301cadf2ccd920a4a98ae90387
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13415153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:383d427b090897c507d37417dfd21667985cf15a9e3e800b87c821eabe372bb6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 17:52:42 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 May 2021 17:52:43 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Wed, 26 May 2021 17:52:44 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 26 May 2021 17:52:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 May 2021 17:52:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 May 2021 17:52:47 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 May 2021 17:52:47 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 May 2021 17:52:47 GMT
VOLUME [/config]
# Wed, 26 May 2021 17:52:47 GMT
VOLUME [/data]
# Wed, 26 May 2021 17:52:47 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 May 2021 17:52:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 May 2021 17:52:49 GMT
EXPOSE 80
# Wed, 26 May 2021 17:52:49 GMT
EXPOSE 443
# Wed, 26 May 2021 17:52:49 GMT
EXPOSE 2019
# Wed, 26 May 2021 17:52:49 GMT
WORKDIR /srv
# Wed, 26 May 2021 17:52:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a305c6848b1bdb9c473c4a3128eff85e1604c1b2d0e78cef80874650b91a49`  
		Last Modified: Wed, 26 May 2021 17:53:57 GMT  
		Size: 300.6 KB (300633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2faea6afac2cf802bf88fd56ee1493ce97eca3a29920702a726ea8e5cd0ea3d`  
		Last Modified: Wed, 26 May 2021 17:53:57 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c196442e5472f13a88f63e7da52cbd15acf171b3d76e87cc47c3073ed0e95d`  
		Last Modified: Wed, 26 May 2021 17:53:59 GMT  
		Size: 10.4 MB (10396489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583f00c174c73f777e3d0cd263a593786c4c341cb20632fafb4246ac0f06f45b`  
		Last Modified: Wed, 26 May 2021 17:53:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:b767e2ec43a11bb1a211e3d7bc76c81d4a256f90084d5747367af6a9730e4f94
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13121818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f930dc44ddd7a57e1d48aaeed66a69653dc4d5c15bdae6c378273cb55287f07b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:12:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:17:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 24 May 2021 18:19:32 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:20:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 24 May 2021 18:20:18 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 24 May 2021 18:20:25 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 24 May 2021 18:20:32 GMT
ENV XDG_DATA_HOME=/data
# Mon, 24 May 2021 18:20:39 GMT
VOLUME [/config]
# Mon, 24 May 2021 18:20:45 GMT
VOLUME [/data]
# Mon, 24 May 2021 18:20:51 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:20:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:21:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:21:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:21:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:21:34 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:21:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:21:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:22:03 GMT
EXPOSE 80
# Mon, 24 May 2021 18:22:10 GMT
EXPOSE 443
# Mon, 24 May 2021 18:22:16 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:22:21 GMT
WORKDIR /srv
# Mon, 24 May 2021 18:22:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25908330df11bb7bc2ed71aa9b4de279db5492df2b03ced3f6650b25821c4584`  
		Last Modified: Wed, 14 Apr 2021 22:16:00 GMT  
		Size: 302.6 KB (302554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a224581e3ba4733f37686f5a5d5375019f9126a0ded6ed20f13e09e898dc735e`  
		Last Modified: Tue, 11 May 2021 01:20:08 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c6214f82b33045060ad6f882d1ed7a5779be7a0883c4da8306ab03e9e2623c`  
		Last Modified: Mon, 24 May 2021 18:23:37 GMT  
		Size: 10.0 MB (10000116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52a67b9935763896cc7c3386cd93b5f7fbc80093549e39f460dc7e170f679f4`  
		Last Modified: Mon, 24 May 2021 18:23:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:40e8d6bc1ad5c4c4f902426841f39a594dd3842c212bed7ecbb66f312b5a4f6e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13938687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c9fccd235488bb04e0075ea4a47a8c102dce45c98cbba05e4d7d0d0ebb13b1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:07:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 10 May 2021 23:41:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 24 May 2021 17:41:40 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 17:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 24 May 2021 17:41:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 24 May 2021 17:41:48 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 24 May 2021 17:41:48 GMT
ENV XDG_DATA_HOME=/data
# Mon, 24 May 2021 17:41:49 GMT
VOLUME [/config]
# Mon, 24 May 2021 17:41:50 GMT
VOLUME [/data]
# Mon, 24 May 2021 17:41:50 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 17:41:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 17:41:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 17:41:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 17:41:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 17:41:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 17:41:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 17:41:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 17:41:55 GMT
EXPOSE 80
# Mon, 24 May 2021 17:41:56 GMT
EXPOSE 443
# Mon, 24 May 2021 17:41:57 GMT
EXPOSE 2019
# Mon, 24 May 2021 17:41:57 GMT
WORKDIR /srv
# Mon, 24 May 2021 17:41:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db3c8b812fcb0d1bfd42c16c2e9ac68f4f3006382c5362e969d1c9eb3a9fab5`  
		Last Modified: Wed, 14 Apr 2021 20:08:26 GMT  
		Size: 300.8 KB (300847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba030675d7bb5bc251d93896d2c81ed8a2f4f4ef2e8e84ad7dfdce9886387c`  
		Last Modified: Mon, 10 May 2021 23:42:29 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03e81629e078650b941a4beb267a6755133e90fa22a688bffb5df188e069c55`  
		Last Modified: Mon, 24 May 2021 17:42:37 GMT  
		Size: 11.0 MB (11029189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbee1e7ec347a65e5e78b46b8fe541241e3f6c13a468785945abd0aaba24545`  
		Last Modified: Mon, 24 May 2021 17:42:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:7e7f52b8b3e06a36bc4b32d552b0b2b30dc863461d3250a691fae68fc89c841b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:acb1d8e470fc9d3be900f5a534a57d59d7e827ad2a4fabbedbacde1d08e850ee
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116540780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eafee2350c73e5c74f40dc4ff4146d3ac64f52d221205b317621567780641a34`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:27:12 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 21:27:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 21:27:13 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:46:27 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 01:48:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 01:48:48 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 01:48:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:48:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 01:48:50 GMT
WORKDIR /go
# Fri, 04 Jun 2021 02:18:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 02:18:24 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 02:18:25 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 02:18:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 02:18:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 02:18:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 02:18:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adcc1eea9eeabb6de296adb3e0c1b0722cf13251ff3e4e2d0a5f7ed8e3d48342`  
		Last Modified: Wed, 14 Apr 2021 21:35:06 GMT  
		Size: 281.3 KB (281269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4ab2625f07be8d5c6e48046a05ff3ecc7f374b794a926fb62247b66b511909`  
		Last Modified: Wed, 14 Apr 2021 21:35:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689510d40a2658530c96a39b304e1561733255af89b84ce6de9f489b3ca1a281`  
		Last Modified: Fri, 04 Jun 2021 01:59:43 GMT  
		Size: 105.7 MB (105740137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4d89f102e3b1bb1c586ebf1bf8ab36d3a58ed7793fdb0f6ceca00bc2b177cd`  
		Last Modified: Fri, 04 Jun 2021 01:59:25 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44fa7996470329a7e8174cb5cbaa52ade2eb5fffabe426b05cab3d2c904e6e0`  
		Last Modified: Fri, 04 Jun 2021 02:19:02 GMT  
		Size: 6.4 MB (6395534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26081f37d859cc0d0f0882b13352f2ef140940d73620b130154c91355054b525`  
		Last Modified: Fri, 04 Jun 2021 02:19:02 GMT  
		Size: 1.3 MB (1311156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0133abdd19ffca66008a8732eca2edf1f571ed52fe2b3d873ed8158282f9f7`  
		Last Modified: Fri, 04 Jun 2021 02:19:01 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:9c6cfad074c68103b20a26d1f2da9f0f8f22b5406a356e5696e1856cf3e5c332
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112301607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfd32aee08fd69ca7dcd229bd475cce45176a90ef6154a872d01333b97e2119c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Fri, 04 Jun 2021 05:29:59 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 04 Jun 2021 05:30:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 04 Jun 2021 05:30:00 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 05:30:00 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 05:32:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 05:33:00 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 05:33:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 05:33:01 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 05:33:01 GMT
WORKDIR /go
# Fri, 04 Jun 2021 07:35:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 07:35:01 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 07:35:01 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 07:35:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 07:35:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 07:35:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 07:35:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90c33f298071ceb1106bce90623a7fe87a3be8510fe9512966f1a7bc5625a47`  
		Last Modified: Fri, 04 Jun 2021 05:41:55 GMT  
		Size: 281.4 KB (281382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f381ff0ec8799fc86bf65aba1711ab973cc107a53a6d134a9a0ba3267477a0fb`  
		Last Modified: Fri, 04 Jun 2021 05:41:55 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d5ab13bd0ab2cb8b8b4b1e08587ddb255e3d3bd2cebd7fcb8ba562bb0974d5`  
		Last Modified: Fri, 04 Jun 2021 05:42:20 GMT  
		Size: 101.9 MB (101944742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2d1d4b06a01686239e04dc869317cdd368448fe45334d9838856be1d149dae`  
		Last Modified: Fri, 04 Jun 2021 05:41:55 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fad5cba6f9b7a0e238d430bcd3ce8b3fc12e6bdc8cdb46008ce5a932e27f229`  
		Last Modified: Fri, 04 Jun 2021 07:36:16 GMT  
		Size: 6.2 MB (6230964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed25c6ff0ab0732ac72d5202c79100508522040b20b4ef01be1fb5e20210ae85`  
		Last Modified: Fri, 04 Jun 2021 07:36:15 GMT  
		Size: 1.2 MB (1221675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c309325d1d11d3a67efbffdd774a27af11a477b9ab43b25e95912d6d72b5c652`  
		Last Modified: Fri, 04 Jun 2021 07:36:15 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:3ce06d10a24fe566699c8997bc0c089e851e46c0f69fa0fff18d0085b4346289
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111232949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cde3b1d7cb6f225fb3b4f3064f07e8f9186fcbff0ecb697e5aa10d00899ea6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 27 May 2021 15:06:45 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 27 May 2021 15:06:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 May 2021 15:06:46 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 07:52:57 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 07:55:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 07:55:34 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 07:55:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 07:55:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 07:55:36 GMT
WORKDIR /go
# Fri, 04 Jun 2021 12:06:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 12:06:59 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 12:06:59 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 12:06:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 12:07:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 12:07:01 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 12:07:01 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7339ea1d6bf57b602a207a1e2f24e2f2d6d0fef53ac31afc17a550368c53e63b`  
		Last Modified: Thu, 27 May 2021 15:19:37 GMT  
		Size: 280.5 KB (280537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c586fedb7a1526f50c1bb5ccadd41167254abbdf9cc445264c5a2cda55bff7f3`  
		Last Modified: Thu, 27 May 2021 15:19:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac424f1791899264fd7faf16b2b868022b332df5c89c65ab7bd4da634a0debcc`  
		Last Modified: Fri, 04 Jun 2021 08:07:59 GMT  
		Size: 101.7 MB (101746953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ea8b8d5ee549723867d0f8a4a54e81bc6e8cffef6b2e29cd0efa53f44d75ae`  
		Last Modified: Fri, 04 Jun 2021 08:07:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73f5e95932571acfe6d65aba85701fb9e0a60e6aef82a4d1eeeeab75717fb1`  
		Last Modified: Fri, 04 Jun 2021 12:08:13 GMT  
		Size: 5.6 MB (5561103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c649a927d5a9a52469a77c3ba79e77cc5b94865a1f8d1085843dbd50573897e3`  
		Last Modified: Fri, 04 Jun 2021 12:08:13 GMT  
		Size: 1.2 MB (1219497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7604724e4d7dadae83d4d023c9f2101e6dcd59c058928794c12cc23a4f34d7f`  
		Last Modified: Fri, 04 Jun 2021 12:08:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5dc91099db737a46c5bb7ca6fe3c0174e49874c492ff48e5eac5fc30a579864b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111775816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73671d0a54a8053b75985bb11523edbe1e3877082dede6664d842d058fc6048b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 27 May 2021 22:17:28 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 27 May 2021 22:17:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 May 2021 22:17:29 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 04:00:14 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 04:01:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 04:01:36 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 04:01:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 04:01:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 04:01:37 GMT
WORKDIR /go
# Fri, 04 Jun 2021 07:44:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 07:44:36 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 07:44:36 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 07:44:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 07:44:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 07:44:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 07:44:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3088b5b3c5c0fab79ca41c188d3696a5053778b6c7d602b2aea8084c094608d1`  
		Last Modified: Thu, 27 May 2021 22:26:43 GMT  
		Size: 281.5 KB (281495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7225fbf94c881dc50b56f5430522fbde8891efa801909d5d9f06261d839cc5`  
		Last Modified: Thu, 27 May 2021 22:26:43 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba82ee9f976e7f9d818f11b866566f142f7ceddface2c0d3d5fe3a6920cc659d`  
		Last Modified: Fri, 04 Jun 2021 04:09:30 GMT  
		Size: 101.1 MB (101096027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506bd15cee9f23181bcd604afe8ec2b150b0321d4d0e741e272734456560caac`  
		Last Modified: Fri, 04 Jun 2021 04:09:12 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83fba387ff0d0e9e65223a37bf6a1e09e7e24774a900e99f743e8c3d455f4fdb`  
		Last Modified: Fri, 04 Jun 2021 07:45:32 GMT  
		Size: 6.5 MB (6484015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84ec75c54b55467ea07ae1ace7ace92b52355954733f1ecbd86d26937d03364`  
		Last Modified: Fri, 04 Jun 2021 07:45:31 GMT  
		Size: 1.2 MB (1201540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91117b691ccdbc0552460233c27811b1de617ff3bc78eac7af1f1f70d7b6f6cb`  
		Last Modified: Fri, 04 Jun 2021 07:45:31 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:7f735b71e3863db84fafaaef6c3299cd3f902d9d99504589d7d8b77ed30fdd1b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110613992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ead49008853a08fc29f3178cf58d7cfcb85b1d9dd361879df0f96cf640dcc94`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:53:57 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 22:54:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:54:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 03:07:09 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 03:08:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 03:09:08 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 03:09:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 03:09:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 03:09:30 GMT
WORKDIR /go
# Fri, 04 Jun 2021 09:16:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 09:16:18 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 09:16:26 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 09:16:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 09:16:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 09:16:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 09:16:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf726c40dc4802009a4b6f0f7947c86242c2c078623e8f1f21343864093b3a9`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 283.4 KB (283413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c17712dac96942b05a27f88ea5346bd57b4cabdb33c153562ef144635225b3`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6104245b6f3bb2cd73fecb2ee6ef3347bedc6f588475449849c4229c3321eb8`  
		Last Modified: Fri, 04 Jun 2021 03:20:31 GMT  
		Size: 99.5 MB (99515576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c228774385f5c8b0c6ad74f4b22b8976926d85634278c36ba33b49f23ac5154`  
		Last Modified: Fri, 04 Jun 2021 03:20:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af27e8f9d4959b48b81f61cb0d645eccfd256ee74635e0396fac0b732c0e57b`  
		Last Modified: Fri, 04 Jun 2021 09:17:36 GMT  
		Size: 6.8 MB (6830629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d43d75e1cc7759d079bd9ad4389f4cd3b79a036ff24add605969b915d46114`  
		Last Modified: Fri, 04 Jun 2021 09:17:35 GMT  
		Size: 1.2 MB (1170519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd193d55e35894d2beb5854ebb790227fb34a033785effbaa520604e248480c`  
		Last Modified: Fri, 04 Jun 2021 09:17:35 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:bb5f24094fadd35d4c5940a0c1f143d212544334b9bce93de93677dbabe4db16
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115475353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23250df470a63b89f2a4832f806630ba5002e9595baed80673428d73b9b8e8a9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:45:11 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:45:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:45:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:26:42 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 01:28:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 01:28:34 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 01:28:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:28:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 01:28:36 GMT
WORKDIR /go
# Fri, 04 Jun 2021 03:02:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 03:02:56 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 03:02:56 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 03:02:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 03:02:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 03:03:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 03:03:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc746875ae346ee6ec3c9080f8a7a50bef3899ea9d5ae9dac45a81bfe861c9d`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 281.7 KB (281708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0242688236000dd8f33d16f89f36da3ef1bb2a7a32bb59a7eb97a18ed3d5158`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0ff47eca4941b373fedcfb40530f4d5ef82aed9a9b83bd7fa6cee6546112fd`  
		Last Modified: Fri, 04 Jun 2021 01:37:12 GMT  
		Size: 104.8 MB (104846719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6991fc153a27c9de6b023272f31bf22b708f788131bd628abeb30592007377a8`  
		Last Modified: Fri, 04 Jun 2021 01:36:59 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b452ba9be082c7a2255414c44dde4b275a327b14d24e947901062089bd7ebf43`  
		Last Modified: Fri, 04 Jun 2021 03:03:37 GMT  
		Size: 6.5 MB (6479039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507d613df3c6f7ea5929ebfe6205e87ae1b89cd044677a765da66d135bb7ef57`  
		Last Modified: Fri, 04 Jun 2021 03:03:37 GMT  
		Size: 1.3 MB (1264524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd9e1c527bba47d9aa0c07957cb156d2c1d205ca81c81e8b00b5b9c0330290b`  
		Last Modified: Fri, 04 Jun 2021 03:03:36 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:0cba0bbebbf26fbfe27a39006a093cfb426976baff4e8c3ec906a2a229be9e69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2808421770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c51b9b016f1a3599a109e39809816252f59ecd94d60ef1b7043ab7404059d79`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 12:10:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 12:37:22 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Jun 2021 12:37:25 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Jun 2021 12:37:29 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Jun 2021 12:37:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Jun 2021 12:38:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:38:25 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Jun 2021 12:38:51 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Jun 2021 12:38:53 GMT
ENV GOLANG_VERSION=1.16.5
# Wed, 09 Jun 2021 12:41:22 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:41:27 GMT
WORKDIR C:\gopath
# Wed, 09 Jun 2021 20:15:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:15:04 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 09 Jun 2021 20:15:06 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:15:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Jun 2021 20:15:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Jun 2021 20:15:46 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7863ef96846d497ea06fe442ea13dcecaf5c248ce238c69800475281a4fa848e`  
		Last Modified: Wed, 09 Jun 2021 12:20:41 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f985a0b4390580a94aa3cbc8ecb01fc33805bb3304c4217dc5ec9fb6626011ca`  
		Last Modified: Wed, 09 Jun 2021 13:03:26 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5adf5cc2989b1cf730e7993bd088f778b31b33bac78f6d9c133226f7bcf4a6`  
		Last Modified: Wed, 09 Jun 2021 13:03:24 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480b981517ab26b6ee7e090e51d040995ac5a6a55410880ea3f0c8255dada3bc`  
		Last Modified: Wed, 09 Jun 2021 13:03:24 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a372a8dcfb8f1152565f4b8c928c202db247ddc21fd9a35838a2278c65ff6f`  
		Last Modified: Wed, 09 Jun 2021 13:03:23 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97090ffba94bc8afc85a54e404c8aca13253969fe01c8b0ac1f8ce3a0b909953`  
		Last Modified: Wed, 09 Jun 2021 13:03:53 GMT  
		Size: 25.4 MB (25445694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb1c026791860f230531a960e59a35d86f3ae617c5b6ad60155718694ed3720`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fca536252ace3ea8e08bcd38a313ad63d7d308f4a1d24734c324d191b65647`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 314.6 KB (314587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3865edd5ab3e6e2858d35fea90d96f24eb95579b3bb7f95674954df09b428a8e`  
		Last Modified: Wed, 09 Jun 2021 13:03:20 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424a1b81819edd902af8893d485a39318ee4023db4db6f9c73ebb8470a5c2310`  
		Last Modified: Wed, 09 Jun 2021 13:03:58 GMT  
		Size: 139.4 MB (139355479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f54cc4fcf8b7300908d2cb4aa6dbfe433cc614c35c200ca655b96d576a40412`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 1.6 KB (1596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ae8d8d0f1afc3ddbfe8673534bd1ae7afdf7662fb5fd73ef017088a251e15c`  
		Last Modified: Wed, 09 Jun 2021 20:20:23 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761852a93f82584033e99d58efb7a7e5fad44135d49f23090e1217932f809891`  
		Last Modified: Wed, 09 Jun 2021 20:20:20 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f24be856334e97a03392fc575807609b5afd8808514d9ca8305700e72834ea`  
		Last Modified: Wed, 09 Jun 2021 20:20:20 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047b293c2c055e53ea3099cdc7cd511d55cb43391cbcfd34e0c3a96ac1d179ca`  
		Last Modified: Wed, 09 Jun 2021 20:20:20 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2806e8d39eec5d338e88005243d0a11fcb7c24dab13df4ee3c5ce9ee0266dd9`  
		Last Modified: Wed, 09 Jun 2021 20:20:21 GMT  
		Size: 1.7 MB (1703136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de952f0fc6af6d7eea8c8d4d424cf97622e0b2628a32387976f4dc8df54efb8`  
		Last Modified: Wed, 09 Jun 2021 20:20:20 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:4481a6011b8d50eca815372f7a8f28afaae493233d49d4ec20b3d3a5abf93fc7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6437000457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4919458e8d791f772cd7dd820598edd51cc401fa898c7e4ddddc19e6bb2890fe`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 12:41:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 12:41:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Jun 2021 12:41:43 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Jun 2021 12:41:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Jun 2021 12:41:49 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Jun 2021 12:44:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:44:27 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Jun 2021 12:45:49 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Jun 2021 12:45:51 GMT
ENV GOLANG_VERSION=1.16.5
# Wed, 09 Jun 2021 12:49:20 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:49:24 GMT
WORKDIR C:\gopath
# Wed, 09 Jun 2021 20:15:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:15:56 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 09 Jun 2021 20:15:59 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:16:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Jun 2021 20:17:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Jun 2021 20:17:28 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c82e82e95dbad4ccc260b42e03767eb07222e2f00ec57a69b3c87b17da1d2fd3`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a881968e28f8c2900b00800a0de406d0e98740558d9564ad738d053e63d9a1e`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab71df915cf7ac4c559039a917269e11faab2d0e6862a01408431df7fb40362f`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82ce560dcbc3235ed87d6c938aa761616dbd299188ae53a51a266eb37f381f6`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bee5ea2f89fe3f3e514b8dfcd823da340447b633c6048e00773d1c30fbbc0e9`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad71deb840b73610184070ebc7c566bd1dac9cc309d53679460697243bab7640`  
		Last Modified: Wed, 09 Jun 2021 13:04:50 GMT  
		Size: 25.4 MB (25441204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16f2a89ed7a230471eb96b67829deb255795564010b0ff2de47179cdfdec1d0`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cc755175ec255452c16e1e41cc78a8cd719d65f70221e7d128c1dc18eec8f2`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 307.7 KB (307689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d153904f724dbfda646a6c5ccdc1eed2545cf7777c8650461abdedafe75bc693`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ec88320a2e6bf1cfef8856b9271f7d2fa4d2ae8e0eb5b9a44175d04a725631`  
		Last Modified: Wed, 09 Jun 2021 13:04:58 GMT  
		Size: 143.8 MB (143821249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419b516d300f276d9a3f98a1d2c47394abb00b15edeaadcb2f5d0ecee3380f14`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 1.6 KB (1576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d420a2d4c5bca557510bd5eaeea0268b05bb6e61104acea0af1e28c7537c8352`  
		Last Modified: Wed, 09 Jun 2021 20:20:41 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06bf21d106193b12d0b9a688698ec718f7fb4514f317565933b89f22da0d1de`  
		Last Modified: Wed, 09 Jun 2021 20:20:38 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64471c2fb9e42024fce3859860cf6a05f584b8c21ff5c776f7c285588f1117fc`  
		Last Modified: Wed, 09 Jun 2021 20:20:38 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f2c847c9bab79f9970336a628d5b7948504e3f2a67f95cac9a1a3f12132673`  
		Last Modified: Wed, 09 Jun 2021 20:20:38 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae1157ef3d362883b0503349e9d7cb6d729fa420af63a826262dca25f7a9fc`  
		Last Modified: Wed, 09 Jun 2021 20:20:39 GMT  
		Size: 1.7 MB (1684468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e122b3fd6e41cb67b3d9b46e55753aa37f1f60c2de7fab150181822a556d2791`  
		Last Modified: Wed, 09 Jun 2021 20:20:38 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:4b4685dba38126a1d8dc692a9cc3f60e145e085f5f2a132b32bdbbcec0109a55
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
$ docker pull caddy@sha256:acb1d8e470fc9d3be900f5a534a57d59d7e827ad2a4fabbedbacde1d08e850ee
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116540780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eafee2350c73e5c74f40dc4ff4146d3ac64f52d221205b317621567780641a34`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:27:12 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 21:27:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 21:27:13 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:46:27 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 01:48:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 01:48:48 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 01:48:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:48:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 01:48:50 GMT
WORKDIR /go
# Fri, 04 Jun 2021 02:18:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 02:18:24 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 02:18:25 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 02:18:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 02:18:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 02:18:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 02:18:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adcc1eea9eeabb6de296adb3e0c1b0722cf13251ff3e4e2d0a5f7ed8e3d48342`  
		Last Modified: Wed, 14 Apr 2021 21:35:06 GMT  
		Size: 281.3 KB (281269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4ab2625f07be8d5c6e48046a05ff3ecc7f374b794a926fb62247b66b511909`  
		Last Modified: Wed, 14 Apr 2021 21:35:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689510d40a2658530c96a39b304e1561733255af89b84ce6de9f489b3ca1a281`  
		Last Modified: Fri, 04 Jun 2021 01:59:43 GMT  
		Size: 105.7 MB (105740137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4d89f102e3b1bb1c586ebf1bf8ab36d3a58ed7793fdb0f6ceca00bc2b177cd`  
		Last Modified: Fri, 04 Jun 2021 01:59:25 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44fa7996470329a7e8174cb5cbaa52ade2eb5fffabe426b05cab3d2c904e6e0`  
		Last Modified: Fri, 04 Jun 2021 02:19:02 GMT  
		Size: 6.4 MB (6395534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26081f37d859cc0d0f0882b13352f2ef140940d73620b130154c91355054b525`  
		Last Modified: Fri, 04 Jun 2021 02:19:02 GMT  
		Size: 1.3 MB (1311156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0133abdd19ffca66008a8732eca2edf1f571ed52fe2b3d873ed8158282f9f7`  
		Last Modified: Fri, 04 Jun 2021 02:19:01 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:9c6cfad074c68103b20a26d1f2da9f0f8f22b5406a356e5696e1856cf3e5c332
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112301607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfd32aee08fd69ca7dcd229bd475cce45176a90ef6154a872d01333b97e2119c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Fri, 04 Jun 2021 05:29:59 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 04 Jun 2021 05:30:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 04 Jun 2021 05:30:00 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 05:30:00 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 05:32:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 05:33:00 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 05:33:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 05:33:01 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 05:33:01 GMT
WORKDIR /go
# Fri, 04 Jun 2021 07:35:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 07:35:01 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 07:35:01 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 07:35:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 07:35:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 07:35:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 07:35:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90c33f298071ceb1106bce90623a7fe87a3be8510fe9512966f1a7bc5625a47`  
		Last Modified: Fri, 04 Jun 2021 05:41:55 GMT  
		Size: 281.4 KB (281382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f381ff0ec8799fc86bf65aba1711ab973cc107a53a6d134a9a0ba3267477a0fb`  
		Last Modified: Fri, 04 Jun 2021 05:41:55 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d5ab13bd0ab2cb8b8b4b1e08587ddb255e3d3bd2cebd7fcb8ba562bb0974d5`  
		Last Modified: Fri, 04 Jun 2021 05:42:20 GMT  
		Size: 101.9 MB (101944742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2d1d4b06a01686239e04dc869317cdd368448fe45334d9838856be1d149dae`  
		Last Modified: Fri, 04 Jun 2021 05:41:55 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fad5cba6f9b7a0e238d430bcd3ce8b3fc12e6bdc8cdb46008ce5a932e27f229`  
		Last Modified: Fri, 04 Jun 2021 07:36:16 GMT  
		Size: 6.2 MB (6230964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed25c6ff0ab0732ac72d5202c79100508522040b20b4ef01be1fb5e20210ae85`  
		Last Modified: Fri, 04 Jun 2021 07:36:15 GMT  
		Size: 1.2 MB (1221675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c309325d1d11d3a67efbffdd774a27af11a477b9ab43b25e95912d6d72b5c652`  
		Last Modified: Fri, 04 Jun 2021 07:36:15 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:3ce06d10a24fe566699c8997bc0c089e851e46c0f69fa0fff18d0085b4346289
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111232949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cde3b1d7cb6f225fb3b4f3064f07e8f9186fcbff0ecb697e5aa10d00899ea6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 27 May 2021 15:06:45 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 27 May 2021 15:06:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 May 2021 15:06:46 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 07:52:57 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 07:55:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 07:55:34 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 07:55:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 07:55:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 07:55:36 GMT
WORKDIR /go
# Fri, 04 Jun 2021 12:06:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 12:06:59 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 12:06:59 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 12:06:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 12:07:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 12:07:01 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 12:07:01 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7339ea1d6bf57b602a207a1e2f24e2f2d6d0fef53ac31afc17a550368c53e63b`  
		Last Modified: Thu, 27 May 2021 15:19:37 GMT  
		Size: 280.5 KB (280537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c586fedb7a1526f50c1bb5ccadd41167254abbdf9cc445264c5a2cda55bff7f3`  
		Last Modified: Thu, 27 May 2021 15:19:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac424f1791899264fd7faf16b2b868022b332df5c89c65ab7bd4da634a0debcc`  
		Last Modified: Fri, 04 Jun 2021 08:07:59 GMT  
		Size: 101.7 MB (101746953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ea8b8d5ee549723867d0f8a4a54e81bc6e8cffef6b2e29cd0efa53f44d75ae`  
		Last Modified: Fri, 04 Jun 2021 08:07:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73f5e95932571acfe6d65aba85701fb9e0a60e6aef82a4d1eeeeab75717fb1`  
		Last Modified: Fri, 04 Jun 2021 12:08:13 GMT  
		Size: 5.6 MB (5561103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c649a927d5a9a52469a77c3ba79e77cc5b94865a1f8d1085843dbd50573897e3`  
		Last Modified: Fri, 04 Jun 2021 12:08:13 GMT  
		Size: 1.2 MB (1219497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7604724e4d7dadae83d4d023c9f2101e6dcd59c058928794c12cc23a4f34d7f`  
		Last Modified: Fri, 04 Jun 2021 12:08:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5dc91099db737a46c5bb7ca6fe3c0174e49874c492ff48e5eac5fc30a579864b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111775816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73671d0a54a8053b75985bb11523edbe1e3877082dede6664d842d058fc6048b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 27 May 2021 22:17:28 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 27 May 2021 22:17:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 May 2021 22:17:29 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 04:00:14 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 04:01:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 04:01:36 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 04:01:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 04:01:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 04:01:37 GMT
WORKDIR /go
# Fri, 04 Jun 2021 07:44:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 07:44:36 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 07:44:36 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 07:44:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 07:44:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 07:44:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 07:44:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3088b5b3c5c0fab79ca41c188d3696a5053778b6c7d602b2aea8084c094608d1`  
		Last Modified: Thu, 27 May 2021 22:26:43 GMT  
		Size: 281.5 KB (281495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7225fbf94c881dc50b56f5430522fbde8891efa801909d5d9f06261d839cc5`  
		Last Modified: Thu, 27 May 2021 22:26:43 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba82ee9f976e7f9d818f11b866566f142f7ceddface2c0d3d5fe3a6920cc659d`  
		Last Modified: Fri, 04 Jun 2021 04:09:30 GMT  
		Size: 101.1 MB (101096027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506bd15cee9f23181bcd604afe8ec2b150b0321d4d0e741e272734456560caac`  
		Last Modified: Fri, 04 Jun 2021 04:09:12 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83fba387ff0d0e9e65223a37bf6a1e09e7e24774a900e99f743e8c3d455f4fdb`  
		Last Modified: Fri, 04 Jun 2021 07:45:32 GMT  
		Size: 6.5 MB (6484015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84ec75c54b55467ea07ae1ace7ace92b52355954733f1ecbd86d26937d03364`  
		Last Modified: Fri, 04 Jun 2021 07:45:31 GMT  
		Size: 1.2 MB (1201540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91117b691ccdbc0552460233c27811b1de617ff3bc78eac7af1f1f70d7b6f6cb`  
		Last Modified: Fri, 04 Jun 2021 07:45:31 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:7f735b71e3863db84fafaaef6c3299cd3f902d9d99504589d7d8b77ed30fdd1b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110613992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ead49008853a08fc29f3178cf58d7cfcb85b1d9dd361879df0f96cf640dcc94`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:53:57 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 22:54:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:54:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 03:07:09 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 03:08:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 03:09:08 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 03:09:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 03:09:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 03:09:30 GMT
WORKDIR /go
# Fri, 04 Jun 2021 09:16:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 09:16:18 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 09:16:26 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 09:16:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 09:16:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 09:16:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 09:16:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf726c40dc4802009a4b6f0f7947c86242c2c078623e8f1f21343864093b3a9`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 283.4 KB (283413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c17712dac96942b05a27f88ea5346bd57b4cabdb33c153562ef144635225b3`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6104245b6f3bb2cd73fecb2ee6ef3347bedc6f588475449849c4229c3321eb8`  
		Last Modified: Fri, 04 Jun 2021 03:20:31 GMT  
		Size: 99.5 MB (99515576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c228774385f5c8b0c6ad74f4b22b8976926d85634278c36ba33b49f23ac5154`  
		Last Modified: Fri, 04 Jun 2021 03:20:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af27e8f9d4959b48b81f61cb0d645eccfd256ee74635e0396fac0b732c0e57b`  
		Last Modified: Fri, 04 Jun 2021 09:17:36 GMT  
		Size: 6.8 MB (6830629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d43d75e1cc7759d079bd9ad4389f4cd3b79a036ff24add605969b915d46114`  
		Last Modified: Fri, 04 Jun 2021 09:17:35 GMT  
		Size: 1.2 MB (1170519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd193d55e35894d2beb5854ebb790227fb34a033785effbaa520604e248480c`  
		Last Modified: Fri, 04 Jun 2021 09:17:35 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:bb5f24094fadd35d4c5940a0c1f143d212544334b9bce93de93677dbabe4db16
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115475353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23250df470a63b89f2a4832f806630ba5002e9595baed80673428d73b9b8e8a9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:45:11 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:45:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:45:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:26:42 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 01:28:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Jun 2021 01:28:34 GMT
ENV GOPATH=/go
# Fri, 04 Jun 2021 01:28:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:28:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Jun 2021 01:28:36 GMT
WORKDIR /go
# Fri, 04 Jun 2021 03:02:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Jun 2021 03:02:56 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 03:02:56 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 03:02:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 03:02:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Jun 2021 03:03:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Jun 2021 03:03:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc746875ae346ee6ec3c9080f8a7a50bef3899ea9d5ae9dac45a81bfe861c9d`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 281.7 KB (281708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0242688236000dd8f33d16f89f36da3ef1bb2a7a32bb59a7eb97a18ed3d5158`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0ff47eca4941b373fedcfb40530f4d5ef82aed9a9b83bd7fa6cee6546112fd`  
		Last Modified: Fri, 04 Jun 2021 01:37:12 GMT  
		Size: 104.8 MB (104846719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6991fc153a27c9de6b023272f31bf22b708f788131bd628abeb30592007377a8`  
		Last Modified: Fri, 04 Jun 2021 01:36:59 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b452ba9be082c7a2255414c44dde4b275a327b14d24e947901062089bd7ebf43`  
		Last Modified: Fri, 04 Jun 2021 03:03:37 GMT  
		Size: 6.5 MB (6479039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507d613df3c6f7ea5929ebfe6205e87ae1b89cd044677a765da66d135bb7ef57`  
		Last Modified: Fri, 04 Jun 2021 03:03:37 GMT  
		Size: 1.3 MB (1264524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd9e1c527bba47d9aa0c07957cb156d2c1d205ca81c81e8b00b5b9c0330290b`  
		Last Modified: Fri, 04 Jun 2021 03:03:36 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:5c8e1831e4df2e628cf1bf9d35260d624c1b15d27abfac59a5431f15f3d0a66a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:0cba0bbebbf26fbfe27a39006a093cfb426976baff4e8c3ec906a2a229be9e69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2808421770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c51b9b016f1a3599a109e39809816252f59ecd94d60ef1b7043ab7404059d79`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 12:10:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 12:37:22 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Jun 2021 12:37:25 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Jun 2021 12:37:29 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Jun 2021 12:37:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Jun 2021 12:38:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:38:25 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Jun 2021 12:38:51 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Jun 2021 12:38:53 GMT
ENV GOLANG_VERSION=1.16.5
# Wed, 09 Jun 2021 12:41:22 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:41:27 GMT
WORKDIR C:\gopath
# Wed, 09 Jun 2021 20:15:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:15:04 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 09 Jun 2021 20:15:06 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:15:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Jun 2021 20:15:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Jun 2021 20:15:46 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7863ef96846d497ea06fe442ea13dcecaf5c248ce238c69800475281a4fa848e`  
		Last Modified: Wed, 09 Jun 2021 12:20:41 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f985a0b4390580a94aa3cbc8ecb01fc33805bb3304c4217dc5ec9fb6626011ca`  
		Last Modified: Wed, 09 Jun 2021 13:03:26 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5adf5cc2989b1cf730e7993bd088f778b31b33bac78f6d9c133226f7bcf4a6`  
		Last Modified: Wed, 09 Jun 2021 13:03:24 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480b981517ab26b6ee7e090e51d040995ac5a6a55410880ea3f0c8255dada3bc`  
		Last Modified: Wed, 09 Jun 2021 13:03:24 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a372a8dcfb8f1152565f4b8c928c202db247ddc21fd9a35838a2278c65ff6f`  
		Last Modified: Wed, 09 Jun 2021 13:03:23 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97090ffba94bc8afc85a54e404c8aca13253969fe01c8b0ac1f8ce3a0b909953`  
		Last Modified: Wed, 09 Jun 2021 13:03:53 GMT  
		Size: 25.4 MB (25445694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb1c026791860f230531a960e59a35d86f3ae617c5b6ad60155718694ed3720`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fca536252ace3ea8e08bcd38a313ad63d7d308f4a1d24734c324d191b65647`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 314.6 KB (314587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3865edd5ab3e6e2858d35fea90d96f24eb95579b3bb7f95674954df09b428a8e`  
		Last Modified: Wed, 09 Jun 2021 13:03:20 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424a1b81819edd902af8893d485a39318ee4023db4db6f9c73ebb8470a5c2310`  
		Last Modified: Wed, 09 Jun 2021 13:03:58 GMT  
		Size: 139.4 MB (139355479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f54cc4fcf8b7300908d2cb4aa6dbfe433cc614c35c200ca655b96d576a40412`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 1.6 KB (1596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ae8d8d0f1afc3ddbfe8673534bd1ae7afdf7662fb5fd73ef017088a251e15c`  
		Last Modified: Wed, 09 Jun 2021 20:20:23 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761852a93f82584033e99d58efb7a7e5fad44135d49f23090e1217932f809891`  
		Last Modified: Wed, 09 Jun 2021 20:20:20 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f24be856334e97a03392fc575807609b5afd8808514d9ca8305700e72834ea`  
		Last Modified: Wed, 09 Jun 2021 20:20:20 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047b293c2c055e53ea3099cdc7cd511d55cb43391cbcfd34e0c3a96ac1d179ca`  
		Last Modified: Wed, 09 Jun 2021 20:20:20 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2806e8d39eec5d338e88005243d0a11fcb7c24dab13df4ee3c5ce9ee0266dd9`  
		Last Modified: Wed, 09 Jun 2021 20:20:21 GMT  
		Size: 1.7 MB (1703136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de952f0fc6af6d7eea8c8d4d424cf97622e0b2628a32387976f4dc8df54efb8`  
		Last Modified: Wed, 09 Jun 2021 20:20:20 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:be2e88c1df8f07111be41e7303360a3a48b2c80edee366850af00d9df909afdb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `caddy:builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:4481a6011b8d50eca815372f7a8f28afaae493233d49d4ec20b3d3a5abf93fc7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6437000457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4919458e8d791f772cd7dd820598edd51cc401fa898c7e4ddddc19e6bb2890fe`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 12:41:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 12:41:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Jun 2021 12:41:43 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Jun 2021 12:41:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Jun 2021 12:41:49 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Jun 2021 12:44:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:44:27 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Jun 2021 12:45:49 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Jun 2021 12:45:51 GMT
ENV GOLANG_VERSION=1.16.5
# Wed, 09 Jun 2021 12:49:20 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:49:24 GMT
WORKDIR C:\gopath
# Wed, 09 Jun 2021 20:15:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:15:56 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 09 Jun 2021 20:15:59 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:16:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Jun 2021 20:17:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Jun 2021 20:17:28 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c82e82e95dbad4ccc260b42e03767eb07222e2f00ec57a69b3c87b17da1d2fd3`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a881968e28f8c2900b00800a0de406d0e98740558d9564ad738d053e63d9a1e`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab71df915cf7ac4c559039a917269e11faab2d0e6862a01408431df7fb40362f`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82ce560dcbc3235ed87d6c938aa761616dbd299188ae53a51a266eb37f381f6`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bee5ea2f89fe3f3e514b8dfcd823da340447b633c6048e00773d1c30fbbc0e9`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad71deb840b73610184070ebc7c566bd1dac9cc309d53679460697243bab7640`  
		Last Modified: Wed, 09 Jun 2021 13:04:50 GMT  
		Size: 25.4 MB (25441204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16f2a89ed7a230471eb96b67829deb255795564010b0ff2de47179cdfdec1d0`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cc755175ec255452c16e1e41cc78a8cd719d65f70221e7d128c1dc18eec8f2`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 307.7 KB (307689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d153904f724dbfda646a6c5ccdc1eed2545cf7777c8650461abdedafe75bc693`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ec88320a2e6bf1cfef8856b9271f7d2fa4d2ae8e0eb5b9a44175d04a725631`  
		Last Modified: Wed, 09 Jun 2021 13:04:58 GMT  
		Size: 143.8 MB (143821249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419b516d300f276d9a3f98a1d2c47394abb00b15edeaadcb2f5d0ecee3380f14`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 1.6 KB (1576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d420a2d4c5bca557510bd5eaeea0268b05bb6e61104acea0af1e28c7537c8352`  
		Last Modified: Wed, 09 Jun 2021 20:20:41 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06bf21d106193b12d0b9a688698ec718f7fb4514f317565933b89f22da0d1de`  
		Last Modified: Wed, 09 Jun 2021 20:20:38 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64471c2fb9e42024fce3859860cf6a05f584b8c21ff5c776f7c285588f1117fc`  
		Last Modified: Wed, 09 Jun 2021 20:20:38 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f2c847c9bab79f9970336a628d5b7948504e3f2a67f95cac9a1a3f12132673`  
		Last Modified: Wed, 09 Jun 2021 20:20:38 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae1157ef3d362883b0503349e9d7cb6d729fa420af63a826262dca25f7a9fc`  
		Last Modified: Wed, 09 Jun 2021 20:20:39 GMT  
		Size: 1.7 MB (1684468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e122b3fd6e41cb67b3d9b46e55753aa37f1f60c2de7fab150181822a556d2791`  
		Last Modified: Wed, 09 Jun 2021 20:20:38 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:8031d689a8e6f47dcc146121b75946348e8b2e94a183e92cac38a489f55759a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:c3b2e52162bebaf3b0d128780b3bffc4aa9ccb6953953892dd9d31495e15dc55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14568035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b59636b1388443a36d8173a6ad50dbcf59de4b7786b8178ad9eb656ad6e9a387`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:11:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:04:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 24 May 2021 18:23:10 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:23:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 24 May 2021 18:23:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 24 May 2021 18:23:13 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 24 May 2021 18:23:14 GMT
ENV XDG_DATA_HOME=/data
# Mon, 24 May 2021 18:23:14 GMT
VOLUME [/config]
# Mon, 24 May 2021 18:23:14 GMT
VOLUME [/data]
# Mon, 24 May 2021 18:23:14 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:23:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:23:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:23:16 GMT
EXPOSE 80
# Mon, 24 May 2021 18:23:16 GMT
EXPOSE 443
# Mon, 24 May 2021 18:23:16 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:23:16 GMT
WORKDIR /srv
# Mon, 24 May 2021 18:23:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8294633c5b5606f8e98aaf81da701b7a7e2018dbf82355d1d73830c677034f19`  
		Last Modified: Wed, 14 Apr 2021 20:12:08 GMT  
		Size: 300.4 KB (300403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16798e0582fce7af9c2ba2c8ee4990d0fd1e58384e170ee9937486253d67bbf1`  
		Last Modified: Tue, 11 May 2021 01:05:00 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba0aa26d56032b74c8c88c24edc5a2f7987ea418aaa0966f93ab53c62802c2f`  
		Last Modified: Mon, 24 May 2021 18:23:47 GMT  
		Size: 11.4 MB (11449656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712687f6a8ba00b8b6cb95bad7426eb9964fff3de9f5a7f66dedf6310e8a8c01`  
		Last Modified: Mon, 24 May 2021 18:23:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:eea14e6e8e0ef54944ef2f6e1b6540a536661e033a1f216e92535b5741c2278e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13786866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e11afe23a7696f3f16192af7de16ece9c2dfb73868f2859b9dbacfe0e604fa4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 17:34:28 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 May 2021 17:34:30 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Wed, 26 May 2021 17:34:30 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 26 May 2021 17:34:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 May 2021 17:34:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 May 2021 17:34:33 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 May 2021 17:34:34 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 May 2021 17:34:34 GMT
VOLUME [/config]
# Wed, 26 May 2021 17:34:34 GMT
VOLUME [/data]
# Wed, 26 May 2021 17:34:34 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 26 May 2021 17:34:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 May 2021 17:34:34 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 May 2021 17:34:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 May 2021 17:34:36 GMT
EXPOSE 80
# Wed, 26 May 2021 17:34:36 GMT
EXPOSE 443
# Wed, 26 May 2021 17:34:36 GMT
EXPOSE 2019
# Wed, 26 May 2021 17:34:36 GMT
WORKDIR /srv
# Wed, 26 May 2021 17:34:36 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c2672622a603ff8b0ed8517cfd5adb30b2b35ae40b42cd4ad0545dcb6d3b10`  
		Last Modified: Wed, 26 May 2021 17:36:11 GMT  
		Size: 300.5 KB (300528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b30604f35cc25a62ae1d71a50c6919ad28a2aa67bfd14bebc1984cec5b2c8b`  
		Last Modified: Wed, 26 May 2021 17:36:12 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7119340f7ca66a456adcbc374cbeb7e1c37c35867123bd3fac943aea26a813a8`  
		Last Modified: Wed, 26 May 2021 17:36:15 GMT  
		Size: 10.9 MB (10858201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392497979deecdb2075178245bdf58e8d1ce55c609d2b1320a869392bc007b3f`  
		Last Modified: Wed, 26 May 2021 17:36:12 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:ea6c90777b37ade094ce3f1f5d0efffe39519d18ec589fa4cfa2b6f0c5028e3a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13561305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8637a19be10382ee673bc51be71c9fa3ce23cfdcd0eb9d9bf8734147818227d4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 10:59:27 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 May 2021 10:59:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Wed, 26 May 2021 10:59:29 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 26 May 2021 10:59:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 May 2021 10:59:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 May 2021 10:59:32 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 May 2021 10:59:32 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 May 2021 10:59:32 GMT
VOLUME [/config]
# Wed, 26 May 2021 10:59:33 GMT
VOLUME [/data]
# Wed, 26 May 2021 10:59:33 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 26 May 2021 10:59:33 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 May 2021 10:59:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 May 2021 10:59:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 May 2021 10:59:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 May 2021 10:59:34 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 May 2021 10:59:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 May 2021 10:59:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 May 2021 10:59:34 GMT
EXPOSE 80
# Wed, 26 May 2021 10:59:35 GMT
EXPOSE 443
# Wed, 26 May 2021 10:59:35 GMT
EXPOSE 2019
# Wed, 26 May 2021 10:59:35 GMT
WORKDIR /srv
# Wed, 26 May 2021 10:59:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca051a8c4175c3d7d75c47c9a60045d2f5b7eb415ce35b56c99e9cab58ae3ba`  
		Last Modified: Wed, 26 May 2021 11:01:09 GMT  
		Size: 299.7 KB (299668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2db810fb832f7bd380a39ff7508fa03cc1854bdd51da4cfa239e07fe96fe4e`  
		Last Modified: Wed, 26 May 2021 11:01:09 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce092d490b7e90c7b37879314c23cb48b38be5392715e2d976bc99bbef8a230`  
		Last Modified: Wed, 26 May 2021 11:01:11 GMT  
		Size: 10.8 MB (10831485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb6eb70297874eea11cf38b8870aa1f896bfd6ec638fd6dc9177d7be039001b`  
		Last Modified: Wed, 26 May 2021 11:01:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:ad6d7adcc7d981edfcc5eb4bb42e1fc561b9d0301cadf2ccd920a4a98ae90387
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13415153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:383d427b090897c507d37417dfd21667985cf15a9e3e800b87c821eabe372bb6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 17:52:42 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 May 2021 17:52:43 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Wed, 26 May 2021 17:52:44 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 26 May 2021 17:52:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 May 2021 17:52:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 May 2021 17:52:47 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 May 2021 17:52:47 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 May 2021 17:52:47 GMT
VOLUME [/config]
# Wed, 26 May 2021 17:52:47 GMT
VOLUME [/data]
# Wed, 26 May 2021 17:52:47 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 May 2021 17:52:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 May 2021 17:52:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 May 2021 17:52:49 GMT
EXPOSE 80
# Wed, 26 May 2021 17:52:49 GMT
EXPOSE 443
# Wed, 26 May 2021 17:52:49 GMT
EXPOSE 2019
# Wed, 26 May 2021 17:52:49 GMT
WORKDIR /srv
# Wed, 26 May 2021 17:52:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a305c6848b1bdb9c473c4a3128eff85e1604c1b2d0e78cef80874650b91a49`  
		Last Modified: Wed, 26 May 2021 17:53:57 GMT  
		Size: 300.6 KB (300633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2faea6afac2cf802bf88fd56ee1493ce97eca3a29920702a726ea8e5cd0ea3d`  
		Last Modified: Wed, 26 May 2021 17:53:57 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c196442e5472f13a88f63e7da52cbd15acf171b3d76e87cc47c3073ed0e95d`  
		Last Modified: Wed, 26 May 2021 17:53:59 GMT  
		Size: 10.4 MB (10396489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583f00c174c73f777e3d0cd263a593786c4c341cb20632fafb4246ac0f06f45b`  
		Last Modified: Wed, 26 May 2021 17:53:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:b767e2ec43a11bb1a211e3d7bc76c81d4a256f90084d5747367af6a9730e4f94
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13121818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f930dc44ddd7a57e1d48aaeed66a69653dc4d5c15bdae6c378273cb55287f07b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:12:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:17:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 24 May 2021 18:19:32 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:20:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 24 May 2021 18:20:18 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 24 May 2021 18:20:25 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 24 May 2021 18:20:32 GMT
ENV XDG_DATA_HOME=/data
# Mon, 24 May 2021 18:20:39 GMT
VOLUME [/config]
# Mon, 24 May 2021 18:20:45 GMT
VOLUME [/data]
# Mon, 24 May 2021 18:20:51 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:20:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:21:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:21:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:21:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:21:34 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:21:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:21:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:22:03 GMT
EXPOSE 80
# Mon, 24 May 2021 18:22:10 GMT
EXPOSE 443
# Mon, 24 May 2021 18:22:16 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:22:21 GMT
WORKDIR /srv
# Mon, 24 May 2021 18:22:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25908330df11bb7bc2ed71aa9b4de279db5492df2b03ced3f6650b25821c4584`  
		Last Modified: Wed, 14 Apr 2021 22:16:00 GMT  
		Size: 302.6 KB (302554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a224581e3ba4733f37686f5a5d5375019f9126a0ded6ed20f13e09e898dc735e`  
		Last Modified: Tue, 11 May 2021 01:20:08 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c6214f82b33045060ad6f882d1ed7a5779be7a0883c4da8306ab03e9e2623c`  
		Last Modified: Mon, 24 May 2021 18:23:37 GMT  
		Size: 10.0 MB (10000116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52a67b9935763896cc7c3386cd93b5f7fbc80093549e39f460dc7e170f679f4`  
		Last Modified: Mon, 24 May 2021 18:23:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:40e8d6bc1ad5c4c4f902426841f39a594dd3842c212bed7ecbb66f312b5a4f6e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13938687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c9fccd235488bb04e0075ea4a47a8c102dce45c98cbba05e4d7d0d0ebb13b1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:07:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 10 May 2021 23:41:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 24 May 2021 17:41:40 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 17:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 24 May 2021 17:41:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 24 May 2021 17:41:48 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 24 May 2021 17:41:48 GMT
ENV XDG_DATA_HOME=/data
# Mon, 24 May 2021 17:41:49 GMT
VOLUME [/config]
# Mon, 24 May 2021 17:41:50 GMT
VOLUME [/data]
# Mon, 24 May 2021 17:41:50 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 17:41:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 17:41:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 17:41:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 17:41:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 17:41:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 17:41:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 17:41:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 17:41:55 GMT
EXPOSE 80
# Mon, 24 May 2021 17:41:56 GMT
EXPOSE 443
# Mon, 24 May 2021 17:41:57 GMT
EXPOSE 2019
# Mon, 24 May 2021 17:41:57 GMT
WORKDIR /srv
# Mon, 24 May 2021 17:41:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db3c8b812fcb0d1bfd42c16c2e9ac68f4f3006382c5362e969d1c9eb3a9fab5`  
		Last Modified: Wed, 14 Apr 2021 20:08:26 GMT  
		Size: 300.8 KB (300847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba030675d7bb5bc251d93896d2c81ed8a2f4f4ef2e8e84ad7dfdce9886387c`  
		Last Modified: Mon, 10 May 2021 23:42:29 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03e81629e078650b941a4beb267a6755133e90fa22a688bffb5df188e069c55`  
		Last Modified: Mon, 24 May 2021 17:42:37 GMT  
		Size: 11.0 MB (11029189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbee1e7ec347a65e5e78b46b8fe541241e3f6c13a468785945abd0aaba24545`  
		Last Modified: Mon, 24 May 2021 17:42:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:d4a3e0eabf14e4f98a9bcf5eada28d1443573b082afe95028d548d5b88a2b33e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2654170862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:736d3aa581b715efdf7c0431ebfbaed21b664091d8e8f7e4595c5f9dabbd2acb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 12:10:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:08:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Jun 2021 20:08:07 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:08:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Jun 2021 20:08:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Jun 2021 20:08:49 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Jun 2021 20:08:51 GMT
VOLUME [c:/config]
# Wed, 09 Jun 2021 20:08:53 GMT
VOLUME [c:/data]
# Wed, 09 Jun 2021 20:08:55 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 09 Jun 2021 20:08:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Jun 2021 20:09:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Jun 2021 20:09:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Jun 2021 20:09:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Jun 2021 20:09:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Jun 2021 20:09:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Jun 2021 20:09:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Jun 2021 20:09:14 GMT
EXPOSE 80
# Wed, 09 Jun 2021 20:09:17 GMT
EXPOSE 443
# Wed, 09 Jun 2021 20:09:19 GMT
EXPOSE 2019
# Wed, 09 Jun 2021 20:09:41 GMT
RUN caddy version
# Wed, 09 Jun 2021 20:09:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7863ef96846d497ea06fe442ea13dcecaf5c248ce238c69800475281a4fa848e`  
		Last Modified: Wed, 09 Jun 2021 12:20:41 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dc18d712eacfb666370e311daaf51e09fc2f76ca762e4592e149fbe6aba561`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 361.4 KB (361380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b774f6019fa0c611532d02bdf31c54e9da56fe2330e3e0745538ef036cfb87`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e977598d13d0ee9ae780f2cf34706c57e810301d20d9fc8286ad9390b9166b`  
		Last Modified: Wed, 09 Jun 2021 20:19:37 GMT  
		Size: 11.9 MB (11906202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7361692fe34486902f2dd9f69cc3bce54c4cb8c5c86ed80a0d75033f25ae5213`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35d39d3918ab9262122b494a653aec25e76a65396f9198d7be955cb9c26c6f3`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66891a50a919af8d3cb83358a7f8d33b2055c143bd3499cc431fd32d053ed393`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519d446a1689a5424a77bf1cbf0f00153b28c6eff9ee22f0f88e0e32b3f6bda3`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534ea2eef93aa67b4ac4bfb48ac5498fa33b02d0b88b9ae60b8ae159addacecc`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19fc40bc9ade11a1755b185c529e961b474d959d45a44b1b1ab5f12e3d17863a`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ef9960b6bac284e65c351bc447bb8931486a0c1c3ee68c9e5a62828b4ae0e`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cfda8707421463aa0f297ce5d4ac3a615f60caf56e6e69a299caa08a04f7da`  
		Last Modified: Wed, 09 Jun 2021 20:19:29 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa0c9ece6e3482cf3ffc8d9a087d113db0f7c249f59bcf06f3ffc65c5e4bce0`  
		Last Modified: Wed, 09 Jun 2021 20:19:29 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6614223fb410a8262956f73a038f6d79b67d5976fe8740b21dfa2121a9cbd7f2`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f354857e070035731eb660ec35ff9f8549b6cc79211bab40ae642d9875f98f8b`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc94f29a4cb79013fce0bf1a5776868fa31912b598231e46883a114d86f712d3`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e536fde913e2e2d5ae24846adca32195330a9be6e7d1c3180ce7ac6bc6a35ae1`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b11db027637bf7abeec6bbcd83920c4eb7c291aeeae4d2886a1563bf41289a6`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3a70d973d27d739faae877290b3184bee11c706ebd4bfa515d180fba88ef0f`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc7b3e3d99424f8d3737a4502a6f50767ae25b699a315155b98700af682b64f`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 292.6 KB (292631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d435932a64bec158a6193fa4a31a1b38e446ec9f63c0b6be3282c3acf3288949`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:e7e7af29e7917229552a0c802147dba99fb7a1427b84296a2c60ea7e19cbcb0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278267906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7184db699efd0a2ce0077179784cc7277e5faa7d07534ea1ce32d61d7f46ebc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 12:41:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:11:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Jun 2021 20:11:30 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:13:06 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Jun 2021 20:13:09 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Jun 2021 20:13:11 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Jun 2021 20:13:15 GMT
VOLUME [c:/config]
# Wed, 09 Jun 2021 20:13:18 GMT
VOLUME [c:/data]
# Wed, 09 Jun 2021 20:13:20 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 09 Jun 2021 20:13:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Jun 2021 20:13:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Jun 2021 20:13:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Jun 2021 20:13:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Jun 2021 20:13:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Jun 2021 20:13:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Jun 2021 20:13:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Jun 2021 20:13:40 GMT
EXPOSE 80
# Wed, 09 Jun 2021 20:13:42 GMT
EXPOSE 443
# Wed, 09 Jun 2021 20:13:45 GMT
EXPOSE 2019
# Wed, 09 Jun 2021 20:14:40 GMT
RUN caddy version
# Wed, 09 Jun 2021 20:14:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c82e82e95dbad4ccc260b42e03767eb07222e2f00ec57a69b3c87b17da1d2fd3`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a28e390d3b8e7b9369b102914eaee6e1fa0d14eb258b628be67f99f32f06f81`  
		Last Modified: Wed, 09 Jun 2021 20:20:01 GMT  
		Size: 357.4 KB (357370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7f07987f083e935103f83e47894b93aceaf05d1ded81dd09eb0bc3c8e45af`  
		Last Modified: Wed, 09 Jun 2021 20:20:01 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e65ddfdcdd60907208873b2a532cc58bc0f57d144430cef2c7630e80e4fd1e`  
		Last Modified: Wed, 09 Jun 2021 20:20:05 GMT  
		Size: 11.9 MB (11896985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58e4679b7ef7e1b9d82f44a6b5055c6916801193550bcce3ce390851224c736`  
		Last Modified: Wed, 09 Jun 2021 20:20:00 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107d803623512ea83de929509cc68f334261f2018c60bde60a99eadd0c2b179`  
		Last Modified: Wed, 09 Jun 2021 20:20:00 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f757538ddb020d145715a4890594958e741fe98366f1a58314361e5a8a3487`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462510ee9cb1c642e2804f8f607f02ccc5c31b63c956b9394bf38c5041b10d8b`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e87709f8365472aa7278651dacfc7eee93b24859a494cf6904b4f7ce80df0a`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5439b862b8218f1d7e0e0269efdbed614475ffbdcbaac06a3953f80b07677a1a`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1950c17917c025587fa23872145ee00eaaa11939dc87314c1aa74119db642d`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84164685053ad8b12a46e198ec2e93143d1df956bbbd4af76c88d0f549031c60`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103b7e93d2e2faefef7bd14bc00910442ce8da843f4fb726e2dba2d97752ddc9`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046d1e0cd75d46944ff833afe00c5dc9835ec1eb72876965a98a1488778910a6`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593a0ce075f6e5e07785dd7cd14aa1c274339da4d6f80495f0d1a85fabdef5db`  
		Last Modified: Wed, 09 Jun 2021 20:19:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14f5cdc43c91f65e6c5879691adc6e392d353807b27465a9b270fe7a06da51c`  
		Last Modified: Wed, 09 Jun 2021 20:19:55 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd488f5f58644d68e5103098932448a58d05a716861b26bf33376e75ad27e61`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c218cc3caa4b354c536ad99d30753a6eb41c52a58c52aafc0655a8482382a07`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3dad29a1e0241680f68697c2b0dbca8e85d0084faef4bdd3e66c8294be80671`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daeda652af05f03b2ec029aa5caa6b49d533546fa8347f5b1db003e8a83a7c30`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 260.8 KB (260840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9779c5588bf525e972d3b02ecaeeee32f3939ef8d54e8a16c52e0e62804e2e42`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:3f315a56b68ba9264142c6087b0db8f08492d6a8f90e8f16604e23920a1753fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:d4a3e0eabf14e4f98a9bcf5eada28d1443573b082afe95028d548d5b88a2b33e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2654170862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:736d3aa581b715efdf7c0431ebfbaed21b664091d8e8f7e4595c5f9dabbd2acb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 12:10:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:08:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Jun 2021 20:08:07 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:08:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Jun 2021 20:08:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Jun 2021 20:08:49 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Jun 2021 20:08:51 GMT
VOLUME [c:/config]
# Wed, 09 Jun 2021 20:08:53 GMT
VOLUME [c:/data]
# Wed, 09 Jun 2021 20:08:55 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 09 Jun 2021 20:08:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Jun 2021 20:09:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Jun 2021 20:09:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Jun 2021 20:09:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Jun 2021 20:09:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Jun 2021 20:09:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Jun 2021 20:09:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Jun 2021 20:09:14 GMT
EXPOSE 80
# Wed, 09 Jun 2021 20:09:17 GMT
EXPOSE 443
# Wed, 09 Jun 2021 20:09:19 GMT
EXPOSE 2019
# Wed, 09 Jun 2021 20:09:41 GMT
RUN caddy version
# Wed, 09 Jun 2021 20:09:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7863ef96846d497ea06fe442ea13dcecaf5c248ce238c69800475281a4fa848e`  
		Last Modified: Wed, 09 Jun 2021 12:20:41 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dc18d712eacfb666370e311daaf51e09fc2f76ca762e4592e149fbe6aba561`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 361.4 KB (361380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b774f6019fa0c611532d02bdf31c54e9da56fe2330e3e0745538ef036cfb87`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e977598d13d0ee9ae780f2cf34706c57e810301d20d9fc8286ad9390b9166b`  
		Last Modified: Wed, 09 Jun 2021 20:19:37 GMT  
		Size: 11.9 MB (11906202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7361692fe34486902f2dd9f69cc3bce54c4cb8c5c86ed80a0d75033f25ae5213`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35d39d3918ab9262122b494a653aec25e76a65396f9198d7be955cb9c26c6f3`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66891a50a919af8d3cb83358a7f8d33b2055c143bd3499cc431fd32d053ed393`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519d446a1689a5424a77bf1cbf0f00153b28c6eff9ee22f0f88e0e32b3f6bda3`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534ea2eef93aa67b4ac4bfb48ac5498fa33b02d0b88b9ae60b8ae159addacecc`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19fc40bc9ade11a1755b185c529e961b474d959d45a44b1b1ab5f12e3d17863a`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ef9960b6bac284e65c351bc447bb8931486a0c1c3ee68c9e5a62828b4ae0e`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cfda8707421463aa0f297ce5d4ac3a615f60caf56e6e69a299caa08a04f7da`  
		Last Modified: Wed, 09 Jun 2021 20:19:29 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa0c9ece6e3482cf3ffc8d9a087d113db0f7c249f59bcf06f3ffc65c5e4bce0`  
		Last Modified: Wed, 09 Jun 2021 20:19:29 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6614223fb410a8262956f73a038f6d79b67d5976fe8740b21dfa2121a9cbd7f2`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f354857e070035731eb660ec35ff9f8549b6cc79211bab40ae642d9875f98f8b`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc94f29a4cb79013fce0bf1a5776868fa31912b598231e46883a114d86f712d3`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e536fde913e2e2d5ae24846adca32195330a9be6e7d1c3180ce7ac6bc6a35ae1`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b11db027637bf7abeec6bbcd83920c4eb7c291aeeae4d2886a1563bf41289a6`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3a70d973d27d739faae877290b3184bee11c706ebd4bfa515d180fba88ef0f`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc7b3e3d99424f8d3737a4502a6f50767ae25b699a315155b98700af682b64f`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 292.6 KB (292631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d435932a64bec158a6193fa4a31a1b38e446ec9f63c0b6be3282c3acf3288949`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:e7e7af29e7917229552a0c802147dba99fb7a1427b84296a2c60ea7e19cbcb0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278267906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7184db699efd0a2ce0077179784cc7277e5faa7d07534ea1ce32d61d7f46ebc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 12:41:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:11:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Jun 2021 20:11:30 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:13:06 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Jun 2021 20:13:09 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Jun 2021 20:13:11 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Jun 2021 20:13:15 GMT
VOLUME [c:/config]
# Wed, 09 Jun 2021 20:13:18 GMT
VOLUME [c:/data]
# Wed, 09 Jun 2021 20:13:20 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 09 Jun 2021 20:13:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Jun 2021 20:13:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Jun 2021 20:13:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Jun 2021 20:13:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Jun 2021 20:13:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Jun 2021 20:13:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Jun 2021 20:13:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Jun 2021 20:13:40 GMT
EXPOSE 80
# Wed, 09 Jun 2021 20:13:42 GMT
EXPOSE 443
# Wed, 09 Jun 2021 20:13:45 GMT
EXPOSE 2019
# Wed, 09 Jun 2021 20:14:40 GMT
RUN caddy version
# Wed, 09 Jun 2021 20:14:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c82e82e95dbad4ccc260b42e03767eb07222e2f00ec57a69b3c87b17da1d2fd3`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a28e390d3b8e7b9369b102914eaee6e1fa0d14eb258b628be67f99f32f06f81`  
		Last Modified: Wed, 09 Jun 2021 20:20:01 GMT  
		Size: 357.4 KB (357370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7f07987f083e935103f83e47894b93aceaf05d1ded81dd09eb0bc3c8e45af`  
		Last Modified: Wed, 09 Jun 2021 20:20:01 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e65ddfdcdd60907208873b2a532cc58bc0f57d144430cef2c7630e80e4fd1e`  
		Last Modified: Wed, 09 Jun 2021 20:20:05 GMT  
		Size: 11.9 MB (11896985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58e4679b7ef7e1b9d82f44a6b5055c6916801193550bcce3ce390851224c736`  
		Last Modified: Wed, 09 Jun 2021 20:20:00 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107d803623512ea83de929509cc68f334261f2018c60bde60a99eadd0c2b179`  
		Last Modified: Wed, 09 Jun 2021 20:20:00 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f757538ddb020d145715a4890594958e741fe98366f1a58314361e5a8a3487`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462510ee9cb1c642e2804f8f607f02ccc5c31b63c956b9394bf38c5041b10d8b`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e87709f8365472aa7278651dacfc7eee93b24859a494cf6904b4f7ce80df0a`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5439b862b8218f1d7e0e0269efdbed614475ffbdcbaac06a3953f80b07677a1a`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1950c17917c025587fa23872145ee00eaaa11939dc87314c1aa74119db642d`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84164685053ad8b12a46e198ec2e93143d1df956bbbd4af76c88d0f549031c60`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103b7e93d2e2faefef7bd14bc00910442ce8da843f4fb726e2dba2d97752ddc9`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046d1e0cd75d46944ff833afe00c5dc9835ec1eb72876965a98a1488778910a6`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593a0ce075f6e5e07785dd7cd14aa1c274339da4d6f80495f0d1a85fabdef5db`  
		Last Modified: Wed, 09 Jun 2021 20:19:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14f5cdc43c91f65e6c5879691adc6e392d353807b27465a9b270fe7a06da51c`  
		Last Modified: Wed, 09 Jun 2021 20:19:55 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd488f5f58644d68e5103098932448a58d05a716861b26bf33376e75ad27e61`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c218cc3caa4b354c536ad99d30753a6eb41c52a58c52aafc0655a8482382a07`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3dad29a1e0241680f68697c2b0dbca8e85d0084faef4bdd3e66c8294be80671`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daeda652af05f03b2ec029aa5caa6b49d533546fa8347f5b1db003e8a83a7c30`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 260.8 KB (260840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9779c5588bf525e972d3b02ecaeeee32f3939ef8d54e8a16c52e0e62804e2e42`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:699404cfeaf1b53b36b5cad0c6d2fe8858034adb85e80f41f14f9fbe13a22366
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:d4a3e0eabf14e4f98a9bcf5eada28d1443573b082afe95028d548d5b88a2b33e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2654170862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:736d3aa581b715efdf7c0431ebfbaed21b664091d8e8f7e4595c5f9dabbd2acb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 12:10:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:08:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Jun 2021 20:08:07 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:08:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Jun 2021 20:08:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Jun 2021 20:08:49 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Jun 2021 20:08:51 GMT
VOLUME [c:/config]
# Wed, 09 Jun 2021 20:08:53 GMT
VOLUME [c:/data]
# Wed, 09 Jun 2021 20:08:55 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 09 Jun 2021 20:08:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Jun 2021 20:09:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Jun 2021 20:09:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Jun 2021 20:09:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Jun 2021 20:09:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Jun 2021 20:09:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Jun 2021 20:09:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Jun 2021 20:09:14 GMT
EXPOSE 80
# Wed, 09 Jun 2021 20:09:17 GMT
EXPOSE 443
# Wed, 09 Jun 2021 20:09:19 GMT
EXPOSE 2019
# Wed, 09 Jun 2021 20:09:41 GMT
RUN caddy version
# Wed, 09 Jun 2021 20:09:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7863ef96846d497ea06fe442ea13dcecaf5c248ce238c69800475281a4fa848e`  
		Last Modified: Wed, 09 Jun 2021 12:20:41 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dc18d712eacfb666370e311daaf51e09fc2f76ca762e4592e149fbe6aba561`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 361.4 KB (361380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b774f6019fa0c611532d02bdf31c54e9da56fe2330e3e0745538ef036cfb87`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e977598d13d0ee9ae780f2cf34706c57e810301d20d9fc8286ad9390b9166b`  
		Last Modified: Wed, 09 Jun 2021 20:19:37 GMT  
		Size: 11.9 MB (11906202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7361692fe34486902f2dd9f69cc3bce54c4cb8c5c86ed80a0d75033f25ae5213`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35d39d3918ab9262122b494a653aec25e76a65396f9198d7be955cb9c26c6f3`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66891a50a919af8d3cb83358a7f8d33b2055c143bd3499cc431fd32d053ed393`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519d446a1689a5424a77bf1cbf0f00153b28c6eff9ee22f0f88e0e32b3f6bda3`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534ea2eef93aa67b4ac4bfb48ac5498fa33b02d0b88b9ae60b8ae159addacecc`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19fc40bc9ade11a1755b185c529e961b474d959d45a44b1b1ab5f12e3d17863a`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ef9960b6bac284e65c351bc447bb8931486a0c1c3ee68c9e5a62828b4ae0e`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cfda8707421463aa0f297ce5d4ac3a615f60caf56e6e69a299caa08a04f7da`  
		Last Modified: Wed, 09 Jun 2021 20:19:29 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa0c9ece6e3482cf3ffc8d9a087d113db0f7c249f59bcf06f3ffc65c5e4bce0`  
		Last Modified: Wed, 09 Jun 2021 20:19:29 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6614223fb410a8262956f73a038f6d79b67d5976fe8740b21dfa2121a9cbd7f2`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f354857e070035731eb660ec35ff9f8549b6cc79211bab40ae642d9875f98f8b`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc94f29a4cb79013fce0bf1a5776868fa31912b598231e46883a114d86f712d3`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e536fde913e2e2d5ae24846adca32195330a9be6e7d1c3180ce7ac6bc6a35ae1`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b11db027637bf7abeec6bbcd83920c4eb7c291aeeae4d2886a1563bf41289a6`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3a70d973d27d739faae877290b3184bee11c706ebd4bfa515d180fba88ef0f`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc7b3e3d99424f8d3737a4502a6f50767ae25b699a315155b98700af682b64f`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 292.6 KB (292631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d435932a64bec158a6193fa4a31a1b38e446ec9f63c0b6be3282c3acf3288949`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:f07a9aef54a1c73076c58ba7037c8840b67601723e6dbf534878e515d02f519d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `caddy:windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:e7e7af29e7917229552a0c802147dba99fb7a1427b84296a2c60ea7e19cbcb0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278267906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7184db699efd0a2ce0077179784cc7277e5faa7d07534ea1ce32d61d7f46ebc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 12:41:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:11:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Jun 2021 20:11:30 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:13:06 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Jun 2021 20:13:09 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Jun 2021 20:13:11 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Jun 2021 20:13:15 GMT
VOLUME [c:/config]
# Wed, 09 Jun 2021 20:13:18 GMT
VOLUME [c:/data]
# Wed, 09 Jun 2021 20:13:20 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 09 Jun 2021 20:13:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Jun 2021 20:13:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Jun 2021 20:13:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Jun 2021 20:13:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Jun 2021 20:13:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Jun 2021 20:13:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Jun 2021 20:13:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Jun 2021 20:13:40 GMT
EXPOSE 80
# Wed, 09 Jun 2021 20:13:42 GMT
EXPOSE 443
# Wed, 09 Jun 2021 20:13:45 GMT
EXPOSE 2019
# Wed, 09 Jun 2021 20:14:40 GMT
RUN caddy version
# Wed, 09 Jun 2021 20:14:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c82e82e95dbad4ccc260b42e03767eb07222e2f00ec57a69b3c87b17da1d2fd3`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a28e390d3b8e7b9369b102914eaee6e1fa0d14eb258b628be67f99f32f06f81`  
		Last Modified: Wed, 09 Jun 2021 20:20:01 GMT  
		Size: 357.4 KB (357370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7f07987f083e935103f83e47894b93aceaf05d1ded81dd09eb0bc3c8e45af`  
		Last Modified: Wed, 09 Jun 2021 20:20:01 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e65ddfdcdd60907208873b2a532cc58bc0f57d144430cef2c7630e80e4fd1e`  
		Last Modified: Wed, 09 Jun 2021 20:20:05 GMT  
		Size: 11.9 MB (11896985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58e4679b7ef7e1b9d82f44a6b5055c6916801193550bcce3ce390851224c736`  
		Last Modified: Wed, 09 Jun 2021 20:20:00 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107d803623512ea83de929509cc68f334261f2018c60bde60a99eadd0c2b179`  
		Last Modified: Wed, 09 Jun 2021 20:20:00 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f757538ddb020d145715a4890594958e741fe98366f1a58314361e5a8a3487`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462510ee9cb1c642e2804f8f607f02ccc5c31b63c956b9394bf38c5041b10d8b`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e87709f8365472aa7278651dacfc7eee93b24859a494cf6904b4f7ce80df0a`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5439b862b8218f1d7e0e0269efdbed614475ffbdcbaac06a3953f80b07677a1a`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1950c17917c025587fa23872145ee00eaaa11939dc87314c1aa74119db642d`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84164685053ad8b12a46e198ec2e93143d1df956bbbd4af76c88d0f549031c60`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103b7e93d2e2faefef7bd14bc00910442ce8da843f4fb726e2dba2d97752ddc9`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046d1e0cd75d46944ff833afe00c5dc9835ec1eb72876965a98a1488778910a6`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593a0ce075f6e5e07785dd7cd14aa1c274339da4d6f80495f0d1a85fabdef5db`  
		Last Modified: Wed, 09 Jun 2021 20:19:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14f5cdc43c91f65e6c5879691adc6e392d353807b27465a9b270fe7a06da51c`  
		Last Modified: Wed, 09 Jun 2021 20:19:55 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd488f5f58644d68e5103098932448a58d05a716861b26bf33376e75ad27e61`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c218cc3caa4b354c536ad99d30753a6eb41c52a58c52aafc0655a8482382a07`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3dad29a1e0241680f68697c2b0dbca8e85d0084faef4bdd3e66c8294be80671`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daeda652af05f03b2ec029aa5caa6b49d533546fa8347f5b1db003e8a83a7c30`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 260.8 KB (260840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9779c5588bf525e972d3b02ecaeeee32f3939ef8d54e8a16c52e0e62804e2e42`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
