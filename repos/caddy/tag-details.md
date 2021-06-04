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
$ docker pull caddy@sha256:1a2f489f3bbeef0cac9397b7064a7908ed3f74b89d6f549825c38f175047d03d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

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

### `caddy:2` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:1d0e1085c4e0fd3af411a60364e53d9e9ded463184467a4f1595116eb2e4c675
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2491869666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dac2e4738ade97d420148e609ac6c7a6db9edb6db52f3a634814cbe64df1d0b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:56:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 24 May 2021 18:14:49 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:15:23 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 24 May 2021 18:15:24 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 24 May 2021 18:15:25 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 24 May 2021 18:15:27 GMT
VOLUME [c:/config]
# Mon, 24 May 2021 18:15:28 GMT
VOLUME [c:/data]
# Mon, 24 May 2021 18:15:29 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:15:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:15:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:15:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:15:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:15:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:15:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:15:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:15:39 GMT
EXPOSE 80
# Mon, 24 May 2021 18:15:40 GMT
EXPOSE 443
# Mon, 24 May 2021 18:15:41 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:16:00 GMT
RUN caddy version
# Mon, 24 May 2021 18:16:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dc51194378204d7114732c3ee4da8d6b390b048e70ae1535a082de3ff67b5c`  
		Last Modified: Wed, 12 May 2021 20:06:24 GMT  
		Size: 5.1 MB (5106604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81697a0f2a55f882f55ccac9401c3dd272607c42f460a8549f30a1ebb26e0c8`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6400e9488fa4d970dad72e844be39d2d75b7d2c31501c6d6b23d6a1bc524f7c1`  
		Last Modified: Mon, 24 May 2021 18:22:57 GMT  
		Size: 11.9 MB (11930419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5b5da05058a691610222ba26189e6f6c28b9ede612bec34b4ed5dea3691b92`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197bdfed68cccee24a939b4dd69fea66e2dc7827a4017bf444bdd2c90e959f6a`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474f7ecfe9858ec31d5203cc051d4063e0ad4acd2af33e4568f49d9e4b75e41b`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e026dffad92f6dace75c209e6f261b00cf847128dd907ffa4ac9f944e9ae054e`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c534d757d31dc1e6130a58f06b95d25d61f32e015e329cd2227a1bed890280`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31071464c175eef4ea5843313a962e550e530c0a4c12fd997c6ace04fed5d0e0`  
		Last Modified: Mon, 24 May 2021 18:22:51 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3035f85e6f0ef498e48d22a196b3dca2d1feff90554b2f1fbbd3062a92ffccd2`  
		Last Modified: Mon, 24 May 2021 18:22:51 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caffd6e1f83b89b2831eab80faf22c370ad73519467e80354cb56ee96eed7fe3`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285714c5a6fb40773b7e624641f8e036180ab3424ee89b84f3fbbd79d7108eec`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872e853821b7661d1e753ef89a95c2525171915b5dec31950f7b05f4492eb40c`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7958b6b43cba2b3e1a20dc772e84541237901c32ec6dba998eb300627b2e343`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8089fe8b99a3884b64fb515b432248ed2433347b16efe53190c08624ec8bcf8f`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e25c6bfe294987f6c4c3a677078ea11dd90d54892fff638abed3d5a8602360c`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1757220b38637dda7da307ac64a4eefb9226cd9e13d613ab9bb839997c0c2aa8`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a748ef821631911b8abd470af8b29305283a82e1b5da1d2459257d8308576a2`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa22970d4f705eac4e8ea2ac4a7f3e89cfc01035b6ff0bf8998c146fe4d9a96`  
		Last Modified: Mon, 24 May 2021 18:22:47 GMT  
		Size: 317.9 KB (317938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2477d94c5c1388771379c903fc8931c2531d21a7ccbef4b3b7e2d6461fb19fdd`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:d530e436d6d892bc2662481a943d230921dd8d5b2a26de0d99c32abb59ce1973
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5819027610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:189fbf35362e472481d308f9fbecfeda8962471fccd521c1cdd2165bfff22c08`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:58:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 24 May 2021 18:16:16 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:17:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 24 May 2021 18:18:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 24 May 2021 18:18:02 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 24 May 2021 18:18:03 GMT
VOLUME [c:/config]
# Mon, 24 May 2021 18:18:04 GMT
VOLUME [c:/data]
# Mon, 24 May 2021 18:18:05 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:18:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:18:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:18:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:18:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:18:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:18:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:18:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:18:14 GMT
EXPOSE 80
# Mon, 24 May 2021 18:18:15 GMT
EXPOSE 443
# Mon, 24 May 2021 18:18:16 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:19:09 GMT
RUN caddy version
# Mon, 24 May 2021 18:19:10 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26858854e9a4d33437022a0cbf481973fa7709cc09d3402af046620cbbe5c0`  
		Last Modified: Wed, 12 May 2021 20:07:13 GMT  
		Size: 5.7 MB (5714091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba52519d045fbbd4b405dea0a101b9ede50767ce1b8b92f0b0a9708dc3a3492`  
		Last Modified: Mon, 24 May 2021 18:23:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073bc62336c22adb06e7c530733538c823c0e30b591f536ca853dd86ff16e632`  
		Last Modified: Mon, 24 May 2021 18:23:26 GMT  
		Size: 17.2 MB (17244195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319fcbb76d6ed2f5920ae3cf875486281ed4d5edc53c630c8c6ad581efc92594`  
		Last Modified: Mon, 24 May 2021 18:23:22 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d372740cbc98799ef99cd14fe521f6c8bc0202f7e6eb418f8db3e6cae94caf60`  
		Last Modified: Mon, 24 May 2021 18:23:21 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c1957ce089769a88ac826364c0cb191ae826407602ccf505c76ee34afa10c8`  
		Last Modified: Mon, 24 May 2021 18:23:20 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e022ba7739dc4609e4838ae24c6930ccdc82d0721cc978c71a7e036122adf228`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5716dc07e962e5602a2cecf1a5b63c75352ad0e48b06b30070ad5cd4a31993`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc94100cd9e1fb3620069275788a9e1b912502dcd7966b4d624ecba5f88690`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7790197c85ec7196ed9b956d8f481e8f382479a3b8e20db4d8e564f14331eb42`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60939c5f58f38df81a8563072d42fcd4fb79292dbf5ce4d31a46f840e777fb88`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d5876f07c48377c92817efa2b077cfe4c05822b08a1916d350b5e8ee682b50`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2933951452131d66acb34683269ade093ebb9faf312436b0a601168cb6e2fe68`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ad33c6332b1b2a8e806339fd2978dd9a8919fc98d48fc0ae6a58ad07870cec`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b44c787b930665927a13e544b5d3d7243caae27d4d9a6f9502f985e8483af61`  
		Last Modified: Mon, 24 May 2021 18:23:16 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e86dd1b42134f467b929f29aa052bdca8a20ccbb6ff1332575ef7843b962243`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3288b716f0b64cb14a9da486b126557c121b9a71476d5aea6a1be399a82bb14b`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83f9226706657b746cb502303856ebeca1a6cda85b1aea65196506c3e3faa4a`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fc7b2fb07d7a4265b695bf44d6d3378e7f0202a6c8fd0d359f766886070802`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 266.6 KB (266650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cde5c4ac8767e62fceac7aed63a74d7935277b8087425319abfe8e22f7bb37`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1435 bytes)  
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
$ docker pull caddy@sha256:fb66ce856e2039c6e0cb70dba12e8a7f50a9cd7ef53905a4307cff6e9220f682
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

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

### `caddy:2-builder` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:5cd5e5c8ae7367744428893e4a407d97f68f70fbd298770c1518b65f3b740476
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646121085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b3e2a6c24449822ef29f7460905fddcbb84871a7dfa5dc27265afa64fa3778`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:24:28 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:24:29 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:24:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:24:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:25:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:25:36 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:26:02 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Jun 2021 01:19:04 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 01:21:38 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Jun 2021 01:21:40 GMT
WORKDIR C:\gopath
# Fri, 04 Jun 2021 02:10:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Jun 2021 02:10:55 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 02:10:56 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 02:10:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 02:11:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Jun 2021 02:11:25 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2a5ccd12170e9f926c3e069a2fa2ed38b5dd5596869ed982bccc50ef80cf1f`  
		Last Modified: Wed, 12 May 2021 12:52:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd5b5fa12081ad53ae688dc454e550dd50bd414c949724180719b0326632c4a`  
		Last Modified: Wed, 12 May 2021 12:52:08 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599ef939f9e7c26d4bc0f8f75820116f6977a64212b86260bc225ae2d850cc31`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bddce42b6f4351510fcb255839a7c55d95546186dce8509782abe959d27d9f0`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2407bf3b614294860b53b94e661f5c57f7dd985934aed5727442f9353bf8c617`  
		Last Modified: Wed, 12 May 2021 12:52:14 GMT  
		Size: 30.2 MB (30189126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b01ea9b4210c3201c1462d7ee78b276d7d5ffac3dca02c9c57a0c77c5b87a2`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27be8fd19f331f65055bbf31138aa28628be7534753008620ec14fc1803ebdf2`  
		Last Modified: Wed, 12 May 2021 12:52:05 GMT  
		Size: 313.1 KB (313094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f8e1e31aa0e91f80a0d7a9cf238278557166647fd937cc7b714778366d586a`  
		Last Modified: Fri, 04 Jun 2021 01:40:04 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ba074ffe696278b5b2037378141f68377dcab07cbcf7c6d31fcd4c097869ce`  
		Last Modified: Fri, 04 Jun 2021 01:42:39 GMT  
		Size: 139.4 MB (139388725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2deb8a1660a185bba3fa7aaabc4cb64555918509a91d9f186f15ec469ec476a0`  
		Last Modified: Fri, 04 Jun 2021 01:40:04 GMT  
		Size: 1.6 KB (1586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bce5d3df849365bd1516c0abf3aa29cee32abb96cc1cdf79c2e7019f2016cc0`  
		Last Modified: Fri, 04 Jun 2021 02:14:37 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc77252a6e317a6fcaeba9d070cfad6c4e568f095056d19727ffe6955e1a1c5a`  
		Last Modified: Fri, 04 Jun 2021 02:14:34 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f53aa8e353d64b1c65256ffeeb6708506ca6a23ee2c94016a8f034452259b0`  
		Last Modified: Fri, 04 Jun 2021 02:14:34 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c500d7c801483b02cfdfc1a272882d3b98559bcfacfb956ef4bb395fadccc61`  
		Last Modified: Fri, 04 Jun 2021 02:14:34 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243445945aa8cf8386f4cb635126e213960fe164cc0b2cf9829c40fb29e06dc4`  
		Last Modified: Fri, 04 Jun 2021 02:14:37 GMT  
		Size: 1.7 MB (1722485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5462596ac55051140e5c69946dc7620a0169d39d4b3a3b826e0daf4a0d924e8`  
		Last Modified: Fri, 04 Jun 2021 02:14:35 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:23de8a02fd104f11187fa0e6f1c50d9a833788ef94cc3d78b82ad3b4f35c9fad
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5988471116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4830f2cecfad3d8daa420d50870e8aa44c459224a23f9ff77de7da22e670b94`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:29:13 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:29:14 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:29:15 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:29:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:31:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:31:45 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:33:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Jun 2021 01:21:50 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 01:26:36 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Jun 2021 01:26:38 GMT
WORKDIR C:\gopath
# Fri, 04 Jun 2021 02:11:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Jun 2021 02:11:34 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 02:11:35 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 02:11:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 02:13:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Jun 2021 02:13:06 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10abf429e12c7b3b7d2b0a791d7cdb47866461a7b63df4ddd4f63acc91e26231`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79955f676504cbf77ec284d8e857d18d17b93c5b8e6438b4062dd80f8632c9d6`  
		Last Modified: Wed, 12 May 2021 12:55:12 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24af485ecab19f81a0c65c0eaec6f6fda8749ca50eb53101abcfc5c079f9b1c2`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b782f6bcd162ee81518d73c6c4fe5c5b731ab38b595c16a55ac185db84b2c9b`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1327fc384f9fff64d41446adcb3bdf585307370ef0024a31a5269bae6f30067d`  
		Last Modified: Wed, 12 May 2021 12:55:18 GMT  
		Size: 30.8 MB (30797956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c50f4b0b5994b4154be9fea2ab6c6a0e4c402c44d44795a5ce82ab6f8de4bc`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e458669a58e08411a0641a721ef1daf4af2a568c4dd61e9a3710b07f73b6ec`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 5.7 MB (5661591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7024df9f6db05baebb2373ac9d80a105fbfaafacf00e75d4b28847d1503ea8dc`  
		Last Modified: Fri, 04 Jun 2021 01:42:57 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b83a1b7a993d551850c2952fac9ce015fd85e6e96491ffc601809c6e4c9013`  
		Last Modified: Fri, 04 Jun 2021 01:45:53 GMT  
		Size: 149.2 MB (149182156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03bac4443c0dacba8f0d8dbd25091bc1d39b3ee36e84604482d40220f39f57d`  
		Last Modified: Fri, 04 Jun 2021 01:42:57 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51201b480eb2d1bd5736f2e118d9ddaafafce32222e161cb63b66a46bf95d9f`  
		Last Modified: Fri, 04 Jun 2021 02:14:54 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10338b4cf9e50762fa10529606ac5ab6d7c227a0aefcce7173718d53ef6b341`  
		Last Modified: Fri, 04 Jun 2021 02:14:51 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa84546d6c6cfa9ed6da4b4400af439e067c8f873c8ef40452cc57c7944a065`  
		Last Modified: Fri, 04 Jun 2021 02:14:51 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071bbd37c903648e3ebd95cc6dcb2b78d6ea639005d65aab5016dd7859a4f17b`  
		Last Modified: Fri, 04 Jun 2021 02:14:51 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2215edc22b4111496ab6990dcdc789842dbeaaa2138be04dcbb3ce883e984e`  
		Last Modified: Fri, 04 Jun 2021 02:14:59 GMT  
		Size: 7.0 MB (7033480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2c9d2207f5d9c10b8413a2bdbb9bb17306d47cd8d1efd70a3593d5343de178`  
		Last Modified: Fri, 04 Jun 2021 02:14:51 GMT  
		Size: 1.4 KB (1408 bytes)  
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
$ docker pull caddy@sha256:c6473228286ce37912a7ba2003a626c415698df940f04e7c88430e4ad01e168a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:5cd5e5c8ae7367744428893e4a407d97f68f70fbd298770c1518b65f3b740476
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646121085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b3e2a6c24449822ef29f7460905fddcbb84871a7dfa5dc27265afa64fa3778`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:24:28 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:24:29 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:24:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:24:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:25:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:25:36 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:26:02 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Jun 2021 01:19:04 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 01:21:38 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Jun 2021 01:21:40 GMT
WORKDIR C:\gopath
# Fri, 04 Jun 2021 02:10:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Jun 2021 02:10:55 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 02:10:56 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 02:10:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 02:11:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Jun 2021 02:11:25 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2a5ccd12170e9f926c3e069a2fa2ed38b5dd5596869ed982bccc50ef80cf1f`  
		Last Modified: Wed, 12 May 2021 12:52:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd5b5fa12081ad53ae688dc454e550dd50bd414c949724180719b0326632c4a`  
		Last Modified: Wed, 12 May 2021 12:52:08 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599ef939f9e7c26d4bc0f8f75820116f6977a64212b86260bc225ae2d850cc31`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bddce42b6f4351510fcb255839a7c55d95546186dce8509782abe959d27d9f0`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2407bf3b614294860b53b94e661f5c57f7dd985934aed5727442f9353bf8c617`  
		Last Modified: Wed, 12 May 2021 12:52:14 GMT  
		Size: 30.2 MB (30189126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b01ea9b4210c3201c1462d7ee78b276d7d5ffac3dca02c9c57a0c77c5b87a2`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27be8fd19f331f65055bbf31138aa28628be7534753008620ec14fc1803ebdf2`  
		Last Modified: Wed, 12 May 2021 12:52:05 GMT  
		Size: 313.1 KB (313094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f8e1e31aa0e91f80a0d7a9cf238278557166647fd937cc7b714778366d586a`  
		Last Modified: Fri, 04 Jun 2021 01:40:04 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ba074ffe696278b5b2037378141f68377dcab07cbcf7c6d31fcd4c097869ce`  
		Last Modified: Fri, 04 Jun 2021 01:42:39 GMT  
		Size: 139.4 MB (139388725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2deb8a1660a185bba3fa7aaabc4cb64555918509a91d9f186f15ec469ec476a0`  
		Last Modified: Fri, 04 Jun 2021 01:40:04 GMT  
		Size: 1.6 KB (1586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bce5d3df849365bd1516c0abf3aa29cee32abb96cc1cdf79c2e7019f2016cc0`  
		Last Modified: Fri, 04 Jun 2021 02:14:37 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc77252a6e317a6fcaeba9d070cfad6c4e568f095056d19727ffe6955e1a1c5a`  
		Last Modified: Fri, 04 Jun 2021 02:14:34 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f53aa8e353d64b1c65256ffeeb6708506ca6a23ee2c94016a8f034452259b0`  
		Last Modified: Fri, 04 Jun 2021 02:14:34 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c500d7c801483b02cfdfc1a272882d3b98559bcfacfb956ef4bb395fadccc61`  
		Last Modified: Fri, 04 Jun 2021 02:14:34 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243445945aa8cf8386f4cb635126e213960fe164cc0b2cf9829c40fb29e06dc4`  
		Last Modified: Fri, 04 Jun 2021 02:14:37 GMT  
		Size: 1.7 MB (1722485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5462596ac55051140e5c69946dc7620a0169d39d4b3a3b826e0daf4a0d924e8`  
		Last Modified: Fri, 04 Jun 2021 02:14:35 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:befa7d7c88cc950857d567f8fcd2ba435be538c6e6443ee1f806e755f27ea4ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `caddy:2-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:23de8a02fd104f11187fa0e6f1c50d9a833788ef94cc3d78b82ad3b4f35c9fad
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5988471116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4830f2cecfad3d8daa420d50870e8aa44c459224a23f9ff77de7da22e670b94`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:29:13 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:29:14 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:29:15 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:29:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:31:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:31:45 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:33:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Jun 2021 01:21:50 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 01:26:36 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Jun 2021 01:26:38 GMT
WORKDIR C:\gopath
# Fri, 04 Jun 2021 02:11:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Jun 2021 02:11:34 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 02:11:35 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 02:11:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 02:13:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Jun 2021 02:13:06 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10abf429e12c7b3b7d2b0a791d7cdb47866461a7b63df4ddd4f63acc91e26231`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79955f676504cbf77ec284d8e857d18d17b93c5b8e6438b4062dd80f8632c9d6`  
		Last Modified: Wed, 12 May 2021 12:55:12 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24af485ecab19f81a0c65c0eaec6f6fda8749ca50eb53101abcfc5c079f9b1c2`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b782f6bcd162ee81518d73c6c4fe5c5b731ab38b595c16a55ac185db84b2c9b`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1327fc384f9fff64d41446adcb3bdf585307370ef0024a31a5269bae6f30067d`  
		Last Modified: Wed, 12 May 2021 12:55:18 GMT  
		Size: 30.8 MB (30797956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c50f4b0b5994b4154be9fea2ab6c6a0e4c402c44d44795a5ce82ab6f8de4bc`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e458669a58e08411a0641a721ef1daf4af2a568c4dd61e9a3710b07f73b6ec`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 5.7 MB (5661591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7024df9f6db05baebb2373ac9d80a105fbfaafacf00e75d4b28847d1503ea8dc`  
		Last Modified: Fri, 04 Jun 2021 01:42:57 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b83a1b7a993d551850c2952fac9ce015fd85e6e96491ffc601809c6e4c9013`  
		Last Modified: Fri, 04 Jun 2021 01:45:53 GMT  
		Size: 149.2 MB (149182156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03bac4443c0dacba8f0d8dbd25091bc1d39b3ee36e84604482d40220f39f57d`  
		Last Modified: Fri, 04 Jun 2021 01:42:57 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51201b480eb2d1bd5736f2e118d9ddaafafce32222e161cb63b66a46bf95d9f`  
		Last Modified: Fri, 04 Jun 2021 02:14:54 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10338b4cf9e50762fa10529606ac5ab6d7c227a0aefcce7173718d53ef6b341`  
		Last Modified: Fri, 04 Jun 2021 02:14:51 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa84546d6c6cfa9ed6da4b4400af439e067c8f873c8ef40452cc57c7944a065`  
		Last Modified: Fri, 04 Jun 2021 02:14:51 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071bbd37c903648e3ebd95cc6dcb2b78d6ea639005d65aab5016dd7859a4f17b`  
		Last Modified: Fri, 04 Jun 2021 02:14:51 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2215edc22b4111496ab6990dcdc789842dbeaaa2138be04dcbb3ce883e984e`  
		Last Modified: Fri, 04 Jun 2021 02:14:59 GMT  
		Size: 7.0 MB (7033480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2c9d2207f5d9c10b8413a2bdbb9bb17306d47cd8d1efd70a3593d5343de178`  
		Last Modified: Fri, 04 Jun 2021 02:14:51 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:c544077722bd97f1b56e46cf2c37d89d460d590defbe607243a750a2ab90a554
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:1d0e1085c4e0fd3af411a60364e53d9e9ded463184467a4f1595116eb2e4c675
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2491869666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dac2e4738ade97d420148e609ac6c7a6db9edb6db52f3a634814cbe64df1d0b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:56:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 24 May 2021 18:14:49 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:15:23 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 24 May 2021 18:15:24 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 24 May 2021 18:15:25 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 24 May 2021 18:15:27 GMT
VOLUME [c:/config]
# Mon, 24 May 2021 18:15:28 GMT
VOLUME [c:/data]
# Mon, 24 May 2021 18:15:29 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:15:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:15:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:15:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:15:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:15:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:15:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:15:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:15:39 GMT
EXPOSE 80
# Mon, 24 May 2021 18:15:40 GMT
EXPOSE 443
# Mon, 24 May 2021 18:15:41 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:16:00 GMT
RUN caddy version
# Mon, 24 May 2021 18:16:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dc51194378204d7114732c3ee4da8d6b390b048e70ae1535a082de3ff67b5c`  
		Last Modified: Wed, 12 May 2021 20:06:24 GMT  
		Size: 5.1 MB (5106604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81697a0f2a55f882f55ccac9401c3dd272607c42f460a8549f30a1ebb26e0c8`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6400e9488fa4d970dad72e844be39d2d75b7d2c31501c6d6b23d6a1bc524f7c1`  
		Last Modified: Mon, 24 May 2021 18:22:57 GMT  
		Size: 11.9 MB (11930419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5b5da05058a691610222ba26189e6f6c28b9ede612bec34b4ed5dea3691b92`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197bdfed68cccee24a939b4dd69fea66e2dc7827a4017bf444bdd2c90e959f6a`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474f7ecfe9858ec31d5203cc051d4063e0ad4acd2af33e4568f49d9e4b75e41b`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e026dffad92f6dace75c209e6f261b00cf847128dd907ffa4ac9f944e9ae054e`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c534d757d31dc1e6130a58f06b95d25d61f32e015e329cd2227a1bed890280`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31071464c175eef4ea5843313a962e550e530c0a4c12fd997c6ace04fed5d0e0`  
		Last Modified: Mon, 24 May 2021 18:22:51 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3035f85e6f0ef498e48d22a196b3dca2d1feff90554b2f1fbbd3062a92ffccd2`  
		Last Modified: Mon, 24 May 2021 18:22:51 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caffd6e1f83b89b2831eab80faf22c370ad73519467e80354cb56ee96eed7fe3`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285714c5a6fb40773b7e624641f8e036180ab3424ee89b84f3fbbd79d7108eec`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872e853821b7661d1e753ef89a95c2525171915b5dec31950f7b05f4492eb40c`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7958b6b43cba2b3e1a20dc772e84541237901c32ec6dba998eb300627b2e343`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8089fe8b99a3884b64fb515b432248ed2433347b16efe53190c08624ec8bcf8f`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e25c6bfe294987f6c4c3a677078ea11dd90d54892fff638abed3d5a8602360c`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1757220b38637dda7da307ac64a4eefb9226cd9e13d613ab9bb839997c0c2aa8`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a748ef821631911b8abd470af8b29305283a82e1b5da1d2459257d8308576a2`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa22970d4f705eac4e8ea2ac4a7f3e89cfc01035b6ff0bf8998c146fe4d9a96`  
		Last Modified: Mon, 24 May 2021 18:22:47 GMT  
		Size: 317.9 KB (317938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2477d94c5c1388771379c903fc8931c2531d21a7ccbef4b3b7e2d6461fb19fdd`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:d530e436d6d892bc2662481a943d230921dd8d5b2a26de0d99c32abb59ce1973
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5819027610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:189fbf35362e472481d308f9fbecfeda8962471fccd521c1cdd2165bfff22c08`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:58:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 24 May 2021 18:16:16 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:17:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 24 May 2021 18:18:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 24 May 2021 18:18:02 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 24 May 2021 18:18:03 GMT
VOLUME [c:/config]
# Mon, 24 May 2021 18:18:04 GMT
VOLUME [c:/data]
# Mon, 24 May 2021 18:18:05 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:18:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:18:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:18:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:18:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:18:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:18:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:18:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:18:14 GMT
EXPOSE 80
# Mon, 24 May 2021 18:18:15 GMT
EXPOSE 443
# Mon, 24 May 2021 18:18:16 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:19:09 GMT
RUN caddy version
# Mon, 24 May 2021 18:19:10 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26858854e9a4d33437022a0cbf481973fa7709cc09d3402af046620cbbe5c0`  
		Last Modified: Wed, 12 May 2021 20:07:13 GMT  
		Size: 5.7 MB (5714091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba52519d045fbbd4b405dea0a101b9ede50767ce1b8b92f0b0a9708dc3a3492`  
		Last Modified: Mon, 24 May 2021 18:23:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073bc62336c22adb06e7c530733538c823c0e30b591f536ca853dd86ff16e632`  
		Last Modified: Mon, 24 May 2021 18:23:26 GMT  
		Size: 17.2 MB (17244195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319fcbb76d6ed2f5920ae3cf875486281ed4d5edc53c630c8c6ad581efc92594`  
		Last Modified: Mon, 24 May 2021 18:23:22 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d372740cbc98799ef99cd14fe521f6c8bc0202f7e6eb418f8db3e6cae94caf60`  
		Last Modified: Mon, 24 May 2021 18:23:21 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c1957ce089769a88ac826364c0cb191ae826407602ccf505c76ee34afa10c8`  
		Last Modified: Mon, 24 May 2021 18:23:20 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e022ba7739dc4609e4838ae24c6930ccdc82d0721cc978c71a7e036122adf228`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5716dc07e962e5602a2cecf1a5b63c75352ad0e48b06b30070ad5cd4a31993`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc94100cd9e1fb3620069275788a9e1b912502dcd7966b4d624ecba5f88690`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7790197c85ec7196ed9b956d8f481e8f382479a3b8e20db4d8e564f14331eb42`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60939c5f58f38df81a8563072d42fcd4fb79292dbf5ce4d31a46f840e777fb88`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d5876f07c48377c92817efa2b077cfe4c05822b08a1916d350b5e8ee682b50`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2933951452131d66acb34683269ade093ebb9faf312436b0a601168cb6e2fe68`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ad33c6332b1b2a8e806339fd2978dd9a8919fc98d48fc0ae6a58ad07870cec`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b44c787b930665927a13e544b5d3d7243caae27d4d9a6f9502f985e8483af61`  
		Last Modified: Mon, 24 May 2021 18:23:16 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e86dd1b42134f467b929f29aa052bdca8a20ccbb6ff1332575ef7843b962243`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3288b716f0b64cb14a9da486b126557c121b9a71476d5aea6a1be399a82bb14b`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83f9226706657b746cb502303856ebeca1a6cda85b1aea65196506c3e3faa4a`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fc7b2fb07d7a4265b695bf44d6d3378e7f0202a6c8fd0d359f766886070802`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 266.6 KB (266650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cde5c4ac8767e62fceac7aed63a74d7935277b8087425319abfe8e22f7bb37`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:fb9fcd910a8050aa2ce11ac6b195722843c6efc46c1cf68fbb3a4172914c2e30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:1d0e1085c4e0fd3af411a60364e53d9e9ded463184467a4f1595116eb2e4c675
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2491869666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dac2e4738ade97d420148e609ac6c7a6db9edb6db52f3a634814cbe64df1d0b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:56:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 24 May 2021 18:14:49 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:15:23 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 24 May 2021 18:15:24 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 24 May 2021 18:15:25 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 24 May 2021 18:15:27 GMT
VOLUME [c:/config]
# Mon, 24 May 2021 18:15:28 GMT
VOLUME [c:/data]
# Mon, 24 May 2021 18:15:29 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:15:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:15:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:15:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:15:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:15:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:15:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:15:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:15:39 GMT
EXPOSE 80
# Mon, 24 May 2021 18:15:40 GMT
EXPOSE 443
# Mon, 24 May 2021 18:15:41 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:16:00 GMT
RUN caddy version
# Mon, 24 May 2021 18:16:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dc51194378204d7114732c3ee4da8d6b390b048e70ae1535a082de3ff67b5c`  
		Last Modified: Wed, 12 May 2021 20:06:24 GMT  
		Size: 5.1 MB (5106604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81697a0f2a55f882f55ccac9401c3dd272607c42f460a8549f30a1ebb26e0c8`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6400e9488fa4d970dad72e844be39d2d75b7d2c31501c6d6b23d6a1bc524f7c1`  
		Last Modified: Mon, 24 May 2021 18:22:57 GMT  
		Size: 11.9 MB (11930419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5b5da05058a691610222ba26189e6f6c28b9ede612bec34b4ed5dea3691b92`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197bdfed68cccee24a939b4dd69fea66e2dc7827a4017bf444bdd2c90e959f6a`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474f7ecfe9858ec31d5203cc051d4063e0ad4acd2af33e4568f49d9e4b75e41b`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e026dffad92f6dace75c209e6f261b00cf847128dd907ffa4ac9f944e9ae054e`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c534d757d31dc1e6130a58f06b95d25d61f32e015e329cd2227a1bed890280`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31071464c175eef4ea5843313a962e550e530c0a4c12fd997c6ace04fed5d0e0`  
		Last Modified: Mon, 24 May 2021 18:22:51 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3035f85e6f0ef498e48d22a196b3dca2d1feff90554b2f1fbbd3062a92ffccd2`  
		Last Modified: Mon, 24 May 2021 18:22:51 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caffd6e1f83b89b2831eab80faf22c370ad73519467e80354cb56ee96eed7fe3`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285714c5a6fb40773b7e624641f8e036180ab3424ee89b84f3fbbd79d7108eec`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872e853821b7661d1e753ef89a95c2525171915b5dec31950f7b05f4492eb40c`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7958b6b43cba2b3e1a20dc772e84541237901c32ec6dba998eb300627b2e343`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8089fe8b99a3884b64fb515b432248ed2433347b16efe53190c08624ec8bcf8f`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e25c6bfe294987f6c4c3a677078ea11dd90d54892fff638abed3d5a8602360c`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1757220b38637dda7da307ac64a4eefb9226cd9e13d613ab9bb839997c0c2aa8`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a748ef821631911b8abd470af8b29305283a82e1b5da1d2459257d8308576a2`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa22970d4f705eac4e8ea2ac4a7f3e89cfc01035b6ff0bf8998c146fe4d9a96`  
		Last Modified: Mon, 24 May 2021 18:22:47 GMT  
		Size: 317.9 KB (317938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2477d94c5c1388771379c903fc8931c2531d21a7ccbef4b3b7e2d6461fb19fdd`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:9d786a7a09f9a8edcfdc2a75b463592913275d75986f55ca9d67f3ba0b848c67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `caddy:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:d530e436d6d892bc2662481a943d230921dd8d5b2a26de0d99c32abb59ce1973
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5819027610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:189fbf35362e472481d308f9fbecfeda8962471fccd521c1cdd2165bfff22c08`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:58:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 24 May 2021 18:16:16 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:17:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 24 May 2021 18:18:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 24 May 2021 18:18:02 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 24 May 2021 18:18:03 GMT
VOLUME [c:/config]
# Mon, 24 May 2021 18:18:04 GMT
VOLUME [c:/data]
# Mon, 24 May 2021 18:18:05 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:18:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:18:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:18:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:18:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:18:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:18:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:18:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:18:14 GMT
EXPOSE 80
# Mon, 24 May 2021 18:18:15 GMT
EXPOSE 443
# Mon, 24 May 2021 18:18:16 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:19:09 GMT
RUN caddy version
# Mon, 24 May 2021 18:19:10 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26858854e9a4d33437022a0cbf481973fa7709cc09d3402af046620cbbe5c0`  
		Last Modified: Wed, 12 May 2021 20:07:13 GMT  
		Size: 5.7 MB (5714091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba52519d045fbbd4b405dea0a101b9ede50767ce1b8b92f0b0a9708dc3a3492`  
		Last Modified: Mon, 24 May 2021 18:23:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073bc62336c22adb06e7c530733538c823c0e30b591f536ca853dd86ff16e632`  
		Last Modified: Mon, 24 May 2021 18:23:26 GMT  
		Size: 17.2 MB (17244195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319fcbb76d6ed2f5920ae3cf875486281ed4d5edc53c630c8c6ad581efc92594`  
		Last Modified: Mon, 24 May 2021 18:23:22 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d372740cbc98799ef99cd14fe521f6c8bc0202f7e6eb418f8db3e6cae94caf60`  
		Last Modified: Mon, 24 May 2021 18:23:21 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c1957ce089769a88ac826364c0cb191ae826407602ccf505c76ee34afa10c8`  
		Last Modified: Mon, 24 May 2021 18:23:20 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e022ba7739dc4609e4838ae24c6930ccdc82d0721cc978c71a7e036122adf228`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5716dc07e962e5602a2cecf1a5b63c75352ad0e48b06b30070ad5cd4a31993`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc94100cd9e1fb3620069275788a9e1b912502dcd7966b4d624ecba5f88690`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7790197c85ec7196ed9b956d8f481e8f382479a3b8e20db4d8e564f14331eb42`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60939c5f58f38df81a8563072d42fcd4fb79292dbf5ce4d31a46f840e777fb88`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d5876f07c48377c92817efa2b077cfe4c05822b08a1916d350b5e8ee682b50`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2933951452131d66acb34683269ade093ebb9faf312436b0a601168cb6e2fe68`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ad33c6332b1b2a8e806339fd2978dd9a8919fc98d48fc0ae6a58ad07870cec`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b44c787b930665927a13e544b5d3d7243caae27d4d9a6f9502f985e8483af61`  
		Last Modified: Mon, 24 May 2021 18:23:16 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e86dd1b42134f467b929f29aa052bdca8a20ccbb6ff1332575ef7843b962243`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3288b716f0b64cb14a9da486b126557c121b9a71476d5aea6a1be399a82bb14b`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83f9226706657b746cb502303856ebeca1a6cda85b1aea65196506c3e3faa4a`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fc7b2fb07d7a4265b695bf44d6d3378e7f0202a6c8fd0d359f766886070802`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 266.6 KB (266650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cde5c4ac8767e62fceac7aed63a74d7935277b8087425319abfe8e22f7bb37`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0`

```console
$ docker pull caddy@sha256:30a03722cf8a666b0534d7ac0e6464a44a165ea0b90ca95c35d744ac27b5d823
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

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

### `caddy:2.3.0` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:1f2f4375fe18c3922246641f9d8147957d674518fbbae4de0ca7262ca9a10c8e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2491953956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a81170266cc4cd4654c2a718b9ce95850c86f3d5007f3df0355cfd20ce5c88a8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:47:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:47:22 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 12 May 2021 19:47:50 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 19:47:52 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 19:47:53 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 19:47:54 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 19:47:54 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 19:47:55 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 12 May 2021 19:47:56 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 19:47:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 19:47:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 19:47:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 19:48:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 19:48:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 19:48:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 19:48:03 GMT
EXPOSE 80
# Wed, 12 May 2021 19:48:04 GMT
EXPOSE 443
# Wed, 12 May 2021 19:48:05 GMT
EXPOSE 2019
# Wed, 12 May 2021 19:48:24 GMT
RUN caddy version
# Wed, 12 May 2021 19:48:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22448182e969b54b9124ea5c2c3274bb690098b2fbc33eb12e5ed9ed7050d5bd`  
		Last Modified: Wed, 12 May 2021 20:05:02 GMT  
		Size: 5.1 MB (5106938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ef42ea7d797590afce1f67735ff57366d32b8e5a47fddd4eeba554353e1632`  
		Last Modified: Wed, 12 May 2021 20:04:59 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6d6a870c119297feb4b26eb7ed0991f682ae7ed54eb6d078b3738540e4b07c`  
		Last Modified: Wed, 12 May 2021 20:05:03 GMT  
		Size: 12.0 MB (12036673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0306e9829e5a6249855c31f445349126971b770e640113282b8a295fc0903798`  
		Last Modified: Wed, 12 May 2021 20:04:59 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c0da71a5fdf88e436b2eda07b3e01abd5e4980c4ff0df44058fcf7404d9d89`  
		Last Modified: Wed, 12 May 2021 20:04:59 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3abf7f593c565e5f425389811e406e60effd5aa026c589da05dda4e12a0e09`  
		Last Modified: Wed, 12 May 2021 20:04:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af7361c77f2298946131dac665a1741fea61580de64d3720faf6bcad8bf6062`  
		Last Modified: Wed, 12 May 2021 20:04:57 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22941e833dbf1fbe60149b43d62e750e53f10b96fc0d3404f9f3557531f94c54`  
		Last Modified: Wed, 12 May 2021 20:04:56 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08de1004b1830150f2bfcf83cac0c69016d14353a11c98fc462bf6e09409fcc6`  
		Last Modified: Wed, 12 May 2021 20:04:56 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86dd223159bafe127872fa6c79d7122fd5ef92ff99047ea461264d3bbdaffa3e`  
		Last Modified: Wed, 12 May 2021 20:04:56 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616751d4c2002ece2f5f071e81f5ffb98eb13c9ccef5fc8d320763b236bd79fe`  
		Last Modified: Wed, 12 May 2021 20:04:54 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e3d1e8fb9e4cc01652992548231f0624c9f312dc460e9c9bc6489b3ccaef13`  
		Last Modified: Wed, 12 May 2021 20:04:54 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7cd9649d7f83a1af93e815ee0e082bc07619910c657f910c373b76801a94afc`  
		Last Modified: Wed, 12 May 2021 20:04:53 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2997645ef7e4b10b2f16f6574088dfed37540a6c331bdd818d19636cd0c288d0`  
		Last Modified: Wed, 12 May 2021 20:04:53 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5329c49b05ecb4af421cd90b549f25d9d332ebd31e9c8c5caabe53e99cd511`  
		Last Modified: Wed, 12 May 2021 20:04:53 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab96feded9e3523c6bba4ca432a0ee98d1ed3058c81cc085615eb5676fa53a6e`  
		Last Modified: Wed, 12 May 2021 20:04:51 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a1045f4017ab5a334bac615e62ee6d6849abba6b196cfdd731760f3fde0c23`  
		Last Modified: Wed, 12 May 2021 20:04:50 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fee82082cb8928038f23a28f9132b659ac38d1bc6bb3afbc4e09dae54e86695`  
		Last Modified: Wed, 12 May 2021 20:04:50 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d0784bf95bc812b62f0220b913b05dd208b220f570884d7e34d7fcc0d37c4f`  
		Last Modified: Wed, 12 May 2021 20:04:51 GMT  
		Size: 295.7 KB (295736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43afb0cbdc146ba20b4aac840c48f5c77d4f58a4fdd0b6cfa0a45217f1bde75`  
		Last Modified: Wed, 12 May 2021 20:04:51 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:9383b916fac221ad685d5162d3f13705bc54b48a8a4cc108c30bec9ebefccbb8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5819185733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be5e85cd4236dadd2e2260e08847f06c7cf8a6bf114d46e5dc8d36a0624eb942`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:49:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:49:55 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 12 May 2021 19:51:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 19:51:31 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 19:51:32 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 19:51:33 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 19:51:35 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 19:51:36 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 12 May 2021 19:51:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 19:51:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 19:51:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 19:51:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 19:51:41 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 19:51:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 19:51:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 19:51:45 GMT
EXPOSE 80
# Wed, 12 May 2021 19:51:46 GMT
EXPOSE 443
# Wed, 12 May 2021 19:51:47 GMT
EXPOSE 2019
# Wed, 12 May 2021 19:52:54 GMT
RUN caddy version
# Wed, 12 May 2021 19:52:55 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb86fc7ebd4b8e0170404d2efc422e3a003119cf835edf347cdba2cb5dcb637e`  
		Last Modified: Wed, 12 May 2021 20:05:24 GMT  
		Size: 5.7 MB (5715678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be0a1b98881464003a76f9c3d552af6aa32676eded40337a2cb740220b8e8b5`  
		Last Modified: Wed, 12 May 2021 20:05:22 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2f0820331f200b69ffc4376c6d900a0eff190f419b5000a08b1b2d643534b6`  
		Last Modified: Wed, 12 May 2021 20:05:26 GMT  
		Size: 17.4 MB (17386489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3493d093c4b99f139a5427c673f7efaa2b5165503ecad87cb8ce5552e11ebf`  
		Last Modified: Wed, 12 May 2021 20:05:20 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fe562a331e468e75447f36e3f25418222bd38dd64ed86e1ed5d135326ca297`  
		Last Modified: Wed, 12 May 2021 20:05:20 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e380b48e44a8409c9d227325699b754573b99734b04ccd9b0afd4d221de4463c`  
		Last Modified: Wed, 12 May 2021 20:05:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4838e63e8d0097db4c9f0b40fb85cb4ca6ab86d367ba5e8e03926567a06fbf6c`  
		Last Modified: Wed, 12 May 2021 20:05:19 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8502433c7f52aac3dd7bda187871008ccc524909273d3ecc731fc21ae788d58`  
		Last Modified: Wed, 12 May 2021 20:05:17 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436d7436a478513cfdd80519a071fb37badf42397c34e5bed6ecb807a0f5f544`  
		Last Modified: Wed, 12 May 2021 20:05:17 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0957a349d9bda1d5d624590e5f8bb02b83605c041e63f495e421a185e7c9cb0b`  
		Last Modified: Wed, 12 May 2021 20:05:17 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5368704288b662f01ec22e1518b4cbfbaebad0f096f0f78b523fbebf1bf8d315`  
		Last Modified: Wed, 12 May 2021 20:05:17 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a57eac0f8fb22c77ed1133dce3b45ff210e67457237188fdd4244a614bcd9b`  
		Last Modified: Wed, 12 May 2021 20:05:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06eb9e82c5d11b8714bdbcc16be6fef89cf5a8e80fa5aec957bb00ea13eb36c3`  
		Last Modified: Wed, 12 May 2021 20:05:14 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b02b72008aedc5b17796c0bdc40233ae777ec8a19530b70983fa5b6f001914c`  
		Last Modified: Wed, 12 May 2021 20:05:14 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e520b47523d14eb979eb9c33ee5803753ddf7192e0f9cc4737e596091333dc45`  
		Last Modified: Wed, 12 May 2021 20:05:14 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cf16fae2c4e03aee1b9269abf928e7299c0912e8d6ce3c646b2398fd0419cf`  
		Last Modified: Wed, 12 May 2021 20:05:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352e7ea39b707bbf4a83cc0c0be3ddf79f71be49669db9f93f17915d9e1235b6`  
		Last Modified: Wed, 12 May 2021 20:05:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da84cbe314c1c929b4ce1e6c633c4e78b61d042c8ed8bcf96da263c53a1d12d3`  
		Last Modified: Wed, 12 May 2021 20:05:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3810c939f9540e16a267e3d1f6a3e3e4162c5b6190d5087acc7eebdf65a014`  
		Last Modified: Wed, 12 May 2021 20:05:12 GMT  
		Size: 280.7 KB (280738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e6e97602e558f4a75b0da2af7de0ccca80cd60b809b803af3f16096fb85332`  
		Last Modified: Wed, 12 May 2021 20:05:16 GMT  
		Size: 1.4 KB (1430 bytes)  
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
$ docker pull caddy@sha256:a696cffd940d6d74a3d9d64064218dc60b80a5920425bb410c4de6f4c3172e4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

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

### `caddy:2.3.0-builder` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:4756dc505e6ec395b18823c70d95790413e5801b94f77ae5d46e1a10bdc4ede6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2640900179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfc8b75896ec44e95f24e5533bddd7260614e6ff52e55b365c61b784f74406fd`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:24:28 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:24:29 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:24:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:24:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:25:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:25:36 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:26:02 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Jun 2021 01:29:32 GMT
ENV GOLANG_VERSION=1.15.13
# Fri, 04 Jun 2021 01:32:20 GMT
RUN $url = 'https://dl.google.com/go/go1.15.13.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'd1cf76a11bbd5158715a3e3b6b7f0c623f5472f7c0e654c858913b74b09e7e81'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Jun 2021 01:32:22 GMT
WORKDIR C:\gopath
# Fri, 04 Jun 2021 02:08:22 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Jun 2021 02:08:23 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 02:08:24 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 04 Jun 2021 02:08:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 02:08:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Jun 2021 02:08:53 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2a5ccd12170e9f926c3e069a2fa2ed38b5dd5596869ed982bccc50ef80cf1f`  
		Last Modified: Wed, 12 May 2021 12:52:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd5b5fa12081ad53ae688dc454e550dd50bd414c949724180719b0326632c4a`  
		Last Modified: Wed, 12 May 2021 12:52:08 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599ef939f9e7c26d4bc0f8f75820116f6977a64212b86260bc225ae2d850cc31`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bddce42b6f4351510fcb255839a7c55d95546186dce8509782abe959d27d9f0`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2407bf3b614294860b53b94e661f5c57f7dd985934aed5727442f9353bf8c617`  
		Last Modified: Wed, 12 May 2021 12:52:14 GMT  
		Size: 30.2 MB (30189126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b01ea9b4210c3201c1462d7ee78b276d7d5ffac3dca02c9c57a0c77c5b87a2`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27be8fd19f331f65055bbf31138aa28628be7534753008620ec14fc1803ebdf2`  
		Last Modified: Wed, 12 May 2021 12:52:05 GMT  
		Size: 313.1 KB (313094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19fdb722d794c570c29393398e01aeba76fc24817dae07b7a02ec0532f25170`  
		Last Modified: Fri, 04 Jun 2021 01:47:10 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbb0afccd74dfc2842317764c8200851d61bc34aca48082e9dc54c02d4a7244`  
		Last Modified: Fri, 04 Jun 2021 01:47:42 GMT  
		Size: 134.2 MB (134167554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a88ed57355e26477db3081fa43e83611fbd18da9e1e56224bfbdeb93a45041`  
		Last Modified: Fri, 04 Jun 2021 01:47:10 GMT  
		Size: 1.6 KB (1588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb8146542aea302c06eb7297f1c6de5b43b097ea8a59438c8ca3a7f0da07282`  
		Last Modified: Fri, 04 Jun 2021 02:14:13 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd1403bd3bedd82145b6e8b502e3bd400330e681a7602c329a5c17673e819ba`  
		Last Modified: Fri, 04 Jun 2021 02:14:10 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e952b0f6eda4f9c804f4982d579e31a9531ac44a7ade922e57579c14a6cd040`  
		Last Modified: Fri, 04 Jun 2021 02:14:10 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37bacdddc782c6fc6c50779c5cd330295a0750143eca0ab3857dc470983da83b`  
		Last Modified: Fri, 04 Jun 2021 02:14:10 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3094290dc8abfcb3f8f48d513fb3d83edc5536178d71c6b3ea1563b5ac3fd7`  
		Last Modified: Fri, 04 Jun 2021 02:14:11 GMT  
		Size: 1.7 MB (1722678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184f437a43a0dc84def60b5ed276d4fab0dac6efcd6d9faaa38c6b34010c914c`  
		Last Modified: Fri, 04 Jun 2021 02:14:10 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:aebe3d665f0cc70bd3b395d8dff30216bfcb4d4341330d87769083deb560a704
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5983273762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e87c9e2029726cb42dc4257966eb6d744b8eae6895faa54773f0f892619fb2c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:29:13 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:29:14 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:29:15 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:29:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:31:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:31:45 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:33:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Jun 2021 01:32:30 GMT
ENV GOLANG_VERSION=1.15.13
# Fri, 04 Jun 2021 01:36:19 GMT
RUN $url = 'https://dl.google.com/go/go1.15.13.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'd1cf76a11bbd5158715a3e3b6b7f0c623f5472f7c0e654c858913b74b09e7e81'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Jun 2021 01:36:21 GMT
WORKDIR C:\gopath
# Fri, 04 Jun 2021 02:08:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Jun 2021 02:09:01 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 02:09:02 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 04 Jun 2021 02:09:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 02:10:28 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Jun 2021 02:10:29 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10abf429e12c7b3b7d2b0a791d7cdb47866461a7b63df4ddd4f63acc91e26231`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79955f676504cbf77ec284d8e857d18d17b93c5b8e6438b4062dd80f8632c9d6`  
		Last Modified: Wed, 12 May 2021 12:55:12 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24af485ecab19f81a0c65c0eaec6f6fda8749ca50eb53101abcfc5c079f9b1c2`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b782f6bcd162ee81518d73c6c4fe5c5b731ab38b595c16a55ac185db84b2c9b`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1327fc384f9fff64d41446adcb3bdf585307370ef0024a31a5269bae6f30067d`  
		Last Modified: Wed, 12 May 2021 12:55:18 GMT  
		Size: 30.8 MB (30797956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c50f4b0b5994b4154be9fea2ab6c6a0e4c402c44d44795a5ce82ab6f8de4bc`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e458669a58e08411a0641a721ef1daf4af2a568c4dd61e9a3710b07f73b6ec`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 5.7 MB (5661591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a21b95e6ca5428dc178b7ad6b4b500c5b0cb661fb69e865c3abe55d78e16db`  
		Last Modified: Fri, 04 Jun 2021 01:47:53 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb72c0f0909032734769975f4f4fe71f5c129640561e668a46415b0f9c75964b`  
		Last Modified: Fri, 04 Jun 2021 01:50:30 GMT  
		Size: 144.0 MB (143988741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72696c2439a938751221fece807cdb307dc14cc9487dc025747f5e2a6b3b448c`  
		Last Modified: Fri, 04 Jun 2021 01:47:53 GMT  
		Size: 1.6 KB (1568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f16d852eacdde87a07532483343b3e23b3aeb247c7c71ec15d850c1aa9015a`  
		Last Modified: Fri, 04 Jun 2021 02:14:24 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7401ba97a3be5e3d392cbece2ee8bddf2b5fc61fa1015133ed747f289f6a54b3`  
		Last Modified: Fri, 04 Jun 2021 02:14:21 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1157a4daad63fb745f2a18882d5cec5139bcc5ccb9a835da512e5937c94fee`  
		Last Modified: Fri, 04 Jun 2021 02:14:21 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:279b9f752ec3b6b685ae75f25e23060ef8f107f9e3bc78191d27c13941399b3a`  
		Last Modified: Fri, 04 Jun 2021 02:14:21 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476767d1d9cbbe82e327049bd4eb6185d6d6c164e6079162c1a328a939f2b33a`  
		Last Modified: Fri, 04 Jun 2021 02:14:24 GMT  
		Size: 7.0 MB (7029561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9811e64e653dd1ad2157706b75ecdd7fc990c4512c847b26fe173cb152ad6ea3`  
		Last Modified: Fri, 04 Jun 2021 02:14:21 GMT  
		Size: 1.4 KB (1368 bytes)  
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
$ docker pull caddy@sha256:23adc745cd747b4787201f0e198e9cf06eee35db2900b40378a171bfda0b141a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `caddy:2.3.0-builder-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:4756dc505e6ec395b18823c70d95790413e5801b94f77ae5d46e1a10bdc4ede6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2640900179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfc8b75896ec44e95f24e5533bddd7260614e6ff52e55b365c61b784f74406fd`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:24:28 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:24:29 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:24:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:24:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:25:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:25:36 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:26:02 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Jun 2021 01:29:32 GMT
ENV GOLANG_VERSION=1.15.13
# Fri, 04 Jun 2021 01:32:20 GMT
RUN $url = 'https://dl.google.com/go/go1.15.13.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'd1cf76a11bbd5158715a3e3b6b7f0c623f5472f7c0e654c858913b74b09e7e81'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Jun 2021 01:32:22 GMT
WORKDIR C:\gopath
# Fri, 04 Jun 2021 02:08:22 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Jun 2021 02:08:23 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 02:08:24 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 04 Jun 2021 02:08:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 02:08:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Jun 2021 02:08:53 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2a5ccd12170e9f926c3e069a2fa2ed38b5dd5596869ed982bccc50ef80cf1f`  
		Last Modified: Wed, 12 May 2021 12:52:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd5b5fa12081ad53ae688dc454e550dd50bd414c949724180719b0326632c4a`  
		Last Modified: Wed, 12 May 2021 12:52:08 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599ef939f9e7c26d4bc0f8f75820116f6977a64212b86260bc225ae2d850cc31`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bddce42b6f4351510fcb255839a7c55d95546186dce8509782abe959d27d9f0`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2407bf3b614294860b53b94e661f5c57f7dd985934aed5727442f9353bf8c617`  
		Last Modified: Wed, 12 May 2021 12:52:14 GMT  
		Size: 30.2 MB (30189126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b01ea9b4210c3201c1462d7ee78b276d7d5ffac3dca02c9c57a0c77c5b87a2`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27be8fd19f331f65055bbf31138aa28628be7534753008620ec14fc1803ebdf2`  
		Last Modified: Wed, 12 May 2021 12:52:05 GMT  
		Size: 313.1 KB (313094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19fdb722d794c570c29393398e01aeba76fc24817dae07b7a02ec0532f25170`  
		Last Modified: Fri, 04 Jun 2021 01:47:10 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbb0afccd74dfc2842317764c8200851d61bc34aca48082e9dc54c02d4a7244`  
		Last Modified: Fri, 04 Jun 2021 01:47:42 GMT  
		Size: 134.2 MB (134167554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a88ed57355e26477db3081fa43e83611fbd18da9e1e56224bfbdeb93a45041`  
		Last Modified: Fri, 04 Jun 2021 01:47:10 GMT  
		Size: 1.6 KB (1588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb8146542aea302c06eb7297f1c6de5b43b097ea8a59438c8ca3a7f0da07282`  
		Last Modified: Fri, 04 Jun 2021 02:14:13 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd1403bd3bedd82145b6e8b502e3bd400330e681a7602c329a5c17673e819ba`  
		Last Modified: Fri, 04 Jun 2021 02:14:10 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e952b0f6eda4f9c804f4982d579e31a9531ac44a7ade922e57579c14a6cd040`  
		Last Modified: Fri, 04 Jun 2021 02:14:10 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37bacdddc782c6fc6c50779c5cd330295a0750143eca0ab3857dc470983da83b`  
		Last Modified: Fri, 04 Jun 2021 02:14:10 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3094290dc8abfcb3f8f48d513fb3d83edc5536178d71c6b3ea1563b5ac3fd7`  
		Last Modified: Fri, 04 Jun 2021 02:14:11 GMT  
		Size: 1.7 MB (1722678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184f437a43a0dc84def60b5ed276d4fab0dac6efcd6d9faaa38c6b34010c914c`  
		Last Modified: Fri, 04 Jun 2021 02:14:10 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:5932f8a859fff326442255a5172a4481285a8a4cd03700acfebaa35ea1b35427
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `caddy:2.3.0-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:aebe3d665f0cc70bd3b395d8dff30216bfcb4d4341330d87769083deb560a704
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5983273762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e87c9e2029726cb42dc4257966eb6d744b8eae6895faa54773f0f892619fb2c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:29:13 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:29:14 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:29:15 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:29:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:31:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:31:45 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:33:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Jun 2021 01:32:30 GMT
ENV GOLANG_VERSION=1.15.13
# Fri, 04 Jun 2021 01:36:19 GMT
RUN $url = 'https://dl.google.com/go/go1.15.13.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'd1cf76a11bbd5158715a3e3b6b7f0c623f5472f7c0e654c858913b74b09e7e81'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Jun 2021 01:36:21 GMT
WORKDIR C:\gopath
# Fri, 04 Jun 2021 02:08:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Jun 2021 02:09:01 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 02:09:02 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 04 Jun 2021 02:09:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 02:10:28 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Jun 2021 02:10:29 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10abf429e12c7b3b7d2b0a791d7cdb47866461a7b63df4ddd4f63acc91e26231`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79955f676504cbf77ec284d8e857d18d17b93c5b8e6438b4062dd80f8632c9d6`  
		Last Modified: Wed, 12 May 2021 12:55:12 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24af485ecab19f81a0c65c0eaec6f6fda8749ca50eb53101abcfc5c079f9b1c2`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b782f6bcd162ee81518d73c6c4fe5c5b731ab38b595c16a55ac185db84b2c9b`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1327fc384f9fff64d41446adcb3bdf585307370ef0024a31a5269bae6f30067d`  
		Last Modified: Wed, 12 May 2021 12:55:18 GMT  
		Size: 30.8 MB (30797956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c50f4b0b5994b4154be9fea2ab6c6a0e4c402c44d44795a5ce82ab6f8de4bc`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e458669a58e08411a0641a721ef1daf4af2a568c4dd61e9a3710b07f73b6ec`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 5.7 MB (5661591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a21b95e6ca5428dc178b7ad6b4b500c5b0cb661fb69e865c3abe55d78e16db`  
		Last Modified: Fri, 04 Jun 2021 01:47:53 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb72c0f0909032734769975f4f4fe71f5c129640561e668a46415b0f9c75964b`  
		Last Modified: Fri, 04 Jun 2021 01:50:30 GMT  
		Size: 144.0 MB (143988741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72696c2439a938751221fece807cdb307dc14cc9487dc025747f5e2a6b3b448c`  
		Last Modified: Fri, 04 Jun 2021 01:47:53 GMT  
		Size: 1.6 KB (1568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f16d852eacdde87a07532483343b3e23b3aeb247c7c71ec15d850c1aa9015a`  
		Last Modified: Fri, 04 Jun 2021 02:14:24 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7401ba97a3be5e3d392cbece2ee8bddf2b5fc61fa1015133ed747f289f6a54b3`  
		Last Modified: Fri, 04 Jun 2021 02:14:21 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1157a4daad63fb745f2a18882d5cec5139bcc5ccb9a835da512e5937c94fee`  
		Last Modified: Fri, 04 Jun 2021 02:14:21 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:279b9f752ec3b6b685ae75f25e23060ef8f107f9e3bc78191d27c13941399b3a`  
		Last Modified: Fri, 04 Jun 2021 02:14:21 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476767d1d9cbbe82e327049bd4eb6185d6d6c164e6079162c1a328a939f2b33a`  
		Last Modified: Fri, 04 Jun 2021 02:14:24 GMT  
		Size: 7.0 MB (7029561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9811e64e653dd1ad2157706b75ecdd7fc990c4512c847b26fe173cb152ad6ea3`  
		Last Modified: Fri, 04 Jun 2021 02:14:21 GMT  
		Size: 1.4 KB (1368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-windowsservercore`

```console
$ docker pull caddy@sha256:49732c7d6a8a6d2d35a490d19e1b75f52b243ffc4579308e82d9b99b8d34d17e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `caddy:2.3.0-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:1f2f4375fe18c3922246641f9d8147957d674518fbbae4de0ca7262ca9a10c8e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2491953956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a81170266cc4cd4654c2a718b9ce95850c86f3d5007f3df0355cfd20ce5c88a8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:47:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:47:22 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 12 May 2021 19:47:50 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 19:47:52 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 19:47:53 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 19:47:54 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 19:47:54 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 19:47:55 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 12 May 2021 19:47:56 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 19:47:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 19:47:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 19:47:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 19:48:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 19:48:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 19:48:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 19:48:03 GMT
EXPOSE 80
# Wed, 12 May 2021 19:48:04 GMT
EXPOSE 443
# Wed, 12 May 2021 19:48:05 GMT
EXPOSE 2019
# Wed, 12 May 2021 19:48:24 GMT
RUN caddy version
# Wed, 12 May 2021 19:48:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22448182e969b54b9124ea5c2c3274bb690098b2fbc33eb12e5ed9ed7050d5bd`  
		Last Modified: Wed, 12 May 2021 20:05:02 GMT  
		Size: 5.1 MB (5106938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ef42ea7d797590afce1f67735ff57366d32b8e5a47fddd4eeba554353e1632`  
		Last Modified: Wed, 12 May 2021 20:04:59 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6d6a870c119297feb4b26eb7ed0991f682ae7ed54eb6d078b3738540e4b07c`  
		Last Modified: Wed, 12 May 2021 20:05:03 GMT  
		Size: 12.0 MB (12036673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0306e9829e5a6249855c31f445349126971b770e640113282b8a295fc0903798`  
		Last Modified: Wed, 12 May 2021 20:04:59 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c0da71a5fdf88e436b2eda07b3e01abd5e4980c4ff0df44058fcf7404d9d89`  
		Last Modified: Wed, 12 May 2021 20:04:59 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3abf7f593c565e5f425389811e406e60effd5aa026c589da05dda4e12a0e09`  
		Last Modified: Wed, 12 May 2021 20:04:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af7361c77f2298946131dac665a1741fea61580de64d3720faf6bcad8bf6062`  
		Last Modified: Wed, 12 May 2021 20:04:57 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22941e833dbf1fbe60149b43d62e750e53f10b96fc0d3404f9f3557531f94c54`  
		Last Modified: Wed, 12 May 2021 20:04:56 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08de1004b1830150f2bfcf83cac0c69016d14353a11c98fc462bf6e09409fcc6`  
		Last Modified: Wed, 12 May 2021 20:04:56 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86dd223159bafe127872fa6c79d7122fd5ef92ff99047ea461264d3bbdaffa3e`  
		Last Modified: Wed, 12 May 2021 20:04:56 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616751d4c2002ece2f5f071e81f5ffb98eb13c9ccef5fc8d320763b236bd79fe`  
		Last Modified: Wed, 12 May 2021 20:04:54 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e3d1e8fb9e4cc01652992548231f0624c9f312dc460e9c9bc6489b3ccaef13`  
		Last Modified: Wed, 12 May 2021 20:04:54 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7cd9649d7f83a1af93e815ee0e082bc07619910c657f910c373b76801a94afc`  
		Last Modified: Wed, 12 May 2021 20:04:53 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2997645ef7e4b10b2f16f6574088dfed37540a6c331bdd818d19636cd0c288d0`  
		Last Modified: Wed, 12 May 2021 20:04:53 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5329c49b05ecb4af421cd90b549f25d9d332ebd31e9c8c5caabe53e99cd511`  
		Last Modified: Wed, 12 May 2021 20:04:53 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab96feded9e3523c6bba4ca432a0ee98d1ed3058c81cc085615eb5676fa53a6e`  
		Last Modified: Wed, 12 May 2021 20:04:51 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a1045f4017ab5a334bac615e62ee6d6849abba6b196cfdd731760f3fde0c23`  
		Last Modified: Wed, 12 May 2021 20:04:50 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fee82082cb8928038f23a28f9132b659ac38d1bc6bb3afbc4e09dae54e86695`  
		Last Modified: Wed, 12 May 2021 20:04:50 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d0784bf95bc812b62f0220b913b05dd208b220f570884d7e34d7fcc0d37c4f`  
		Last Modified: Wed, 12 May 2021 20:04:51 GMT  
		Size: 295.7 KB (295736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43afb0cbdc146ba20b4aac840c48f5c77d4f58a4fdd0b6cfa0a45217f1bde75`  
		Last Modified: Wed, 12 May 2021 20:04:51 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:9383b916fac221ad685d5162d3f13705bc54b48a8a4cc108c30bec9ebefccbb8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5819185733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be5e85cd4236dadd2e2260e08847f06c7cf8a6bf114d46e5dc8d36a0624eb942`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:49:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:49:55 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 12 May 2021 19:51:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 19:51:31 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 19:51:32 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 19:51:33 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 19:51:35 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 19:51:36 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 12 May 2021 19:51:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 19:51:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 19:51:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 19:51:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 19:51:41 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 19:51:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 19:51:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 19:51:45 GMT
EXPOSE 80
# Wed, 12 May 2021 19:51:46 GMT
EXPOSE 443
# Wed, 12 May 2021 19:51:47 GMT
EXPOSE 2019
# Wed, 12 May 2021 19:52:54 GMT
RUN caddy version
# Wed, 12 May 2021 19:52:55 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb86fc7ebd4b8e0170404d2efc422e3a003119cf835edf347cdba2cb5dcb637e`  
		Last Modified: Wed, 12 May 2021 20:05:24 GMT  
		Size: 5.7 MB (5715678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be0a1b98881464003a76f9c3d552af6aa32676eded40337a2cb740220b8e8b5`  
		Last Modified: Wed, 12 May 2021 20:05:22 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2f0820331f200b69ffc4376c6d900a0eff190f419b5000a08b1b2d643534b6`  
		Last Modified: Wed, 12 May 2021 20:05:26 GMT  
		Size: 17.4 MB (17386489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3493d093c4b99f139a5427c673f7efaa2b5165503ecad87cb8ce5552e11ebf`  
		Last Modified: Wed, 12 May 2021 20:05:20 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fe562a331e468e75447f36e3f25418222bd38dd64ed86e1ed5d135326ca297`  
		Last Modified: Wed, 12 May 2021 20:05:20 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e380b48e44a8409c9d227325699b754573b99734b04ccd9b0afd4d221de4463c`  
		Last Modified: Wed, 12 May 2021 20:05:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4838e63e8d0097db4c9f0b40fb85cb4ca6ab86d367ba5e8e03926567a06fbf6c`  
		Last Modified: Wed, 12 May 2021 20:05:19 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8502433c7f52aac3dd7bda187871008ccc524909273d3ecc731fc21ae788d58`  
		Last Modified: Wed, 12 May 2021 20:05:17 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436d7436a478513cfdd80519a071fb37badf42397c34e5bed6ecb807a0f5f544`  
		Last Modified: Wed, 12 May 2021 20:05:17 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0957a349d9bda1d5d624590e5f8bb02b83605c041e63f495e421a185e7c9cb0b`  
		Last Modified: Wed, 12 May 2021 20:05:17 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5368704288b662f01ec22e1518b4cbfbaebad0f096f0f78b523fbebf1bf8d315`  
		Last Modified: Wed, 12 May 2021 20:05:17 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a57eac0f8fb22c77ed1133dce3b45ff210e67457237188fdd4244a614bcd9b`  
		Last Modified: Wed, 12 May 2021 20:05:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06eb9e82c5d11b8714bdbcc16be6fef89cf5a8e80fa5aec957bb00ea13eb36c3`  
		Last Modified: Wed, 12 May 2021 20:05:14 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b02b72008aedc5b17796c0bdc40233ae777ec8a19530b70983fa5b6f001914c`  
		Last Modified: Wed, 12 May 2021 20:05:14 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e520b47523d14eb979eb9c33ee5803753ddf7192e0f9cc4737e596091333dc45`  
		Last Modified: Wed, 12 May 2021 20:05:14 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cf16fae2c4e03aee1b9269abf928e7299c0912e8d6ce3c646b2398fd0419cf`  
		Last Modified: Wed, 12 May 2021 20:05:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352e7ea39b707bbf4a83cc0c0be3ddf79f71be49669db9f93f17915d9e1235b6`  
		Last Modified: Wed, 12 May 2021 20:05:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da84cbe314c1c929b4ce1e6c633c4e78b61d042c8ed8bcf96da263c53a1d12d3`  
		Last Modified: Wed, 12 May 2021 20:05:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3810c939f9540e16a267e3d1f6a3e3e4162c5b6190d5087acc7eebdf65a014`  
		Last Modified: Wed, 12 May 2021 20:05:12 GMT  
		Size: 280.7 KB (280738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e6e97602e558f4a75b0da2af7de0ccca80cd60b809b803af3f16096fb85332`  
		Last Modified: Wed, 12 May 2021 20:05:16 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-windowsservercore-1809`

```console
$ docker pull caddy@sha256:c7bcc9f9c51fc07386f4fe2a7b3dd9a5b8e1f0a5dd6f9422f80f67ed8fab2a54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `caddy:2.3.0-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:1f2f4375fe18c3922246641f9d8147957d674518fbbae4de0ca7262ca9a10c8e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2491953956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a81170266cc4cd4654c2a718b9ce95850c86f3d5007f3df0355cfd20ce5c88a8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:47:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:47:22 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 12 May 2021 19:47:50 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 19:47:52 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 19:47:53 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 19:47:54 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 19:47:54 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 19:47:55 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 12 May 2021 19:47:56 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 19:47:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 19:47:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 19:47:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 19:48:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 19:48:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 19:48:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 19:48:03 GMT
EXPOSE 80
# Wed, 12 May 2021 19:48:04 GMT
EXPOSE 443
# Wed, 12 May 2021 19:48:05 GMT
EXPOSE 2019
# Wed, 12 May 2021 19:48:24 GMT
RUN caddy version
# Wed, 12 May 2021 19:48:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22448182e969b54b9124ea5c2c3274bb690098b2fbc33eb12e5ed9ed7050d5bd`  
		Last Modified: Wed, 12 May 2021 20:05:02 GMT  
		Size: 5.1 MB (5106938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ef42ea7d797590afce1f67735ff57366d32b8e5a47fddd4eeba554353e1632`  
		Last Modified: Wed, 12 May 2021 20:04:59 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6d6a870c119297feb4b26eb7ed0991f682ae7ed54eb6d078b3738540e4b07c`  
		Last Modified: Wed, 12 May 2021 20:05:03 GMT  
		Size: 12.0 MB (12036673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0306e9829e5a6249855c31f445349126971b770e640113282b8a295fc0903798`  
		Last Modified: Wed, 12 May 2021 20:04:59 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c0da71a5fdf88e436b2eda07b3e01abd5e4980c4ff0df44058fcf7404d9d89`  
		Last Modified: Wed, 12 May 2021 20:04:59 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3abf7f593c565e5f425389811e406e60effd5aa026c589da05dda4e12a0e09`  
		Last Modified: Wed, 12 May 2021 20:04:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af7361c77f2298946131dac665a1741fea61580de64d3720faf6bcad8bf6062`  
		Last Modified: Wed, 12 May 2021 20:04:57 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22941e833dbf1fbe60149b43d62e750e53f10b96fc0d3404f9f3557531f94c54`  
		Last Modified: Wed, 12 May 2021 20:04:56 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08de1004b1830150f2bfcf83cac0c69016d14353a11c98fc462bf6e09409fcc6`  
		Last Modified: Wed, 12 May 2021 20:04:56 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86dd223159bafe127872fa6c79d7122fd5ef92ff99047ea461264d3bbdaffa3e`  
		Last Modified: Wed, 12 May 2021 20:04:56 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616751d4c2002ece2f5f071e81f5ffb98eb13c9ccef5fc8d320763b236bd79fe`  
		Last Modified: Wed, 12 May 2021 20:04:54 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e3d1e8fb9e4cc01652992548231f0624c9f312dc460e9c9bc6489b3ccaef13`  
		Last Modified: Wed, 12 May 2021 20:04:54 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7cd9649d7f83a1af93e815ee0e082bc07619910c657f910c373b76801a94afc`  
		Last Modified: Wed, 12 May 2021 20:04:53 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2997645ef7e4b10b2f16f6574088dfed37540a6c331bdd818d19636cd0c288d0`  
		Last Modified: Wed, 12 May 2021 20:04:53 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5329c49b05ecb4af421cd90b549f25d9d332ebd31e9c8c5caabe53e99cd511`  
		Last Modified: Wed, 12 May 2021 20:04:53 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab96feded9e3523c6bba4ca432a0ee98d1ed3058c81cc085615eb5676fa53a6e`  
		Last Modified: Wed, 12 May 2021 20:04:51 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a1045f4017ab5a334bac615e62ee6d6849abba6b196cfdd731760f3fde0c23`  
		Last Modified: Wed, 12 May 2021 20:04:50 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fee82082cb8928038f23a28f9132b659ac38d1bc6bb3afbc4e09dae54e86695`  
		Last Modified: Wed, 12 May 2021 20:04:50 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d0784bf95bc812b62f0220b913b05dd208b220f570884d7e34d7fcc0d37c4f`  
		Last Modified: Wed, 12 May 2021 20:04:51 GMT  
		Size: 295.7 KB (295736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43afb0cbdc146ba20b4aac840c48f5c77d4f58a4fdd0b6cfa0a45217f1bde75`  
		Last Modified: Wed, 12 May 2021 20:04:51 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:f73f193e59a09b16da5bcff4472514d0a9cd0c045457cfd4c1869f1f3f1f9441
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `caddy:2.3.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:9383b916fac221ad685d5162d3f13705bc54b48a8a4cc108c30bec9ebefccbb8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5819185733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be5e85cd4236dadd2e2260e08847f06c7cf8a6bf114d46e5dc8d36a0624eb942`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:49:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:49:55 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 12 May 2021 19:51:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 19:51:31 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 19:51:32 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 19:51:33 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 19:51:35 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 19:51:36 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 12 May 2021 19:51:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 19:51:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 19:51:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 19:51:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 19:51:41 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 19:51:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 19:51:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 19:51:45 GMT
EXPOSE 80
# Wed, 12 May 2021 19:51:46 GMT
EXPOSE 443
# Wed, 12 May 2021 19:51:47 GMT
EXPOSE 2019
# Wed, 12 May 2021 19:52:54 GMT
RUN caddy version
# Wed, 12 May 2021 19:52:55 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb86fc7ebd4b8e0170404d2efc422e3a003119cf835edf347cdba2cb5dcb637e`  
		Last Modified: Wed, 12 May 2021 20:05:24 GMT  
		Size: 5.7 MB (5715678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be0a1b98881464003a76f9c3d552af6aa32676eded40337a2cb740220b8e8b5`  
		Last Modified: Wed, 12 May 2021 20:05:22 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2f0820331f200b69ffc4376c6d900a0eff190f419b5000a08b1b2d643534b6`  
		Last Modified: Wed, 12 May 2021 20:05:26 GMT  
		Size: 17.4 MB (17386489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3493d093c4b99f139a5427c673f7efaa2b5165503ecad87cb8ce5552e11ebf`  
		Last Modified: Wed, 12 May 2021 20:05:20 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fe562a331e468e75447f36e3f25418222bd38dd64ed86e1ed5d135326ca297`  
		Last Modified: Wed, 12 May 2021 20:05:20 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e380b48e44a8409c9d227325699b754573b99734b04ccd9b0afd4d221de4463c`  
		Last Modified: Wed, 12 May 2021 20:05:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4838e63e8d0097db4c9f0b40fb85cb4ca6ab86d367ba5e8e03926567a06fbf6c`  
		Last Modified: Wed, 12 May 2021 20:05:19 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8502433c7f52aac3dd7bda187871008ccc524909273d3ecc731fc21ae788d58`  
		Last Modified: Wed, 12 May 2021 20:05:17 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436d7436a478513cfdd80519a071fb37badf42397c34e5bed6ecb807a0f5f544`  
		Last Modified: Wed, 12 May 2021 20:05:17 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0957a349d9bda1d5d624590e5f8bb02b83605c041e63f495e421a185e7c9cb0b`  
		Last Modified: Wed, 12 May 2021 20:05:17 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5368704288b662f01ec22e1518b4cbfbaebad0f096f0f78b523fbebf1bf8d315`  
		Last Modified: Wed, 12 May 2021 20:05:17 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a57eac0f8fb22c77ed1133dce3b45ff210e67457237188fdd4244a614bcd9b`  
		Last Modified: Wed, 12 May 2021 20:05:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06eb9e82c5d11b8714bdbcc16be6fef89cf5a8e80fa5aec957bb00ea13eb36c3`  
		Last Modified: Wed, 12 May 2021 20:05:14 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b02b72008aedc5b17796c0bdc40233ae777ec8a19530b70983fa5b6f001914c`  
		Last Modified: Wed, 12 May 2021 20:05:14 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e520b47523d14eb979eb9c33ee5803753ddf7192e0f9cc4737e596091333dc45`  
		Last Modified: Wed, 12 May 2021 20:05:14 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cf16fae2c4e03aee1b9269abf928e7299c0912e8d6ce3c646b2398fd0419cf`  
		Last Modified: Wed, 12 May 2021 20:05:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352e7ea39b707bbf4a83cc0c0be3ddf79f71be49669db9f93f17915d9e1235b6`  
		Last Modified: Wed, 12 May 2021 20:05:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da84cbe314c1c929b4ce1e6c633c4e78b61d042c8ed8bcf96da263c53a1d12d3`  
		Last Modified: Wed, 12 May 2021 20:05:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3810c939f9540e16a267e3d1f6a3e3e4162c5b6190d5087acc7eebdf65a014`  
		Last Modified: Wed, 12 May 2021 20:05:12 GMT  
		Size: 280.7 KB (280738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e6e97602e558f4a75b0da2af7de0ccca80cd60b809b803af3f16096fb85332`  
		Last Modified: Wed, 12 May 2021 20:05:16 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.1`

```console
$ docker pull caddy@sha256:1a2f489f3bbeef0cac9397b7064a7908ed3f74b89d6f549825c38f175047d03d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

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

### `caddy:2.4.1` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:1d0e1085c4e0fd3af411a60364e53d9e9ded463184467a4f1595116eb2e4c675
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2491869666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dac2e4738ade97d420148e609ac6c7a6db9edb6db52f3a634814cbe64df1d0b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:56:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 24 May 2021 18:14:49 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:15:23 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 24 May 2021 18:15:24 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 24 May 2021 18:15:25 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 24 May 2021 18:15:27 GMT
VOLUME [c:/config]
# Mon, 24 May 2021 18:15:28 GMT
VOLUME [c:/data]
# Mon, 24 May 2021 18:15:29 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:15:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:15:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:15:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:15:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:15:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:15:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:15:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:15:39 GMT
EXPOSE 80
# Mon, 24 May 2021 18:15:40 GMT
EXPOSE 443
# Mon, 24 May 2021 18:15:41 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:16:00 GMT
RUN caddy version
# Mon, 24 May 2021 18:16:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dc51194378204d7114732c3ee4da8d6b390b048e70ae1535a082de3ff67b5c`  
		Last Modified: Wed, 12 May 2021 20:06:24 GMT  
		Size: 5.1 MB (5106604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81697a0f2a55f882f55ccac9401c3dd272607c42f460a8549f30a1ebb26e0c8`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6400e9488fa4d970dad72e844be39d2d75b7d2c31501c6d6b23d6a1bc524f7c1`  
		Last Modified: Mon, 24 May 2021 18:22:57 GMT  
		Size: 11.9 MB (11930419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5b5da05058a691610222ba26189e6f6c28b9ede612bec34b4ed5dea3691b92`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197bdfed68cccee24a939b4dd69fea66e2dc7827a4017bf444bdd2c90e959f6a`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474f7ecfe9858ec31d5203cc051d4063e0ad4acd2af33e4568f49d9e4b75e41b`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e026dffad92f6dace75c209e6f261b00cf847128dd907ffa4ac9f944e9ae054e`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c534d757d31dc1e6130a58f06b95d25d61f32e015e329cd2227a1bed890280`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31071464c175eef4ea5843313a962e550e530c0a4c12fd997c6ace04fed5d0e0`  
		Last Modified: Mon, 24 May 2021 18:22:51 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3035f85e6f0ef498e48d22a196b3dca2d1feff90554b2f1fbbd3062a92ffccd2`  
		Last Modified: Mon, 24 May 2021 18:22:51 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caffd6e1f83b89b2831eab80faf22c370ad73519467e80354cb56ee96eed7fe3`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285714c5a6fb40773b7e624641f8e036180ab3424ee89b84f3fbbd79d7108eec`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872e853821b7661d1e753ef89a95c2525171915b5dec31950f7b05f4492eb40c`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7958b6b43cba2b3e1a20dc772e84541237901c32ec6dba998eb300627b2e343`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8089fe8b99a3884b64fb515b432248ed2433347b16efe53190c08624ec8bcf8f`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e25c6bfe294987f6c4c3a677078ea11dd90d54892fff638abed3d5a8602360c`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1757220b38637dda7da307ac64a4eefb9226cd9e13d613ab9bb839997c0c2aa8`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a748ef821631911b8abd470af8b29305283a82e1b5da1d2459257d8308576a2`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa22970d4f705eac4e8ea2ac4a7f3e89cfc01035b6ff0bf8998c146fe4d9a96`  
		Last Modified: Mon, 24 May 2021 18:22:47 GMT  
		Size: 317.9 KB (317938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2477d94c5c1388771379c903fc8931c2531d21a7ccbef4b3b7e2d6461fb19fdd`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:d530e436d6d892bc2662481a943d230921dd8d5b2a26de0d99c32abb59ce1973
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5819027610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:189fbf35362e472481d308f9fbecfeda8962471fccd521c1cdd2165bfff22c08`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:58:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 24 May 2021 18:16:16 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:17:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 24 May 2021 18:18:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 24 May 2021 18:18:02 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 24 May 2021 18:18:03 GMT
VOLUME [c:/config]
# Mon, 24 May 2021 18:18:04 GMT
VOLUME [c:/data]
# Mon, 24 May 2021 18:18:05 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:18:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:18:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:18:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:18:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:18:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:18:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:18:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:18:14 GMT
EXPOSE 80
# Mon, 24 May 2021 18:18:15 GMT
EXPOSE 443
# Mon, 24 May 2021 18:18:16 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:19:09 GMT
RUN caddy version
# Mon, 24 May 2021 18:19:10 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26858854e9a4d33437022a0cbf481973fa7709cc09d3402af046620cbbe5c0`  
		Last Modified: Wed, 12 May 2021 20:07:13 GMT  
		Size: 5.7 MB (5714091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba52519d045fbbd4b405dea0a101b9ede50767ce1b8b92f0b0a9708dc3a3492`  
		Last Modified: Mon, 24 May 2021 18:23:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073bc62336c22adb06e7c530733538c823c0e30b591f536ca853dd86ff16e632`  
		Last Modified: Mon, 24 May 2021 18:23:26 GMT  
		Size: 17.2 MB (17244195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319fcbb76d6ed2f5920ae3cf875486281ed4d5edc53c630c8c6ad581efc92594`  
		Last Modified: Mon, 24 May 2021 18:23:22 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d372740cbc98799ef99cd14fe521f6c8bc0202f7e6eb418f8db3e6cae94caf60`  
		Last Modified: Mon, 24 May 2021 18:23:21 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c1957ce089769a88ac826364c0cb191ae826407602ccf505c76ee34afa10c8`  
		Last Modified: Mon, 24 May 2021 18:23:20 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e022ba7739dc4609e4838ae24c6930ccdc82d0721cc978c71a7e036122adf228`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5716dc07e962e5602a2cecf1a5b63c75352ad0e48b06b30070ad5cd4a31993`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc94100cd9e1fb3620069275788a9e1b912502dcd7966b4d624ecba5f88690`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7790197c85ec7196ed9b956d8f481e8f382479a3b8e20db4d8e564f14331eb42`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60939c5f58f38df81a8563072d42fcd4fb79292dbf5ce4d31a46f840e777fb88`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d5876f07c48377c92817efa2b077cfe4c05822b08a1916d350b5e8ee682b50`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2933951452131d66acb34683269ade093ebb9faf312436b0a601168cb6e2fe68`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ad33c6332b1b2a8e806339fd2978dd9a8919fc98d48fc0ae6a58ad07870cec`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b44c787b930665927a13e544b5d3d7243caae27d4d9a6f9502f985e8483af61`  
		Last Modified: Mon, 24 May 2021 18:23:16 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e86dd1b42134f467b929f29aa052bdca8a20ccbb6ff1332575ef7843b962243`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3288b716f0b64cb14a9da486b126557c121b9a71476d5aea6a1be399a82bb14b`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83f9226706657b746cb502303856ebeca1a6cda85b1aea65196506c3e3faa4a`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fc7b2fb07d7a4265b695bf44d6d3378e7f0202a6c8fd0d359f766886070802`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 266.6 KB (266650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cde5c4ac8767e62fceac7aed63a74d7935277b8087425319abfe8e22f7bb37`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1435 bytes)  
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
$ docker pull caddy@sha256:fb66ce856e2039c6e0cb70dba12e8a7f50a9cd7ef53905a4307cff6e9220f682
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

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

### `caddy:2.4.1-builder` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:5cd5e5c8ae7367744428893e4a407d97f68f70fbd298770c1518b65f3b740476
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646121085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b3e2a6c24449822ef29f7460905fddcbb84871a7dfa5dc27265afa64fa3778`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:24:28 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:24:29 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:24:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:24:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:25:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:25:36 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:26:02 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Jun 2021 01:19:04 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 01:21:38 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Jun 2021 01:21:40 GMT
WORKDIR C:\gopath
# Fri, 04 Jun 2021 02:10:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Jun 2021 02:10:55 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 02:10:56 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 02:10:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 02:11:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Jun 2021 02:11:25 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2a5ccd12170e9f926c3e069a2fa2ed38b5dd5596869ed982bccc50ef80cf1f`  
		Last Modified: Wed, 12 May 2021 12:52:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd5b5fa12081ad53ae688dc454e550dd50bd414c949724180719b0326632c4a`  
		Last Modified: Wed, 12 May 2021 12:52:08 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599ef939f9e7c26d4bc0f8f75820116f6977a64212b86260bc225ae2d850cc31`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bddce42b6f4351510fcb255839a7c55d95546186dce8509782abe959d27d9f0`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2407bf3b614294860b53b94e661f5c57f7dd985934aed5727442f9353bf8c617`  
		Last Modified: Wed, 12 May 2021 12:52:14 GMT  
		Size: 30.2 MB (30189126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b01ea9b4210c3201c1462d7ee78b276d7d5ffac3dca02c9c57a0c77c5b87a2`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27be8fd19f331f65055bbf31138aa28628be7534753008620ec14fc1803ebdf2`  
		Last Modified: Wed, 12 May 2021 12:52:05 GMT  
		Size: 313.1 KB (313094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f8e1e31aa0e91f80a0d7a9cf238278557166647fd937cc7b714778366d586a`  
		Last Modified: Fri, 04 Jun 2021 01:40:04 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ba074ffe696278b5b2037378141f68377dcab07cbcf7c6d31fcd4c097869ce`  
		Last Modified: Fri, 04 Jun 2021 01:42:39 GMT  
		Size: 139.4 MB (139388725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2deb8a1660a185bba3fa7aaabc4cb64555918509a91d9f186f15ec469ec476a0`  
		Last Modified: Fri, 04 Jun 2021 01:40:04 GMT  
		Size: 1.6 KB (1586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bce5d3df849365bd1516c0abf3aa29cee32abb96cc1cdf79c2e7019f2016cc0`  
		Last Modified: Fri, 04 Jun 2021 02:14:37 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc77252a6e317a6fcaeba9d070cfad6c4e568f095056d19727ffe6955e1a1c5a`  
		Last Modified: Fri, 04 Jun 2021 02:14:34 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f53aa8e353d64b1c65256ffeeb6708506ca6a23ee2c94016a8f034452259b0`  
		Last Modified: Fri, 04 Jun 2021 02:14:34 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c500d7c801483b02cfdfc1a272882d3b98559bcfacfb956ef4bb395fadccc61`  
		Last Modified: Fri, 04 Jun 2021 02:14:34 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243445945aa8cf8386f4cb635126e213960fe164cc0b2cf9829c40fb29e06dc4`  
		Last Modified: Fri, 04 Jun 2021 02:14:37 GMT  
		Size: 1.7 MB (1722485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5462596ac55051140e5c69946dc7620a0169d39d4b3a3b826e0daf4a0d924e8`  
		Last Modified: Fri, 04 Jun 2021 02:14:35 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1-builder` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:23de8a02fd104f11187fa0e6f1c50d9a833788ef94cc3d78b82ad3b4f35c9fad
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5988471116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4830f2cecfad3d8daa420d50870e8aa44c459224a23f9ff77de7da22e670b94`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:29:13 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:29:14 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:29:15 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:29:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:31:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:31:45 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:33:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Jun 2021 01:21:50 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 01:26:36 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Jun 2021 01:26:38 GMT
WORKDIR C:\gopath
# Fri, 04 Jun 2021 02:11:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Jun 2021 02:11:34 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 02:11:35 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 02:11:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 02:13:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Jun 2021 02:13:06 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10abf429e12c7b3b7d2b0a791d7cdb47866461a7b63df4ddd4f63acc91e26231`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79955f676504cbf77ec284d8e857d18d17b93c5b8e6438b4062dd80f8632c9d6`  
		Last Modified: Wed, 12 May 2021 12:55:12 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24af485ecab19f81a0c65c0eaec6f6fda8749ca50eb53101abcfc5c079f9b1c2`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b782f6bcd162ee81518d73c6c4fe5c5b731ab38b595c16a55ac185db84b2c9b`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1327fc384f9fff64d41446adcb3bdf585307370ef0024a31a5269bae6f30067d`  
		Last Modified: Wed, 12 May 2021 12:55:18 GMT  
		Size: 30.8 MB (30797956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c50f4b0b5994b4154be9fea2ab6c6a0e4c402c44d44795a5ce82ab6f8de4bc`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e458669a58e08411a0641a721ef1daf4af2a568c4dd61e9a3710b07f73b6ec`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 5.7 MB (5661591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7024df9f6db05baebb2373ac9d80a105fbfaafacf00e75d4b28847d1503ea8dc`  
		Last Modified: Fri, 04 Jun 2021 01:42:57 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b83a1b7a993d551850c2952fac9ce015fd85e6e96491ffc601809c6e4c9013`  
		Last Modified: Fri, 04 Jun 2021 01:45:53 GMT  
		Size: 149.2 MB (149182156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03bac4443c0dacba8f0d8dbd25091bc1d39b3ee36e84604482d40220f39f57d`  
		Last Modified: Fri, 04 Jun 2021 01:42:57 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51201b480eb2d1bd5736f2e118d9ddaafafce32222e161cb63b66a46bf95d9f`  
		Last Modified: Fri, 04 Jun 2021 02:14:54 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10338b4cf9e50762fa10529606ac5ab6d7c227a0aefcce7173718d53ef6b341`  
		Last Modified: Fri, 04 Jun 2021 02:14:51 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa84546d6c6cfa9ed6da4b4400af439e067c8f873c8ef40452cc57c7944a065`  
		Last Modified: Fri, 04 Jun 2021 02:14:51 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071bbd37c903648e3ebd95cc6dcb2b78d6ea639005d65aab5016dd7859a4f17b`  
		Last Modified: Fri, 04 Jun 2021 02:14:51 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2215edc22b4111496ab6990dcdc789842dbeaaa2138be04dcbb3ce883e984e`  
		Last Modified: Fri, 04 Jun 2021 02:14:59 GMT  
		Size: 7.0 MB (7033480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2c9d2207f5d9c10b8413a2bdbb9bb17306d47cd8d1efd70a3593d5343de178`  
		Last Modified: Fri, 04 Jun 2021 02:14:51 GMT  
		Size: 1.4 KB (1408 bytes)  
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
$ docker pull caddy@sha256:c6473228286ce37912a7ba2003a626c415698df940f04e7c88430e4ad01e168a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `caddy:2.4.1-builder-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:5cd5e5c8ae7367744428893e4a407d97f68f70fbd298770c1518b65f3b740476
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646121085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b3e2a6c24449822ef29f7460905fddcbb84871a7dfa5dc27265afa64fa3778`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:24:28 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:24:29 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:24:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:24:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:25:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:25:36 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:26:02 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Jun 2021 01:19:04 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 01:21:38 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Jun 2021 01:21:40 GMT
WORKDIR C:\gopath
# Fri, 04 Jun 2021 02:10:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Jun 2021 02:10:55 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 02:10:56 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 02:10:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 02:11:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Jun 2021 02:11:25 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2a5ccd12170e9f926c3e069a2fa2ed38b5dd5596869ed982bccc50ef80cf1f`  
		Last Modified: Wed, 12 May 2021 12:52:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd5b5fa12081ad53ae688dc454e550dd50bd414c949724180719b0326632c4a`  
		Last Modified: Wed, 12 May 2021 12:52:08 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599ef939f9e7c26d4bc0f8f75820116f6977a64212b86260bc225ae2d850cc31`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bddce42b6f4351510fcb255839a7c55d95546186dce8509782abe959d27d9f0`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2407bf3b614294860b53b94e661f5c57f7dd985934aed5727442f9353bf8c617`  
		Last Modified: Wed, 12 May 2021 12:52:14 GMT  
		Size: 30.2 MB (30189126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b01ea9b4210c3201c1462d7ee78b276d7d5ffac3dca02c9c57a0c77c5b87a2`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27be8fd19f331f65055bbf31138aa28628be7534753008620ec14fc1803ebdf2`  
		Last Modified: Wed, 12 May 2021 12:52:05 GMT  
		Size: 313.1 KB (313094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f8e1e31aa0e91f80a0d7a9cf238278557166647fd937cc7b714778366d586a`  
		Last Modified: Fri, 04 Jun 2021 01:40:04 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ba074ffe696278b5b2037378141f68377dcab07cbcf7c6d31fcd4c097869ce`  
		Last Modified: Fri, 04 Jun 2021 01:42:39 GMT  
		Size: 139.4 MB (139388725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2deb8a1660a185bba3fa7aaabc4cb64555918509a91d9f186f15ec469ec476a0`  
		Last Modified: Fri, 04 Jun 2021 01:40:04 GMT  
		Size: 1.6 KB (1586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bce5d3df849365bd1516c0abf3aa29cee32abb96cc1cdf79c2e7019f2016cc0`  
		Last Modified: Fri, 04 Jun 2021 02:14:37 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc77252a6e317a6fcaeba9d070cfad6c4e568f095056d19727ffe6955e1a1c5a`  
		Last Modified: Fri, 04 Jun 2021 02:14:34 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f53aa8e353d64b1c65256ffeeb6708506ca6a23ee2c94016a8f034452259b0`  
		Last Modified: Fri, 04 Jun 2021 02:14:34 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c500d7c801483b02cfdfc1a272882d3b98559bcfacfb956ef4bb395fadccc61`  
		Last Modified: Fri, 04 Jun 2021 02:14:34 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243445945aa8cf8386f4cb635126e213960fe164cc0b2cf9829c40fb29e06dc4`  
		Last Modified: Fri, 04 Jun 2021 02:14:37 GMT  
		Size: 1.7 MB (1722485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5462596ac55051140e5c69946dc7620a0169d39d4b3a3b826e0daf4a0d924e8`  
		Last Modified: Fri, 04 Jun 2021 02:14:35 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.1-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:befa7d7c88cc950857d567f8fcd2ba435be538c6e6443ee1f806e755f27ea4ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `caddy:2.4.1-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:23de8a02fd104f11187fa0e6f1c50d9a833788ef94cc3d78b82ad3b4f35c9fad
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5988471116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4830f2cecfad3d8daa420d50870e8aa44c459224a23f9ff77de7da22e670b94`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:29:13 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:29:14 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:29:15 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:29:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:31:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:31:45 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:33:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Jun 2021 01:21:50 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 01:26:36 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Jun 2021 01:26:38 GMT
WORKDIR C:\gopath
# Fri, 04 Jun 2021 02:11:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Jun 2021 02:11:34 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 02:11:35 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 02:11:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 02:13:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Jun 2021 02:13:06 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10abf429e12c7b3b7d2b0a791d7cdb47866461a7b63df4ddd4f63acc91e26231`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79955f676504cbf77ec284d8e857d18d17b93c5b8e6438b4062dd80f8632c9d6`  
		Last Modified: Wed, 12 May 2021 12:55:12 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24af485ecab19f81a0c65c0eaec6f6fda8749ca50eb53101abcfc5c079f9b1c2`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b782f6bcd162ee81518d73c6c4fe5c5b731ab38b595c16a55ac185db84b2c9b`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1327fc384f9fff64d41446adcb3bdf585307370ef0024a31a5269bae6f30067d`  
		Last Modified: Wed, 12 May 2021 12:55:18 GMT  
		Size: 30.8 MB (30797956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c50f4b0b5994b4154be9fea2ab6c6a0e4c402c44d44795a5ce82ab6f8de4bc`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e458669a58e08411a0641a721ef1daf4af2a568c4dd61e9a3710b07f73b6ec`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 5.7 MB (5661591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7024df9f6db05baebb2373ac9d80a105fbfaafacf00e75d4b28847d1503ea8dc`  
		Last Modified: Fri, 04 Jun 2021 01:42:57 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b83a1b7a993d551850c2952fac9ce015fd85e6e96491ffc601809c6e4c9013`  
		Last Modified: Fri, 04 Jun 2021 01:45:53 GMT  
		Size: 149.2 MB (149182156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03bac4443c0dacba8f0d8dbd25091bc1d39b3ee36e84604482d40220f39f57d`  
		Last Modified: Fri, 04 Jun 2021 01:42:57 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51201b480eb2d1bd5736f2e118d9ddaafafce32222e161cb63b66a46bf95d9f`  
		Last Modified: Fri, 04 Jun 2021 02:14:54 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10338b4cf9e50762fa10529606ac5ab6d7c227a0aefcce7173718d53ef6b341`  
		Last Modified: Fri, 04 Jun 2021 02:14:51 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa84546d6c6cfa9ed6da4b4400af439e067c8f873c8ef40452cc57c7944a065`  
		Last Modified: Fri, 04 Jun 2021 02:14:51 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071bbd37c903648e3ebd95cc6dcb2b78d6ea639005d65aab5016dd7859a4f17b`  
		Last Modified: Fri, 04 Jun 2021 02:14:51 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2215edc22b4111496ab6990dcdc789842dbeaaa2138be04dcbb3ce883e984e`  
		Last Modified: Fri, 04 Jun 2021 02:14:59 GMT  
		Size: 7.0 MB (7033480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2c9d2207f5d9c10b8413a2bdbb9bb17306d47cd8d1efd70a3593d5343de178`  
		Last Modified: Fri, 04 Jun 2021 02:14:51 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.1-windowsservercore`

```console
$ docker pull caddy@sha256:c544077722bd97f1b56e46cf2c37d89d460d590defbe607243a750a2ab90a554
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `caddy:2.4.1-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:1d0e1085c4e0fd3af411a60364e53d9e9ded463184467a4f1595116eb2e4c675
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2491869666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dac2e4738ade97d420148e609ac6c7a6db9edb6db52f3a634814cbe64df1d0b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:56:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 24 May 2021 18:14:49 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:15:23 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 24 May 2021 18:15:24 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 24 May 2021 18:15:25 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 24 May 2021 18:15:27 GMT
VOLUME [c:/config]
# Mon, 24 May 2021 18:15:28 GMT
VOLUME [c:/data]
# Mon, 24 May 2021 18:15:29 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:15:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:15:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:15:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:15:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:15:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:15:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:15:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:15:39 GMT
EXPOSE 80
# Mon, 24 May 2021 18:15:40 GMT
EXPOSE 443
# Mon, 24 May 2021 18:15:41 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:16:00 GMT
RUN caddy version
# Mon, 24 May 2021 18:16:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dc51194378204d7114732c3ee4da8d6b390b048e70ae1535a082de3ff67b5c`  
		Last Modified: Wed, 12 May 2021 20:06:24 GMT  
		Size: 5.1 MB (5106604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81697a0f2a55f882f55ccac9401c3dd272607c42f460a8549f30a1ebb26e0c8`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6400e9488fa4d970dad72e844be39d2d75b7d2c31501c6d6b23d6a1bc524f7c1`  
		Last Modified: Mon, 24 May 2021 18:22:57 GMT  
		Size: 11.9 MB (11930419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5b5da05058a691610222ba26189e6f6c28b9ede612bec34b4ed5dea3691b92`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197bdfed68cccee24a939b4dd69fea66e2dc7827a4017bf444bdd2c90e959f6a`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474f7ecfe9858ec31d5203cc051d4063e0ad4acd2af33e4568f49d9e4b75e41b`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e026dffad92f6dace75c209e6f261b00cf847128dd907ffa4ac9f944e9ae054e`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c534d757d31dc1e6130a58f06b95d25d61f32e015e329cd2227a1bed890280`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31071464c175eef4ea5843313a962e550e530c0a4c12fd997c6ace04fed5d0e0`  
		Last Modified: Mon, 24 May 2021 18:22:51 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3035f85e6f0ef498e48d22a196b3dca2d1feff90554b2f1fbbd3062a92ffccd2`  
		Last Modified: Mon, 24 May 2021 18:22:51 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caffd6e1f83b89b2831eab80faf22c370ad73519467e80354cb56ee96eed7fe3`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285714c5a6fb40773b7e624641f8e036180ab3424ee89b84f3fbbd79d7108eec`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872e853821b7661d1e753ef89a95c2525171915b5dec31950f7b05f4492eb40c`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7958b6b43cba2b3e1a20dc772e84541237901c32ec6dba998eb300627b2e343`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8089fe8b99a3884b64fb515b432248ed2433347b16efe53190c08624ec8bcf8f`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e25c6bfe294987f6c4c3a677078ea11dd90d54892fff638abed3d5a8602360c`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1757220b38637dda7da307ac64a4eefb9226cd9e13d613ab9bb839997c0c2aa8`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a748ef821631911b8abd470af8b29305283a82e1b5da1d2459257d8308576a2`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa22970d4f705eac4e8ea2ac4a7f3e89cfc01035b6ff0bf8998c146fe4d9a96`  
		Last Modified: Mon, 24 May 2021 18:22:47 GMT  
		Size: 317.9 KB (317938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2477d94c5c1388771379c903fc8931c2531d21a7ccbef4b3b7e2d6461fb19fdd`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.1-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:d530e436d6d892bc2662481a943d230921dd8d5b2a26de0d99c32abb59ce1973
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5819027610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:189fbf35362e472481d308f9fbecfeda8962471fccd521c1cdd2165bfff22c08`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:58:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 24 May 2021 18:16:16 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:17:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 24 May 2021 18:18:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 24 May 2021 18:18:02 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 24 May 2021 18:18:03 GMT
VOLUME [c:/config]
# Mon, 24 May 2021 18:18:04 GMT
VOLUME [c:/data]
# Mon, 24 May 2021 18:18:05 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:18:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:18:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:18:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:18:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:18:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:18:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:18:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:18:14 GMT
EXPOSE 80
# Mon, 24 May 2021 18:18:15 GMT
EXPOSE 443
# Mon, 24 May 2021 18:18:16 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:19:09 GMT
RUN caddy version
# Mon, 24 May 2021 18:19:10 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26858854e9a4d33437022a0cbf481973fa7709cc09d3402af046620cbbe5c0`  
		Last Modified: Wed, 12 May 2021 20:07:13 GMT  
		Size: 5.7 MB (5714091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba52519d045fbbd4b405dea0a101b9ede50767ce1b8b92f0b0a9708dc3a3492`  
		Last Modified: Mon, 24 May 2021 18:23:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073bc62336c22adb06e7c530733538c823c0e30b591f536ca853dd86ff16e632`  
		Last Modified: Mon, 24 May 2021 18:23:26 GMT  
		Size: 17.2 MB (17244195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319fcbb76d6ed2f5920ae3cf875486281ed4d5edc53c630c8c6ad581efc92594`  
		Last Modified: Mon, 24 May 2021 18:23:22 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d372740cbc98799ef99cd14fe521f6c8bc0202f7e6eb418f8db3e6cae94caf60`  
		Last Modified: Mon, 24 May 2021 18:23:21 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c1957ce089769a88ac826364c0cb191ae826407602ccf505c76ee34afa10c8`  
		Last Modified: Mon, 24 May 2021 18:23:20 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e022ba7739dc4609e4838ae24c6930ccdc82d0721cc978c71a7e036122adf228`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5716dc07e962e5602a2cecf1a5b63c75352ad0e48b06b30070ad5cd4a31993`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc94100cd9e1fb3620069275788a9e1b912502dcd7966b4d624ecba5f88690`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7790197c85ec7196ed9b956d8f481e8f382479a3b8e20db4d8e564f14331eb42`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60939c5f58f38df81a8563072d42fcd4fb79292dbf5ce4d31a46f840e777fb88`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d5876f07c48377c92817efa2b077cfe4c05822b08a1916d350b5e8ee682b50`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2933951452131d66acb34683269ade093ebb9faf312436b0a601168cb6e2fe68`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ad33c6332b1b2a8e806339fd2978dd9a8919fc98d48fc0ae6a58ad07870cec`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b44c787b930665927a13e544b5d3d7243caae27d4d9a6f9502f985e8483af61`  
		Last Modified: Mon, 24 May 2021 18:23:16 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e86dd1b42134f467b929f29aa052bdca8a20ccbb6ff1332575ef7843b962243`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3288b716f0b64cb14a9da486b126557c121b9a71476d5aea6a1be399a82bb14b`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83f9226706657b746cb502303856ebeca1a6cda85b1aea65196506c3e3faa4a`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fc7b2fb07d7a4265b695bf44d6d3378e7f0202a6c8fd0d359f766886070802`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 266.6 KB (266650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cde5c4ac8767e62fceac7aed63a74d7935277b8087425319abfe8e22f7bb37`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.1-windowsservercore-1809`

```console
$ docker pull caddy@sha256:fb9fcd910a8050aa2ce11ac6b195722843c6efc46c1cf68fbb3a4172914c2e30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `caddy:2.4.1-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:1d0e1085c4e0fd3af411a60364e53d9e9ded463184467a4f1595116eb2e4c675
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2491869666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dac2e4738ade97d420148e609ac6c7a6db9edb6db52f3a634814cbe64df1d0b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:56:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 24 May 2021 18:14:49 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:15:23 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 24 May 2021 18:15:24 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 24 May 2021 18:15:25 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 24 May 2021 18:15:27 GMT
VOLUME [c:/config]
# Mon, 24 May 2021 18:15:28 GMT
VOLUME [c:/data]
# Mon, 24 May 2021 18:15:29 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:15:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:15:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:15:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:15:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:15:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:15:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:15:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:15:39 GMT
EXPOSE 80
# Mon, 24 May 2021 18:15:40 GMT
EXPOSE 443
# Mon, 24 May 2021 18:15:41 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:16:00 GMT
RUN caddy version
# Mon, 24 May 2021 18:16:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dc51194378204d7114732c3ee4da8d6b390b048e70ae1535a082de3ff67b5c`  
		Last Modified: Wed, 12 May 2021 20:06:24 GMT  
		Size: 5.1 MB (5106604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81697a0f2a55f882f55ccac9401c3dd272607c42f460a8549f30a1ebb26e0c8`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6400e9488fa4d970dad72e844be39d2d75b7d2c31501c6d6b23d6a1bc524f7c1`  
		Last Modified: Mon, 24 May 2021 18:22:57 GMT  
		Size: 11.9 MB (11930419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5b5da05058a691610222ba26189e6f6c28b9ede612bec34b4ed5dea3691b92`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197bdfed68cccee24a939b4dd69fea66e2dc7827a4017bf444bdd2c90e959f6a`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474f7ecfe9858ec31d5203cc051d4063e0ad4acd2af33e4568f49d9e4b75e41b`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e026dffad92f6dace75c209e6f261b00cf847128dd907ffa4ac9f944e9ae054e`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c534d757d31dc1e6130a58f06b95d25d61f32e015e329cd2227a1bed890280`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31071464c175eef4ea5843313a962e550e530c0a4c12fd997c6ace04fed5d0e0`  
		Last Modified: Mon, 24 May 2021 18:22:51 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3035f85e6f0ef498e48d22a196b3dca2d1feff90554b2f1fbbd3062a92ffccd2`  
		Last Modified: Mon, 24 May 2021 18:22:51 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caffd6e1f83b89b2831eab80faf22c370ad73519467e80354cb56ee96eed7fe3`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285714c5a6fb40773b7e624641f8e036180ab3424ee89b84f3fbbd79d7108eec`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872e853821b7661d1e753ef89a95c2525171915b5dec31950f7b05f4492eb40c`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7958b6b43cba2b3e1a20dc772e84541237901c32ec6dba998eb300627b2e343`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8089fe8b99a3884b64fb515b432248ed2433347b16efe53190c08624ec8bcf8f`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e25c6bfe294987f6c4c3a677078ea11dd90d54892fff638abed3d5a8602360c`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1757220b38637dda7da307ac64a4eefb9226cd9e13d613ab9bb839997c0c2aa8`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a748ef821631911b8abd470af8b29305283a82e1b5da1d2459257d8308576a2`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa22970d4f705eac4e8ea2ac4a7f3e89cfc01035b6ff0bf8998c146fe4d9a96`  
		Last Modified: Mon, 24 May 2021 18:22:47 GMT  
		Size: 317.9 KB (317938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2477d94c5c1388771379c903fc8931c2531d21a7ccbef4b3b7e2d6461fb19fdd`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.1-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:9d786a7a09f9a8edcfdc2a75b463592913275d75986f55ca9d67f3ba0b848c67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `caddy:2.4.1-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:d530e436d6d892bc2662481a943d230921dd8d5b2a26de0d99c32abb59ce1973
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5819027610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:189fbf35362e472481d308f9fbecfeda8962471fccd521c1cdd2165bfff22c08`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:58:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 24 May 2021 18:16:16 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:17:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 24 May 2021 18:18:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 24 May 2021 18:18:02 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 24 May 2021 18:18:03 GMT
VOLUME [c:/config]
# Mon, 24 May 2021 18:18:04 GMT
VOLUME [c:/data]
# Mon, 24 May 2021 18:18:05 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:18:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:18:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:18:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:18:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:18:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:18:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:18:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:18:14 GMT
EXPOSE 80
# Mon, 24 May 2021 18:18:15 GMT
EXPOSE 443
# Mon, 24 May 2021 18:18:16 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:19:09 GMT
RUN caddy version
# Mon, 24 May 2021 18:19:10 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26858854e9a4d33437022a0cbf481973fa7709cc09d3402af046620cbbe5c0`  
		Last Modified: Wed, 12 May 2021 20:07:13 GMT  
		Size: 5.7 MB (5714091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba52519d045fbbd4b405dea0a101b9ede50767ce1b8b92f0b0a9708dc3a3492`  
		Last Modified: Mon, 24 May 2021 18:23:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073bc62336c22adb06e7c530733538c823c0e30b591f536ca853dd86ff16e632`  
		Last Modified: Mon, 24 May 2021 18:23:26 GMT  
		Size: 17.2 MB (17244195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319fcbb76d6ed2f5920ae3cf875486281ed4d5edc53c630c8c6ad581efc92594`  
		Last Modified: Mon, 24 May 2021 18:23:22 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d372740cbc98799ef99cd14fe521f6c8bc0202f7e6eb418f8db3e6cae94caf60`  
		Last Modified: Mon, 24 May 2021 18:23:21 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c1957ce089769a88ac826364c0cb191ae826407602ccf505c76ee34afa10c8`  
		Last Modified: Mon, 24 May 2021 18:23:20 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e022ba7739dc4609e4838ae24c6930ccdc82d0721cc978c71a7e036122adf228`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5716dc07e962e5602a2cecf1a5b63c75352ad0e48b06b30070ad5cd4a31993`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc94100cd9e1fb3620069275788a9e1b912502dcd7966b4d624ecba5f88690`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7790197c85ec7196ed9b956d8f481e8f382479a3b8e20db4d8e564f14331eb42`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60939c5f58f38df81a8563072d42fcd4fb79292dbf5ce4d31a46f840e777fb88`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d5876f07c48377c92817efa2b077cfe4c05822b08a1916d350b5e8ee682b50`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2933951452131d66acb34683269ade093ebb9faf312436b0a601168cb6e2fe68`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ad33c6332b1b2a8e806339fd2978dd9a8919fc98d48fc0ae6a58ad07870cec`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b44c787b930665927a13e544b5d3d7243caae27d4d9a6f9502f985e8483af61`  
		Last Modified: Mon, 24 May 2021 18:23:16 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e86dd1b42134f467b929f29aa052bdca8a20ccbb6ff1332575ef7843b962243`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3288b716f0b64cb14a9da486b126557c121b9a71476d5aea6a1be399a82bb14b`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83f9226706657b746cb502303856ebeca1a6cda85b1aea65196506c3e3faa4a`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fc7b2fb07d7a4265b695bf44d6d3378e7f0202a6c8fd0d359f766886070802`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 266.6 KB (266650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cde5c4ac8767e62fceac7aed63a74d7935277b8087425319abfe8e22f7bb37`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1435 bytes)  
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
$ docker pull caddy@sha256:fb66ce856e2039c6e0cb70dba12e8a7f50a9cd7ef53905a4307cff6e9220f682
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

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

### `caddy:builder` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:5cd5e5c8ae7367744428893e4a407d97f68f70fbd298770c1518b65f3b740476
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646121085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b3e2a6c24449822ef29f7460905fddcbb84871a7dfa5dc27265afa64fa3778`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:24:28 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:24:29 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:24:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:24:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:25:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:25:36 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:26:02 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Jun 2021 01:19:04 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 01:21:38 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Jun 2021 01:21:40 GMT
WORKDIR C:\gopath
# Fri, 04 Jun 2021 02:10:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Jun 2021 02:10:55 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 02:10:56 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 02:10:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 02:11:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Jun 2021 02:11:25 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2a5ccd12170e9f926c3e069a2fa2ed38b5dd5596869ed982bccc50ef80cf1f`  
		Last Modified: Wed, 12 May 2021 12:52:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd5b5fa12081ad53ae688dc454e550dd50bd414c949724180719b0326632c4a`  
		Last Modified: Wed, 12 May 2021 12:52:08 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599ef939f9e7c26d4bc0f8f75820116f6977a64212b86260bc225ae2d850cc31`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bddce42b6f4351510fcb255839a7c55d95546186dce8509782abe959d27d9f0`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2407bf3b614294860b53b94e661f5c57f7dd985934aed5727442f9353bf8c617`  
		Last Modified: Wed, 12 May 2021 12:52:14 GMT  
		Size: 30.2 MB (30189126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b01ea9b4210c3201c1462d7ee78b276d7d5ffac3dca02c9c57a0c77c5b87a2`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27be8fd19f331f65055bbf31138aa28628be7534753008620ec14fc1803ebdf2`  
		Last Modified: Wed, 12 May 2021 12:52:05 GMT  
		Size: 313.1 KB (313094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f8e1e31aa0e91f80a0d7a9cf238278557166647fd937cc7b714778366d586a`  
		Last Modified: Fri, 04 Jun 2021 01:40:04 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ba074ffe696278b5b2037378141f68377dcab07cbcf7c6d31fcd4c097869ce`  
		Last Modified: Fri, 04 Jun 2021 01:42:39 GMT  
		Size: 139.4 MB (139388725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2deb8a1660a185bba3fa7aaabc4cb64555918509a91d9f186f15ec469ec476a0`  
		Last Modified: Fri, 04 Jun 2021 01:40:04 GMT  
		Size: 1.6 KB (1586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bce5d3df849365bd1516c0abf3aa29cee32abb96cc1cdf79c2e7019f2016cc0`  
		Last Modified: Fri, 04 Jun 2021 02:14:37 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc77252a6e317a6fcaeba9d070cfad6c4e568f095056d19727ffe6955e1a1c5a`  
		Last Modified: Fri, 04 Jun 2021 02:14:34 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f53aa8e353d64b1c65256ffeeb6708506ca6a23ee2c94016a8f034452259b0`  
		Last Modified: Fri, 04 Jun 2021 02:14:34 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c500d7c801483b02cfdfc1a272882d3b98559bcfacfb956ef4bb395fadccc61`  
		Last Modified: Fri, 04 Jun 2021 02:14:34 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243445945aa8cf8386f4cb635126e213960fe164cc0b2cf9829c40fb29e06dc4`  
		Last Modified: Fri, 04 Jun 2021 02:14:37 GMT  
		Size: 1.7 MB (1722485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5462596ac55051140e5c69946dc7620a0169d39d4b3a3b826e0daf4a0d924e8`  
		Last Modified: Fri, 04 Jun 2021 02:14:35 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:23de8a02fd104f11187fa0e6f1c50d9a833788ef94cc3d78b82ad3b4f35c9fad
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5988471116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4830f2cecfad3d8daa420d50870e8aa44c459224a23f9ff77de7da22e670b94`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:29:13 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:29:14 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:29:15 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:29:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:31:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:31:45 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:33:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Jun 2021 01:21:50 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 01:26:36 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Jun 2021 01:26:38 GMT
WORKDIR C:\gopath
# Fri, 04 Jun 2021 02:11:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Jun 2021 02:11:34 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 02:11:35 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 02:11:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 02:13:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Jun 2021 02:13:06 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10abf429e12c7b3b7d2b0a791d7cdb47866461a7b63df4ddd4f63acc91e26231`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79955f676504cbf77ec284d8e857d18d17b93c5b8e6438b4062dd80f8632c9d6`  
		Last Modified: Wed, 12 May 2021 12:55:12 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24af485ecab19f81a0c65c0eaec6f6fda8749ca50eb53101abcfc5c079f9b1c2`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b782f6bcd162ee81518d73c6c4fe5c5b731ab38b595c16a55ac185db84b2c9b`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1327fc384f9fff64d41446adcb3bdf585307370ef0024a31a5269bae6f30067d`  
		Last Modified: Wed, 12 May 2021 12:55:18 GMT  
		Size: 30.8 MB (30797956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c50f4b0b5994b4154be9fea2ab6c6a0e4c402c44d44795a5ce82ab6f8de4bc`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e458669a58e08411a0641a721ef1daf4af2a568c4dd61e9a3710b07f73b6ec`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 5.7 MB (5661591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7024df9f6db05baebb2373ac9d80a105fbfaafacf00e75d4b28847d1503ea8dc`  
		Last Modified: Fri, 04 Jun 2021 01:42:57 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b83a1b7a993d551850c2952fac9ce015fd85e6e96491ffc601809c6e4c9013`  
		Last Modified: Fri, 04 Jun 2021 01:45:53 GMT  
		Size: 149.2 MB (149182156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03bac4443c0dacba8f0d8dbd25091bc1d39b3ee36e84604482d40220f39f57d`  
		Last Modified: Fri, 04 Jun 2021 01:42:57 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51201b480eb2d1bd5736f2e118d9ddaafafce32222e161cb63b66a46bf95d9f`  
		Last Modified: Fri, 04 Jun 2021 02:14:54 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10338b4cf9e50762fa10529606ac5ab6d7c227a0aefcce7173718d53ef6b341`  
		Last Modified: Fri, 04 Jun 2021 02:14:51 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa84546d6c6cfa9ed6da4b4400af439e067c8f873c8ef40452cc57c7944a065`  
		Last Modified: Fri, 04 Jun 2021 02:14:51 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071bbd37c903648e3ebd95cc6dcb2b78d6ea639005d65aab5016dd7859a4f17b`  
		Last Modified: Fri, 04 Jun 2021 02:14:51 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2215edc22b4111496ab6990dcdc789842dbeaaa2138be04dcbb3ce883e984e`  
		Last Modified: Fri, 04 Jun 2021 02:14:59 GMT  
		Size: 7.0 MB (7033480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2c9d2207f5d9c10b8413a2bdbb9bb17306d47cd8d1efd70a3593d5343de178`  
		Last Modified: Fri, 04 Jun 2021 02:14:51 GMT  
		Size: 1.4 KB (1408 bytes)  
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
$ docker pull caddy@sha256:c6473228286ce37912a7ba2003a626c415698df940f04e7c88430e4ad01e168a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:5cd5e5c8ae7367744428893e4a407d97f68f70fbd298770c1518b65f3b740476
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646121085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b3e2a6c24449822ef29f7460905fddcbb84871a7dfa5dc27265afa64fa3778`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:24:28 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:24:29 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:24:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:24:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:25:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:25:36 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:26:02 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Jun 2021 01:19:04 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 01:21:38 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Jun 2021 01:21:40 GMT
WORKDIR C:\gopath
# Fri, 04 Jun 2021 02:10:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Jun 2021 02:10:55 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 02:10:56 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 02:10:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 02:11:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Jun 2021 02:11:25 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2a5ccd12170e9f926c3e069a2fa2ed38b5dd5596869ed982bccc50ef80cf1f`  
		Last Modified: Wed, 12 May 2021 12:52:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd5b5fa12081ad53ae688dc454e550dd50bd414c949724180719b0326632c4a`  
		Last Modified: Wed, 12 May 2021 12:52:08 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599ef939f9e7c26d4bc0f8f75820116f6977a64212b86260bc225ae2d850cc31`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bddce42b6f4351510fcb255839a7c55d95546186dce8509782abe959d27d9f0`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2407bf3b614294860b53b94e661f5c57f7dd985934aed5727442f9353bf8c617`  
		Last Modified: Wed, 12 May 2021 12:52:14 GMT  
		Size: 30.2 MB (30189126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b01ea9b4210c3201c1462d7ee78b276d7d5ffac3dca02c9c57a0c77c5b87a2`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27be8fd19f331f65055bbf31138aa28628be7534753008620ec14fc1803ebdf2`  
		Last Modified: Wed, 12 May 2021 12:52:05 GMT  
		Size: 313.1 KB (313094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f8e1e31aa0e91f80a0d7a9cf238278557166647fd937cc7b714778366d586a`  
		Last Modified: Fri, 04 Jun 2021 01:40:04 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ba074ffe696278b5b2037378141f68377dcab07cbcf7c6d31fcd4c097869ce`  
		Last Modified: Fri, 04 Jun 2021 01:42:39 GMT  
		Size: 139.4 MB (139388725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2deb8a1660a185bba3fa7aaabc4cb64555918509a91d9f186f15ec469ec476a0`  
		Last Modified: Fri, 04 Jun 2021 01:40:04 GMT  
		Size: 1.6 KB (1586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bce5d3df849365bd1516c0abf3aa29cee32abb96cc1cdf79c2e7019f2016cc0`  
		Last Modified: Fri, 04 Jun 2021 02:14:37 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc77252a6e317a6fcaeba9d070cfad6c4e568f095056d19727ffe6955e1a1c5a`  
		Last Modified: Fri, 04 Jun 2021 02:14:34 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f53aa8e353d64b1c65256ffeeb6708506ca6a23ee2c94016a8f034452259b0`  
		Last Modified: Fri, 04 Jun 2021 02:14:34 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c500d7c801483b02cfdfc1a272882d3b98559bcfacfb956ef4bb395fadccc61`  
		Last Modified: Fri, 04 Jun 2021 02:14:34 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243445945aa8cf8386f4cb635126e213960fe164cc0b2cf9829c40fb29e06dc4`  
		Last Modified: Fri, 04 Jun 2021 02:14:37 GMT  
		Size: 1.7 MB (1722485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5462596ac55051140e5c69946dc7620a0169d39d4b3a3b826e0daf4a0d924e8`  
		Last Modified: Fri, 04 Jun 2021 02:14:35 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:befa7d7c88cc950857d567f8fcd2ba435be538c6e6443ee1f806e755f27ea4ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `caddy:builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:23de8a02fd104f11187fa0e6f1c50d9a833788ef94cc3d78b82ad3b4f35c9fad
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5988471116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4830f2cecfad3d8daa420d50870e8aa44c459224a23f9ff77de7da22e670b94`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:29:13 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:29:14 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:29:15 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:29:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:31:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:31:45 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:33:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Jun 2021 01:21:50 GMT
ENV GOLANG_VERSION=1.16.5
# Fri, 04 Jun 2021 01:26:36 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Jun 2021 01:26:38 GMT
WORKDIR C:\gopath
# Fri, 04 Jun 2021 02:11:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 04 Jun 2021 02:11:34 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 04 Jun 2021 02:11:35 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 04 Jun 2021 02:11:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Jun 2021 02:13:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 04 Jun 2021 02:13:06 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10abf429e12c7b3b7d2b0a791d7cdb47866461a7b63df4ddd4f63acc91e26231`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79955f676504cbf77ec284d8e857d18d17b93c5b8e6438b4062dd80f8632c9d6`  
		Last Modified: Wed, 12 May 2021 12:55:12 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24af485ecab19f81a0c65c0eaec6f6fda8749ca50eb53101abcfc5c079f9b1c2`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b782f6bcd162ee81518d73c6c4fe5c5b731ab38b595c16a55ac185db84b2c9b`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1327fc384f9fff64d41446adcb3bdf585307370ef0024a31a5269bae6f30067d`  
		Last Modified: Wed, 12 May 2021 12:55:18 GMT  
		Size: 30.8 MB (30797956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c50f4b0b5994b4154be9fea2ab6c6a0e4c402c44d44795a5ce82ab6f8de4bc`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e458669a58e08411a0641a721ef1daf4af2a568c4dd61e9a3710b07f73b6ec`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 5.7 MB (5661591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7024df9f6db05baebb2373ac9d80a105fbfaafacf00e75d4b28847d1503ea8dc`  
		Last Modified: Fri, 04 Jun 2021 01:42:57 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b83a1b7a993d551850c2952fac9ce015fd85e6e96491ffc601809c6e4c9013`  
		Last Modified: Fri, 04 Jun 2021 01:45:53 GMT  
		Size: 149.2 MB (149182156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03bac4443c0dacba8f0d8dbd25091bc1d39b3ee36e84604482d40220f39f57d`  
		Last Modified: Fri, 04 Jun 2021 01:42:57 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51201b480eb2d1bd5736f2e118d9ddaafafce32222e161cb63b66a46bf95d9f`  
		Last Modified: Fri, 04 Jun 2021 02:14:54 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10338b4cf9e50762fa10529606ac5ab6d7c227a0aefcce7173718d53ef6b341`  
		Last Modified: Fri, 04 Jun 2021 02:14:51 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa84546d6c6cfa9ed6da4b4400af439e067c8f873c8ef40452cc57c7944a065`  
		Last Modified: Fri, 04 Jun 2021 02:14:51 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071bbd37c903648e3ebd95cc6dcb2b78d6ea639005d65aab5016dd7859a4f17b`  
		Last Modified: Fri, 04 Jun 2021 02:14:51 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2215edc22b4111496ab6990dcdc789842dbeaaa2138be04dcbb3ce883e984e`  
		Last Modified: Fri, 04 Jun 2021 02:14:59 GMT  
		Size: 7.0 MB (7033480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2c9d2207f5d9c10b8413a2bdbb9bb17306d47cd8d1efd70a3593d5343de178`  
		Last Modified: Fri, 04 Jun 2021 02:14:51 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:1a2f489f3bbeef0cac9397b7064a7908ed3f74b89d6f549825c38f175047d03d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

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

### `caddy:latest` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:1d0e1085c4e0fd3af411a60364e53d9e9ded463184467a4f1595116eb2e4c675
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2491869666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dac2e4738ade97d420148e609ac6c7a6db9edb6db52f3a634814cbe64df1d0b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:56:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 24 May 2021 18:14:49 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:15:23 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 24 May 2021 18:15:24 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 24 May 2021 18:15:25 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 24 May 2021 18:15:27 GMT
VOLUME [c:/config]
# Mon, 24 May 2021 18:15:28 GMT
VOLUME [c:/data]
# Mon, 24 May 2021 18:15:29 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:15:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:15:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:15:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:15:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:15:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:15:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:15:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:15:39 GMT
EXPOSE 80
# Mon, 24 May 2021 18:15:40 GMT
EXPOSE 443
# Mon, 24 May 2021 18:15:41 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:16:00 GMT
RUN caddy version
# Mon, 24 May 2021 18:16:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dc51194378204d7114732c3ee4da8d6b390b048e70ae1535a082de3ff67b5c`  
		Last Modified: Wed, 12 May 2021 20:06:24 GMT  
		Size: 5.1 MB (5106604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81697a0f2a55f882f55ccac9401c3dd272607c42f460a8549f30a1ebb26e0c8`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6400e9488fa4d970dad72e844be39d2d75b7d2c31501c6d6b23d6a1bc524f7c1`  
		Last Modified: Mon, 24 May 2021 18:22:57 GMT  
		Size: 11.9 MB (11930419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5b5da05058a691610222ba26189e6f6c28b9ede612bec34b4ed5dea3691b92`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197bdfed68cccee24a939b4dd69fea66e2dc7827a4017bf444bdd2c90e959f6a`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474f7ecfe9858ec31d5203cc051d4063e0ad4acd2af33e4568f49d9e4b75e41b`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e026dffad92f6dace75c209e6f261b00cf847128dd907ffa4ac9f944e9ae054e`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c534d757d31dc1e6130a58f06b95d25d61f32e015e329cd2227a1bed890280`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31071464c175eef4ea5843313a962e550e530c0a4c12fd997c6ace04fed5d0e0`  
		Last Modified: Mon, 24 May 2021 18:22:51 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3035f85e6f0ef498e48d22a196b3dca2d1feff90554b2f1fbbd3062a92ffccd2`  
		Last Modified: Mon, 24 May 2021 18:22:51 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caffd6e1f83b89b2831eab80faf22c370ad73519467e80354cb56ee96eed7fe3`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285714c5a6fb40773b7e624641f8e036180ab3424ee89b84f3fbbd79d7108eec`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872e853821b7661d1e753ef89a95c2525171915b5dec31950f7b05f4492eb40c`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7958b6b43cba2b3e1a20dc772e84541237901c32ec6dba998eb300627b2e343`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8089fe8b99a3884b64fb515b432248ed2433347b16efe53190c08624ec8bcf8f`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e25c6bfe294987f6c4c3a677078ea11dd90d54892fff638abed3d5a8602360c`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1757220b38637dda7da307ac64a4eefb9226cd9e13d613ab9bb839997c0c2aa8`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a748ef821631911b8abd470af8b29305283a82e1b5da1d2459257d8308576a2`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa22970d4f705eac4e8ea2ac4a7f3e89cfc01035b6ff0bf8998c146fe4d9a96`  
		Last Modified: Mon, 24 May 2021 18:22:47 GMT  
		Size: 317.9 KB (317938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2477d94c5c1388771379c903fc8931c2531d21a7ccbef4b3b7e2d6461fb19fdd`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:d530e436d6d892bc2662481a943d230921dd8d5b2a26de0d99c32abb59ce1973
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5819027610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:189fbf35362e472481d308f9fbecfeda8962471fccd521c1cdd2165bfff22c08`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:58:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 24 May 2021 18:16:16 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:17:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 24 May 2021 18:18:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 24 May 2021 18:18:02 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 24 May 2021 18:18:03 GMT
VOLUME [c:/config]
# Mon, 24 May 2021 18:18:04 GMT
VOLUME [c:/data]
# Mon, 24 May 2021 18:18:05 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:18:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:18:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:18:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:18:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:18:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:18:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:18:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:18:14 GMT
EXPOSE 80
# Mon, 24 May 2021 18:18:15 GMT
EXPOSE 443
# Mon, 24 May 2021 18:18:16 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:19:09 GMT
RUN caddy version
# Mon, 24 May 2021 18:19:10 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26858854e9a4d33437022a0cbf481973fa7709cc09d3402af046620cbbe5c0`  
		Last Modified: Wed, 12 May 2021 20:07:13 GMT  
		Size: 5.7 MB (5714091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba52519d045fbbd4b405dea0a101b9ede50767ce1b8b92f0b0a9708dc3a3492`  
		Last Modified: Mon, 24 May 2021 18:23:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073bc62336c22adb06e7c530733538c823c0e30b591f536ca853dd86ff16e632`  
		Last Modified: Mon, 24 May 2021 18:23:26 GMT  
		Size: 17.2 MB (17244195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319fcbb76d6ed2f5920ae3cf875486281ed4d5edc53c630c8c6ad581efc92594`  
		Last Modified: Mon, 24 May 2021 18:23:22 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d372740cbc98799ef99cd14fe521f6c8bc0202f7e6eb418f8db3e6cae94caf60`  
		Last Modified: Mon, 24 May 2021 18:23:21 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c1957ce089769a88ac826364c0cb191ae826407602ccf505c76ee34afa10c8`  
		Last Modified: Mon, 24 May 2021 18:23:20 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e022ba7739dc4609e4838ae24c6930ccdc82d0721cc978c71a7e036122adf228`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5716dc07e962e5602a2cecf1a5b63c75352ad0e48b06b30070ad5cd4a31993`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc94100cd9e1fb3620069275788a9e1b912502dcd7966b4d624ecba5f88690`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7790197c85ec7196ed9b956d8f481e8f382479a3b8e20db4d8e564f14331eb42`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60939c5f58f38df81a8563072d42fcd4fb79292dbf5ce4d31a46f840e777fb88`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d5876f07c48377c92817efa2b077cfe4c05822b08a1916d350b5e8ee682b50`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2933951452131d66acb34683269ade093ebb9faf312436b0a601168cb6e2fe68`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ad33c6332b1b2a8e806339fd2978dd9a8919fc98d48fc0ae6a58ad07870cec`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b44c787b930665927a13e544b5d3d7243caae27d4d9a6f9502f985e8483af61`  
		Last Modified: Mon, 24 May 2021 18:23:16 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e86dd1b42134f467b929f29aa052bdca8a20ccbb6ff1332575ef7843b962243`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3288b716f0b64cb14a9da486b126557c121b9a71476d5aea6a1be399a82bb14b`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83f9226706657b746cb502303856ebeca1a6cda85b1aea65196506c3e3faa4a`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fc7b2fb07d7a4265b695bf44d6d3378e7f0202a6c8fd0d359f766886070802`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 266.6 KB (266650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cde5c4ac8767e62fceac7aed63a74d7935277b8087425319abfe8e22f7bb37`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:c544077722bd97f1b56e46cf2c37d89d460d590defbe607243a750a2ab90a554
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:1d0e1085c4e0fd3af411a60364e53d9e9ded463184467a4f1595116eb2e4c675
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2491869666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dac2e4738ade97d420148e609ac6c7a6db9edb6db52f3a634814cbe64df1d0b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:56:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 24 May 2021 18:14:49 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:15:23 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 24 May 2021 18:15:24 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 24 May 2021 18:15:25 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 24 May 2021 18:15:27 GMT
VOLUME [c:/config]
# Mon, 24 May 2021 18:15:28 GMT
VOLUME [c:/data]
# Mon, 24 May 2021 18:15:29 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:15:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:15:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:15:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:15:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:15:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:15:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:15:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:15:39 GMT
EXPOSE 80
# Mon, 24 May 2021 18:15:40 GMT
EXPOSE 443
# Mon, 24 May 2021 18:15:41 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:16:00 GMT
RUN caddy version
# Mon, 24 May 2021 18:16:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dc51194378204d7114732c3ee4da8d6b390b048e70ae1535a082de3ff67b5c`  
		Last Modified: Wed, 12 May 2021 20:06:24 GMT  
		Size: 5.1 MB (5106604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81697a0f2a55f882f55ccac9401c3dd272607c42f460a8549f30a1ebb26e0c8`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6400e9488fa4d970dad72e844be39d2d75b7d2c31501c6d6b23d6a1bc524f7c1`  
		Last Modified: Mon, 24 May 2021 18:22:57 GMT  
		Size: 11.9 MB (11930419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5b5da05058a691610222ba26189e6f6c28b9ede612bec34b4ed5dea3691b92`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197bdfed68cccee24a939b4dd69fea66e2dc7827a4017bf444bdd2c90e959f6a`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474f7ecfe9858ec31d5203cc051d4063e0ad4acd2af33e4568f49d9e4b75e41b`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e026dffad92f6dace75c209e6f261b00cf847128dd907ffa4ac9f944e9ae054e`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c534d757d31dc1e6130a58f06b95d25d61f32e015e329cd2227a1bed890280`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31071464c175eef4ea5843313a962e550e530c0a4c12fd997c6ace04fed5d0e0`  
		Last Modified: Mon, 24 May 2021 18:22:51 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3035f85e6f0ef498e48d22a196b3dca2d1feff90554b2f1fbbd3062a92ffccd2`  
		Last Modified: Mon, 24 May 2021 18:22:51 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caffd6e1f83b89b2831eab80faf22c370ad73519467e80354cb56ee96eed7fe3`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285714c5a6fb40773b7e624641f8e036180ab3424ee89b84f3fbbd79d7108eec`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872e853821b7661d1e753ef89a95c2525171915b5dec31950f7b05f4492eb40c`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7958b6b43cba2b3e1a20dc772e84541237901c32ec6dba998eb300627b2e343`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8089fe8b99a3884b64fb515b432248ed2433347b16efe53190c08624ec8bcf8f`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e25c6bfe294987f6c4c3a677078ea11dd90d54892fff638abed3d5a8602360c`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1757220b38637dda7da307ac64a4eefb9226cd9e13d613ab9bb839997c0c2aa8`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a748ef821631911b8abd470af8b29305283a82e1b5da1d2459257d8308576a2`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa22970d4f705eac4e8ea2ac4a7f3e89cfc01035b6ff0bf8998c146fe4d9a96`  
		Last Modified: Mon, 24 May 2021 18:22:47 GMT  
		Size: 317.9 KB (317938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2477d94c5c1388771379c903fc8931c2531d21a7ccbef4b3b7e2d6461fb19fdd`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:d530e436d6d892bc2662481a943d230921dd8d5b2a26de0d99c32abb59ce1973
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5819027610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:189fbf35362e472481d308f9fbecfeda8962471fccd521c1cdd2165bfff22c08`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:58:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 24 May 2021 18:16:16 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:17:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 24 May 2021 18:18:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 24 May 2021 18:18:02 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 24 May 2021 18:18:03 GMT
VOLUME [c:/config]
# Mon, 24 May 2021 18:18:04 GMT
VOLUME [c:/data]
# Mon, 24 May 2021 18:18:05 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:18:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:18:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:18:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:18:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:18:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:18:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:18:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:18:14 GMT
EXPOSE 80
# Mon, 24 May 2021 18:18:15 GMT
EXPOSE 443
# Mon, 24 May 2021 18:18:16 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:19:09 GMT
RUN caddy version
# Mon, 24 May 2021 18:19:10 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26858854e9a4d33437022a0cbf481973fa7709cc09d3402af046620cbbe5c0`  
		Last Modified: Wed, 12 May 2021 20:07:13 GMT  
		Size: 5.7 MB (5714091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba52519d045fbbd4b405dea0a101b9ede50767ce1b8b92f0b0a9708dc3a3492`  
		Last Modified: Mon, 24 May 2021 18:23:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073bc62336c22adb06e7c530733538c823c0e30b591f536ca853dd86ff16e632`  
		Last Modified: Mon, 24 May 2021 18:23:26 GMT  
		Size: 17.2 MB (17244195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319fcbb76d6ed2f5920ae3cf875486281ed4d5edc53c630c8c6ad581efc92594`  
		Last Modified: Mon, 24 May 2021 18:23:22 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d372740cbc98799ef99cd14fe521f6c8bc0202f7e6eb418f8db3e6cae94caf60`  
		Last Modified: Mon, 24 May 2021 18:23:21 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c1957ce089769a88ac826364c0cb191ae826407602ccf505c76ee34afa10c8`  
		Last Modified: Mon, 24 May 2021 18:23:20 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e022ba7739dc4609e4838ae24c6930ccdc82d0721cc978c71a7e036122adf228`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5716dc07e962e5602a2cecf1a5b63c75352ad0e48b06b30070ad5cd4a31993`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc94100cd9e1fb3620069275788a9e1b912502dcd7966b4d624ecba5f88690`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7790197c85ec7196ed9b956d8f481e8f382479a3b8e20db4d8e564f14331eb42`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60939c5f58f38df81a8563072d42fcd4fb79292dbf5ce4d31a46f840e777fb88`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d5876f07c48377c92817efa2b077cfe4c05822b08a1916d350b5e8ee682b50`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2933951452131d66acb34683269ade093ebb9faf312436b0a601168cb6e2fe68`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ad33c6332b1b2a8e806339fd2978dd9a8919fc98d48fc0ae6a58ad07870cec`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b44c787b930665927a13e544b5d3d7243caae27d4d9a6f9502f985e8483af61`  
		Last Modified: Mon, 24 May 2021 18:23:16 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e86dd1b42134f467b929f29aa052bdca8a20ccbb6ff1332575ef7843b962243`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3288b716f0b64cb14a9da486b126557c121b9a71476d5aea6a1be399a82bb14b`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83f9226706657b746cb502303856ebeca1a6cda85b1aea65196506c3e3faa4a`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fc7b2fb07d7a4265b695bf44d6d3378e7f0202a6c8fd0d359f766886070802`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 266.6 KB (266650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cde5c4ac8767e62fceac7aed63a74d7935277b8087425319abfe8e22f7bb37`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:fb9fcd910a8050aa2ce11ac6b195722843c6efc46c1cf68fbb3a4172914c2e30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:1d0e1085c4e0fd3af411a60364e53d9e9ded463184467a4f1595116eb2e4c675
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2491869666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dac2e4738ade97d420148e609ac6c7a6db9edb6db52f3a634814cbe64df1d0b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:56:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 24 May 2021 18:14:49 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:15:23 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 24 May 2021 18:15:24 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 24 May 2021 18:15:25 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 24 May 2021 18:15:27 GMT
VOLUME [c:/config]
# Mon, 24 May 2021 18:15:28 GMT
VOLUME [c:/data]
# Mon, 24 May 2021 18:15:29 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:15:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:15:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:15:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:15:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:15:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:15:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:15:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:15:39 GMT
EXPOSE 80
# Mon, 24 May 2021 18:15:40 GMT
EXPOSE 443
# Mon, 24 May 2021 18:15:41 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:16:00 GMT
RUN caddy version
# Mon, 24 May 2021 18:16:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dc51194378204d7114732c3ee4da8d6b390b048e70ae1535a082de3ff67b5c`  
		Last Modified: Wed, 12 May 2021 20:06:24 GMT  
		Size: 5.1 MB (5106604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81697a0f2a55f882f55ccac9401c3dd272607c42f460a8549f30a1ebb26e0c8`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6400e9488fa4d970dad72e844be39d2d75b7d2c31501c6d6b23d6a1bc524f7c1`  
		Last Modified: Mon, 24 May 2021 18:22:57 GMT  
		Size: 11.9 MB (11930419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5b5da05058a691610222ba26189e6f6c28b9ede612bec34b4ed5dea3691b92`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197bdfed68cccee24a939b4dd69fea66e2dc7827a4017bf444bdd2c90e959f6a`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474f7ecfe9858ec31d5203cc051d4063e0ad4acd2af33e4568f49d9e4b75e41b`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e026dffad92f6dace75c209e6f261b00cf847128dd907ffa4ac9f944e9ae054e`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c534d757d31dc1e6130a58f06b95d25d61f32e015e329cd2227a1bed890280`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31071464c175eef4ea5843313a962e550e530c0a4c12fd997c6ace04fed5d0e0`  
		Last Modified: Mon, 24 May 2021 18:22:51 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3035f85e6f0ef498e48d22a196b3dca2d1feff90554b2f1fbbd3062a92ffccd2`  
		Last Modified: Mon, 24 May 2021 18:22:51 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caffd6e1f83b89b2831eab80faf22c370ad73519467e80354cb56ee96eed7fe3`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285714c5a6fb40773b7e624641f8e036180ab3424ee89b84f3fbbd79d7108eec`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872e853821b7661d1e753ef89a95c2525171915b5dec31950f7b05f4492eb40c`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7958b6b43cba2b3e1a20dc772e84541237901c32ec6dba998eb300627b2e343`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8089fe8b99a3884b64fb515b432248ed2433347b16efe53190c08624ec8bcf8f`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e25c6bfe294987f6c4c3a677078ea11dd90d54892fff638abed3d5a8602360c`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1757220b38637dda7da307ac64a4eefb9226cd9e13d613ab9bb839997c0c2aa8`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a748ef821631911b8abd470af8b29305283a82e1b5da1d2459257d8308576a2`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa22970d4f705eac4e8ea2ac4a7f3e89cfc01035b6ff0bf8998c146fe4d9a96`  
		Last Modified: Mon, 24 May 2021 18:22:47 GMT  
		Size: 317.9 KB (317938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2477d94c5c1388771379c903fc8931c2531d21a7ccbef4b3b7e2d6461fb19fdd`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:9d786a7a09f9a8edcfdc2a75b463592913275d75986f55ca9d67f3ba0b848c67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `caddy:windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:d530e436d6d892bc2662481a943d230921dd8d5b2a26de0d99c32abb59ce1973
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5819027610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:189fbf35362e472481d308f9fbecfeda8962471fccd521c1cdd2165bfff22c08`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:58:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 24 May 2021 18:16:16 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:17:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 24 May 2021 18:18:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 24 May 2021 18:18:02 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 24 May 2021 18:18:03 GMT
VOLUME [c:/config]
# Mon, 24 May 2021 18:18:04 GMT
VOLUME [c:/data]
# Mon, 24 May 2021 18:18:05 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:18:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:18:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:18:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:18:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:18:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:18:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:18:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:18:14 GMT
EXPOSE 80
# Mon, 24 May 2021 18:18:15 GMT
EXPOSE 443
# Mon, 24 May 2021 18:18:16 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:19:09 GMT
RUN caddy version
# Mon, 24 May 2021 18:19:10 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26858854e9a4d33437022a0cbf481973fa7709cc09d3402af046620cbbe5c0`  
		Last Modified: Wed, 12 May 2021 20:07:13 GMT  
		Size: 5.7 MB (5714091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba52519d045fbbd4b405dea0a101b9ede50767ce1b8b92f0b0a9708dc3a3492`  
		Last Modified: Mon, 24 May 2021 18:23:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073bc62336c22adb06e7c530733538c823c0e30b591f536ca853dd86ff16e632`  
		Last Modified: Mon, 24 May 2021 18:23:26 GMT  
		Size: 17.2 MB (17244195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319fcbb76d6ed2f5920ae3cf875486281ed4d5edc53c630c8c6ad581efc92594`  
		Last Modified: Mon, 24 May 2021 18:23:22 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d372740cbc98799ef99cd14fe521f6c8bc0202f7e6eb418f8db3e6cae94caf60`  
		Last Modified: Mon, 24 May 2021 18:23:21 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c1957ce089769a88ac826364c0cb191ae826407602ccf505c76ee34afa10c8`  
		Last Modified: Mon, 24 May 2021 18:23:20 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e022ba7739dc4609e4838ae24c6930ccdc82d0721cc978c71a7e036122adf228`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5716dc07e962e5602a2cecf1a5b63c75352ad0e48b06b30070ad5cd4a31993`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc94100cd9e1fb3620069275788a9e1b912502dcd7966b4d624ecba5f88690`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7790197c85ec7196ed9b956d8f481e8f382479a3b8e20db4d8e564f14331eb42`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60939c5f58f38df81a8563072d42fcd4fb79292dbf5ce4d31a46f840e777fb88`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d5876f07c48377c92817efa2b077cfe4c05822b08a1916d350b5e8ee682b50`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2933951452131d66acb34683269ade093ebb9faf312436b0a601168cb6e2fe68`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ad33c6332b1b2a8e806339fd2978dd9a8919fc98d48fc0ae6a58ad07870cec`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b44c787b930665927a13e544b5d3d7243caae27d4d9a6f9502f985e8483af61`  
		Last Modified: Mon, 24 May 2021 18:23:16 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e86dd1b42134f467b929f29aa052bdca8a20ccbb6ff1332575ef7843b962243`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3288b716f0b64cb14a9da486b126557c121b9a71476d5aea6a1be399a82bb14b`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83f9226706657b746cb502303856ebeca1a6cda85b1aea65196506c3e3faa4a`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fc7b2fb07d7a4265b695bf44d6d3378e7f0202a6c8fd0d359f766886070802`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 266.6 KB (266650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cde5c4ac8767e62fceac7aed63a74d7935277b8087425319abfe8e22f7bb37`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
